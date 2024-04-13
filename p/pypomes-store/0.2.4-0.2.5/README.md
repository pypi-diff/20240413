# Comparing `tmp/pypomes_store-0.2.4.tar.gz` & `tmp/pypomes_store-0.2.5.tar.gz`

## Comparing `pypomes_store-0.2.4.tar` & `pypomes_store-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/src/__init__.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/src/pypomes_store/minio_client.py
+-rw-r--r--   0        0        0    14698 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.5/PKG-INFO
```

### Comparing `pypomes_store-0.2.4/src/pypomes_store/__init__.py` & `pypomes_store-0.2.5/src/pypomes_store/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from .minio_client import (
+    MinioCM
+)
 from .minio_pomes import (
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup,
 )
 
 __all__ = [
+    # minio_client
+    "MinioCM",
     # minio_pomes
     "MINIO_BUCKET", "MINIO_HOST", "MINIO_ACCESS_KEY",
     "MINIO_SECRET_KEY", "MINIO_SECURE_ACCESS", "MINIO_TEMP_PATH",
     "minio_access", "minio_file_store", "minio_object_store", "minio_object_stat",
     "minio_object_delete", "minio_objects_list", "minio_object_retrieve", "minio_object_exists",
     "minio_object_tags_retrieve", "minio_file_retrieve", "minio_setup",
 ]
```

### Comparing `pypomes_store-0.2.4/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.2.5/src/pypomes_store/minio_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,67 +6,69 @@
 from minio.datatypes import Object as MinioObject
 from minio.commonconfig import Tags
 from pathlib import Path
 from pypomes_core import APP_PREFIX, TEMP_DIR, env_get_bool, env_get_str, env_get_path
 from typing import Final
 from unidecode import unidecode
 
+from .minio_client import MinioCM
+
 MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET")
 MINIO_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_HOST")
 MINIO_ACCESS_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
 MINIO_SECRET_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
 MINIO_SECURE_ACCESS: Final[bool] = env_get_bool(f"{APP_PREFIX}_MINIO_SECURE_ACCESS")
 MINIO_TEMP_PATH: Final[Path] = env_get_path(f"{APP_PREFIX}_MINIO_TEMP_PATH", TEMP_DIR)
 
 
-def minio_setup(errors: list[str]) -> bool:
+def minio_access(errors: list[str]) -> Minio:
     """
-    Prepare the *MinIO* client for operations.
-
-    This function should be called just once, at startup,
-    to make sure the interaction with the MinIo service is fully functional.
+    Obtain and return a *MinIO* client object.
 
     :param errors: incidental error messages
-    :return: True if service is fully functional
+    :return: the MinIO client object
     """
     # initialize the return variable
-    result: bool = False
+    result: Minio | None = None
 
-    # obtain the MinIO client and proceed
+    # obtain the MinIO client
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
-            if not minio_client.bucket_exists(bucket_name=MINIO_BUCKET):
-                minio_client.make_bucket(bucket_name=MINIO_BUCKET)
-            result = True
+        result = Minio(endpoint=MINIO_HOST,
+                       access_key=MINIO_ACCESS_KEY,
+                       secret_key=MINIO_SECRET_KEY,
+                       secure=MINIO_SECURE_ACCESS)
+
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
-def minio_access(errors: list[str]) -> Minio:
+def minio_setup(errors: list[str]) -> bool:
     """
-    Obtain and return the *MinIO* client object.
+    Prepare the *MinIO* client for operations.
+
+    This function should be called just once, at startup,
+    to make sure the interaction with the MinIo service is fully functional.
 
     :param errors: incidental error messages
-    :return: the MinIO client object
+    :return: True if service is fully functional
     """
     # initialize the return variable
-    result: Minio | None = None
+    result: bool = False
 
-    # obtain the MinIO client
+    # obtain the MinIO client and proceed
     try:
-        result = Minio(endpoint=MINIO_HOST,
-                       access_key=MINIO_ACCESS_KEY,
-                       secret_key=MINIO_SECRET_KEY,
-                       secure=MINIO_SECURE_ACCESS)
-
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
+            if not minio_client.bucket_exists(bucket_name=MINIO_BUCKET):
+                minio_client.make_bucket(bucket_name=MINIO_BUCKET)
+            result = True
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_file_store(errors: list[str], basepath: Path | str,
@@ -79,18 +81,18 @@
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
     :param mimetype: the file mimetype
     :param tags: optional metadata describing the file
     """
     # obtain the MinIO client and proceed
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
             remotepath: Path = Path(basepath) / identifier
             # have tags been defined ?
             if tags is None or len(tags) == 0:
                 # no
                 doc_tags = None
             else:
                 # sim, store them
@@ -117,18 +119,18 @@
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
     :return: information about the file retrieved
     """
     # obtain the MinIO client and proceed
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
             remotepath: Path = Path(basepath) / identifier
             try:
                 result = minio_client.fget_object(bucket_name=MINIO_BUCKET,
                                                   object_name=f"{remotepath}",
                                                   file_path=filepath)
             except Exception as e:
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
@@ -175,18 +177,18 @@
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: MinioObject | None = None
 
     # obtain the MinIO client and proceed
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
             remotepath: Path = Path(basepath) / identifier
             try:
                 result = minio_client.stat_object(bucket_name=MINIO_BUCKET,
                                                   object_name=f"{remotepath}")
             except Exception as e:
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
                     errors.append(__minio_except_msg(e))
@@ -253,18 +255,18 @@
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     """
     # obtain the MinIO client and proceed
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
             # was the identifier provided ?
             if identifier is None:
                 # no, remove the folder
                 __minio_folder_delete(errors, minio_client, basepath)
             else:
                 # yes, remove the object
                 remotepath: str = os.path.join(basepath, identifier)
@@ -286,55 +288,54 @@
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     :return: the metadata about the object
     """
     # initialize the return variable
     result: dict | None = None
-
-    # obtain the MinIO client
-    minio_client: Minio = minio_access(errors)
-
-    # was the MinIO client obtained ?
-    if minio_client:
-        # yes, proceed
-        remotepath: str = os.path.join(basepath, identifier)
-        try:
-            tags: Tags = minio_client.get_object_tags(bucket_name=MINIO_BUCKET,
-                                                      object_name=remotepath)
-            if tags is not None and len(tags) > 0:
-                result = {}
-                for key, value in tags.items():
-                    result[key] = value
-        except Exception as e:
-            if not hasattr(e, "code") or e.code != "NoSuchKey":
-                errors.append(__minio_except_msg(e))
+    try:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
+            remotepath: str = os.path.join(basepath, identifier)
+            try:
+                tags: Tags = minio_client.get_object_tags(bucket_name=MINIO_BUCKET,
+                                                          object_name=remotepath)
+                if tags is not None and len(tags) > 0:
+                    result = {}
+                    for key, value in tags.items():
+                        result[key] = value
+            except Exception as e:
+                if not hasattr(e, "code") or e.code != "NoSuchKey":
+                    errors.append(__minio_except_msg(e))
+    except Exception as e:
+        errors.append(__minio_except_msg(e))
 
     return result
 
 
-# retorna a lista de objetos na pasta identificada pelo argumento - None se pasta não existe
 def minio_objects_list(errors: list[str], basepath: str, recursive: bool = False) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
-    :return: the iterator into the list of objects
+    :return: the iterator into the list of objects, 'None' if the folder does not exist
     """
     # initialize the return variable
     result: Iterator | None = None
 
     # obtain the MinIO client and proceed
     try:
-        with Minio(endpoint=MINIO_HOST,
-                   access_key=MINIO_ACCESS_KEY,
-                   secret_key=MINIO_SECRET_KEY,
-                   secure=MINIO_SECURE_ACCESS) as minio_client:
+        with MinioCM(endpoint=MINIO_HOST,
+                     access_key=MINIO_ACCESS_KEY,
+                     secret_key=MINIO_SECRET_KEY,
+                     secure=MINIO_SECURE_ACCESS) as minio_client:
             result = minio_client.list_objects(bucket_name=MINIO_BUCKET,
                                                prefix=basepath,
                                                recursive=recursive)
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypomes_store-0.2.4/LICENSE` & `pypomes_store-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.4/pyproject.toml` & `pypomes_store-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_store-0.2.4/PKG-INFO` & `pypomes_store-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_store
-Version: 0.2.4
+Version: 0.2.5
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

