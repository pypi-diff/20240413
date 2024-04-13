# Comparing `tmp/restx-0.1.6.tar.gz` & `tmp/restx-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restx-0.1.6.tar", max compression
+gzip compressed data, was "restx-0.1.7.tar", max compression
```

## Comparing `restx-0.1.6.tar` & `restx-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-13 18:56:50.492130 restx-0.1.6/LICENSE
--rw-r--r--   0        0        0      259 2024-04-13 18:56:50.492130 restx-0.1.6/README.md
--rw-r--r--   0        0        0     1160 2024-04-13 18:56:50.492130 restx-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 18:56:50.492130 restx-0.1.6/restx/__init__.py
--rwxr-xr-x   0        0        0     2272 2024-04-13 18:56:50.492130 restx-0.1.6/restx/cli.py
--rw-r--r--   0        0        0      140 2024-04-13 18:56:50.492130 restx-0.1.6/restx/enums.py
--rw-r--r--   0        0        0     3153 2024-04-13 18:56:50.492130 restx-0.1.6/restx/utils.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 restx-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 19:09:05.417220 restx-0.1.7/LICENSE
+-rw-r--r--   0        0        0      259 2024-04-13 19:09:05.421220 restx-0.1.7/README.md
+-rw-r--r--   0        0        0     1160 2024-04-13 19:09:05.421220 restx-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 19:09:05.421220 restx-0.1.7/restx/__init__.py
+-rwxr-xr-x   0        0        0     2272 2024-04-13 19:09:05.421220 restx-0.1.7/restx/cli.py
+-rw-r--r--   0        0        0      140 2024-04-13 19:09:05.421220 restx-0.1.7/restx/enums.py
+-rw-r--r--   0        0        0     3153 2024-04-13 19:09:05.421220 restx-0.1.7/restx/utils.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 restx-0.1.7/PKG-INFO
```

### Comparing `restx-0.1.6/LICENSE` & `restx-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `restx-0.1.6/pyproject.toml` & `restx-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "A CLI app for performing RESTX operations via HTTP requests."
 include = [
   "LICENSE",
 ]
 license = "MIT"
 name = "restx"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 httpx = "^0.27.0"
 python = ">=3.10,<4.0"
 rich = "^13.7.1"
 typer = "^0.12.3"
```

### Comparing `restx-0.1.6/restx/cli.py` & `restx-0.1.7/restx/cli.py`

 * *Files identical despite different names*

### Comparing `restx-0.1.6/restx/utils.py` & `restx-0.1.7/restx/utils.py`

 * *Files identical despite different names*

### Comparing `restx-0.1.6/PKG-INFO` & `restx-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restx
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI app for performing RESTX operations via HTTP requests.
 License: MIT
 Author: Arjun Umathanu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

