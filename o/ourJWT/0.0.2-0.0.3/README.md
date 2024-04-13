# Comparing `tmp/ourJWT-0.0.2.tar.gz` & `tmp/ourJWT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.0.2.tar", last modified: Fri Apr 12 19:09:42 2024, max compression
+gzip compressed data, was "ourJWT-0.0.3.tar", last modified: Fri Apr 12 21:36:09 2024, max compression
```

## Comparing `ourJWT-0.0.2.tar` & `ourJWT-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 19:09:42.148186 ourJWT-0.0.2/PKG-INFO
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/ourJWT/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     2467 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      150 2024-04-12 19:04:02.000000 ourJWT-0.0.2/ourJWT/__init__.py
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     1077 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/ourJWT.egg-info/
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-12 19:09:42.148186 ourJWT-0.0.2/setup.cfg
--rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-12 19:04:07.000000 ourJWT-0.0.2/setup.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 21:36:09.752671 ourJWT-0.0.3/PKG-INFO
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/ourJWT/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     2462 2024-04-12 21:36:06.000000 ourJWT-0.0.3/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.0.3/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      153 2024-04-12 21:30:49.000000 ourJWT-0.0.3/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     1084 2024-04-12 21:33:56.000000 ourJWT-0.0.3/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 21:36:09.752671 ourJWT-0.0.3/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-12 21:36:09.000000 ourJWT-0.0.3/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-12 21:36:09.752671 ourJWT-0.0.3/setup.cfg
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-12 21:31:05.000000 ourJWT-0.0.3/setup.py
```

### Comparing `ourJWT-0.0.2/ourJWT/OUR_class.py` & `ourJWT-0.0.3/ourJWT/OUR_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import jwt
 
-import OUR_exception
+from . import OUR_exception
 
 good_iss = "OUR_Transcendence"
 
 
 class Decoder:
     pub_key: str
 
     def __init__(self, pub_key):
+        if pub_key is None:
+             raise OUR_exception.NoKey
         self.pub_key = pub_key
-        if self.pub_key is None:
-            raise OUR_exception.NoKey
 
 
 
     def decode(self, to_decode):
         """
         decode the given JWT into a dict.
 
@@ -48,17 +48,17 @@
 
 
 
 class Encoder:
     private_key: str
 
     def __init__(self, priv_key):
-        self.private_key = priv_key
-        if self.private_key is None:
+        if priv_key is None:
             raise OUR_exception.NoKey
+        self.private_key = priv_key
 
     def encode(self, to_encode, type):
         """
         Encodes the given payload into a JWT (JSON Web Token).
 
         Args:
             to_encode (dict): The payload to be encoded into the JWT.
```

### Comparing `ourJWT-0.0.2/ourJWT/decorators.py` & `ourJWT-0.0.3/ourJWT/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.http import HttpRequest, response
 
-import OUR_exception, OUR_class
+from . import OUR_exception, OUR_class
 
 
 class HttpResponseUnauthorized(response.HttpResponse):
     status_code = 401
 
 
 def auth_required(function, decoder: OUR_class.Decoder):
```

### Comparing `ourJWT-0.0.2/setup.py` & `ourJWT-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.0.2',
+    version='0.0.3',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

