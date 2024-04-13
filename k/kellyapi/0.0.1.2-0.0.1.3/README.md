# Comparing `tmp/kellyapi-0.0.1.2.tar.gz` & `tmp/kellyapi-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.1.2.tar", last modified: Sat Apr 13 13:52:02 2024, max compression
+gzip compressed data, was "kellyapi-0.0.1.3.tar", last modified: Sat Apr 13 14:26:47 2024, max compression
```

## Comparing `kellyapi-0.0.1.2.tar` & `kellyapi-0.0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:47.386553 kellyapi-0.0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 14:26:47.386553 kellyapi-0.0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:47.386553 kellyapi-0.0.1.3/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:47.386553 kellyapi-0.0.1.3/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 14:26:47.000000 kellyapi-0.0.1.3/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 14:26:47.000000 kellyapi-0.0.1.3/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:26:47.000000 kellyapi-0.0.1.3/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 14:26:47.000000 kellyapi-0.0.1.3/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 14:26:47.000000 kellyapi-0.0.1.3/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:26:47.386553 kellyapi-0.0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 14:26:40.000000 kellyapi-0.0.1.3/setup.py
```

### Comparing `kellyapi-0.0.1.2/LICENSE` & `kellyapi-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.2/PKG-INFO` & `kellyapi-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.2/README.md` & `kellyapi-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.2/kellyapi/api.py` & `kellyapi-0.0.1.3/kellyapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     async def _fetch(self, route, timeout=60, **params):
         try:
             async with self.session() as client:
                 resp = await client.get(
                     self.api + route,
                     params=params,
-                    headers={"X-Kelly-KEY": self.api_key},
+                    headers={"Kelly-API-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
@@ -53,16 +53,16 @@
         return self._parse_result(response)
 
     async def _post_json(self, route, data, timeout=60):
         try:
             async with self.session() as client:
                 resp = await client.post(
                     self.api + route,
-                    data=data,
-                    headers={"X-Kelly-KEY": self.api_key},
+                    json=data,
+                    headers={"Kelly-API-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
@@ -77,16 +77,16 @@
         return self._parse_result(response)
 
     async def _post_data(self, route, data, timeout=60):
         try:
             async with self.session() as client:
                 resp = await client.post(
                     self.api + route,
-                    data=data,
-                    headers={"X-Kelly-KEY": self.api_key},
+                    json=data,
+                    headers={"Kelly-API-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
```

### Comparing `kellyapi-0.0.1.2/kellyapi/errors.py` & `kellyapi-0.0.1.3/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.2/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.1.3/kellyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.2/setup.py` & `kellyapi-0.0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.1.2",
+    version="0.0.1.3",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

