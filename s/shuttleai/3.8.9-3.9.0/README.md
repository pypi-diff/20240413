# Comparing `tmp/shuttleai-3.8.9.tar.gz` & `tmp/shuttleai-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.9.tar", last modified: Sat Apr  6 16:45:19 2024, max compression
+gzip compressed data, was "shuttleai-3.9.0.tar", last modified: Sat Apr 13 20:33:18 2024, max compression
```

## Comparing `shuttleai-3.8.9.tar` & `shuttleai-3.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:45:19.759038 shuttleai-3.8.9/
--rw-rw-rw-   0        0        0     4116 2024-04-06 16:45:19.757038 shuttleai-3.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 16:45:19.759038 shuttleai-3.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1274 2024-04-06 16:44:02.000000 shuttleai-3.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:45:19.705037 shuttleai-3.8.9/shuttleai/
--rw-rw-rw-   0        0        0      586 2024-04-06 16:43:12.000000 shuttleai-3.8.9/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.9/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:45:19.750041 shuttleai-3.8.9/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.9/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17305 2024-04-06 16:44:30.000000 shuttleai-3.8.9/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15216 2024-04-06 16:44:27.000000 shuttleai-3.8.9/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.9/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:45:19.753038 shuttleai-3.8.9/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.9/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.9/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:45:19.755040 shuttleai-3.8.9/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4116 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-06 16:45:19.000000 shuttleai-3.8.9/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.571834 shuttleai-3.9.0/
+-rw-rw-rw-   0        0        0     4116 2024-04-13 20:33:18.568831 shuttleai-3.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 20:33:18.572840 shuttleai-3.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2024-04-13 20:32:36.000000 shuttleai-3.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.540833 shuttleai-3.9.0/shuttleai/
+-rw-rw-rw-   0        0        0      586 2024-04-06 16:43:12.000000 shuttleai-3.9.0/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.9.0/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.560840 shuttleai-3.9.0/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.9.0/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17395 2024-04-13 20:32:43.000000 shuttleai-3.9.0/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15216 2024-04-06 16:44:27.000000 shuttleai-3.9.0/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.9.0/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.565834 shuttleai-3.9.0/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.9.0/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.9.0/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:33:18.566831 shuttleai-3.9.0/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4116 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-13 20:33:18.000000 shuttleai-3.9.0/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.9/PKG-INFO` & `shuttleai-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.9
+Version: 3.9.0
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shuttleai-3.8.9/README.md` & `shuttleai-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/setup.py` & `shuttleai-3.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text(encoding="utf-8")
 
 setup(
     include_package_data=True,
     name='shuttleai', 
-    version='3.8.9',
+    version='3.9.0',
     author='shuttle',
     author_email='noreply@shuttleai.app',
     description="Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai",
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages(),
     classifiers=[
```

### Comparing `shuttleai-3.8.9/shuttleai/__init__.py` & `shuttleai-3.9.0/shuttleai/__init__.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/shuttleai/cli.py` & `shuttleai-3.9.0/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/shuttleai/client/_async.py` & `shuttleai-3.9.0/shuttleai/client/_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 @Author: ShuttleAI
-@Date: 4-6-2024
+@Date: 4-13-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
     Union,
@@ -306,15 +306,16 @@
             log.error(f"Failed to get chat completions: {e}")
             raise
 
     async def images_generations(
         self,
         model: str,
         prompt: str,
-        n: int = 1
+        n: int = 1,
+        **kwargs
     ) -> Union[Image, ShuttleError]:
         """
         Generate images using a model.
 
         Args:
             model (str): The model name.
             prompt (str): The prompt for image generation.
@@ -324,15 +325,15 @@
             Image: The generated image.
 
         Raises:
             ShuttleError: If the API request fails.
             Aiohttp.ClientError: If the API request is invalid.
         """
         try:
-            data = {"model": model, "prompt": prompt, "n": n}
+            data = {"model": model, "prompt": prompt, "n": n, **kwargs}
             response = await self._make_request(
                 "POST", "images/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
                 return Image.from_dict(response)
             except:
                 try:
@@ -342,16 +343,17 @@
         except aiohttp.ClientError as e:
             log.error(f"Failed to generate images: {e}")
             raise
 
     async def audio_generations(
         self,
         input: str,
-        voice: str,
-        model: str = "ElevenLabs"
+        voice: str = None,
+        model: str = "eleven-labs",
+        **kwargs
     ) -> Union[Audio, ShuttleError]:
         """
         Generate audio using a model.
 
         Args:
             input (str): The input for audio generation.
             voice (str): The desired voice for the audio.
@@ -361,15 +363,15 @@
             Audio: The generated audio.
 
         Raises:
             ShuttleError: If the API request fails.
             Aiohttp.ClientError: If the API request is invalid.
         """
         try:
-            data = {"model": model, "input": input, "voice": voice}
+            data = {"model": model, "input": input, **({"voice": voice} if voice else {}), **kwargs}
             response = await self._make_request(
                 "POST", "audio/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
                 return Audio.from_dict(response)
             except:
                 try:
```

### Comparing `shuttleai-3.8.9/shuttleai/client/_sync.py` & `shuttleai-3.9.0/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/shuttleai/log.py` & `shuttleai-3.9.0/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/shuttleai/schemas/schemas.py` & `shuttleai-3.9.0/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.9/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.9.0/shuttleai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.9
+Version: 3.9.0
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

