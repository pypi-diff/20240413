# Comparing `tmp/firestore_wrapper-0.3.3.tar.gz` & `tmp/firestore_wrapper-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestore_wrapper-0.3.3.tar", last modified: Sun Apr  7 22:54:18 2024, max compression
+gzip compressed data, was "firestore_wrapper-0.3.4.tar", last modified: Sat Apr 13 05:50:12 2024, max compression
```

## Comparing `firestore_wrapper-0.3.3.tar` & `firestore_wrapper-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:54:18.418593 firestore_wrapper-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:54:18.418593 firestore_wrapper-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:54:18.418593 firestore_wrapper-0.3.3/firestore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/collection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/document_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/firestore_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/firestore_wrapper/utility_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 22:54:18.418593 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-07 22:54:18.000000 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 22:54:18.000000 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 22:54:18.000000 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 22:54:18.000000 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 22:54:18.000000 firestore_wrapper-0.3.3/firestore_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 22:54:18.418593 firestore_wrapper-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 22:54:11.000000 firestore_wrapper-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:50:12.940531 firestore_wrapper-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-13 05:50:12.940531 firestore_wrapper-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:50:12.940531 firestore_wrapper-0.3.4/firestore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/collection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/document_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/firestore_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/firestore_wrapper/utility_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:50:12.940531 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-13 05:50:12.000000 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 05:50:12.000000 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:50:12.000000 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 05:50:12.000000 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 05:50:12.000000 firestore_wrapper-0.3.4/firestore_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:50:12.940531 firestore_wrapper-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-13 05:50:05.000000 firestore_wrapper-0.3.4/setup.py
```

### Comparing `firestore_wrapper-0.3.3/LICENSE` & `firestore_wrapper-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/PKG-INFO` & `firestore_wrapper-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore_wrapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.3/README.md` & `firestore_wrapper-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/backup_manager.py` & `firestore_wrapper-0.3.4/firestore_wrapper/backup_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self._backup_folder = backup_folder
         self.collections_to_backup = collections
         self.ensure_backup()
 
     @property
     def backup_folder(self) -> str:
         v = self._backup_folder
-        if '~' in v:
+        if v is not None and '~' in v:
             v = os.path.expanduser(v)
         return v
 
     @backup_folder.setter
     def backup_folder(self, value: str):
         self._backup_folder = value
```

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/collection_manager.py` & `firestore_wrapper-0.3.4/firestore_wrapper/collection_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/core.py` & `firestore_wrapper-0.3.4/firestore_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/document_manager.py` & `firestore_wrapper-0.3.4/firestore_wrapper/document_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/firestore_base.py` & `firestore_wrapper-0.3.4/firestore_wrapper/firestore_base.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/query_manager.py` & `firestore_wrapper-0.3.4/firestore_wrapper/query_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/schema_utils.py` & `firestore_wrapper-0.3.4/firestore_wrapper/schema_utils.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper/utility_manager.py` & `firestore_wrapper-0.3.4/firestore_wrapper/utility_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper.egg-info/PKG-INFO` & `firestore_wrapper-0.3.4/firestore_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestore-wrapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
```

### Comparing `firestore_wrapper-0.3.3/firestore_wrapper.egg-info/SOURCES.txt` & `firestore_wrapper-0.3.4/firestore_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.3.3/setup.py` & `firestore_wrapper-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='firestore_wrapper',
-    version='0.3.3',
+    version='0.3.4',
     packages=find_packages(),
     description='A custom wrapper for Google Firestore.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
```

