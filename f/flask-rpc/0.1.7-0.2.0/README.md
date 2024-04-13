# Comparing `tmp/flask_rpc-0.1.7.tar.gz` & `tmp/flask_rpc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.1.7.tar` & `flask_rpc-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.1.7/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.7/LICENSE
--rw-r--r--   0        0        0     2523 2024-04-12 20:16:40.012404 flask_rpc-0.1.7/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.7/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.7/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.7/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.1.7/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.7/app/models/users.py
--rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.7/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.7/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.7/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      286 2024-04-12 19:45:53.495758 flask_rpc-0.1.7/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      229 2024-04-12 19:46:23.649313 flask_rpc-0.1.7/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      221 2024-04-12 19:46:13.766886 flask_rpc-0.1.7/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.7/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1546 2024-04-12 19:46:38.040859 flask_rpc-0.1.7/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.1.7/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-12 20:35:52.504822 flask_rpc-0.1.7/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.7/flask_rpc/latest.py
--rw-r--r--   0        0        0     2911 2024-04-12 20:04:57.691367 flask_rpc-0.1.7/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.7/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.1.7/requirements_dev.txt
--rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.7/test.py
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 flask_rpc-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2511 2024-04-13 09:42:00.789713 flask_rpc-0.2.0/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.0/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.0/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.0/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.0/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.0/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.0/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.0/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.0/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.0/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.0/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.0/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.0/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.0/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-13 09:21:27.176917 flask_rpc-0.2.0/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      365 2024-04-13 09:42:00.794800 flask_rpc-0.2.0/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.0/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-13 10:00:02.958869 flask_rpc-0.2.0/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.0/flask_rpc/latest.py
+-rw-r--r--   0        0        0     2954 2024-04-13 09:50:13.701241 flask_rpc-0.2.0/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.0/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.0/test.py
+-rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 flask_rpc-0.2.0/PKG-INFO
```

### Comparing `flask_rpc-0.1.7/.gitignore` & `flask_rpc-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/LICENSE` & `flask_rpc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/README.md` & `flask_rpc-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 from flask import Flask
 
 from flask_rpc.latest import RPC, RPCResponse
 
 
 def add_numbers(data):
     if isinstance(data, list):
-        return RPCResponse.successful_response(
+        return RPCResponse.success(
             sum(data),
             "Function 'add_numbers' executed successfully"
         )
 
 
 app = Flask(__name__)
 rpc = RPC(app, url_prefix="/rpc")  # or RPC(blueprint)
```

### Comparing `flask_rpc-0.1.7/app/__init__.py` & `flask_rpc-0.2.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/app/models/clients.py` & `flask_rpc-0.2.0/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/app/models/users.py` & `flask_rpc-0.2.0/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.2.0/app/rpc/clients/funcs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,60 +2,60 @@
 from flask_rpc.latest import RPCResponse
 
 
 def create_client(data):
     status, message, result = Clients.create(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, data)
+        return RPCResponse.fail(message, data)
 
-    return RPCResponse.successful_response(
+    return RPCResponse.success(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
 def read_client(data):
     status, message, result = Clients.read(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, data)
+        return RPCResponse.fail(message, data)
 
-    return RPCResponse.successful_response(
+    return RPCResponse.success(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
 def update_client(data):
     status, message, result = Clients.update(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, data)
+        return RPCResponse.fail(message, data)
 
-    return RPCResponse.successful_response(
+    return RPCResponse.success(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
 def delete_client(data):
     status, message, result = Clients.delete(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, data)
+        return RPCResponse.fail(message, data)
 
-    return RPCResponse.successful_response(
+    return RPCResponse.success(
         {"client_id": result.client_id, "name": result.name}
     )
```

### Comparing `flask_rpc-0.1.7/app/templates/index.html` & `flask_rpc-0.2.0/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/flask_rpc/version_1_0.py` & `flask_rpc-0.2.0/flask_rpc/version_1_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,39 @@
     function: str
     data: t.Any
 
 
 class RPCRequest:
     @classmethod
     def build(
-        cls, function: str, data: t.Optional[t.Dict[str, t.Any]] = None
+        cls,
+        function: str,
+        data: t.Optional[str, int, float, bool, list[t.Any], t.Dict[str, t.Any]] = None,
     ) -> t.Dict[str, t.Any]:
         return {"frpc": 1.0, "function": function, "data": data}
 
 
 class RPCResponse:
     @classmethod
-    def failed_response(cls, message: str = None, data: t.Dict[str, t.Any] = None):
+    def fail(
+        cls,
+        message: str = None,
+        data: t.Optional[str, int, float, bool, list[t.Any], t.Dict[str, t.Any]] = None,
+    ):
         r = {"frpc": 1.0, "ok": False}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
 
     @classmethod
-    def successful_response(
+    def success(
         cls,
         data: t.Union[str, int, float, list, bool, t.Dict[str, t.Any]] = None,
         message: str = None,
     ):
         r = {"frpc": 1.0, "ok": True}
 
         if message:
@@ -75,32 +81,32 @@
             view_func=self._rpc_route,
             provide_automatic_options=True,
             methods=["POST"],
         )
 
     def _rpc_route(self):
         if not request.is_json:
-            return RPCResponse.failed_response("Request must be JSON.")
+            return RPCResponse.fail("Request must be JSON.")
 
         if not request.json:
-            return RPCResponse.failed_response("Request must not be empty.")
+            return RPCResponse.fail("Request must not be empty.")
 
         if not request.json.get("frpc") == 1.0:
-            return RPCResponse.failed_response("Invalid Flask-RPC version.")
+            return RPCResponse.fail("Invalid Flask-RPC version.")
 
         try:
             rpcm = RPCModel(**request.json)
         except ValidationError:
-            return RPCResponse.failed_response("Invalid request.")
+            return RPCResponse.fail("Invalid request.")
 
         try:
             assert rpcm.function in self.LOOKUP
         except AssertionError:
-            return RPCResponse.failed_response("Invalid function.")
+            return RPCResponse.fail("Invalid function.")
 
         if successful_response := self.LOOKUP[rpcm.function](rpcm.data):
             return successful_response
 
-        return RPCResponse.failed_response("Unsuccessful command execution.")
+        return RPCResponse.fail("Unsuccessful command execution.")
 
 
 __all__ = ["RPC", "RPCResponse", "RPCModel"]
```

### Comparing `flask_rpc-0.1.7/pyproject.toml` & `flask_rpc-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.7/test.py` & `flask_rpc-0.2.0/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pprint import pprint
 
 import click
 import faker
 import requests
 
-from flask_rpc.latest import RPCRequest
+from flask_rpc.latest import RPCRequest as Req
 
 
 @click.group("run")
 def run():
     pass
 
 
@@ -29,104 +29,114 @@
     )
     pprint(response.json(), indent=2)
 
 
 # Using the RCPRequest class to make a request to the server
 
 @run.command("create-class")
-def create():
+def create_class():
     f = faker.Faker()
 
     click.echo("Creating a client...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients",
-        json=RPCRequest.build(
+        json=Req.build(
             function="create",
             data={"name": f.name()}
         )
     )
     pprint(response.json(), indent=2)
 
 
 @run.command("read")
-def create():
+def read():
     click.echo("Reading client...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients",
-        json={
-            "frpc": 1.0,  # Required
-            "function": "read",
-            "data": {
-                "client_id": 1
-            }
-        }
+        json=Req.build(
+            function="read",
+            data={"client_id": 1}
+        )
     )
     pprint(response.json(), indent=2)
 
 
 @run.command("read-fail")
-def create():
+def read_fail():
     click.echo("Reading client...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients/read",
-        json={
-            "frpc": 1.0,  # Required
-            "function": "read",
-            "data": {
-                "client_id": 1111
-            }
-        }
+        json=Req.build(
+            function="read",
+            data={"client_id": 11111}
+        )
     )
     pprint(response.json(), indent=2)
 
 
 @run.command("update")
-def create():
+def update():
     click.echo("Updating client...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients/update",
-        json={
-            "frpc": 1.0,  # Required
-            "function": "update",
-            "data": {
-                "client_id": 1,
-                "name": "Jane Doe"
-            }
-        }
+        json=Req.build(
+            function="update",
+            data={"client_id": 1, "name": "John Doe"}
+        )
     )
     pprint(response.json(), indent=2)
 
 
 @run.command("delete")
-def create():
+def delete():
     click.echo("Deleting client...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients",
-        json={
-            "frpc": 1.0,  # Required
-            "function": "delete",
-            "data": {
-                "client_id": 1
-            }
-        }
+        json=Req.build(
+            function="delete",
+            data={"client_id": 1}
+        )
     )
     pprint(response.json(), indent=2)
 
 
 @run.command("fail")
-def create():
+def fail():
     click.echo("Sending bad command...")
     response = requests.post(
         "http://127.0.0.1:5000/rpc/clients",
-        json={
-            "frpc": 1.0,  # Required
-            "function": "fail",
-            "data": {
-                "client_id": 1
-            }
-        }
+        json=Req.build(
+            function="fail",
+            data={"client_id": 1}
+        )
+    )
+    pprint(response.json(), indent=2)
+
+
+@run.command("t1")
+def test1():
+    click.echo("Running function...")
+    response = requests.post(
+        "http://127.0.0.1:5000/rpc/tester",
+        json=Req.build(
+            function="add_numbers",
+            data=[1, 2, 3]
+        )
+    )
+    pprint(response.json(), indent=2)
+
+
+@run.command("t2")
+def test2():
+    click.echo("Running function...")
+    response = requests.post(
+        "http://127.0.0.1:5000/rpc/tester",
+        json=Req.build(
+            function="add_string",
+            data="World"
+        )
     )
     pprint(response.json(), indent=2)
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `flask_rpc-0.1.7/PKG-INFO` & `flask_rpc-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.1.7
+Version: 0.2.0
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -74,15 +74,15 @@
 from flask import Flask
 
 from flask_rpc.latest import RPC, RPCResponse
 
 
 def add_numbers(data):
     if isinstance(data, list):
-        return RPCResponse.successful_response(
+        return RPCResponse.success(
             sum(data),
             "Function 'add_numbers' executed successfully"
         )
 
 
 app = Flask(__name__)
 rpc = RPC(app, url_prefix="/rpc")  # or RPC(blueprint)
```

