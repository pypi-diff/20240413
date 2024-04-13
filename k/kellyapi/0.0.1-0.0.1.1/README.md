# Comparing `tmp/kellyapi-0.0.1.tar.gz` & `tmp/kellyapi-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.1.tar", last modified: Sat Apr 13 13:21:29 2024, max compression
+gzip compressed data, was "kellyapi-0.0.1.1.tar", last modified: Sat Apr 13 13:31:03 2024, max compression
```

## Comparing `kellyapi-0.0.1.tar` & `kellyapi-0.0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:21:29.983453 kellyapi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 13:21:16.000000 kellyapi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-13 13:21:29.983453 kellyapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:21:16.000000 kellyapi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:21:29.983453 kellyapi-0.0.1/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:21:16.000000 kellyapi-0.0.1/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-13 13:21:16.000000 kellyapi-0.0.1/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:21:16.000000 kellyapi-0.0.1/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:21:29.983453 kellyapi-0.0.1/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-13 13:21:29.000000 kellyapi-0.0.1/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:21:29.000000 kellyapi-0.0.1/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:21:29.000000 kellyapi-0.0.1/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:21:29.000000 kellyapi-0.0.1/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:21:29.000000 kellyapi-0.0.1/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:21:29.983453 kellyapi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-13 13:21:16.000000 kellyapi-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:31:03.000000 kellyapi-0.0.1.1/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:31:03.724940 kellyapi-0.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-13 13:30:59.000000 kellyapi-0.0.1.1/setup.py
```

### Comparing `kellyapi-0.0.1/LICENSE` & `kellyapi-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1/PKG-INFO` & `kellyapi-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1/README.md` & `kellyapi-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1/kellyapi/api.py` & `kellyapi-0.0.1.1/kellyapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,43 +125,43 @@
             prompt=prompt,
             negative_prompt=negative_prompt,
             model=model,
             style=style,
             width=width,
             height=height,
         )
-        content = await self._post_data("generate", json=kwargs)
+        content = await self._post_data("generate", data=kwargs)
         image = BytesIO(content)
         image = "image.png"
         return image
 
     async def llm_models(self):
         content = await self._fetch("llm-models")
         return content
 
     async def llm(self, prompt: str, model: str = "ChatGPT", character: str = "KelyAI"):
         kwargs = dict(prompt=prompt, model=model, character=character)
-        content = await self._post_json("llm", json=kwargs)
+        content = await self._post_json("llm", data=kwargs)
         return content.message
 
     async def upscale(self, image: str):
         kwargs = dict(image=image)
-        content = await self._post_data("upscale", json=kwargs)
+        content = await self._post_data("upscale", data=kwargs)
         image = BytesIO(content)
         image = "image.png"
         return image
 
     async def voice_models(self):
         content = await self._fetch("voice-models")
         return content
 
     async def text2voice(self, text: str, model: str = "en-US_LisaExpressive"):
         kwargs = dict(text=text, model=model)
-        content = await self._post_data("text2voice", json=kwargs)
+        content = await self._post_data("text2voice", data=kwargs)
         image = BytesIO(content)
         image = "image.png"
         return image
 
     async def voice2text(self, audio: str):
         kwargs = dict(audio=audio)
-        content = await self._post_json("voice2text", json=kwargs)
+        content = await self._post_json("voice2text", data=kwargs)
         return content.result
```

### Comparing `kellyapi-0.0.1/kellyapi/errors.py` & `kellyapi-0.0.1.1/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.1/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.1.1/kellyapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.1/setup.py` & `kellyapi-0.0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.1",
+    version="0.0.1.1",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```

