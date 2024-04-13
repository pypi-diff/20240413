# Comparing `tmp/ourJWT-0.0.3.tar.gz` & `tmp/ourJWT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.0.3.tar", last modified: Fri Apr 12 21:36:09 2024, max compression
+gzip compressed data, was "ourJWT-0.0.4.tar", last modified: Sat Apr 13 09:37:12 2024, max compression
```

## Comparing `ourJWT-0.0.3.tar` & `ourJWT-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 21:36:09.752671 ourJWT-0.0.3/PKG-INFO
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/ourJWT/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     2462 2024-04-12 21:36:06.000000 ourJWT-0.0.3/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.0.3/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-12 21:30:49.000000 ourJWT-0.0.3/ourJWT/__init__.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     1084 2024-04-12 21:33:56.000000 ourJWT-0.0.3/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/ourJWT.egg-info/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-12 21:36:09.752671 ourJWT-0.0.3/setup.cfg
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-12 21:31:05.000000 ourJWT-0.0.3/setup.py
+drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.390422 ourJWT-0.0.4/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      448 2024-04-13 09:37:12.390422 ourJWT-0.0.4/PKG-INFO
+drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.386422 ourJWT-0.0.4/ourJWT/
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)     2462 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/OUR_class.py
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/OUR_exception.py
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/__init__.py
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)     1195 2024-04-13 07:58:22.000000 ourJWT-0.0.4/ourJWT/decorators.py
+drwxrwxr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-13 09:37:12.386422 ourJWT-0.0.4/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      448 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/PKG-INFO
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/SOURCES.txt
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/dependency_links.txt
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/requires.txt
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-13 09:37:12.000000 ourJWT-0.0.4/ourJWT.egg-info/top_level.txt
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-13 09:37:12.390422 ourJWT-0.0.4/setup.cfg
+-rw-rw-r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-13 09:36:58.000000 ourJWT-0.0.4/setup.py
```

### Comparing `ourJWT-0.0.3/ourJWT/OUR_class.py` & `ourJWT-0.0.4/ourJWT/OUR_class.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.0.3/ourJWT/decorators.py` & `ourJWT-0.0.4/ourJWT/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from . import OUR_exception, OUR_class
 
 
 class HttpResponseUnauthorized(response.HttpResponse):
     status_code = 401
 
 
-def auth_required(function, decoder: OUR_class.Decoder):
-    def wrapper(request: HttpRequest):
-        auth: str = request.headers["Authorization"]
-        if auth is None:
-            return response.HttpResponseBadRequest(reason="No Authorization header found in request")
-        auth_type = auth.split(" ")[0]
-        if (auth_type) != "Bearer":
-            return response.HttpResponseBadRequest(reason="Type not Bearer")
-        auth_token = auth.split(" ")[1]
-        if auth_token is None:
-            return response.HttpResponseBadRequest(reason="No auth token detected")
-        try:
-            auth_decoded = decoder.decode(auth_token)
-        except (OUR_exception.BadSubject,
-                OUR_exception.RefusedToken,
-                OUR_exception.ExpiredToken):
-            return HttpResponseUnauthorized(reason="Bad auth token")
-        return function(request, auth_decoded)
-
-    return wrapper
+def auth_required(decoder: OUR_class.Decoder):
+    def decorator(function):
+        def wrapper(request: HttpRequest):
+            auth: str = request.headers["Authorization"]
+            if auth is None:
+                return response.HttpResponseBadRequest(reason="No Authorization header found in request")
+            auth_type = auth.split(" ")[0]
+            if (auth_type) != "Bearer":
+                return response.HttpResponseBadRequest(reason="Type not Bearer")
+            auth_token = auth.split(" ")[1]
+            if auth_token is None:
+                return response.HttpResponseBadRequest(reason="No auth token detected")
+            try:
+                auth_decoded = decoder.decode(auth_token)
+            except (OUR_exception.BadSubject,
+                    OUR_exception.RefusedToken,
+                    OUR_exception.ExpiredToken):
+                return HttpResponseUnauthorized(reason="Bad auth token")
+            return function(request, auth_decoded)
+        return wrapper
+    return decorator
```

### Comparing `ourJWT-0.0.3/setup.py` & `ourJWT-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.0.3',
+    version='0.0.4',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

