# Comparing `tmp/pg_purepy-0.9.4.tar.gz` & `tmp/pg_purepy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_purepy-0.9.4.tar", max compression
+gzip compressed data, was "pg_purepy-0.9.5.tar", max compression
```

## Comparing `pg_purepy-0.9.4.tar` & `pg_purepy-0.9.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      423 2021-07-04 22:53:41.121324 pg_purepy-0.9.4/README.rst
--rw-r--r--   0        0        0     2203 2023-11-25 21:15:23.252256 pg_purepy-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1324 2023-11-25 21:13:14.619844 pg_purepy-0.9.4/src/pg_purepy/__init__.py
--rw-r--r--   0        0        0    20735 2023-11-25 21:21:45.382956 pg_purepy-0.9.4/src/pg_purepy/connection.py
--rw-r--r--   0        0        0     3688 2023-11-25 21:31:00.315936 pg_purepy-0.9.4/src/pg_purepy/conversion/__init__.py
--rw-r--r--   0        0        0     2981 2022-02-19 03:55:52.860474 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5639 2023-11-25 21:08:34.898609 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2985 2021-10-27 01:54:19.898864 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2332 2022-02-19 03:55:52.897140 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc
--rw-r--r--   0        0        0     3882 2023-11-19 09:21:07.134321 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-311.pyc
--rw-r--r--   0        0        0     2314 2021-10-27 11:58:23.491037 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc
--rw-r--r--   0        0        0     2165 2022-02-19 03:55:52.863807 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc
--rw-r--r--   0        0        0     2722 2023-06-09 02:41:09.098525 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-311.pyc
--rw-r--r--   0        0        0     2119 2021-07-14 19:52:47.209081 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc
--rw-r--r--   0        0        0     1071 2022-02-19 03:55:52.870473 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc
--rw-r--r--   0        0        0     2323 2023-11-19 09:21:06.970989 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-311.pyc
--rw-r--r--   0        0        0     1073 2021-10-27 01:54:19.905530 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc
--rw-r--r--   0        0        0     2121 2022-02-19 03:55:52.870473 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc
--rw-r--r--   0        0        0     2918 2023-11-19 09:21:06.970989 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2021-07-14 19:52:47.219080 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc
--rw-r--r--   0        0        0     3071 2022-02-19 03:55:52.870473 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-11-19 09:21:06.970989 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-311.pyc
--rw-r--r--   0        0        0     3044 2021-07-14 17:40:29.727817 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc
--rw-r--r--   0        0        0     3329 2022-02-19 03:55:52.873807 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc
--rw-r--r--   0        0        0     4921 2023-11-19 09:21:06.974323 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-311.pyc
--rw-r--r--   0        0        0     3248 2021-07-14 19:52:47.219080 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc
--rw-r--r--   0        0        0     2181 2022-02-19 03:55:52.893807 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc
--rw-r--r--   0        0        0     2925 2023-11-19 09:21:06.987656 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-311.pyc
--rw-r--r--   0        0        0     2107 2021-07-14 02:31:07.635634 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc
--rw-r--r--   0        0        0     1742 2022-02-19 03:55:52.893807 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc
--rw-r--r--   0        0        0     2347 2023-11-19 09:21:07.134321 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-311.pyc
--rw-r--r--   0        0        0     1676 2021-10-27 01:54:19.925530 pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc
--rw-r--r--   0        0        0     3643 2023-11-19 09:15:56.354089 pg_purepy-0.9.4/src/pg_purepy/conversion/_parse_hstore.py
--rw-r--r--   0        0        0     1567 2021-07-14 19:42:37.122921 pg_purepy-0.9.4/src/pg_purepy/conversion/abc.py
--rw-r--r--   0        0        0     3097 2023-11-19 06:32:25.813229 pg_purepy-0.9.4/src/pg_purepy/conversion/array_parse.py
--rw-r--r--   0        0        0     1410 2023-11-19 06:38:54.950061 pg_purepy-0.9.4/src/pg_purepy/conversion/arrays.py
--rw-r--r--   0        0        0     2064 2023-11-19 06:34:31.692662 pg_purepy-0.9.4/src/pg_purepy/conversion/basics.py
--rw-r--r--   0        0        0     3503 2023-11-19 06:30:04.340493 pg_purepy-0.9.4/src/pg_purepy/conversion/dt.py
--rw-r--r--   0        0        0     1853 2023-11-19 06:33:04.569723 pg_purepy-0.9.4/src/pg_purepy/conversion/enums.py
--rw-r--r--   0        0        0     1162 2023-11-19 09:19:57.748319 pg_purepy-0.9.4/src/pg_purepy/conversion/hstore.py
--rw-r--r--   0        0        0     4749 2023-11-24 19:57:31.435541 pg_purepy-0.9.4/src/pg_purepy/dbapi.py
--rw-r--r--   0        0        0     1363 2023-11-24 19:57:38.768827 pg_purepy-0.9.4/src/pg_purepy/exc.py
--rw-r--r--   0        0        0    10793 2023-11-19 09:38:36.515179 pg_purepy-0.9.4/src/pg_purepy/messages.py
--rw-r--r--   0        0        0    15362 2023-11-24 19:57:31.435541 pg_purepy-0.9.4/src/pg_purepy/pool.py
--rw-r--r--   0        0        0    47722 2023-11-25 21:31:05.182571 pg_purepy-0.9.4/src/pg_purepy/protocol.py
--rw-r--r--   0        0        0        0 2023-11-18 19:05:39.950450 pg_purepy-0.9.4/src/pg_purepy/py.typed
--rw-r--r--   0        0        0     3032 2023-11-24 19:58:26.408515 pg_purepy-0.9.4/src/pg_purepy/util.py
--rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 pg_purepy-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      423 2021-07-04 22:53:41.121324 pg_purepy-0.9.5/README.rst
+-rw-r--r--   0        0        0     2226 2023-12-20 23:52:18.764415 pg_purepy-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     1364 2023-12-20 23:48:16.679236 pg_purepy-0.9.5/src/pg_purepy/__init__.py
+-rw-r--r--   0        0        0    20834 2023-12-20 23:45:48.563484 pg_purepy-0.9.5/src/pg_purepy/connection.py
+-rw-r--r--   0        0        0     3688 2023-11-25 21:31:00.315936 pg_purepy-0.9.5/src/pg_purepy/conversion/__init__.py
+-rw-r--r--   0        0        0     2981 2022-02-19 03:55:52.860474 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5760 2023-12-20 23:43:57.997502 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2985 2021-10-27 01:54:19.898864 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2332 2022-02-19 03:55:52.897140 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc
+-rw-r--r--   0        0        0     3882 2023-11-19 09:21:07.134321 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-311.pyc
+-rw-r--r--   0        0        0     2314 2021-10-27 11:58:23.491037 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc
+-rw-r--r--   0        0        0     2165 2022-02-19 03:55:52.863807 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc
+-rw-r--r--   0        0        0     2722 2023-06-09 02:41:09.098525 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-311.pyc
+-rw-r--r--   0        0        0     2119 2021-07-14 19:52:47.209081 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc
+-rw-r--r--   0        0        0     1071 2022-02-19 03:55:52.870473 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc
+-rw-r--r--   0        0        0     2323 2023-11-19 09:21:06.970989 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-311.pyc
+-rw-r--r--   0        0        0     1073 2021-10-27 01:54:19.905530 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc
+-rw-r--r--   0        0        0     2121 2022-02-19 03:55:52.870473 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc
+-rw-r--r--   0        0        0     2918 2023-11-19 09:21:06.970989 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2021-07-14 19:52:47.219080 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc
+-rw-r--r--   0        0        0     3071 2022-02-19 03:55:52.870473 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-11-19 09:21:06.970989 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-311.pyc
+-rw-r--r--   0        0        0     3044 2021-07-14 17:40:29.727817 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc
+-rw-r--r--   0        0        0     3329 2022-02-19 03:55:52.873807 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc
+-rw-r--r--   0        0        0     4921 2023-11-19 09:21:06.974323 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-311.pyc
+-rw-r--r--   0        0        0     3248 2021-07-14 19:52:47.219080 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc
+-rw-r--r--   0        0        0     2181 2022-02-19 03:55:52.893807 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc
+-rw-r--r--   0        0        0     2925 2023-11-19 09:21:06.987656 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-311.pyc
+-rw-r--r--   0        0        0     2107 2021-07-14 02:31:07.635634 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc
+-rw-r--r--   0        0        0     1742 2022-02-19 03:55:52.893807 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc
+-rw-r--r--   0        0        0     2347 2023-11-19 09:21:07.134321 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2021-10-27 01:54:19.925530 pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc
+-rw-r--r--   0        0        0     3643 2023-11-19 09:15:56.354089 pg_purepy-0.9.5/src/pg_purepy/conversion/_parse_hstore.py
+-rw-r--r--   0        0        0     1567 2021-07-14 19:42:37.122921 pg_purepy-0.9.5/src/pg_purepy/conversion/abc.py
+-rw-r--r--   0        0        0     3097 2023-11-19 06:32:25.813229 pg_purepy-0.9.5/src/pg_purepy/conversion/array_parse.py
+-rw-r--r--   0        0        0     1410 2023-11-19 06:38:54.950061 pg_purepy-0.9.5/src/pg_purepy/conversion/arrays.py
+-rw-r--r--   0        0        0     2064 2023-11-19 06:34:31.692662 pg_purepy-0.9.5/src/pg_purepy/conversion/basics.py
+-rw-r--r--   0        0        0     3503 2023-11-19 06:30:04.340493 pg_purepy-0.9.5/src/pg_purepy/conversion/dt.py
+-rw-r--r--   0        0        0     1853 2023-11-19 06:33:04.569723 pg_purepy-0.9.5/src/pg_purepy/conversion/enums.py
+-rw-r--r--   0        0        0     1162 2023-11-19 09:19:57.748319 pg_purepy-0.9.5/src/pg_purepy/conversion/hstore.py
+-rw-r--r--   0        0        0     4749 2023-11-24 19:57:31.435541 pg_purepy-0.9.5/src/pg_purepy/dbapi.py
+-rw-r--r--   0        0        0     1481 2023-12-20 23:45:41.070197 pg_purepy-0.9.5/src/pg_purepy/exc.py
+-rw-r--r--   0        0        0    10793 2023-11-19 09:38:36.515179 pg_purepy-0.9.5/src/pg_purepy/messages.py
+-rw-r--r--   0        0        0    15355 2023-12-20 23:46:03.490058 pg_purepy-0.9.5/src/pg_purepy/pool.py
+-rw-r--r--   0        0        0    47723 2023-12-20 23:51:27.781395 pg_purepy-0.9.5/src/pg_purepy/protocol.py
+-rw-r--r--   0        0        0        0 2023-11-18 19:05:39.950450 pg_purepy-0.9.5/src/pg_purepy/py.typed
+-rw-r--r--   0        0        0     3032 2023-11-24 19:58:26.408515 pg_purepy-0.9.5/src/pg_purepy/util.py
+-rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 pg_purepy-0.9.5/PKG-INFO
```

### Comparing `pg_purepy-0.9.4/pyproject.toml` & `pg_purepy-0.9.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pg-purepy"
-version = "0.9.4"
+version = "0.9.5"
 description = "A pure-Python anyio-based PostgreSQL adapter."
 authors = ["Lura Skye <l@veriny.tf>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Database",
     "Topic :: Database :: Front-Ends",
@@ -28,17 +28,18 @@
 sphinxcontrib-jquery = ">=4.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3"
 trio = ">=0.23.1"
 isort = ">=5.12.0"
 pytest-cov = ">=4.1.0"
-mypy = ">=1.7.0"
-ruff = ">=0.1.6"
-ujson = "^5.8.0"
+mypy = ">=1.7.1"
+ruff = ">=0.1.8"
+ujson = ">=5.8.0"
+pyright = ">=1.1.342"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinxcontrib-trio", "sphinx-autodoc-typehints", "sphinx-rtd-theme",
     "sphinx-inline-tabs"]
 
 [tool.pytest.ini_options]
 log_cli_level = "5"
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/__init__.py` & `pg_purepy-0.9.5/src/pg_purepy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     PostgresqlError as PostgresqlError,
     ConnectionForciblyKilledError as ConnectionForciblyKilledError,
     ProtocolParseError as ProtocolParseError,
     MissingPasswordError as MissingPasswordError,
     UnknownMessageError as UnknownMessageError,
     IllegalStateError as IllegalStateError,
     ConnectionInTransactionWarning as ConnectionInTransactionWarning,
+    MissingRowError as MissingRowError,
 )
 from pg_purepy.messages import (
     ErrorOrNoticeResponse as ErrorOrNoticeResponse,
     ErrorResponseFieldType as ErrorResponseFieldType,
     RowDescription as RowDescription,
     ColumnDescription as ColumnDescription,
     UnrecoverableDatabaseError as UnrecoverableDatabaseError,
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/connection.py` & `pg_purepy-0.9.5/src/pg_purepy/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import anyio
 from anyio import EndOfStream, Lock
 from anyio.abc import ByteStream, SocketStream
 from anyio.streams.tls import TLSStream
 
 from pg_purepy.conversion.abc import Converter
 from pg_purepy.dbapi import convert_paramstyle
-from pg_purepy.exc import IllegalStateError, PostgresqlError
+from pg_purepy.exc import IllegalStateError, MissingRowError, PostgresqlError
 from pg_purepy.messages import (
     BackendKeyData,
     BaseDatabaseError,
     BindComplete,
     CommandComplete,
     DataRow,
     ErrorOrNoticeResponse,
@@ -425,25 +425,27 @@
             return [i async for i in q]
 
     async def fetch_one(
         self,
         query: str | PreparedStatementInfo,
         *params: Any,
         **kwargs: Any,
-    ) -> DataRow | None:
+    ) -> DataRow:
         """
         Like :meth:`.fetch`, but only fetches one row.
+
+        :raises MissingRowError: If there's no row in the result.
         """
 
         row = await self.fetch(query, *params, **kwargs)
 
         try:
             return row[0]
         except IndexError:
-            return None
+            raise MissingRowError() from None
 
     async def execute(
         self,
         query: str | PreparedStatementInfo,
         *params: Any,
         max_rows: int | None = None,
         **kwargs: Any,
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__init__.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,36 @@
 magic:    0xa70d0d0a
-moddate:  0xe4616265 (Sat Nov 25 21:06:44 2023 UTC)
-files sz: 3619
+moddate:  0x94676265 (Sat Nov 25 21:31:00 2023 UTC)
+files sz: 3688
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
-      046c046d055a050100640164056c066d075a0701000900640164066c086d
-      095a0a6d0b5a0c01006e132300650d2400720b0100640164066c0e6d095a
-      0a6d0b5a0c010059006e047700780359007701640164076c0f6d105a1001
-      00640164086c116d125a120100640164096c136d145a146d155a156d165a
-      166d175a1701006401640a6c186d195a196d1a5a1a6d1b5a1b6d1c5a1c6d
-      1d5a1d6d1e5a1e6d1f5a1f01006401640b6c206d215a2101006507720664
-      01640c6c226d235a230100640d640e9c01642b641784065a2464185a2564
-      19840065254400a6000000ab0000000000000000005a26641a5a27020065
-      2465276526a6020000ab0200000000000000005a28641b5a29641c840065
-      294400a6000000ab0000000000000000005a2a641d5a2b02006524652b65
-      2a641eac0ea6030000ab0300000000000000005a2c641f5a2d6420840065
-      2d4400a6000000ab0000000000000000005a2e64215a2f02006524652f65
-      2ea6020000ab0200000000000000005a3064225a316423840065314400a6
-      000000ab0000000000000000005a3264245a330200652465336532a60200
-      00ab0200000000000000005a3402006514a6000000ab0000000000000000
-      005a350200651264256535a6020000ab0200000000000000005a36020065
-      15a6000000ab0000000000000000005a37642c642984045a38642a5a3964
-      035300
+      046c046d055a050100640164056c066d075a070100640164066c086d095a
+      0901000900640164076c0a6d0b5a0b6d0c5a0d010002006507650b6408ac
+      09a6020000ab0200000000000000005a0e6e132300650f2400720b010064
+      0164076c106d0b5a0e6d0c5a0d010059006e047700780359007701640164
+      0a6c116d125a1201006401640b6c136d145a1401006401640c6c156d165a
+      166d175a176d185a186d195a1901006401640d6c1a6d1b5a1b6d1c5a1c6d
+      1d5a1d6d1e5a1e6d1f5a1f6d205a206d215a2101006401640e6c226d235a
+      230100650972066401640f6c246d255a250100640864109c01642d641984
+      065a26641a5a27641b840065274400a6000000ab0000000000000000005a
+      28641c5a290200652665296528a6020000ab0200000000000000005a2a64
+      1d5a2b641e8400652b4400a6000000ab0000000000000000005a2c641f5a
+      2d02006526652d652c6420ac10a6030000ab0300000000000000005a2e64
+      215a2f64228400652f4400a6000000ab0000000000000000005a3064235a
+      310200652665316530a6020000ab0200000000000000005a3264245a3364
+      25840065334400a6000000ab0000000000000000005a3464265a35020065
+      2665356534a6020000ab0200000000000000005a3602006516a6000000ab
+      0000000000000000005a370200651464276537a6020000ab020000000000
+      0000005a3802006517a6000000ab0000000000000000005a39642e642b84
+      045a3a642c5a3b64035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nPackage containing the converterss for Python types to PostgreSQL types.\n')
                  4 STORE_NAME               0 (__doc__)
    
      5           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('annotations',))
@@ -47,264 +48,282 @@
                 28 LOAD_CONST               4 (('Sequence',))
                 30 IMPORT_NAME              4 (collections.abc)
                 32 IMPORT_FROM              5 (Sequence)
                 34 STORE_NAME               5 (Sequence)
                 36 POP_TOP
    
      9          38 LOAD_CONST               1 (0)
-                40 LOAD_CONST               5 (('TYPE_CHECKING',))
-                42 IMPORT_NAME              6 (typing)
-                44 IMPORT_FROM              7 (TYPE_CHECKING)
-                46 STORE_NAME               7 (TYPE_CHECKING)
+                40 LOAD_CONST               5 (('partial',))
+                42 IMPORT_NAME              6 (functools)
+                44 IMPORT_FROM              7 (partial)
+                46 STORE_NAME               7 (partial)
                 48 POP_TOP
    
-    11          50 NOP
-   
-    12          52 LOAD_CONST               1 (0)
-                54 LOAD_CONST               6 (('loads', 'dumps'))
-                56 IMPORT_NAME              8 (ujson)
-                58 IMPORT_FROM              9 (loads)
-                60 STORE_NAME              10 (json_loads)
-                62 IMPORT_FROM             11 (dumps)
-                64 STORE_NAME              12 (json_dumps)
-                66 POP_TOP
-                68 JUMP_FORWARD            19 (to 108)
-           >>   70 PUSH_EXC_INFO
-   
-    13          72 LOAD_NAME               13 (ModuleNotFoundError)
-                74 CHECK_EXC_MATCH
-                76 POP_JUMP_FORWARD_IF_FALSE    11 (to 100)
+    10          50 LOAD_CONST               1 (0)
+                52 LOAD_CONST               6 (('TYPE_CHECKING',))
+                54 IMPORT_NAME              8 (typing)
+                56 IMPORT_FROM              9 (TYPE_CHECKING)
+                58 STORE_NAME               9 (TYPE_CHECKING)
+                60 POP_TOP
+   
+    12          62 NOP
+   
+    13          64 LOAD_CONST               1 (0)
+                66 LOAD_CONST               7 (('dumps', 'loads'))
+                68 IMPORT_NAME             10 (ujson)
+                70 IMPORT_FROM             11 (dumps)
+                72 STORE_NAME              11 (dumps)
+                74 IMPORT_FROM             12 (loads)
+                76 STORE_NAME              13 (json_loads)
                 78 POP_TOP
    
-    14          80 LOAD_CONST               1 (0)
-                82 LOAD_CONST               6 (('loads', 'dumps'))
-                84 IMPORT_NAME             14 (json)
-                86 IMPORT_FROM              9 (loads)
-                88 STORE_NAME              10 (json_loads)
-                90 IMPORT_FROM             11 (dumps)
-                92 STORE_NAME              12 (json_dumps)
-                94 POP_TOP
-                96 POP_EXCEPT
-                98 JUMP_FORWARD             4 (to 108)
-   
-    13     >>  100 RERAISE                  0
-           >>  102 COPY                     3
-               104 POP_EXCEPT
-               106 RERAISE                  1
-   
-    17     >>  108 LOAD_CONST               1 (0)
-               110 LOAD_CONST               7 (('Converter',))
-               112 IMPORT_NAME             15 (pg_purepy.conversion.abc)
-               114 IMPORT_FROM             16 (Converter)
-               116 STORE_NAME              16 (Converter)
-               118 POP_TOP
-   
-    18         120 LOAD_CONST               1 (0)
-               122 LOAD_CONST               8 (('ArrayConverter',))
-               124 IMPORT_NAME             17 (pg_purepy.conversion.arrays)
-               126 IMPORT_FROM             18 (ArrayConverter)
-               128 STORE_NAME              18 (ArrayConverter)
-               130 POP_TOP
-   
-    19         132 LOAD_CONST               1 (0)
-               134 LOAD_CONST               9 (('BoolConverter', 'ByteaConverter', 'SimpleFunctionConverter', 'TextConverter'))
-               136 IMPORT_NAME             19 (pg_purepy.conversion.basics)
-               138 IMPORT_FROM             20 (BoolConverter)
-               140 STORE_NAME              20 (BoolConverter)
-               142 IMPORT_FROM             21 (ByteaConverter)
-               144 STORE_NAME              21 (ByteaConverter)
-               146 IMPORT_FROM             22 (SimpleFunctionConverter)
-               148 STORE_NAME              22 (SimpleFunctionConverter)
-               150 IMPORT_FROM             23 (TextConverter)
-               152 STORE_NAME              23 (TextConverter)
-               154 POP_TOP
-   
-    25         156 LOAD_CONST               1 (0)
-               158 LOAD_CONST              10 (('STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER'))
-               160 IMPORT_NAME             24 (pg_purepy.conversion.dt)
-               162 IMPORT_FROM             25 (STATIC_DATE_CONVERTER)
-               164 STORE_NAME              25 (STATIC_DATE_CONVERTER)
-               166 IMPORT_FROM             26 (STATIC_DATEA_CONVERTER)
-               168 STORE_NAME              26 (STATIC_DATEA_CONVERTER)
-               170 IMPORT_FROM             27 (STATIC_TIME_CONVERTER)
-               172 STORE_NAME              27 (STATIC_TIME_CONVERTER)
-               174 IMPORT_FROM             28 (STATIC_TIMESTAMPNOTZ_CONVERTER)
-               176 STORE_NAME              28 (STATIC_TIMESTAMPNOTZ_CONVERTER)
-               178 IMPORT_FROM             29 (STATIC_TIMESTAMPNOTZA_CONVERTER)
-               180 STORE_NAME              29 (STATIC_TIMESTAMPNOTZA_CONVERTER)
-               182 IMPORT_FROM             30 (STATIC_TIMESTAMPTZ_CONVERTER)
-               184 STORE_NAME              30 (STATIC_TIMESTAMPTZ_CONVERTER)
-               186 IMPORT_FROM             31 (STATIC_TIMESTAMPTZA_CONVERTER)
-               188 STORE_NAME              31 (STATIC_TIMESTAMPTZA_CONVERTER)
-               190 POP_TOP
-   
-    34         192 LOAD_CONST               1 (0)
-               194 LOAD_CONST              11 (('EnumConverter',))
-               196 IMPORT_NAME             32 (pg_purepy.conversion.enums)
-               198 IMPORT_FROM             33 (EnumConverter)
-               200 STORE_NAME              33 (EnumConverter)
-               202 POP_TOP
-   
-    36         204 LOAD_NAME                7 (TYPE_CHECKING)
-               206 POP_JUMP_FORWARD_IF_FALSE     6 (to 220)
-   
-    37         208 LOAD_CONST               1 (0)
-               210 LOAD_CONST              12 (('SansIOClient',))
-               212 IMPORT_NAME             34 (pg_purepy.protocol)
-               214 IMPORT_FROM             35 (SansIOClient)
-               216 STORE_NAME              35 (SansIOClient)
-               218 POP_TOP
-   
-    44     >>  220 LOAD_CONST              13 (False)
-   
-    40         222 LOAD_CONST              14 (('quote_inner',))
-               224 BUILD_CONST_KEY_MAP      1
-               226 LOAD_CONST              43 (('oids', 'Sequence[int]', 'cvs', 'Sequence[Converter]', 'quote_inner', 'bool', 'return', 'list[Converter]'))
-               228 LOAD_CONST              23 (<code object _make_array_converters, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 40>)
-               230 MAKE_FUNCTION            6 (kwdefaults, annotations)
-               232 STORE_NAME              36 (_make_array_converters)
-   
-    52         234 LOAD_CONST              24 ((20, 21, 23, 26, 27, 28, 29))
-               236 STORE_NAME              37 (KNOWN_INT_OIDS)
-   
-    53         238 LOAD_CONST              25 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 53>)
-               240 MAKE_FUNCTION            0
-               242 LOAD_NAME               37 (KNOWN_INT_OIDS)
-               244 GET_ITER
-               246 PRECALL                  0
-               250 CALL                     0
-               260 STORE_NAME              38 (INT_CONVERTERS)
-   
-    54         262 LOAD_CONST              26 ((1016, 1005, 1007, 1028, 1010, 1011, 1012))
-               264 STORE_NAME              39 (KNOWN_INTA_OIDS)
-   
-    55         266 PUSH_NULL
-               268 LOAD_NAME               36 (_make_array_converters)
-               270 LOAD_NAME               39 (KNOWN_INTA_OIDS)
-               272 LOAD_NAME               38 (INT_CONVERTERS)
-               274 PRECALL                  2
-               278 CALL                     2
-               288 STORE_NAME              40 (INTA_CONVERTERS)
-   
-    57         290 LOAD_CONST              27 ((18, 19, 25))
-               292 STORE_NAME              41 (KNOWN_TEXT_OIDS)
-   
-    58         294 LOAD_CONST              28 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 58>)
-               296 MAKE_FUNCTION            0
-               298 LOAD_NAME               41 (KNOWN_TEXT_OIDS)
-               300 GET_ITER
-               302 PRECALL                  0
-               306 CALL                     0
-               316 STORE_NAME              42 (STR_CONVERTERS)
-   
-    59         318 LOAD_CONST              29 ((1009, 1002, 1003))
-               320 STORE_NAME              43 (KNOWN_STRA_OIDS)
-   
-    60         322 PUSH_NULL
-               324 LOAD_NAME               36 (_make_array_converters)
-               326 LOAD_NAME               43 (KNOWN_STRA_OIDS)
-               328 LOAD_NAME               42 (STR_CONVERTERS)
-               330 LOAD_CONST              30 (True)
-               332 KW_NAMES                14
-               334 PRECALL                  3
-               338 CALL                     3
-               348 STORE_NAME              44 (STRA_CONVERTERS)
-   
-    62         350 LOAD_CONST              31 ((700, 701))
-               352 STORE_NAME              45 (KNOWN_FLOAT_OIDS)
-   
-    63         354 LOAD_CONST              32 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 63>)
-               356 MAKE_FUNCTION            0
-               358 LOAD_NAME               45 (KNOWN_FLOAT_OIDS)
-               360 GET_ITER
-               362 PRECALL                  0
-               366 CALL                     0
-               376 STORE_NAME              46 (FLOAT_CONVERTERS)
-   
-    64         378 LOAD_CONST              33 ((1021, 1022))
-               380 STORE_NAME              47 (KNOWN_FLOATA_OIDS)
-   
-    65         382 PUSH_NULL
-               384 LOAD_NAME               36 (_make_array_converters)
-               386 LOAD_NAME               47 (KNOWN_FLOATA_OIDS)
-               388 LOAD_NAME               46 (FLOAT_CONVERTERS)
-               390 PRECALL                  2
-               394 CALL                     2
-               404 STORE_NAME              48 (FLOATA_CONVERTERS)
-   
-    67         406 LOAD_CONST              34 ((114, 3802))
-               408 STORE_NAME              49 (KNOWN_JSON_OIDS)
-   
-    68         410 LOAD_CONST              35 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 68>)
-               412 MAKE_FUNCTION            0
-               414 LOAD_NAME               49 (KNOWN_JSON_OIDS)
-               416 GET_ITER
-               418 PRECALL                  0
-               422 CALL                     0
-               432 STORE_NAME              50 (JSON_CONVERTERS)
-   
-    69         434 LOAD_CONST              36 ((199, 3807))
-               436 STORE_NAME              51 (KNOWN_JSONA_OIDS)
-   
-    70         438 PUSH_NULL
-               440 LOAD_NAME               36 (_make_array_converters)
-               442 LOAD_NAME               51 (KNOWN_JSONA_OIDS)
-               444 LOAD_NAME               50 (JSON_CONVERTERS)
-               446 PRECALL                  2
-               450 CALL                     2
-               460 STORE_NAME              52 (JSONA_CONVERTERS)
-   
-    72         462 PUSH_NULL
-               464 LOAD_NAME               20 (BoolConverter)
-               466 PRECALL                  0
-               470 CALL                     0
-               480 STORE_NAME              53 (STATIC_BOOLEAN_CONVERTER)
-   
-    73         482 PUSH_NULL
-               484 LOAD_NAME               18 (ArrayConverter)
-               486 LOAD_CONST              37 (1000)
-               488 LOAD_NAME               53 (STATIC_BOOLEAN_CONVERTER)
-               490 PRECALL                  2
-               494 CALL                     2
-               504 STORE_NAME              54 (STATIC_BOOLEANA_CONVERTER)
-   
-    74         506 PUSH_NULL
-               508 LOAD_NAME               21 (ByteaConverter)
-               510 PRECALL                  0
-               514 CALL                     0
-               524 STORE_NAME              55 (STATIC_BYTES_CONVERTER)
-   
-    77         526 LOAD_CONST              44 (('protocol', 'SansIOClient', 'return', 'None'))
-               528 LOAD_CONST              41 (<code object apply_default_converters, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 77>)
-               530 MAKE_FUNCTION            4 (annotations)
-               532 STORE_NAME              56 (apply_default_converters)
-   
-   111         534 LOAD_CONST              42 (('Converter', 'apply_default_converters', 'EnumConverter', 'ArrayConverter'))
-               536 STORE_NAME              57 (__all__)
-               538 LOAD_CONST               3 (None)
-               540 RETURN_VALUE
+    15          80 PUSH_NULL
+                82 LOAD_NAME                7 (partial)
+                84 LOAD_NAME               11 (dumps)
+                86 LOAD_CONST               8 (False)
+                88 KW_NAMES                 9
+                90 PRECALL                  2
+                94 CALL                     2
+               104 STORE_NAME              14 (json_dumps)
+               106 JUMP_FORWARD            19 (to 146)
+           >>  108 PUSH_EXC_INFO
+   
+    16         110 LOAD_NAME               15 (ModuleNotFoundError)
+               112 CHECK_EXC_MATCH
+               114 POP_JUMP_FORWARD_IF_FALSE    11 (to 138)
+               116 POP_TOP
+   
+    17         118 LOAD_CONST               1 (0)
+               120 LOAD_CONST               7 (('dumps', 'loads'))
+               122 IMPORT_NAME             16 (json)
+               124 IMPORT_FROM             11 (dumps)
+               126 STORE_NAME              14 (json_dumps)
+               128 IMPORT_FROM             12 (loads)
+               130 STORE_NAME              13 (json_loads)
+               132 POP_TOP
+               134 POP_EXCEPT
+               136 JUMP_FORWARD             4 (to 146)
+   
+    16     >>  138 RERAISE                  0
+           >>  140 COPY                     3
+               142 POP_EXCEPT
+               144 RERAISE                  1
+   
+    20     >>  146 LOAD_CONST               1 (0)
+               148 LOAD_CONST              10 (('Converter',))
+               150 IMPORT_NAME             17 (pg_purepy.conversion.abc)
+               152 IMPORT_FROM             18 (Converter)
+               154 STORE_NAME              18 (Converter)
+               156 POP_TOP
+   
+    21         158 LOAD_CONST               1 (0)
+               160 LOAD_CONST              11 (('ArrayConverter',))
+               162 IMPORT_NAME             19 (pg_purepy.conversion.arrays)
+               164 IMPORT_FROM             20 (ArrayConverter)
+               166 STORE_NAME              20 (ArrayConverter)
+               168 POP_TOP
+   
+    22         170 LOAD_CONST               1 (0)
+               172 LOAD_CONST              12 (('BoolConverter', 'ByteaConverter', 'SimpleFunctionConverter', 'TextConverter'))
+               174 IMPORT_NAME             21 (pg_purepy.conversion.basics)
+               176 IMPORT_FROM             22 (BoolConverter)
+               178 STORE_NAME              22 (BoolConverter)
+               180 IMPORT_FROM             23 (ByteaConverter)
+               182 STORE_NAME              23 (ByteaConverter)
+               184 IMPORT_FROM             24 (SimpleFunctionConverter)
+               186 STORE_NAME              24 (SimpleFunctionConverter)
+               188 IMPORT_FROM             25 (TextConverter)
+               190 STORE_NAME              25 (TextConverter)
+               192 POP_TOP
+   
+    28         194 LOAD_CONST               1 (0)
+               196 LOAD_CONST              13 (('STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER'))
+               198 IMPORT_NAME             26 (pg_purepy.conversion.dt)
+               200 IMPORT_FROM             27 (STATIC_DATE_CONVERTER)
+               202 STORE_NAME              27 (STATIC_DATE_CONVERTER)
+               204 IMPORT_FROM             28 (STATIC_DATEA_CONVERTER)
+               206 STORE_NAME              28 (STATIC_DATEA_CONVERTER)
+               208 IMPORT_FROM             29 (STATIC_TIME_CONVERTER)
+               210 STORE_NAME              29 (STATIC_TIME_CONVERTER)
+               212 IMPORT_FROM             30 (STATIC_TIMESTAMPNOTZ_CONVERTER)
+               214 STORE_NAME              30 (STATIC_TIMESTAMPNOTZ_CONVERTER)
+               216 IMPORT_FROM             31 (STATIC_TIMESTAMPNOTZA_CONVERTER)
+               218 STORE_NAME              31 (STATIC_TIMESTAMPNOTZA_CONVERTER)
+               220 IMPORT_FROM             32 (STATIC_TIMESTAMPTZ_CONVERTER)
+               222 STORE_NAME              32 (STATIC_TIMESTAMPTZ_CONVERTER)
+               224 IMPORT_FROM             33 (STATIC_TIMESTAMPTZA_CONVERTER)
+               226 STORE_NAME              33 (STATIC_TIMESTAMPTZA_CONVERTER)
+               228 POP_TOP
+   
+    37         230 LOAD_CONST               1 (0)
+               232 LOAD_CONST              14 (('EnumConverter',))
+               234 IMPORT_NAME             34 (pg_purepy.conversion.enums)
+               236 IMPORT_FROM             35 (EnumConverter)
+               238 STORE_NAME              35 (EnumConverter)
+               240 POP_TOP
+   
+    39         242 LOAD_NAME                9 (TYPE_CHECKING)
+               244 POP_JUMP_FORWARD_IF_FALSE     6 (to 258)
+   
+    40         246 LOAD_CONST               1 (0)
+               248 LOAD_CONST              15 (('SansIOClient',))
+               250 IMPORT_NAME             36 (pg_purepy.protocol)
+               252 IMPORT_FROM             37 (SansIOClient)
+               254 STORE_NAME              37 (SansIOClient)
+               256 POP_TOP
+   
+    47     >>  258 LOAD_CONST               8 (False)
+   
+    43         260 LOAD_CONST              16 (('quote_inner',))
+               262 BUILD_CONST_KEY_MAP      1
+               264 LOAD_CONST              45 (('oids', 'Sequence[int]', 'cvs', 'Sequence[Converter]', 'quote_inner', 'bool', 'return', 'list[Converter]'))
+               266 LOAD_CONST              25 (<code object _make_array_converters, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 43>)
+               268 MAKE_FUNCTION            6 (kwdefaults, annotations)
+               270 STORE_NAME              38 (_make_array_converters)
+   
+    55         272 LOAD_CONST              26 ((20, 21, 23, 26, 27, 28, 29))
+               274 STORE_NAME              39 (KNOWN_INT_OIDS)
+   
+    56         276 LOAD_CONST              27 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 56>)
+               278 MAKE_FUNCTION            0
+               280 LOAD_NAME               39 (KNOWN_INT_OIDS)
+               282 GET_ITER
+               284 PRECALL                  0
+               288 CALL                     0
+               298 STORE_NAME              40 (INT_CONVERTERS)
+   
+    57         300 LOAD_CONST              28 ((1016, 1005, 1007, 1028, 1010, 1011, 1012))
+               302 STORE_NAME              41 (KNOWN_INTA_OIDS)
+   
+    58         304 PUSH_NULL
+               306 LOAD_NAME               38 (_make_array_converters)
+               308 LOAD_NAME               41 (KNOWN_INTA_OIDS)
+               310 LOAD_NAME               40 (INT_CONVERTERS)
+               312 PRECALL                  2
+               316 CALL                     2
+               326 STORE_NAME              42 (INTA_CONVERTERS)
+   
+    60         328 LOAD_CONST              29 ((18, 19, 25))
+               330 STORE_NAME              43 (KNOWN_TEXT_OIDS)
+   
+    61         332 LOAD_CONST              30 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 61>)
+               334 MAKE_FUNCTION            0
+               336 LOAD_NAME               43 (KNOWN_TEXT_OIDS)
+               338 GET_ITER
+               340 PRECALL                  0
+               344 CALL                     0
+               354 STORE_NAME              44 (STR_CONVERTERS)
+   
+    62         356 LOAD_CONST              31 ((1009, 1002, 1003))
+               358 STORE_NAME              45 (KNOWN_STRA_OIDS)
+   
+    63         360 PUSH_NULL
+               362 LOAD_NAME               38 (_make_array_converters)
+               364 LOAD_NAME               45 (KNOWN_STRA_OIDS)
+               366 LOAD_NAME               44 (STR_CONVERTERS)
+               368 LOAD_CONST              32 (True)
+               370 KW_NAMES                16
+               372 PRECALL                  3
+               376 CALL                     3
+               386 STORE_NAME              46 (STRA_CONVERTERS)
+   
+    65         388 LOAD_CONST              33 ((700, 701))
+               390 STORE_NAME              47 (KNOWN_FLOAT_OIDS)
+   
+    66         392 LOAD_CONST              34 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 66>)
+               394 MAKE_FUNCTION            0
+               396 LOAD_NAME               47 (KNOWN_FLOAT_OIDS)
+               398 GET_ITER
+               400 PRECALL                  0
+               404 CALL                     0
+               414 STORE_NAME              48 (FLOAT_CONVERTERS)
+   
+    67         416 LOAD_CONST              35 ((1021, 1022))
+               418 STORE_NAME              49 (KNOWN_FLOATA_OIDS)
+   
+    68         420 PUSH_NULL
+               422 LOAD_NAME               38 (_make_array_converters)
+               424 LOAD_NAME               49 (KNOWN_FLOATA_OIDS)
+               426 LOAD_NAME               48 (FLOAT_CONVERTERS)
+               428 PRECALL                  2
+               432 CALL                     2
+               442 STORE_NAME              50 (FLOATA_CONVERTERS)
+   
+    70         444 LOAD_CONST              36 ((114, 3802))
+               446 STORE_NAME              51 (KNOWN_JSON_OIDS)
+   
+    71         448 LOAD_CONST              37 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 71>)
+               450 MAKE_FUNCTION            0
+               452 LOAD_NAME               51 (KNOWN_JSON_OIDS)
+               454 GET_ITER
+               456 PRECALL                  0
+               460 CALL                     0
+               470 STORE_NAME              52 (JSON_CONVERTERS)
+   
+    72         472 LOAD_CONST              38 ((199, 3807))
+               474 STORE_NAME              53 (KNOWN_JSONA_OIDS)
+   
+    73         476 PUSH_NULL
+               478 LOAD_NAME               38 (_make_array_converters)
+               480 LOAD_NAME               53 (KNOWN_JSONA_OIDS)
+               482 LOAD_NAME               52 (JSON_CONVERTERS)
+               484 PRECALL                  2
+               488 CALL                     2
+               498 STORE_NAME              54 (JSONA_CONVERTERS)
+   
+    75         500 PUSH_NULL
+               502 LOAD_NAME               22 (BoolConverter)
+               504 PRECALL                  0
+               508 CALL                     0
+               518 STORE_NAME              55 (STATIC_BOOLEAN_CONVERTER)
+   
+    76         520 PUSH_NULL
+               522 LOAD_NAME               20 (ArrayConverter)
+               524 LOAD_CONST              39 (1000)
+               526 LOAD_NAME               55 (STATIC_BOOLEAN_CONVERTER)
+               528 PRECALL                  2
+               532 CALL                     2
+               542 STORE_NAME              56 (STATIC_BOOLEANA_CONVERTER)
+   
+    77         544 PUSH_NULL
+               546 LOAD_NAME               23 (ByteaConverter)
+               548 PRECALL                  0
+               552 CALL                     0
+               562 STORE_NAME              57 (STATIC_BYTES_CONVERTER)
+   
+    80         564 LOAD_CONST              46 (('protocol', 'SansIOClient', 'return', 'None'))
+               566 LOAD_CONST              43 (<code object apply_default_converters, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 80>)
+               568 MAKE_FUNCTION            4 (annotations)
+               570 STORE_NAME              58 (apply_default_converters)
+   
+   114         572 LOAD_CONST              44 (('Converter', 'apply_default_converters', 'EnumConverter', 'ArrayConverter'))
+               574 STORE_NAME              59 (__all__)
+               576 LOAD_CONST               3 (None)
+               578 RETURN_VALUE
    ExceptionTable:
-     52 to 66 -> 70 [0]
-     70 to 94 -> 102 [1] lasti
-     100 to 100 -> 102 [1] lasti
+     64 to 104 -> 108 [0]
+     108 to 132 -> 140 [1] lasti
+     138 to 138 -> 140 [1] lasti
    consts
       '\nPackage containing the converterss for Python types to PostgreSQL types.\n'
       0
       ('annotations',)
       None
       ('Sequence',)
+      ('partial',)
       ('TYPE_CHECKING',)
-      ('loads', 'dumps')
+      ('dumps', 'loads')
+      False
+      ('ensure_ascii',)
       ('Converter',)
       ('ArrayConverter',)
       ('BoolConverter', 'ByteaConverter', 'SimpleFunctionConverter', 'TextConverter')
       ('STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER')
       ('EnumConverter',)
       ('SansIOClient',)
-      False
       ('quote_inner',)
       'oids'
       'Sequence[int]'
       'cvs'
       'Sequence[Converter]'
       'quote_inner'
       'bool'
@@ -317,30 +336,30 @@
          flags     : 16777219
          code
             0x8702970088026601640184087401000000000000000000007c007c0164
             02ac03a6030000ab0300000000000000004400a6000000ab000000000000
             0000005300
                        0 MAKE_CELL                2 (quote_inner)
          
-          40           2 RESUME                   0
+          43           2 RESUME                   0
          
-          46           4 LOAD_CLOSURE             2 (quote_inner)
+          49           4 LOAD_CLOSURE             2 (quote_inner)
                        6 BUILD_TUPLE              1
-                       8 LOAD_CONST               1 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 46>)
+                       8 LOAD_CONST               1 (<code object <listcomp>, file "/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py", line 49>)
                       10 MAKE_FUNCTION            8 (closure)
          
-          48          12 LOAD_GLOBAL              1 (NULL + zip)
+          51          12 LOAD_GLOBAL              1 (NULL + zip)
                       24 LOAD_FAST                0 (oids)
                       26 LOAD_FAST                1 (cvs)
                       28 LOAD_CONST               2 (True)
                       30 KW_NAMES                 3
                       32 PRECALL                  3
                       36 CALL                     3
          
-          46          46 GET_ITER
+          49          46 GET_ITER
                       48 PRECALL                  0
                       52 CALL                     0
                       62 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
@@ -348,65 +367,65 @@
                stacksize : 7
                flags     : 16777235
                code
                   0x9501970067007c005d175c0200007d017d027401000000000000000000
                   007c017c028903ac00a6030000ab03000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-                46           2 RESUME                   0
+                49           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                
-                48          10 UNPACK_SEQUENCE          2
+                51          10 UNPACK_SEQUENCE          2
                             14 STORE_FAST               1 (oid)
                             16 STORE_FAST               2 (cv)
                
-                47          18 LOAD_GLOBAL              1 (NULL + ArrayConverter)
+                50          18 LOAD_GLOBAL              1 (NULL + ArrayConverter)
                             30 LOAD_FAST                1 (oid)
                             32 LOAD_FAST                2 (cv)
                             34 LOAD_DEREF               3 (quote_inner)
                             36 KW_NAMES                 0
                             38 PRECALL                  3
                             42 CALL                     3
                
-                46          52 LIST_APPEND              2
+                49          52 LIST_APPEND              2
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                   ('quote_inner',)
                names      ('ArrayConverter',)
                varnames   ('.0', 'oid', 'cv')
                freevars   ('quote_inner',)
                cellvars   ()
                filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
                name       '<listcomp>'
-               firstlineno 46
+               firstlineno 49
                lnotab 0x0a0208ff22ff
             True
             ('strict',)
          names      ('zip',)
          varnames   ('oids', 'cvs', 'quote_inner')
          freevars   ()
          cellvars   ('quote_inner',)
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       '_make_array_converters'
-         firstlineno 40
+         firstlineno 43
          lnotab 0x0406080222fe
       (20, 21, 23, 26, 27, 28, 29)
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 16777219
          code
             0x970067007c005d1d7d017401000000000000000000007c017402000000
             00000000000000740400000000000000000000a6030000ab030000000000
             00000091028c1e5300
-          53           0 RESUME                   0
+          56           0 RESUME                   0
                        2 BUILD_LIST               0
                        4 LOAD_FAST                0 (.0)
                  >>    6 FOR_ITER                29 (to 66)
                        8 STORE_FAST               1 (oid)
                       10 LOAD_GLOBAL              1 (NULL + SimpleFunctionConverter)
                       22 LOAD_FAST                1 (oid)
                       24 LOAD_GLOBAL              2 (int)
@@ -419,27 +438,27 @@
          consts
          names      ('SimpleFunctionConverter', 'int', 'str')
          varnames   ('.0', 'oid')
          freevars   ()
          cellvars   ()
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       '<listcomp>'
-         firstlineno 53
+         firstlineno 56
          lnotab 0x
       (1016, 1005, 1007, 1028, 1010, 1011, 1012)
       (18, 19, 25)
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 16777219
          code
             0x970067007c005d117d017401000000000000000000007c01a6010000ab
             01000000000000000091028c125300
-          58           0 RESUME                   0
+          61           0 RESUME                   0
                        2 BUILD_LIST               0
                        4 LOAD_FAST                0 (.0)
                  >>    6 FOR_ITER                17 (to 42)
                        8 STORE_FAST               1 (oid)
                       10 LOAD_GLOBAL              1 (NULL + TextConverter)
                       22 LOAD_FAST                1 (oid)
                       24 PRECALL                  1
@@ -450,29 +469,29 @@
          consts
          names      ('TextConverter',)
          varnames   ('.0', 'oid')
          freevars   ()
          cellvars   ()
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       '<listcomp>'
-         firstlineno 58
+         firstlineno 61
          lnotab 0x
       (1009, 1002, 1003)
       True
       (700, 701)
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 16777219
          code
             0x970067007c005d1d7d017401000000000000000000007c017402000000
             00000000000000740400000000000000000000a6030000ab030000000000
             00000091028c1e5300
-          63           0 RESUME                   0
+          66           0 RESUME                   0
                        2 BUILD_LIST               0
                        4 LOAD_FAST                0 (.0)
                  >>    6 FOR_ITER                29 (to 66)
                        8 STORE_FAST               1 (oid)
                       10 LOAD_GLOBAL              1 (NULL + SimpleFunctionConverter)
                       22 LOAD_FAST                1 (oid)
                       24 LOAD_GLOBAL              2 (float)
@@ -485,28 +504,28 @@
          consts
          names      ('SimpleFunctionConverter', 'float', 'str')
          varnames   ('.0', 'oid')
          freevars   ()
          cellvars   ()
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       '<listcomp>'
-         firstlineno 63
+         firstlineno 66
          lnotab 0x
       (1021, 1022)
       (114, 3802)
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 16777219
          code
             0x970067007c005d1d7d017401000000000000000000007c017402000000
             00000000000000740400000000000000000000a6030000ab030000000000
             00000091028c1e5300
-          68           0 RESUME                   0
+          71           0 RESUME                   0
                        2 BUILD_LIST               0
                        4 LOAD_FAST                0 (.0)
                  >>    6 FOR_ITER                29 (to 66)
                        8 STORE_FAST               1 (oid)
                       10 LOAD_GLOBAL              1 (NULL + SimpleFunctionConverter)
                       22 LOAD_FAST                1 (oid)
                       24 LOAD_GLOBAL              2 (json_loads)
@@ -519,15 +538,15 @@
          consts
          names      ('SimpleFunctionConverter', 'json_loads', 'json_dumps')
          varnames   ('.0', 'oid')
          freevars   ()
          cellvars   ()
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       '<listcomp>'
-         firstlineno 68
+         firstlineno 71
          lnotab 0x
       (199, 3807)
       1000
       'protocol'
       'SansIOClient'
       'None'
       code
@@ -558,116 +577,116 @@
             000000742400000000000000000000a6010000ab01000000000000000001
             007c00a00a00000000000000000000000000000000000000007426000000
             00000000000000a6010000ab01000000000000000001007c00a00a000000
             0000000000000000000000000000000000742800000000000000000000a6
             010000ab01000000000000000001007c00a00a0000000000000000000000
             000000000000000000742600000000000000000000a6010000ab01000000
             0000000000010064015300
-          77           0 RESUME                   0
+          80           0 RESUME                   0
          
-          83           2 LOAD_GLOBAL              1 (NULL + itertools)
+          86           2 LOAD_GLOBAL              1 (NULL + itertools)
                       14 LOAD_ATTR                1 (chain)
          
-          84          24 LOAD_GLOBAL              4 (INT_CONVERTERS)
+          87          24 LOAD_GLOBAL              4 (INT_CONVERTERS)
                       36 LOAD_GLOBAL              6 (INTA_CONVERTERS)
          
-          85          48 LOAD_GLOBAL              8 (STR_CONVERTERS)
+          88          48 LOAD_GLOBAL              8 (STR_CONVERTERS)
                       60 LOAD_GLOBAL             10 (STRA_CONVERTERS)
          
-          86          72 LOAD_GLOBAL             12 (FLOAT_CONVERTERS)
+          89          72 LOAD_GLOBAL             12 (FLOAT_CONVERTERS)
                       84 LOAD_GLOBAL             14 (FLOATA_CONVERTERS)
          
-          87          96 LOAD_GLOBAL             16 (JSON_CONVERTERS)
+          90          96 LOAD_GLOBAL             16 (JSON_CONVERTERS)
                      108 LOAD_GLOBAL             18 (JSONA_CONVERTERS)
          
-          83         120 PRECALL                  8
+          86         120 PRECALL                  8
                      124 CALL                     8
                      134 GET_ITER
                  >>  136 FOR_ITER                23 (to 184)
                      138 STORE_FAST               1 (cv)
          
-          89         140 LOAD_FAST                0 (protocol)
+          92         140 LOAD_FAST                0 (protocol)
                      142 LOAD_METHOD             10 (add_converter)
                      164 LOAD_FAST                1 (cv)
                      166 PRECALL                  1
                      170 CALL                     1
                      180 POP_TOP
                      182 JUMP_BACKWARD           24 (to 136)
          
-          92     >>  184 LOAD_FAST                0 (protocol)
+          95     >>  184 LOAD_FAST                0 (protocol)
                      186 LOAD_METHOD             10 (add_converter)
                      208 LOAD_GLOBAL             22 (STATIC_BOOLEAN_CONVERTER)
                      220 PRECALL                  1
                      224 CALL                     1
                      234 POP_TOP
          
-          93         236 LOAD_FAST                0 (protocol)
+          96         236 LOAD_FAST                0 (protocol)
                      238 LOAD_METHOD             10 (add_converter)
                      260 LOAD_GLOBAL             24 (STATIC_BOOLEANA_CONVERTER)
                      272 PRECALL                  1
                      276 CALL                     1
                      286 POP_TOP
          
-          95         288 LOAD_FAST                0 (protocol)
+          98         288 LOAD_FAST                0 (protocol)
                      290 LOAD_METHOD             10 (add_converter)
                      312 LOAD_GLOBAL             26 (STATIC_BYTES_CONVERTER)
                      324 PRECALL                  1
                      328 CALL                     1
                      338 POP_TOP
          
-          98         340 LOAD_FAST                0 (protocol)
+         101         340 LOAD_FAST                0 (protocol)
                      342 LOAD_METHOD             10 (add_converter)
                      364 LOAD_GLOBAL             28 (STATIC_TIMESTAMPTZ_CONVERTER)
                      376 PRECALL                  1
                      380 CALL                     1
                      390 POP_TOP
          
-          99         392 LOAD_FAST                0 (protocol)
+         102         392 LOAD_FAST                0 (protocol)
                      394 LOAD_METHOD             10 (add_converter)
                      416 LOAD_GLOBAL             30 (STATIC_TIMESTAMPTZA_CONVERTER)
                      428 PRECALL                  1
                      432 CALL                     1
                      442 POP_TOP
          
-         101         444 LOAD_FAST                0 (protocol)
+         104         444 LOAD_FAST                0 (protocol)
                      446 LOAD_METHOD             10 (add_converter)
                      468 LOAD_GLOBAL             32 (STATIC_TIMESTAMPNOTZ_CONVERTER)
                      480 PRECALL                  1
                      484 CALL                     1
                      494 POP_TOP
          
-         102         496 LOAD_FAST                0 (protocol)
+         105         496 LOAD_FAST                0 (protocol)
                      498 LOAD_METHOD             10 (add_converter)
                      520 LOAD_GLOBAL             34 (STATIC_TIMESTAMPNOTZA_CONVERTER)
                      532 PRECALL                  1
                      536 CALL                     1
                      546 POP_TOP
          
-         104         548 LOAD_FAST                0 (protocol)
+         107         548 LOAD_FAST                0 (protocol)
                      550 LOAD_METHOD             10 (add_converter)
                      572 LOAD_GLOBAL             36 (STATIC_DATE_CONVERTER)
                      584 PRECALL                  1
                      588 CALL                     1
                      598 POP_TOP
          
-         105         600 LOAD_FAST                0 (protocol)
+         108         600 LOAD_FAST                0 (protocol)
                      602 LOAD_METHOD             10 (add_converter)
                      624 LOAD_GLOBAL             38 (STATIC_DATEA_CONVERTER)
                      636 PRECALL                  1
                      640 CALL                     1
                      650 POP_TOP
          
-         107         652 LOAD_FAST                0 (protocol)
+         110         652 LOAD_FAST                0 (protocol)
                      654 LOAD_METHOD             10 (add_converter)
                      676 LOAD_GLOBAL             40 (STATIC_TIME_CONVERTER)
                      688 PRECALL                  1
                      692 CALL                     1
                      702 POP_TOP
          
-         108         704 LOAD_FAST                0 (protocol)
+         111         704 LOAD_FAST                0 (protocol)
                      706 LOAD_METHOD             10 (add_converter)
                      728 LOAD_GLOBAL             38 (STATIC_DATEA_CONVERTER)
                      740 PRECALL                  1
                      744 CALL                     1
                      754 POP_TOP
                      756 LOAD_CONST               1 (None)
                      758 RETURN_VALUE
@@ -676,25 +695,25 @@
             None
          names      ('itertools', 'chain', 'INT_CONVERTERS', 'INTA_CONVERTERS', 'STR_CONVERTERS', 'STRA_CONVERTERS', 'FLOAT_CONVERTERS', 'FLOATA_CONVERTERS', 'JSON_CONVERTERS', 'JSONA_CONVERTERS', 'add_converter', 'STATIC_BOOLEAN_CONVERTER', 'STATIC_BOOLEANA_CONVERTER', 'STATIC_BYTES_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER')
          varnames   ('protocol', 'cv')
          freevars   ()
          cellvars   ()
          filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
          name       'apply_default_converters'
-         firstlineno 77
+         firstlineno 80
          lnotab
             0x0206160118011801180118fc14062c0334013402340334013402340134
             02340134023401
       ('Converter', 'apply_default_converters', 'EnumConverter', 'ArrayConverter')
       ('oids', 'Sequence[int]', 'cvs', 'Sequence[Converter]', 'quote_inner', 'bool', 'return', 'list[Converter]')
       ('protocol', 'SansIOClient', 'return', 'None')
-   names      ('__doc__', '__future__', 'annotations', 'itertools', 'collections.abc', 'Sequence', 'typing', 'TYPE_CHECKING', 'ujson', 'loads', 'json_loads', 'dumps', 'json_dumps', 'ModuleNotFoundError', 'json', 'pg_purepy.conversion.abc', 'Converter', 'pg_purepy.conversion.arrays', 'ArrayConverter', 'pg_purepy.conversion.basics', 'BoolConverter', 'ByteaConverter', 'SimpleFunctionConverter', 'TextConverter', 'pg_purepy.conversion.dt', 'STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER', 'pg_purepy.conversion.enums', 'EnumConverter', 'pg_purepy.protocol', 'SansIOClient', '_make_array_converters', 'KNOWN_INT_OIDS', 'INT_CONVERTERS', 'KNOWN_INTA_OIDS', 'INTA_CONVERTERS', 'KNOWN_TEXT_OIDS', 'STR_CONVERTERS', 'KNOWN_STRA_OIDS', 'STRA_CONVERTERS', 'KNOWN_FLOAT_OIDS', 'FLOAT_CONVERTERS', 'KNOWN_FLOATA_OIDS', 'FLOATA_CONVERTERS', 'KNOWN_JSON_OIDS', 'JSON_CONVERTERS', 'KNOWN_JSONA_OIDS', 'JSONA_CONVERTERS', 'STATIC_BOOLEAN_CONVERTER', 'STATIC_BOOLEANA_CONVERTER', 'STATIC_BYTES_CONVERTER', 'apply_default_converters', '__all__')
+   names      ('__doc__', '__future__', 'annotations', 'itertools', 'collections.abc', 'Sequence', 'functools', 'partial', 'typing', 'TYPE_CHECKING', 'ujson', 'dumps', 'loads', 'json_loads', 'json_dumps', 'ModuleNotFoundError', 'json', 'pg_purepy.conversion.abc', 'Converter', 'pg_purepy.conversion.arrays', 'ArrayConverter', 'pg_purepy.conversion.basics', 'BoolConverter', 'ByteaConverter', 'SimpleFunctionConverter', 'TextConverter', 'pg_purepy.conversion.dt', 'STATIC_DATE_CONVERTER', 'STATIC_DATEA_CONVERTER', 'STATIC_TIME_CONVERTER', 'STATIC_TIMESTAMPNOTZ_CONVERTER', 'STATIC_TIMESTAMPNOTZA_CONVERTER', 'STATIC_TIMESTAMPTZ_CONVERTER', 'STATIC_TIMESTAMPTZA_CONVERTER', 'pg_purepy.conversion.enums', 'EnumConverter', 'pg_purepy.protocol', 'SansIOClient', '_make_array_converters', 'KNOWN_INT_OIDS', 'INT_CONVERTERS', 'KNOWN_INTA_OIDS', 'INTA_CONVERTERS', 'KNOWN_TEXT_OIDS', 'STR_CONVERTERS', 'KNOWN_STRA_OIDS', 'STRA_CONVERTERS', 'KNOWN_FLOAT_OIDS', 'FLOAT_CONVERTERS', 'KNOWN_FLOATA_OIDS', 'FLOATA_CONVERTERS', 'KNOWN_JSON_OIDS', 'JSON_CONVERTERS', 'KNOWN_JSONA_OIDS', 'JSONA_CONVERTERS', 'STATIC_BOOLEAN_CONVERTER', 'STATIC_BOOLEANA_CONVERTER', 'STATIC_BYTES_CONVERTER', 'apply_default_converters', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/laura/dev/libs/sailor/pg-purepy/src/pg_purepy/conversion/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020104040c0208010c010c0202011401080114ff08040c010c0118
-      0624090c0204010c0702fc0c0c04011801040118020401180104011c0204
-      0118010401180204011801040118021401180114030822
+      0x00ff020104040c0208010c010c010c02020110021e01080114ff08040c
+      010c01180624090c0204010c0702fc0c0c04011801040118020401180104
+      011c02040118010401180204011801040118021401180114030822
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/_parse_hstore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/abc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/array_parse.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/arrays.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/basics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/dt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/enums.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-311.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc` & `pg_purepy-0.9.5/src/pg_purepy/conversion/__pycache__/hstore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/_parse_hstore.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/_parse_hstore.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/abc.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/abc.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/array_parse.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/array_parse.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/arrays.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/arrays.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/basics.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/basics.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/dt.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/dt.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/enums.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/enums.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/conversion/hstore.py` & `pg_purepy-0.9.5/src/pg_purepy/conversion/hstore.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/dbapi.py` & `pg_purepy-0.9.5/src/pg_purepy/dbapi.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/exc.py` & `pg_purepy-0.9.5/src/pg_purepy/exc.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,7 +51,13 @@
     """
 
 
 class ConnectionInTransactionWarning(ResourceWarning):
     """
     Raised when a connection is returned to a connection pool whilst it is still in a transaction.
     """
+
+
+class MissingRowError(ValueError):
+    """
+    Raised when there's no row during a ``fetch_one`` operation.
+    """
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/messages.py` & `pg_purepy-0.9.5/src/pg_purepy/messages.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/src/pg_purepy/pool.py` & `pg_purepy-0.9.5/src/pg_purepy/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         Fetches the result of a query on the next available connection. See
         :meth:`.AsyncPostgresConnection.fetch` for more information.
         """
 
         async with self._checkout_connection() as conn:
             return await conn.fetch(query, *params, **kwargs)
 
-    async def fetch_one(self, query: str, *params: Any, **kwargs: Any) -> DataRow | None:
+    async def fetch_one(self, query: str, *params: Any, **kwargs: Any) -> DataRow:
         """
         Like :meth:`.fetch`, but only returns one row. See
         :meth:`.AsyncPostgresConnection.fetch_one` for more information.
         """
 
         async with self._checkout_connection() as conn:
             return await conn.fetch_one(query, *params, **kwargs)
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/protocol.py` & `pg_purepy-0.9.5/src/pg_purepy/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1160,15 +1160,15 @@
                 self._current_packet_remaining = size - len(message_data)
                 # reset buffer, otherwise we try and read the message code off again >.>
                 self._buffer = bytearray()
                 return NEED_DATA
             else:  # noqa: RET505
                 # yes enough data, set the buffer to the data after the size bytes for future
                 # processing
-                self._buffer = self._buffer[size + 5:]
+                self._buffer = self._buffer[size + 5 :]
 
         code = BackendMessageCode(code)
         self._logger.trace(f"Got incoming message {code!r}")
 
         try:
             method = getattr(self, f"_handle_during_{self.state.name}")
         except AttributeError:
```

### Comparing `pg_purepy-0.9.4/src/pg_purepy/util.py` & `pg_purepy-0.9.5/src/pg_purepy/util.py`

 * *Files identical despite different names*

### Comparing `pg_purepy-0.9.4/PKG-INFO` & `pg_purepy-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-purepy
-Version: 0.9.4
+Version: 0.9.5
 Summary: A pure-Python anyio-based PostgreSQL adapter.
 License: LGPL-3.0-or-later
 Author: Lura Skye
 Author-email: l@veriny.tf
 Requires-Python: >=3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

