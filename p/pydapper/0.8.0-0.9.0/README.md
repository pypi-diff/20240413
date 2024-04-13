# Comparing `tmp/pydapper-0.8.0.tar.gz` & `tmp/pydapper-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydapper-0.8.0.tar", max compression
+gzip compressed data, was "pydapper-0.9.0.tar", max compression
```

## Comparing `pydapper-0.8.0.tar` & `pydapper-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1126 2023-03-19 19:37:44.922223 pydapper-0.8.0/LICENSE
--rw-r--r--   0        0        0     2768 2023-03-19 19:37:44.922223 pydapper-0.8.0/README.md
--rw-r--r--   0        0        0      623 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/__init__.py
--rw-r--r--   0        0        0       65 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/bigquery/__init__.py
--rw-r--r--   0        0        0      557 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/bigquery/google_bigquery_client.py
--rw-r--r--   0        0        0    21773 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/commands.py
--rw-r--r--   0        0        0     1659 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/dsn_parser.py
--rw-r--r--   0        0        0      164 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/exceptions.py
--rw-r--r--   0        0        0     3716 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/main.py
--rw-r--r--   0        0        0       37 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/mssql/__init__.py
--rw-r--r--   0        0        0     1303 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/mssql/pymssql.py
--rw-r--r--   0        0        0       65 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/mysql/__init__.py
--rw-r--r--   0        0        0     1634 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/mysql/mysql_connector_python.py
--rw-r--r--   0        0        0       79 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/oracle/__init__.py
--rw-r--r--   0        0        0      863 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/oracle/cx_Oracle.py
--rw-r--r--   0        0        0      859 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/oracle/oracledb.py
--rw-r--r--   0        0        0       72 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/postgresql/__init__.py
--rw-r--r--   0        0        0     1526 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/postgresql/aiopg.py
--rw-r--r--   0        0        0      740 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/postgresql/psycopg2.py
--rw-r--r--   0        0        0        0 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/py.typed
--rw-r--r--   0        0        0       37 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/sqlite/__init__.py
--rw-r--r--   0        0        0      664 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/sqlite/sqlite3.py
--rw-r--r--   0        0        0     1821 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/types.py
--rw-r--r--   0        0        0     1737 2023-03-19 19:37:44.926223 pydapper-0.8.0/pydapper/utils.py
--rw-r--r--   0        0        0     3743 2023-03-19 19:37:44.926223 pydapper-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 pydapper-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-11-23 15:07:56.663939 pydapper-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2612 2023-11-23 15:07:56.663939 pydapper-0.9.0/README.md
+-rw-r--r--   0        0        0      623 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/__init__.py
+-rw-r--r--   0        0        0       65 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/bigquery/__init__.py
+-rw-r--r--   0        0        0      557 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/bigquery/google_bigquery_client.py
+-rw-r--r--   0        0        0    21811 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/commands.py
+-rw-r--r--   0        0        0     1659 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/dsn_parser.py
+-rw-r--r--   0        0        0      164 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/exceptions.py
+-rw-r--r--   0        0        0     3716 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/main.py
+-rw-r--r--   0        0        0       37 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/mssql/__init__.py
+-rw-r--r--   0        0        0     1303 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/mssql/pymssql.py
+-rw-r--r--   0        0        0       65 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/mysql/__init__.py
+-rw-r--r--   0        0        0     1634 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/mysql/mysql_connector_python.py
+-rw-r--r--   0        0        0       79 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/oracle/__init__.py
+-rw-r--r--   0        0        0      863 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/oracle/cx_Oracle.py
+-rw-r--r--   0        0        0      859 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/oracle/oracledb.py
+-rw-r--r--   0        0        0       72 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/postgresql/__init__.py
+-rw-r--r--   0        0        0     1526 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/postgresql/aiopg.py
+-rw-r--r--   0        0        0      740 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/postgresql/psycopg2.py
+-rw-r--r--   0        0        0        0 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/py.typed
+-rw-r--r--   0        0        0       37 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/sqlite/__init__.py
+-rw-r--r--   0        0        0      664 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/sqlite/sqlite3.py
+-rw-r--r--   0        0        0     1821 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/types.py
+-rw-r--r--   0        0        0     1737 2023-11-23 15:07:56.667939 pydapper-0.9.0/pydapper/utils.py
+-rw-r--r--   0        0        0     4387 2023-11-23 15:07:56.667939 pydapper-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5334 1970-01-01 00:00:00.000000 pydapper-0.9.0/PKG-INFO
```

### Comparing `pydapper-0.8.0/LICENSE` & `pydapper-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/README.md` & `pydapper-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-[![test](https://github.com/zschumacher/pydapper/actions/workflows/test.yml/badge.svg)](https://github.com/zschumacher/pydapper/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/pydapper.svg)](https://badge.fury.io/py/pydapper)
 [![Documentation Status](https://readthedocs.org/projects/pydapper/badge/?version=latest)](https://pydapper.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/zschumacher/pydapper/branch/main/graph/badge.svg?token=3X1IR81HL2)](https://codecov.io/gh/zschumacher/pydapper)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydapper)
```

### Comparing `pydapper-0.8.0/pydapper/__init__.py` & `pydapper-0.9.0/pydapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/bigquery/google_bigquery_client.py` & `pydapper-0.9.0/pydapper/bigquery/google_bigquery_client.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/commands.py` & `pydapper-0.9.0/pydapper/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 return [tuple(safe_getattr(p, name) for name in self.ordered_param_names) for p in self._param]
 
             return tuple(safe_getattr(self._param, name) for name in self.ordered_param_names)
         return tuple()
 
     @cached_property
     def prepared_sql(self) -> str:
-        if self._param:
+        if self._param and len(self.ordered_param_names) > 0:
             pattern = re.compile("|".join(re.escape(f"?{name}?") for name in self.ordered_param_names))
 
             def sub_param_with_placeholder(m: Match) -> str:
                 matched_placeholder = m.group(0)
                 matched_param_name = matched_placeholder.strip("?")
                 return self.get_param_placeholder(matched_param_name)
```

### Comparing `pydapper-0.8.0/pydapper/dsn_parser.py` & `pydapper-0.9.0/pydapper/dsn_parser.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/main.py` & `pydapper-0.9.0/pydapper/main.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/mssql/pymssql.py` & `pydapper-0.9.0/pydapper/mssql/pymssql.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/mysql/mysql_connector_python.py` & `pydapper-0.9.0/pydapper/mysql/mysql_connector_python.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/oracle/cx_Oracle.py` & `pydapper-0.9.0/pydapper/oracle/cx_Oracle.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/oracle/oracledb.py` & `pydapper-0.9.0/pydapper/oracle/oracledb.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/postgresql/aiopg.py` & `pydapper-0.9.0/pydapper/postgresql/aiopg.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/postgresql/psycopg2.py` & `pydapper-0.9.0/pydapper/postgresql/psycopg2.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/sqlite/sqlite3.py` & `pydapper-0.9.0/pydapper/sqlite/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/types.py` & `pydapper-0.9.0/pydapper/types.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pydapper/utils.py` & `pydapper-0.9.0/pydapper/utils.py`

 * *Files identical despite different names*

### Comparing `pydapper-0.8.0/pyproject.toml` & `pydapper-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydapper"
-version = "0.8.0"
+version = "0.9.0"
 description = "A pure python lib inspired by the dotnet lib dapper"
 authors = ["Zach Schumacher <zschu15@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python',
@@ -27,43 +27,43 @@
     'Topic :: Database',
     'Topic :: Database :: Database Engines/Servers'
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 dsnparse = "^0.1.15"
-psycopg2-binary = { version = "^2.9.2", optional = true }
+psycopg2-binary = { version = "^2.9.9", optional = true }
 pymssql = { version = "^2.2.6", optional = true }
 types-psycopg2 = { version = "^2.9.4", optional = true }
 types-pymssql = { version = "^2.1.0", optional = true }
 cached-property = "^1.5.2"
 mysql-connector-python = {version = "^8.0.28", optional = true}
 cx-Oracle = { version = "^8.3.0", optional = true }
 oracledb = { version = "^1.1.1", optional = true }
 aiopg = { version = "^1.3.3", optional = true }
 coro-context-manager = "^0.1.1"
-google-cloud-bigquery = {version = "^3.4.1", optional = true}
-google-cloud-bigquery-storage = {version = "^2.17.0", optional = true}
-pyarrow = {version = "^10.0.1", optional = true}
+google-cloud-bigquery = {version = "^3.11.4", optional = true}
+google-cloud-bigquery-storage = {version = "^2.22.0", optional = true}
+pyarrow = {version = "^13.0.0", optional = true}
 numpy = {version = "^1.24.2", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "*"
 coverage = "*"
 devtools = "*"
 Faker = "*"
 isort = "*"
 mypy = "*"
 pytest = "7.*.*"
-pytest-cov = "3.*.*"
+pytest-cov = "4.*.*"
 mkdocs = "1.*.*"
-mkdocs-material = "8.*.*"
+mkdocs-material = "9.*.*"
 markdown-include = "*"
 codecov = "*"
-pytest-asyncio = "^0.19.0"
+pytest-asyncio = "0.21.*"
 pytest-mock = "*"
 pytest-vcr = "^1.0.2"
 
 [tool.poetry.extras]
 psycopg2 = ["psycopg2-binary", "types-psycopg2"]
 pymssql = ["pymssql", "types-pymssql"]
 mysql-connector-python = ["mysql-connector-python"]
@@ -136,10 +136,23 @@
     "if TYPE_CHECKING:",
     "raise NotImplementedError",
     "Protocol",
     "except ImportError",
     "@abstractmethod",
     "@overload"
 ]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+norecursedirs = ["venv", ".venv"]
+markers = [
+    "bigquery: marks tests that require bigquery (deselect with '-m \"not bigquery\"')",
+    "core: marks core tests (deselect with '-m \"not core\"')",
+    "mysql: marks tests that require mysql (deselect with '-m \"not mysql\"')",
+    "oracle: marks tests that require oracle (deselect with '-m \"not oracle\"')",
+    "postgresql: marks tests that require postgres (deselect with '-m \"not postgres\"')",
+    "sqlite: marks tests that require sqlite (deselect with '-m \"not sqlite\"')",
+    "mssql: marks tests that require mssql (deselect with '-m \"not mssql\")"
+]
```

### Comparing `pydapper-0.8.0/PKG-INFO` & `pydapper-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydapper
-Version: 0.8.0
+Version: 0.9.0
 Summary: A pure python lib inspired by the dotnet lib dapper
 License: MIT
 Author: Zach Schumacher
 Author-email: zschu15@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,20 +17,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aiopg
 Provides-Extra: all
 Provides-Extra: cx-oracle
@@ -41,27 +36,26 @@
 Provides-Extra: psycopg2
 Provides-Extra: pymssql
 Requires-Dist: aiopg (>=1.3.3,<2.0.0) ; extra == "aiopg" or extra == "all"
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: coro-context-manager (>=0.1.1,<0.2.0)
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "cx-oracle" or extra == "all"
 Requires-Dist: dsnparse (>=0.1.15,<0.2.0)
-Requires-Dist: google-cloud-bigquery (>=3.4.1,<4.0.0) ; extra == "google-cloud-bigquery" or extra == "all"
-Requires-Dist: google-cloud-bigquery-storage (>=2.17.0,<3.0.0) ; extra == "google-cloud-bigquery-storage" or extra == "all"
+Requires-Dist: google-cloud-bigquery (>=3.11.4,<4.0.0) ; extra == "google-cloud-bigquery" or extra == "all"
+Requires-Dist: google-cloud-bigquery-storage (>=2.22.0,<3.0.0) ; extra == "google-cloud-bigquery-storage" or extra == "all"
 Requires-Dist: mysql-connector-python (>=8.0.28,<9.0.0) ; extra == "mysql-connector-python" or extra == "all"
 Requires-Dist: numpy (>=1.24.2,<2.0.0) ; extra == "google-cloud-bigquery-storage" or extra == "all"
 Requires-Dist: oracledb (>=1.1.1,<2.0.0) ; extra == "oracledb" or extra == "all"
-Requires-Dist: psycopg2-binary (>=2.9.2,<3.0.0) ; extra == "psycopg2"
-Requires-Dist: pyarrow (>=10.0.1,<11.0.0) ; extra == "google-cloud-bigquery-storage" or extra == "all"
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "psycopg2"
+Requires-Dist: pyarrow (>=13.0.0,<14.0.0) ; extra == "google-cloud-bigquery-storage" or extra == "all"
 Requires-Dist: pymssql (>=2.2.6,<3.0.0) ; extra == "pymssql" or extra == "all"
 Requires-Dist: types-psycopg2 (>=2.9.4,<3.0.0) ; extra == "psycopg2" or extra == "all"
 Requires-Dist: types-pymssql (>=2.1.0,<3.0.0) ; extra == "pymssql" or extra == "all"
 Description-Content-Type: text/markdown
 
-[![test](https://github.com/zschumacher/pydapper/actions/workflows/test.yml/badge.svg)](https://github.com/zschumacher/pydapper/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/pydapper.svg)](https://badge.fury.io/py/pydapper)
 [![Documentation Status](https://readthedocs.org/projects/pydapper/badge/?version=latest)](https://pydapper.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/zschumacher/pydapper/branch/main/graph/badge.svg?token=3X1IR81HL2)](https://codecov.io/gh/zschumacher/pydapper)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydapper)
```

