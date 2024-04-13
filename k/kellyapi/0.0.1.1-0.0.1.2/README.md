# Comparing `tmp/kellyapi-0.0.1.1.tar.gz` & `tmp/kellyapi-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.1.1.tar", last modified: Sat Apr 13 13:31:03 2024, max compression
+gzip compressed data, was "kellyapi-0.0.1.2.tar", last modified: Sat Apr 13 13:52:02 2024, max compression
```

## Comparing `kellyapi-0.0.1.1.tar` & `kellyapi-0.0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:52:02.000000 kellyapi-0.0.1.2/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:52:02.569789 kellyapi-0.0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 13:51:57.000000 kellyapi-0.0.1.2/setup.py
```

### Comparing `kellyapi-0.0.1.1/LICENSE` & `kellyapi-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.1/PKG-INFO` & `kellyapi-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.1/README.md` & `kellyapi-0.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.1/kellyapi/api.py` & `kellyapi-0.0.1.2/kellyapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     self.api + route,
                     params=params,
                     headers={"X-Kelly-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
-                        "Invalid API key, Get an api key from @ARQRobot"
+                        "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
                     raise ConnectionError()
                 response = await resp.json()
         except asyncio.TimeoutError:
             raise TimeoutError
         except ContentTypeError:
@@ -59,15 +59,15 @@
                     self.api + route,
                     data=data,
                     headers={"X-Kelly-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
-                        "Invalid API key, Get an api key from @ARQRobot"
+                        "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
                     raise ConnectionError()
                 response = await resp.json()
         except asyncio.TimeoutError:
             raise TimeoutError
         except ContentTypeError:
@@ -83,15 +83,15 @@
                     self.api + route,
                     data=data,
                     headers={"X-Kelly-KEY": self.api_key},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
-                        "Invalid API key, Get an api key from @ARQRobot"
+                        "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
                     raise ConnectionError()
                 response = await resp.read()
         except asyncio.TimeoutError:
             raise TimeoutError
         except ContentTypeError:
@@ -154,14 +154,14 @@
         content = await self._fetch("voice-models")
         return content
 
     async def text2voice(self, text: str, model: str = "en-US_LisaExpressive"):
         kwargs = dict(text=text, model=model)
         content = await self._post_data("text2voice", data=kwargs)
         image = BytesIO(content)
-        image = "image.png"
+        image = "voice.ogg"
         return image
 
     async def voice2text(self, audio: str):
         kwargs = dict(audio=audio)
         content = await self._post_json("voice2text", data=kwargs)
         return content.result
```

### Comparing `kellyapi-0.0.1.1/kellyapi/errors.py` & `kellyapi-0.0.1.2/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1.1/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.1.2/kellyapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1.1/setup.py` & `kellyapi-0.0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.1.1",
+    version="0.0.1.2",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

