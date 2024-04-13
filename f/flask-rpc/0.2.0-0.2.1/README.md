# Comparing `tmp/flask_rpc-0.2.0.tar.gz` & `tmp/flask_rpc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.2.0.tar` & `flask_rpc-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.0/LICENSE
--rw-r--r--   0        0        0     2511 2024-04-13 09:42:00.789713 flask_rpc-0.2.0/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.0/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.0/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.0/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.0/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.0/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.0/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.0/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.0/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.0/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.0/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.0/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.0/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.0/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      196 2024-04-13 09:21:27.176917 flask_rpc-0.2.0/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      365 2024-04-13 09:42:00.794800 flask_rpc-0.2.0/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.0/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-13 10:00:02.958869 flask_rpc-0.2.0/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.0/flask_rpc/latest.py
--rw-r--r--   0        0        0     2954 2024-04-13 09:50:13.701241 flask_rpc-0.2.0/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.0/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.0/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.0/test.py
--rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 flask_rpc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2511 2024-04-13 09:42:00.789713 flask_rpc-0.2.1/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.1/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.1/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.1/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.1/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.1/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.1/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.1/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.1/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.1/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.1/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.1/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.1/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.1/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-13 10:27:45.421471 flask_rpc-0.2.1/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.1/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.1/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-13 10:30:28.293994 flask_rpc-0.2.1/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.1/flask_rpc/latest.py
+-rw-r--r--   0        0        0     3045 2024-04-13 10:25:44.176323 flask_rpc-0.2.1/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.1/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.1/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.1/test.py
+-rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 flask_rpc-0.2.1/PKG-INFO
```

### Comparing `flask_rpc-0.2.0/.gitignore` & `flask_rpc-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/LICENSE` & `flask_rpc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/README.md` & `flask_rpc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/app/__init__.py` & `flask_rpc-0.2.1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/app/models/clients.py` & `flask_rpc-0.2.1/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/app/models/users.py` & `flask_rpc-0.2.1/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.2.1/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/app/templates/index.html` & `flask_rpc-0.2.1/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/flask_rpc/version_1_0.py` & `flask_rpc-0.2.1/flask_rpc/version_1_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,45 @@
 
 
 class RPCRequest:
     @classmethod
     def build(
         cls,
         function: str,
-        data: t.Optional[str, int, float, bool, list[t.Any], t.Dict[str, t.Any]] = None,
+        data: t.Union[
+            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
+        ] = None,
     ) -> t.Dict[str, t.Any]:
         return {"frpc": 1.0, "function": function, "data": data}
 
 
 class RPCResponse:
     @classmethod
     def fail(
         cls,
         message: str = None,
-        data: t.Optional[str, int, float, bool, list[t.Any], t.Dict[str, t.Any]] = None,
+        data: t.Union[
+            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
+        ] = None,
     ):
         r = {"frpc": 1.0, "ok": False}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
 
     @classmethod
     def success(
         cls,
-        data: t.Union[str, int, float, list, bool, t.Dict[str, t.Any]] = None,
+        data: t.Union[
+            str, int, float, bool, t.List[t.Any], t.Dict[str, t.Any], None
+        ] = None,
         message: str = None,
     ):
         r = {"frpc": 1.0, "ok": True}
 
         if message:
             r["message"] = message
         if data:
```

### Comparing `flask_rpc-0.2.0/pyproject.toml` & `flask_rpc-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/test.py` & `flask_rpc-0.2.1/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.0/PKG-INFO` & `flask_rpc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.2.0
+Version: 0.2.1
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

