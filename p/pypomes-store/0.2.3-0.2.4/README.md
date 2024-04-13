# Comparing `tmp/pypomes_store-0.2.3.tar.gz` & `tmp/pypomes_store-0.2.4.tar.gz`

## Comparing `pypomes_store-0.2.3.tar` & `pypomes_store-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/README.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pypomes_store-0.2.4/PKG-INFO
```

### Comparing `pypomes_store-0.2.3/src/pypomes_store/__init__.py` & `pypomes_store-0.2.4/src/pypomes_store/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.3/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.2.4/src/pypomes_store/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.3/LICENSE` & `pypomes_store-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.2.3/pyproject.toml` & `pypomes_store-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "minio>=7.2.5",
     "pip>=24.0",
-    "pypomes_core>=0.7.0",
+    "pypomes_core>=0.8.4",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
```

### Comparing `pypomes_store-0.2.3/PKG-INFO` & `pypomes_store-0.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: pypomes_store
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: minio>=7.2.5
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.7.0
+Requires-Dist: pypomes-core>=0.8.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.42.0
```

