# Comparing `tmp/aioxdl-0.0.16.tar.gz` & `tmp/aioxdl-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxdl-0.0.16.tar", last modified: Fri Apr 12 10:29:06 2024, max compression
+gzip compressed data, was "aioxdl-0.0.17.tar", last modified: Fri Apr 12 16:55:27 2024, max compression
```

## Comparing `aioxdl-0.0.16.tar` & `aioxdl-0.0.17.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.519681 aioxdl-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 10:28:59.000000 aioxdl-0.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:29:06.519681 aioxdl-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 10:28:59.000000 aioxdl-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.515681 aioxdl-0.0.16/aioxdl/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-12 10:28:59.000000 aioxdl-0.0.16/aioxdl/module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:29:06.519681 aioxdl-0.0.16/aioxdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 10:29:06.000000 aioxdl-0.0.16/aioxdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:29:06.519681 aioxdl-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 10:28:59.000000 aioxdl-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:27.977017 aioxdl-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 16:55:21.000000 aioxdl-0.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 16:55:27.977017 aioxdl-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 16:55:21.000000 aioxdl-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:27.977017 aioxdl-0.0.17/aioxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 16:55:21.000000 aioxdl-0.0.17/aioxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 16:55:21.000000 aioxdl-0.0.17/aioxdl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-12 16:55:21.000000 aioxdl-0.0.17/aioxdl/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 16:55:21.000000 aioxdl-0.0.17/aioxdl/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:27.977017 aioxdl-0.0.17/aioxdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 16:55:27.000000 aioxdl-0.0.17/aioxdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:55:27.977017 aioxdl-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-12 16:55:21.000000 aioxdl-0.0.17/setup.py
```

### Comparing `aioxdl-0.0.16/LICENSE` & `aioxdl-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.16/PKG-INFO` & `aioxdl-0.0.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.16
+Version: 0.0.17
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.16 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.17 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.16/README.md` & `aioxdl-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `aioxdl-0.0.16/aioxdl/module.py` & `aioxdl-0.0.17/aioxdl/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import os, time, aiohttp, asyncio
-from urllib.parse import unquote, urlparse
+import time, aiohttp, asyncio
+from aioxdl.scripts import Scripted
 from yt_dlp import YoutubeDL, DownloadError
 from aioxdl.functions import Hkeys, EXlogger
 #=================================================================================================
 
 class Downloader:
 
     def __init__(self, message=None):
         self.tsize = 0
         self.dsize = 0
         self.stime = 0
         self.error = None
         self.chunk = 1024
         self.imssg = message
-        self.etime = "ERROR : Timeout"
+        self.etime = Scripted.DATA01
+        self.comnd = {"quiet": True,  "no_warnings": True, "logger": EXlogger()}
 
 #=================================================================================================
 
     async def filename(self, filelink):
-        command = {"quiet": True,  "no_warnings": True, "logger": EXlogger()}
-        with YoutubeDL(command) as ydl:
+        with YoutubeDL(self.comnd) as ydl:
             try:
                 resultse = ydl.extract_info(filelink, download=False)
                 filename = ydl.prepare_filename(resultse, outtmpl=Hkeys.DATA01)
             except DownloadError:
                 filename = None
             except Exception:
                 filename = None
@@ -55,14 +55,15 @@
                         if not chunks:
                             break
                         handlexo.write(chunks)
                         self.dsize += self.chunk
                         try: await self.display(progress)
                         except Exception: pass
 
+                await response.release()
                 return location if location else None
 
 #=================================================================================================
 
     async def start(self, url, flocations, timeout=1000, progress=None):
         try:
             self.stime = time.time()
```

### Comparing `aioxdl-0.0.16/aioxdl.egg-info/PKG-INFO` & `aioxdl-0.0.17/aioxdl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioxdl
-Version: 0.0.16
+Version: 0.0.17
 Summary: Python fast downloader
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,downloader,aiohttp
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioxdl Version: 0.0.16 Summary: Python fast
+Metadata-Version: 2.1 Name: aioxdl Version: 0.0.17 Summary: Python fast
 downloader Home-page: https://github.com/Clinton-Abraham Author: Clinton-
 Abraham Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
 python,downloader,aiohttp Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `aioxdl-0.0.16/setup.py` & `aioxdl-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules']
 setup(
     name='aioxdl',
     license='MIT',
     zip_safe=False,
-    version='0.0.16',
+    version='0.0.17',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.9',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='Python fast downloader',
```

