# Comparing `tmp/Flask-Cognito-1.8.tar.gz` & `tmp/Flask-Cognito-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Cognito-1.8.tar", last modified: Tue Jan  8 12:35:05 2019, max compression
+gzip compressed data, was "dist/Flask-Cognito-1.9.tar", last modified: Tue Jan  8 12:42:51 2019, max compression
```

## Comparing `Flask-Cognito-1.8.tar` & `Flask-Cognito-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 cyber      (501) staff       (20)        0 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/
-drwxr-xr-x   0 cyber      (501) staff       (20)        0 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/
--rw-r--r--   0 cyber      (501) staff       (20)     2651 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/PKG-INFO
--rw-r--r--   0 cyber      (501) staff       (20)      255 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/SOURCES.txt
--rw-r--r--   0 cyber      (501) staff       (20)        1 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/dependency_links.txt
--rw-r--r--   0 cyber      (501) staff       (20)        1 2019-01-06 11:25:53.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/not-zip-safe
--rw-r--r--   0 cyber      (501) staff       (20)       39 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/requires.txt
--rw-r--r--   0 cyber      (501) staff       (20)       14 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/Flask_Cognito.egg-info/top_level.txt
--rw-r--r--   0 cyber      (501) staff       (20)     2651 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/PKG-INFO
--rw-r--r--   0 cyber      (501) staff       (20)     1518 2019-01-08 12:34:51.000000 Flask-Cognito-1.8/README.md
--rw-r--r--   0 cyber      (501) staff       (20)     5844 2019-01-08 12:27:20.000000 Flask-Cognito-1.8/flask_cognito.py
--rw-r--r--   0 cyber      (501) staff       (20)       38 2019-01-08 12:35:05.000000 Flask-Cognito-1.8/setup.cfg
--rw-r--r--   0 cyber      (501) staff       (20)     1226 2019-01-08 12:35:01.000000 Flask-Cognito-1.8/setup.py
+drwxr-xr-x   0 cyber      (501) staff       (20)        0 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/
+drwxr-xr-x   0 cyber      (501) staff       (20)        0 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/
+-rw-r--r--   0 cyber      (501) staff       (20)     2651 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/PKG-INFO
+-rw-r--r--   0 cyber      (501) staff       (20)      255 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber      (501) staff       (20)        1 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber      (501) staff       (20)        1 2019-01-06 11:25:53.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/not-zip-safe
+-rw-r--r--   0 cyber      (501) staff       (20)       39 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/requires.txt
+-rw-r--r--   0 cyber      (501) staff       (20)       14 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/Flask_Cognito.egg-info/top_level.txt
+-rw-r--r--   0 cyber      (501) staff       (20)     2651 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/PKG-INFO
+-rw-r--r--   0 cyber      (501) staff       (20)     1518 2019-01-08 12:34:51.000000 Flask-Cognito-1.9/README.md
+-rw-r--r--   0 cyber      (501) staff       (20)     5854 2019-01-08 12:42:22.000000 Flask-Cognito-1.9/flask_cognito.py
+-rw-r--r--   0 cyber      (501) staff       (20)       38 2019-01-08 12:42:51.000000 Flask-Cognito-1.9/setup.cfg
+-rw-r--r--   0 cyber      (501) staff       (20)     1226 2019-01-08 12:38:20.000000 Flask-Cognito-1.9/setup.py
```

### Comparing `Flask-Cognito-1.8/Flask_Cognito.egg-info/PKG-INFO` & `Flask-Cognito-1.9/Flask_Cognito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cognito
-Version: 1.8
+Version: 1.9
 Summary: Authenticate users to Cognito user pool via JWT.
 Home-page: https://github.com/jetbridge/flask-cognito
 Author: Mischa Spiegelmock
 Author-email: mischa@mvstg.biz
 License: ABRMS
 Description: Flask-Cognito
         -------------
```

### Comparing `Flask-Cognito-1.8/PKG-INFO` & `Flask-Cognito-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cognito
-Version: 1.8
+Version: 1.9
 Summary: Authenticate users to Cognito user pool via JWT.
 Home-page: https://github.com/jetbridge/flask-cognito
 Author: Mischa Spiegelmock
 Author-email: mischa@mvstg.biz
 License: ABRMS
 Description: Flask-Cognito
         -------------
```

### Comparing `Flask-Cognito-1.8/README.md` & `Flask-Cognito-1.9/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Cognito-1.8/flask_cognito.py` & `Flask-Cognito-1.9/flask_cognito.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.status_code = status_code
         self.headers = headers
 
     def __repr__(self):
         return f'CognitoAuthError: {self.error}'
 
     def __str__(self):
-        return f'{self.error} {self.description}'
+        return f'{self.error} - {self.description}'
 
 
 class CognitoAuth(object):
     def __init__(self, app=None):
         self.app = app
         if app is not None:
             self.init_app(app)
@@ -146,11 +146,11 @@
         raise CognitoAuthError('Authorization Required', f'Request does not contain a well-formed access token in the "{auth_header_name}" header beginning with "{auth_header_prefix}"')
 
     try:
         # check if token is signed by userpool
         payload = _cog.decode_token(token=token)
     except CognitoJWTException as e:
         log.exception(e)
-        raise CognitoAuthError('Invalid Cognito Authentication Token') from e
+        raise CognitoAuthError('Invalid Cognito Authentication Token', str(e)) from e
 
     _request_ctx_stack.top.cogauth_cognito_jwt = payload
     _request_ctx_stack.top.cogauth_current_user = _cog.get_user(payload)
```

### Comparing `Flask-Cognito-1.8/setup.py` & `Flask-Cognito-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='Flask-Cognito',
-    version='1.8',
+    version='1.9',
     url='https://github.com/jetbridge/flask-cognito',
     license='ABRMS',
     author='Mischa Spiegelmock',
     author_email='mischa@mvstg.biz',
     description='Authenticate users to Cognito user pool via JWT.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

