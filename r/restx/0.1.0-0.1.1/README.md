# Comparing `tmp/restx-0.1.0.tar.gz` & `tmp/restx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restx-0.1.0.tar", max compression
+gzip compressed data, was "restx-0.1.1.tar", max compression
```

## Comparing `restx-0.1.0.tar` & `restx-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2024-04-13 08:36:11.424182 restx-0.1.0/LICENSE
--rw-r--r--   0        0        0       83 2024-04-13 10:09:24.428188 restx-0.1.0/README.md
--rw-r--r--   0        0        0      545 2024-04-13 10:09:24.910289 restx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 08:02:36.161963 restx-0.1.0/restx/__init__.py
--rw-r--r--   0        0        0      364 2024-04-13 08:40:43.514130 restx-0.1.0/restx/cli.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 restx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 08:36:11.424182 restx-0.1.1/LICENSE
+-rw-r--r--   0        0        0       83 2024-04-13 10:09:24.428188 restx-0.1.1/README.md
+-rw-r--r--   0        0        0      592 2024-04-13 10:20:06.376250 restx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 08:02:36.161963 restx-0.1.1/restx/__init__.py
+-rw-r--r--   0        0        0      364 2024-04-13 08:40:43.514130 restx-0.1.1/restx/cli.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 restx-0.1.1/PKG-INFO
```

### Comparing `restx-0.1.0/LICENSE` & `restx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `restx-0.1.0/pyproject.toml` & `restx-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Arjun Umathanu"]
 description = "A CLI app for performing RESTX operations via HTTP requests."
 license = "MIT"
 name = "restx"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 httpx = "^0.27.0"
 python = ">=3.9,<4.0"
 rich = "^13.7.1"
 typer = "^0.12.3"
 
@@ -19,7 +19,10 @@
 pytest-mock = "^3.14.0"
 pytest-sugar = "^1.0.0"
 ruff = "^0.3.7"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
+
+[tool.poetry.scripts]
+restx = "restx.cli:app"
```

### Comparing `restx-0.1.0/PKG-INFO` & `restx-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restx
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CLI app for performing RESTX operations via HTTP requests.
 License: MIT
 Author: Arjun Umathanu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

