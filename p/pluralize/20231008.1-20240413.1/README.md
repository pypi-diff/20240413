# Comparing `tmp/pluralize-20231008.1.tar.gz` & `tmp/pluralize-20240413.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralize-20231008.1.tar", last modified: Sun Nov 12 03:32:39 2023, max compression
+gzip compressed data, was "pluralize-20240413.1.tar", last modified: Sat Apr 13 17:39:06 2024, max compression
```

## Comparing `pluralize-20231008.1.tar` & `pluralize-20240413.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-12 03:32:39.547695 pluralize-20231008.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2023-11-12 03:32:39.547695 pluralize-20231008.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20231008.1/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-12 03:32:39.544361 pluralize-20231008.1/pluralize/
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)     5488 2023-11-12 03:32:21.000000 pluralize-20231008.1/pluralize/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-12 03:32:39.544361 pluralize-20231008.1/pluralize.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2023-11-12 03:32:39.000000 pluralize-20231008.1/pluralize.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2023-11-12 03:32:39.000000 pluralize-20231008.1/pluralize.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-11-12 03:32:39.000000 pluralize-20231008.1/pluralize.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2023-11-12 03:32:39.000000 pluralize-20231008.1/pluralize.egg-info/top_level.txt
--rw-rw-r--   0 mdipierro  (1000) mdipierro  (1000)      563 2023-10-08 22:00:58.000000 pluralize-20231008.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2023-11-12 03:32:39.547695 pluralize-20231008.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2023-11-12 03:32:39.544361 pluralize-20231008.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20231008.1/tests/test_simple.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.724103 pluralize-20240413.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-04-13 17:39:06.724103 pluralize-20240413.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20240413.1/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.720769 pluralize-20240413.1/pluralize/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5555 2024-04-13 07:11:53.000000 pluralize-20240413.1/pluralize/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.724103 pluralize-20240413.1/pluralize.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2024-04-13 17:39:06.000000 pluralize-20240413.1/pluralize.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      563 2024-04-13 07:10:28.000000 pluralize-20240413.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-04-13 17:39:06.724103 pluralize-20240413.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-04-13 17:39:06.720769 pluralize-20240413.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20240413.1/tests/test_simple.py
```

### Comparing `pluralize-20231008.1/PKG-INFO` & `pluralize-20240413.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20231008.1
+Version: 20240413.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20231008.1/README.md` & `pluralize-20240413.1/README.md`

 * *Files identical despite different names*

### Comparing `pluralize-20231008.1/pluralize/__init__.py` & `pluralize-20240413.1/pluralize/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import json
 import threading
 import ast
 
-__version__ = "20231008.1"
+__version__ = "20240413.1"
 
 re_language = re.compile(r"^\w\w(-\w+)*.json$")
 
 
 class lazyT(object):
 
     """accesssory object used to represent a T("string")"""
@@ -103,14 +103,16 @@
         """retuns a lazyT object"""
         if isinstance(text, lazyT):
             return text
         return lazyT(self._translator, text)
 
     def _translator(self, text, **kwargs):
         """translates/pluralizes"""
+        if not isinstance(text, str):
+            text = str(text)
         if getattr(self.local, "language", None):
             n = kwargs.get("n", 1)
             translations = self.local.language.get(text)
             if translations is None:
                 self.missing.add(text)
             elif isinstance(translations, dict) and translations:
                 k = max(int(i) for i in translations.keys() if int(i) <= n)
```

### Comparing `pluralize-20231008.1/pluralize.egg-info/PKG-INFO` & `pluralize-20240413.1/pluralize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20231008.1
+Version: 20240413.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20231008.1/pyproject.toml` & `pluralize-20240413.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluralize"
-version = "20231008.1"
+version = "20240413.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "i18n + pluralization library with multi-plural form support and thread safe for web apps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pluralize-20231008.1/tests/test_simple.py` & `pluralize-20240413.1/tests/test_simple.py`

 * *Files identical despite different names*

