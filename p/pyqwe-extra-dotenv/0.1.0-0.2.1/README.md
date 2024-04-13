# Comparing `tmp/pyqwe_extra_dotenv-0.1.0.tar.gz` & `tmp/pyqwe_extra_dotenv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqwe_extra_dotenv-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyqwe_extra_dotenv-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyqwe_extra_dotenv-0.1.0.tar` & `pyqwe_extra_dotenv-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,6 @@
--rw-r--r--   0        0        0     1160 2024-03-30 10:38:18.664140 pyqwe_extra_dotenv-0.1.0/.gitignore
--rw-r--r--   0        0        0      239 2024-03-30 12:32:55.592877 pyqwe_extra_dotenv-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0     5459 2024-03-30 12:32:54.626696 pyqwe_extra_dotenv-0.1.0/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0        4 2024-03-30 12:32:53.604917 pyqwe_extra_dotenv-0.1.0/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0    18014 2024-03-30 12:32:53.592364 pyqwe_extra_dotenv-0.1.0/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0     1170 2024-03-30 12:32:54.726559 pyqwe_extra_dotenv-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2024-03-30 12:32:54.754203 pyqwe_extra_dotenv-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      320 2024-03-30 12:35:12.564211 pyqwe_extra_dotenv-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      288 2024-03-30 12:32:54.743327 pyqwe_extra_dotenv-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      430 2024-03-30 12:33:16.047646 pyqwe_extra_dotenv-0.1.0/.idea/pyqwe-extra-dotenv.iml
--rw-r--r--   0        0        0      508 2024-03-30 13:03:23.948951 pyqwe_extra_dotenv-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe_extra_dotenv-0.1.0/LICENSE
--rw-r--r--   0        0        0      336 2024-03-30 12:58:53.385392 pyqwe_extra_dotenv-0.1.0/README.md
--rw-r--r--   0        0        0      684 2024-03-30 13:03:23.879508 pyqwe_extra_dotenv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2517 2024-03-30 12:56:06.900248 pyqwe_extra_dotenv-0.1.0/pyqwe_extra_dotenv/__init__.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 pyqwe_extra_dotenv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1160 2024-03-30 10:38:18.664140 pyqwe_extra_dotenv-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe_extra_dotenv-0.2.1/LICENSE
+-rw-r--r--   0        0        0      336 2024-03-30 12:58:53.385392 pyqwe_extra_dotenv-0.2.1/README.md
+-rw-r--r--   0        0        0      683 2024-04-13 12:41:44.698176 pyqwe_extra_dotenv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2517 2024-04-13 12:41:58.698043 pyqwe_extra_dotenv-0.2.1/pyqwe_extra_dotenv/__init__.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 pyqwe_extra_dotenv-0.2.1/PKG-INFO
```

### Comparing `pyqwe_extra_dotenv-0.1.0/.gitignore` & `pyqwe_extra_dotenv-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqwe_extra_dotenv-0.1.0/LICENSE` & `pyqwe_extra_dotenv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqwe_extra_dotenv-0.1.0/pyproject.toml` & `pyqwe_extra_dotenv-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pyqwe-extra-dotenv"
 description = 'A package that provides python-dotenv functionality for pyqwe. This package can only be used with pyqwe.'
 authors = [{ name = "David Carmichael", email = "david@uilix.com" }]
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version"]
 dependencies = [
     "python-dotenv"
 ]
```

### Comparing `pyqwe_extra_dotenv-0.1.0/pyqwe_extra_dotenv/__init__.py` & `pyqwe_extra_dotenv-0.2.1/pyqwe_extra_dotenv/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 try:
     import pyqwe
 except ImportError:
     raise ImportError("pyqwe not found")
 
-__version__ = "0.1.0"
+__version__ = "0.2.1"
 
 
 class EnvVarNotFound(Exception):
     pass
 
 
 class Colr:
```

### Comparing `pyqwe_extra_dotenv-0.1.0/PKG-INFO` & `pyqwe_extra_dotenv-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyqwe-extra-dotenv
-Version: 0.1.0
+Version: 0.2.1
 Summary: A package that provides python-dotenv functionality for pyqwe. This package can only be used with pyqwe.
 Author-email: David Carmichael <david@uilix.com>
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: python-dotenv
 Project-URL: Source, https://github.com/CheeseCake87/pyqwe
 
 # 🏎️💨 pyqwe-extra-dotenv
```

