# Comparing `tmp/restx-0.1.5.tar.gz` & `tmp/restx-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restx-0.1.5.tar", max compression
+gzip compressed data, was "restx-0.1.6.tar", max compression
```

## Comparing `restx-0.1.5.tar` & `restx-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-13 17:51:18.207713 restx-0.1.5/LICENSE
--rw-r--r--   0        0        0      259 2024-04-13 17:51:18.207713 restx-0.1.5/README.md
--rw-r--r--   0        0        0     1160 2024-04-13 17:51:18.207713 restx-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 17:51:18.207713 restx-0.1.5/restx/__init__.py
--rwxr-xr-x   0        0        0     1834 2024-04-13 17:51:18.207713 restx-0.1.5/restx/cli.py
--rw-r--r--   0        0        0      140 2024-04-13 17:51:18.207713 restx-0.1.5/restx/enums.py
--rw-r--r--   0        0        0     2780 2024-04-13 17:51:18.207713 restx-0.1.5/restx/utils.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 restx-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 18:56:50.492130 restx-0.1.6/LICENSE
+-rw-r--r--   0        0        0      259 2024-04-13 18:56:50.492130 restx-0.1.6/README.md
+-rw-r--r--   0        0        0     1160 2024-04-13 18:56:50.492130 restx-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 18:56:50.492130 restx-0.1.6/restx/__init__.py
+-rwxr-xr-x   0        0        0     2272 2024-04-13 18:56:50.492130 restx-0.1.6/restx/cli.py
+-rw-r--r--   0        0        0      140 2024-04-13 18:56:50.492130 restx-0.1.6/restx/enums.py
+-rw-r--r--   0        0        0     3153 2024-04-13 18:56:50.492130 restx-0.1.6/restx/utils.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 restx-0.1.6/PKG-INFO
```

### Comparing `restx-0.1.5/LICENSE` & `restx-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `restx-0.1.5/pyproject.toml` & `restx-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 description = "A CLI app for performing RESTX operations via HTTP requests."
 include = [
   "LICENSE",
 ]
 license = "MIT"
 name = "restx"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 httpx = "^0.27.0"
 python = ">=3.10,<4.0"
 rich = "^13.7.1"
 typer = "^0.12.3"
```

### Comparing `restx-0.1.5/restx/cli.py` & `restx-0.1.6/restx/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,61 +5,73 @@
 
 
 app = typer.Typer()
 console = Console()
 
 
 @app.command()
-def get(url: str, headers: str = None) -> None:
+def get(
+    url: str,
+    headers: str = typer.Option(None, "--header", "-H", help="Custom headers"),
+) -> None:
     """Send a GET request."""
     response, response_time = crud_manager(
         url=url, method="GET", headers=headers
     ).values()
     print_additional_info(response, response_time)
     print_response_body(response)
 
 
 @app.command()
 def post(
-    url: str, payload: str = typer.Option(..., "--payload", "-p", help="Payload data")
+    url: str,
+    payload: str = typer.Option(..., "--payload", "-p", help="Payload data"),
+    headers: str = typer.Option(None, "--header", "-H", help="Custom headers"),
 ) -> None:
     """Send a POST request."""
     response, response_time = crud_manager(
-        url=url, method="POST", payload=payload
+        url=url, method="POST", payload=payload, headers=headers
     ).values()
     print_additional_info(response, response_time)
     print_response_body(response)
 
 
 @app.command()
 def put(
-    url: str, payload: str = typer.Option(..., "--payload", "-p", help="Payload data")
+    url: str,
+    payload: str = typer.Option(..., "--payload", "-p", help="Payload data"),
+    headers: str = typer.Option(None, "--header", "-H", help="Custom headers"),
 ) -> None:
     """Send a PUT request."""
     response, response_time = crud_manager(
-        url=url, method="PUT", payload=payload
+        url=url, method="PUT", payload=payload, headers=headers
     ).values()
     print_additional_info(response, response_time)
     print_response_body(response)
 
 
 @app.command()
 def patch(
-    url: str, payload: str = typer.Option(..., "--payload", "-p", help="Payload data")
+    url: str,
+    payload: str = typer.Option(..., "--payload", "-p", help="Payload data"),
+    headers: str = typer.Option(None, "--header", "-H", help="Custom headers"),
 ) -> None:
     """Send a PATCH request."""
     response, response_time = crud_manager(
-        url=url, method="PATCH", payload=payload
+        url=url, method="PATCH", payload=payload, headers=headers
     ).values()
     print_additional_info(response, response_time)
     print_response_body(response)
 
 
 @app.command()
-def delete(url: str, headers: str = None) -> None:
+def delete(
+    url: str,
+    headers: str = typer.Option(None, "--header", "-H", help="Custom headers"),
+) -> None:
     """Send a DELETE request."""
     response, response_time = crud_manager(
         url=url, method="DELETE", headers=headers
     ).values()
     print_additional_info(response, response_time)
     print_response_body(response)
```

### Comparing `restx-0.1.5/restx/utils.py` & `restx-0.1.6/restx/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,41 @@
     method: str = DEFAULT_METHOD,
 ) -> dict[str, Any]:
     """Perform an HTTP request based on the user choice."""
     start_time: datetime = datetime.now()
     CHOICE: str = method.upper()
     with Client() as client:
         if CHOICE == HTTPMethod.GET.value:
-            response: Response = client.get(url, headers=headers)
+            response: Response = client.get(
+                url,
+                headers=json.loads(headers) if headers else headers,
+            )
         elif CHOICE == HTTPMethod.POST.value:
             response: Response = client.post(
-                url, json=json.loads(payload), headers=headers
+                url,
+                json=json.loads(payload),
+                headers=json.loads(headers) if headers else headers,
             )
         elif CHOICE == HTTPMethod.PUT.value:
             response: Response = client.put(
-                url, json=json.loads(payload), headers=headers
+                url,
+                json=json.loads(payload),
+                headers=json.loads(headers) if headers else headers,
             )
         elif CHOICE == HTTPMethod.PATCH.value:
             response: Response = client.patch(
-                url, json=json.loads(payload), headers=headers
+                url,
+                json=json.loads(payload),
+                headers=json.loads(headers) if headers else headers,
             )
         elif CHOICE == HTTPMethod.DELETE.value:
-            response: Response = client.delete(url, headers=headers)
+            response: Response = client.delete(
+                url,
+                headers=json.loads(headers) if headers else headers,
+            )
         else:
             raise ValueError(f"Unsupported HTTP method: {method}")
     end_time: datetime = datetime.now()
     response_time: timedelta = end_time - start_time
     return {"response": response, "response_time": response_time}
```

### Comparing `restx-0.1.5/PKG-INFO` & `restx-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restx
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI app for performing RESTX operations via HTTP requests.
 License: MIT
 Author: Arjun Umathanu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

