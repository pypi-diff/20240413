# Comparing `tmp/jsonapi_python-0.1.1.tar.gz` & `tmp/jsonapi_python-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonapi_python-0.1.1.tar", max compression
+gzip compressed data, was "jsonapi_python-0.1.1.post1.tar", max compression
```

## Comparing `jsonapi_python-0.1.1.tar` & `jsonapi_python-0.1.1.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-13 09:11:28.846071 jsonapi_python-0.1.1/LICENSE
--rw-r--r--   0        0        0      594 2024-04-12 14:09:23.699821 jsonapi_python-0.1.1/README.md
--rw-r--r--   0        0        0      665 2024-04-13 09:32:41.305747 jsonapi_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      403 2024-04-13 01:55:43.193899 jsonapi_python-0.1.1/src/pyjsonapi/__init__.py
--rw-r--r--   0        0        0     5491 2024-04-13 01:51:45.220274 jsonapi_python-0.1.1/src/pyjsonapi/model.py
--rw-r--r--   0        0        0     5364 2024-04-13 01:48:55.780366 jsonapi_python-0.1.1/src/pyjsonapi/relationship.py
--rw-r--r--   0        0        0     5045 2024-04-13 09:08:47.538122 jsonapi_python-0.1.1/src/pyjsonapi/session.py
--rw-r--r--   0        0        0      396 2024-04-12 11:30:57.611377 jsonapi_python-0.1.1/src/pyjsonapi/utils.py
--rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 jsonapi_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-13 09:11:28.846071 jsonapi_python-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0      594 2024-04-12 14:09:23.699821 jsonapi_python-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      796 2024-04-13 09:40:17.739081 jsonapi_python-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0      409 2024-04-13 09:40:22.515675 jsonapi_python-0.1.1.post1/src/pyjsonapi/__init__.py
+-rw-r--r--   0        0        0     5491 2024-04-13 01:51:45.220274 jsonapi_python-0.1.1.post1/src/pyjsonapi/model.py
+-rw-r--r--   0        0        0     5364 2024-04-13 01:48:55.780366 jsonapi_python-0.1.1.post1/src/pyjsonapi/relationship.py
+-rw-r--r--   0        0        0     5045 2024-04-13 09:08:47.538122 jsonapi_python-0.1.1.post1/src/pyjsonapi/session.py
+-rw-r--r--   0        0        0      396 2024-04-12 11:30:57.611377 jsonapi_python-0.1.1.post1/src/pyjsonapi/utils.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 jsonapi_python-0.1.1.post1/PKG-INFO
```

### Comparing `jsonapi_python-0.1.1/LICENSE` & `jsonapi_python-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonapi_python-0.1.1/README.md` & `jsonapi_python-0.1.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `jsonapi_python-0.1.1/pyproject.toml` & `jsonapi_python-0.1.1.post1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsonapi-python"
-version = "0.1.1"
+version = "0.1.1.post1"
 description = "Python JSON:API implementation"
 authors = ["david-why <david_why@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "pyjsonapi", from = "src" }
@@ -14,14 +14,18 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
+[project.urls]
+Homepage = "https://github.com/david-why/pyjsonapi"
+Issues = "https://github.com/david-why/pyjsonapi/issues"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 aiohttp = "^3.9.3"
 pydantic = "^2.6.4"
```

### Comparing `jsonapi_python-0.1.1/src/pyjsonapi/model.py` & `jsonapi_python-0.1.1.post1/src/pyjsonapi/model.py`

 * *Files identical despite different names*

### Comparing `jsonapi_python-0.1.1/src/pyjsonapi/relationship.py` & `jsonapi_python-0.1.1.post1/src/pyjsonapi/relationship.py`

 * *Files identical despite different names*

### Comparing `jsonapi_python-0.1.1/src/pyjsonapi/session.py` & `jsonapi_python-0.1.1.post1/src/pyjsonapi/session.py`

 * *Files identical despite different names*

### Comparing `jsonapi_python-0.1.1/PKG-INFO` & `jsonapi_python-0.1.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonapi-python
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: Python JSON:API implementation
 License: MIT
 Author: david-why
 Author-email: david_why@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

