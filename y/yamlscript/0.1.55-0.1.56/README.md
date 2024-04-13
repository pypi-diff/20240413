# Comparing `tmp/yamlscript-0.1.55.tar.gz` & `tmp/yamlscript-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlscript-0.1.55.tar", last modified: Fri Apr 12 19:34:47 2024, max compression
+gzip compressed data, was "yamlscript-0.1.56.tar", last modified: Sat Apr 13 20:22:30 2024, max compression
```

## Comparing `yamlscript-0.1.55.tar` & `yamlscript-0.1.56.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.358009 yamlscript-0.1.55/
--rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.000000 yamlscript-0.1.55/.long_description.md
--rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-04-12 19:34:47.000000 yamlscript-0.1.55/MANIFEST.in
--rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-12 19:34:47.358009 yamlscript-0.1.55/PKG-INFO
--rw-rw-r--   0 ingy      (1000) ingy      (1000)     3082 2024-04-11 15:16:19.000000 yamlscript-0.1.55/ReadMe.md
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.358009 yamlscript-0.1.55/lib/
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.358009 yamlscript-0.1.55/lib/yamlscript/
--rw-r--r--   0 ingy      (1000) ingy      (1000)     4365 2024-04-12 19:28:29.000000 yamlscript-0.1.55/lib/yamlscript/__init__.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.358009 yamlscript-0.1.55/lib/yamlscript.egg-info/
--rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-12 19:34:47.000000 yamlscript-0.1.55/lib/yamlscript.egg-info/PKG-INFO
--rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-04-12 19:34:47.000000 yamlscript-0.1.55/lib/yamlscript.egg-info/SOURCES.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-04-12 19:34:47.000000 yamlscript-0.1.55/lib/yamlscript.egg-info/dependency_links.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-04-12 19:34:47.000000 yamlscript-0.1.55/lib/yamlscript.egg-info/requires.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-04-12 19:34:47.000000 yamlscript-0.1.55/lib/yamlscript.egg-info/top_level.txt
--rw-rw-r--   0 ingy      (1000) ingy      (1000)       79 2024-04-12 19:34:47.358009 yamlscript-0.1.55/setup.cfg
--rw-r--r--   0 ingy      (1000) ingy      (1000)     1146 2024-04-12 19:28:30.000000 yamlscript-0.1.55/setup.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-12 19:34:47.358009 yamlscript-0.1.55/test/
--rw-rw-r--   0 ingy      (1000) ingy      (1000)      144 2024-03-28 18:44:00.000000 yamlscript-0.1.55/test/test.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.212419 yamlscript-0.1.56/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.000000 yamlscript-0.1.56/.long_description.md
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-04-13 20:22:30.000000 yamlscript-0.1.56/MANIFEST.in
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-13 20:22:30.212419 yamlscript-0.1.56/PKG-INFO
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     3082 2024-04-13 19:42:42.000000 yamlscript-0.1.56/ReadMe.md
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.212419 yamlscript-0.1.56/lib/
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.212419 yamlscript-0.1.56/lib/yamlscript/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     4365 2024-04-13 20:17:23.000000 yamlscript-0.1.56/lib/yamlscript/__init__.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.212419 yamlscript-0.1.56/lib/yamlscript.egg-info/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-13 20:22:30.000000 yamlscript-0.1.56/lib/yamlscript.egg-info/PKG-INFO
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-04-13 20:22:30.000000 yamlscript-0.1.56/lib/yamlscript.egg-info/SOURCES.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-04-13 20:22:30.000000 yamlscript-0.1.56/lib/yamlscript.egg-info/dependency_links.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-04-13 20:22:30.000000 yamlscript-0.1.56/lib/yamlscript.egg-info/requires.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-04-13 20:22:30.000000 yamlscript-0.1.56/lib/yamlscript.egg-info/top_level.txt
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)       79 2024-04-13 20:22:30.212419 yamlscript-0.1.56/setup.cfg
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     1146 2024-04-13 20:17:23.000000 yamlscript-0.1.56/setup.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-13 20:22:30.212419 yamlscript-0.1.56/test/
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)      144 2024-03-28 18:44:00.000000 yamlscript-0.1.56/test/test.py
```

### Comparing `yamlscript-0.1.55/PKG-INFO` & `yamlscript-0.1.56/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.55
+Version: 0.1.56
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.55/ReadMe.md` & `yamlscript-0.1.56/ReadMe.md`

 * *Files identical despite different names*

### Comparing `yamlscript-0.1.55/lib/yamlscript/__init__.py` & `yamlscript-0.1.56/lib/yamlscript/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 The load() method takes a YAMLScript string as input and returns the Python
 object that the YAMLScript code evaluates to.
 """
 
 # This value is automatically updated by 'make bump'.
 # The version number is used to find the correct shared library file.
 # We currently only support binding to an exact version of libyamlscript.
-yamlscript_version = '0.1.55'
+yamlscript_version = '0.1.56'
 
 import os, sys
 import ctypes
 import json
 
 # Require Python 3.6 or greater:
 assert sys.version_info >= (3, 6), \
```

### Comparing `yamlscript-0.1.55/lib/yamlscript.egg-info/PKG-INFO` & `yamlscript-0.1.56/lib/yamlscript.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.55
+Version: 0.1.56
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.55/setup.py` & `yamlscript-0.1.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '0.1.55'
+version = '0.1.56'
 
 from setuptools import setup
 import pathlib
 
 root = pathlib.Path(__file__).parent.resolve()
 
 long_description = \
```

