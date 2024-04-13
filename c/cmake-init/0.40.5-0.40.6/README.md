# Comparing `tmp/cmake-init-0.40.5.tar.gz` & `tmp/cmake-init-0.40.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake-init-0.40.5.tar", last modified: Thu Mar 21 22:54:06 2024, max compression
+gzip compressed data, was "cmake-init-0.40.6.tar", last modified: Sat Apr 13 11:47:56 2024, max compression
```

## Comparing `cmake-init-0.40.5.tar` & `cmake-init-0.40.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 22:54:06.925502 cmake-init-0.40.5/
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-03-21 22:54:06.925502 cmake-init-0.40.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 22:54:06.925502 cmake-init-0.40.5/cmake_init.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 22:54:06.925502 cmake-init-0.40.5/cmake_init_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init_lib/cmake_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-21 22:54:06.000000 cmake-init-0.40.5/cmake_init_lib/template.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 22:54:06.925502 cmake-init-0.40.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-21 22:53:59.000000 cmake-init-0.40.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:47:56.889462 cmake-init-0.40.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-13 11:47:56.889462 cmake-init-0.40.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:47:56.889462 cmake-init-0.40.6/cmake_init.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14389 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:47:56.889462 cmake-init-0.40.6/cmake_init_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init_lib/cmake_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-13 11:47:56.000000 cmake-init-0.40.6/cmake_init_lib/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:47:56.889462 cmake-init-0.40.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-13 11:47:47.000000 cmake-init-0.40.6/setup.py
```

### Comparing `cmake-init-0.40.5/PKG-INFO` & `cmake-init-0.40.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.40.5
+Version: 0.40.6
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.40.5/cmake_init.egg-info/PKG-INFO` & `cmake-init-0.40.6/cmake_init.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmake-init
-Version: 0.40.5
+Version: 0.40.6
 Summary: The missing CMake project initializer
 Home-page: https://github.com/friendlyanon/cmake-init
 Author: friendlyanon
 Author-email: friendlyanon_@hotmail.com
 License: GPLv3+
 Description: # `cmake-init` - The missing CMake project initializer
```

### Comparing `cmake-init-0.40.5/cmake_init_lib/cmake_init.py` & `cmake-init-0.40.6/cmake_init_lib/cmake_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 import platform
 import re
 import subprocess
 import sys
 import zipfile
 
-__version__ = "0.40.5"
+__version__ = "0.40.6"
 
 is_windows = os.name == "nt"
 
 compile_template = None
 
 
 class Language:
```

### Comparing `cmake-init-0.40.5/cmake_init_lib/template.py` & `cmake-init-0.40.6/cmake_init_lib/template.py`

 * *Files identical despite different names*

### Comparing `cmake-init-0.40.5/setup.py` & `cmake-init-0.40.6/setup.py`

 * *Files identical despite different names*

