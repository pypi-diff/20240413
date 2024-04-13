# Comparing `tmp/grid3-0.1.7.tar.gz` & `tmp/grid3-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid3-0.1.7.tar", max compression
+gzip compressed data, was "grid3-0.1.8.tar", max compression
```

## Comparing `grid3-0.1.7.tar` & `grid3-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11350 2023-10-31 23:30:25.227865 grid3-0.1.7/LICENSE
--rw-r--r--   0        0        0     1598 2023-11-01 20:49:25.182303 grid3-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-03 01:26:02.905821 grid3-0.1.7/grid3/__init__.py
--rw-r--r--   0        0        0     7600 2023-05-05 23:39:20.557684 grid3-0.1.7/grid3/graphql.py
--rw-r--r--   0        0        0     1916 2024-02-10 08:21:26.935548 grid3-0.1.7/grid3/grid_cli.py
--rw-r--r--   0        0        0     1831 2023-10-31 20:59:05.691085 grid3-0.1.7/grid3/network.py
--rw-r--r--   0        0        0     1919 2023-10-31 21:00:20.491570 grid3-0.1.7/grid3/proxy.py
--rw-r--r--   0        0        0     4739 2024-02-12 23:59:39.914194 grid3-0.1.7/grid3/rmb.py
--rw-r--r--   0        0        0     5012 2024-04-10 06:55:46.225908 grid3-0.1.7/grid3/tfchain.py
--rw-r--r--   0        0        0     4216 2023-07-18 23:52:01.722433 grid3-0.1.7/grid3/types.py
--rw-r--r--   0        0        0      614 2024-04-10 06:56:18.442808 grid3-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 grid3-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-10-31 23:30:25.227865 grid3-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1598 2023-11-01 20:49:25.182303 grid3-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 01:26:02.905821 grid3-0.1.8/grid3/__init__.py
+-rw-r--r--   0        0        0     7784 2024-04-11 00:54:44.140740 grid3-0.1.8/grid3/graphql.py
+-rw-r--r--   0        0        0     1916 2024-02-10 08:21:26.935548 grid3-0.1.8/grid3/grid_cli.py
+-rw-r--r--   0        0        0     1527 2024-04-13 01:52:26.586523 grid3-0.1.8/grid3/minting.py
+-rw-r--r--   0        0        0     1831 2023-10-31 20:59:05.691085 grid3-0.1.8/grid3/network.py
+-rw-r--r--   0        0        0     1919 2023-10-31 21:00:20.491570 grid3-0.1.8/grid3/proxy.py
+-rw-r--r--   0        0        0     4739 2024-02-12 23:59:39.914194 grid3-0.1.8/grid3/rmb.py
+-rw-r--r--   0        0        0     5012 2024-04-10 06:55:46.225908 grid3-0.1.8/grid3/tfchain.py
+-rw-r--r--   0        0        0     4216 2023-07-18 23:52:01.722433 grid3-0.1.8/grid3/types.py
+-rw-r--r--   0        0        0      614 2024-04-13 20:31:07.969903 grid3-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 grid3-0.1.8/PKG-INFO
```

### Comparing `grid3-0.1.7/LICENSE` & `grid3-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/README.md` & `grid3-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/graphql.py` & `grid3-0.1.8/grid3/graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
     def __init__(self, url=None, fetch_schema=True):
         self.transport = RequestsHTTPTransport(url=url, verify=True, retries=3)
         self.client = Client(transport=self.transport,
                              fetch_schema_from_transport=True)
         self.fetching_schema = False
         # Really meant as a convenience for interactive use, probably not safe, or needed, for code that immediately runs queries. Actually, seems there's a lock on opening the transport, so it's not unsafe. We get some errors if we try to do stuff that requires the schema too soon, but do we really want a locking mechanism in here?
+        # Now I'm getting a lot of errors like below that go away if I fetch_schema first
+        # gql.transport.exceptions.TransportAlreadyConnected: Transport is already connected
+
         if fetch_schema:
             self.fetching_schema = True
             self.schema_event = threading.Event()
             threading.Thread(target=self.fetch_schema, args=[True]).start()
 
         self._dsl_schema = None
```

### Comparing `grid3-0.1.7/grid3/grid_cli.py` & `grid3-0.1.8/grid3/grid_cli.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/network.py` & `grid3-0.1.8/grid3/network.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/proxy.py` & `grid3-0.1.8/grid3/proxy.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/rmb.py` & `grid3-0.1.8/grid3/rmb.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/tfchain.py` & `grid3-0.1.8/grid3/tfchain.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/grid3/types.py` & `grid3-0.1.8/grid3/types.py`

 * *Files identical despite different names*

### Comparing `grid3-0.1.7/pyproject.toml` & `grid3-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grid3"
-version = "0.1.7"
+version = "0.1.8"
 description = "Modules for interacting with ThreeFold Grid v3."
 authors = ["Scott Yeager <scott@threefold.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "grid3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `grid3-0.1.7/PKG-INFO` & `grid3-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid3
-Version: 0.1.7
+Version: 0.1.8
 Summary: Modules for interacting with ThreeFold Grid v3.
 License: Apache-2.0
 Author: Scott Yeager
 Author-email: scott@threefold.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

