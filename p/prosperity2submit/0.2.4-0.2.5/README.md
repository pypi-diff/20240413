# Comparing `tmp/prosperity2submit-0.2.4.tar.gz` & `tmp/prosperity2submit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.4.tar", last modified: Thu Apr 11 09:12:45 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.5.tar", last modified: Sat Apr 13 14:28:44 2024, max compression
```

## Comparing `prosperity2submit-0.2.4.tar` & `prosperity2submit-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.618817 prosperity2submit-0.2.4/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-11 09:12:43.000000 prosperity2submit-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-13 14:28:40.000000 prosperity2submit-0.2.5/prosperity2submit/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:28:44.000000 prosperity2submit-0.2.5/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-13 14:28:42.000000 prosperity2submit-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:28:44.865189 prosperity2submit-0.2.5/setup.cfg
```

### Comparing `prosperity2submit-0.2.4/LICENSE` & `prosperity2submit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.4/PKG-INFO` & `prosperity2submit-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.4/README.md` & `prosperity2submit-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.4/prosperity2submit/__main__.py` & `prosperity2submit-0.2.5/prosperity2submit/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.4/prosperity2submit/core.py` & `prosperity2submit-0.2.5/prosperity2submit/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import keyring
-# This import needs to exist to prevent a 1024-character pasting limit on macOS
-# See https://stackoverflow.com/a/53871077
-import readline
 import requests
 import sys
 import time
 import webbrowser
 from collections import defaultdict
 from functools import partial
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 from pathlib import Path
 from requests_toolbelt import MultipartEncoder
 from typing import Any, Optional
 
+try:
+    # This import needs to happen to prevent a 1024-character pasting limit on macOS
+    # See https://stackoverflow.com/a/53871077
+    import readline
+except ImportError:
+    pass
+
 KEYRING_SERVICE = "prosperity2submit"
 KEYRING_USERNAME = "prosperity-id-token"
 
 API_BASE_URL = "https://bz97lt8b1e.execute-api.eu-west-1.amazonaws.com/prod"
 
 def refresh_token() -> None:
     print("""
```

### Comparing `prosperity2submit-0.2.4/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.5/prosperity2submit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.4/pyproject.toml` & `prosperity2submit-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.4"
+version = "0.2.5"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

