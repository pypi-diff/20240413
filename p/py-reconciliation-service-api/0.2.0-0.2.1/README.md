# Comparing `tmp/py_reconciliation_service_api-0.2.0.tar.gz` & `tmp/py_reconciliation_service_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_reconciliation_service_api-0.2.0.tar", max compression
+gzip compressed data, was "py_reconciliation_service_api-0.2.1.tar", max compression
```

## Comparing `py_reconciliation_service_api-0.2.0.tar` & `py_reconciliation_service_api-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1253 2024-01-12 04:46:02.882904 py_reconciliation_service_api-0.2.0/README.md
--rw-r--r--   0        0        0     3973 2024-01-12 04:02:08.393942 py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/__init__.py
--rw-r--r--   0        0        0      200 2024-01-11 06:25:30.046388 py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/models/__init__.py
--rw-r--r--   0        0        0     1267 2024-01-12 04:34:30.943186 py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/models/manifest.py
--rw-r--r--   0        0        0     1387 2024-01-12 03:02:00.675391 py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/models/reconciliation.py
--rw-r--r--   0        0        0        0 2024-01-08 20:32:36.670349 py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/py.typed
--rw-r--r--   0        0        0      959 2024-01-12 04:52:06.842764 py_reconciliation_service_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 py_reconciliation_service_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1253 2024-01-12 04:46:02.882904 py_reconciliation_service_api-0.2.1/README.md
+-rw-r--r--   0        0        0     3973 2024-01-12 04:02:08.393942 py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/__init__.py
+-rw-r--r--   0        0        0      200 2024-01-11 06:25:30.046388 py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/models/__init__.py
+-rw-r--r--   0        0        0     1267 2024-01-12 04:34:30.943186 py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/models/manifest.py
+-rw-r--r--   0        0        0     1387 2024-01-12 03:02:00.675391 py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/models/reconciliation.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:32:36.670349 py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/py.typed
+-rw-r--r--   0        0        0      957 2024-04-13 03:46:47.127221 py_reconciliation_service_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 py_reconciliation_service_api-0.2.1/PKG-INFO
```

### Comparing `py_reconciliation_service_api-0.2.0/README.md` & `py_reconciliation_service_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/__init__.py` & `py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/__init__.py`

 * *Files identical despite different names*

### Comparing `py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/models/manifest.py` & `py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/models/manifest.py`

 * *Files identical despite different names*

### Comparing `py_reconciliation_service_api-0.2.0/py_reconciliation_service_api/models/reconciliation.py` & `py_reconciliation_service_api-0.2.1/py_reconciliation_service_api/models/reconciliation.py`

 * *Files identical despite different names*

### Comparing `py_reconciliation_service_api-0.2.0/pyproject.toml` & `py_reconciliation_service_api-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-reconciliation-service-api"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for the Reconciliation Service API"
 authors = ["Daniel Erenrich <daniel@erenrich.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{ include = "py_reconciliation_service_api" }]
 
 classifiers = ["Topic :: Internet :: WWW/HTTP"]
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 Homepage = "https://github.com/derenrich/py-reconciliation-service-api"
 Repository = "https://github.com/derenrich/py-reconciliation-service-api.git"
 Issues = "https://github.com/derenrich/py-reconciliation-service-api/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^2.5.3"
+pydantic = "~2.5"
 httpx = "^0.26.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 ruff = "^0.1.11"
 pytest-asyncio = "^0.23.3"
```

### Comparing `py_reconciliation_service_api-0.2.0/PKG-INFO` & `py_reconciliation_service_api-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: py-reconciliation-service-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for the Reconciliation Service API
 License: GPL-3.0-or-later
 Keywords: reconciliation,api,client
 Author: Daniel Erenrich
 Author-email: daniel@erenrich.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: pydantic (>=2.5,<2.6)
 Project-URL: Homepage, https://github.com/derenrich/py-reconciliation-service-api
 Project-URL: Issues, https://github.com/derenrich/py-reconciliation-service-api/issues
 Project-URL: Repository, https://github.com/derenrich/py-reconciliation-service-api.git
 Description-Content-Type: text/markdown
 
 Python Reconciliation Service API
 =================================
```

