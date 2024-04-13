# Comparing `tmp/agenius-4.0.1.post1.tar.gz` & `tmp/agenius-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenius-4.0.1.post1.tar", last modified: Fri Jun  3 22:03:37 2022, max compression
+gzip compressed data, was "agenius-4.0.2.tar", last modified: Sat Apr 13 12:39:49 2024, max compression
```

## Comparing `agenius-4.0.1.post1.tar` & `agenius-4.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dopebnan  (1000) dopebnan  (1000)        0 2022-06-03 22:03:37.194920 agenius-4.0.1.post1/
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)    35149 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/COPYING
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     7652 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/COPYING.LESSER
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     1070 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/COPYING.ORIGINAL.txt
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      398 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/LICENSE.md
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      105 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/MANIFEST.in
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     4334 2022-06-03 22:03:37.194920 agenius-4.0.1.post1/PKG-INFO
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     3287 2022-06-03 21:30:13.000000 agenius-4.0.1.post1/README.md
-drwxrwxr-x   0 dopebnan  (1000) dopebnan  (1000)        0 2022-06-03 22:03:37.190920 agenius-4.0.1.post1/agenius/
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      298 2022-06-03 21:51:33.000000 agenius-4.0.1.post1/agenius/__init__.py
-drwxrwxr-x   0 dopebnan  (1000) dopebnan  (1000)        0 2022-06-03 22:03:37.190920 agenius-4.0.1.post1/agenius/api_calls/
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)       61 2022-06-03 21:51:23.000000 agenius-4.0.1.post1/agenius/api_calls/__init__.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     3685 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/agenius/api_calls/api.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     2295 2022-06-03 21:47:43.000000 agenius-4.0.1.post1/agenius/api_calls/base.py
-drwxrwxr-x   0 dopebnan  (1000) dopebnan  (1000)        0 2022-06-03 22:03:37.194920 agenius-4.0.1.post1/agenius/class_types/
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)       97 2022-06-03 21:51:33.000000 agenius-4.0.1.post1/agenius/class_types/__init__.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     1492 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/agenius/class_types/album.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     1322 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/agenius/class_types/artist.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      583 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/agenius/class_types/base.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     1636 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/agenius/class_types/song.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      111 2022-06-03 21:31:45.000000 agenius-4.0.1.post1/agenius/errors.py
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     6442 2022-06-03 21:42:46.000000 agenius-4.0.1.post1/agenius/main.py
-drwxrwxr-x   0 dopebnan  (1000) dopebnan  (1000)        0 2022-06-03 22:03:37.190920 agenius-4.0.1.post1/agenius.egg-info/
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     4334 2022-06-03 22:03:36.000000 agenius-4.0.1.post1/agenius.egg-info/PKG-INFO
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)      536 2022-06-03 22:03:37.000000 agenius-4.0.1.post1/agenius.egg-info/SOURCES.txt
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)        1 2022-06-03 22:03:36.000000 agenius-4.0.1.post1/agenius.egg-info/dependency_links.txt
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)       40 2022-06-03 22:03:37.000000 agenius-4.0.1.post1/agenius.egg-info/requires.txt
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)        8 2022-06-03 22:03:37.000000 agenius-4.0.1.post1/agenius.egg-info/top_level.txt
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)       85 2022-06-03 21:15:30.000000 agenius-4.0.1.post1/pyproject.toml
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)       38 2022-06-03 22:03:37.194920 agenius-4.0.1.post1/setup.cfg
--rw-rw-r--   0 dopebnan  (1000) dopebnan  (1000)     1335 2022-06-03 22:01:18.000000 agenius-4.0.1.post1/setup.py
+drwxr-xr-x   0 dopebnan  (1000) wheel      (998)        0 2024-04-13 12:39:49.330178 agenius-4.0.2/
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)    35149 2023-10-13 00:33:01.000000 agenius-4.0.2/COPYING
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     7652 2023-10-13 00:33:01.000000 agenius-4.0.2/COPYING.LESSER
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     1070 2023-10-13 00:33:01.000000 agenius-4.0.2/COPYING.ORIGINAL.txt
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      398 2023-10-13 00:33:01.000000 agenius-4.0.2/LICENSE.md
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      105 2023-10-13 00:33:01.000000 agenius-4.0.2/MANIFEST.in
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     4399 2024-04-13 12:39:49.330178 agenius-4.0.2/PKG-INFO
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     3287 2023-10-13 00:33:01.000000 agenius-4.0.2/README.md
+drwxr-xr-x   0 dopebnan  (1000) wheel      (998)        0 2024-04-13 12:39:49.330178 agenius-4.0.2/agenius/
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      298 2024-04-13 12:28:03.000000 agenius-4.0.2/agenius/__init__.py
+drwxr-xr-x   0 dopebnan  (1000) wheel      (998)        0 2024-04-13 12:39:49.330178 agenius-4.0.2/agenius/api_calls/
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)       61 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/api_calls/__init__.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     3685 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/api_calls/api.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     2295 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/api_calls/base.py
+drwxr-xr-x   0 dopebnan  (1000) wheel      (998)        0 2024-04-13 12:39:49.330178 agenius-4.0.2/agenius/class_types/
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)       97 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/class_types/__init__.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     1492 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/class_types/album.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     1310 2024-04-13 12:13:11.000000 agenius-4.0.2/agenius/class_types/artist.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      583 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/class_types/base.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     1638 2024-04-13 12:34:17.000000 agenius-4.0.2/agenius/class_types/song.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      111 2023-10-13 00:33:01.000000 agenius-4.0.2/agenius/errors.py
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     6486 2024-04-13 12:31:18.000000 agenius-4.0.2/agenius/main.py
+drwxr-xr-x   0 dopebnan  (1000) wheel      (998)        0 2024-04-13 12:39:49.330178 agenius-4.0.2/agenius.egg-info/
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     4399 2024-04-13 12:39:49.000000 agenius-4.0.2/agenius.egg-info/PKG-INFO
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)      536 2024-04-13 12:39:49.000000 agenius-4.0.2/agenius.egg-info/SOURCES.txt
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)        1 2024-04-13 12:39:49.000000 agenius-4.0.2/agenius.egg-info/dependency_links.txt
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)       40 2024-04-13 12:39:49.000000 agenius-4.0.2/agenius.egg-info/requires.txt
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)        8 2024-04-13 12:39:49.000000 agenius-4.0.2/agenius.egg-info/top_level.txt
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)       85 2023-10-13 00:33:01.000000 agenius-4.0.2/pyproject.toml
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)       38 2024-04-13 12:39:49.330178 agenius-4.0.2/setup.cfg
+-rw-r--r--   0 dopebnan  (1000) wheel      (998)     1331 2024-04-13 12:28:03.000000 agenius-4.0.2/setup.py
```

### Comparing `agenius-4.0.1.post1/COPYING` & `agenius-4.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/COPYING.LESSER` & `agenius-4.0.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/COPYING.ORIGINAL.txt` & `agenius-4.0.2/COPYING.ORIGINAL.txt`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/PKG-INFO` & `agenius-4.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: agenius
-Version: 4.0.1.post1
+Version: 4.0.2
 Summary: A LyricsGenius fork with async ready features.
 Home-page: https://github.com/dopebnan/AGenius.py
 Author: dopebnan
 Author-email: 82271322+dopebnan@users.noreply.github.com
-License: LGPLv3
+License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/dopebnan/AGenius.py/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Software Development :: Libraries
@@ -18,14 +18,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: COPYING.ORIGINAL.txt
+Requires-Dist: beautifulsoup4>=4.6.0
+Requires-Dist: aiohttp<4,>=3.6.0
 
 <div align="center">
 
 # AGenius.py
 
 [![Latest Release](https://img.shields.io/pypi/v/agenius?color=brightgreen&label=%20)](https://github.com/dopebnan/AGenius.py/releases "Releases")
 ![Python Version](https://img.shields.io/pypi/pyversions/agenius)
```

### Comparing `agenius-4.0.1.post1/README.md` & `agenius-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/agenius/api_calls/api.py` & `agenius-4.0.2/agenius/api_calls/api.py`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/agenius/api_calls/base.py` & `agenius-4.0.2/agenius/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/agenius/class_types/album.py` & `agenius-4.0.2/agenius/class_types/album.py`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/agenius/class_types/artist.py` & `agenius-4.0.2/agenius/class_types/artist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Copyright (c) 2018, 2020, 2021 John W. Miller
+Copyright (c) 2023 John W. Miller
 Originally part of LyricsGenius, licensed under the MIT License.
 
-Copyright (C) 2022 dopebnan
+Copyright (C) 2024 dopebnan
 This file is part of AGenius.py.
 You should have received a copy of the GNU Lesser General Public License along with AGenius.py.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 from .base import BaseEntity
```

### Comparing `agenius-4.0.1.post1/agenius/class_types/base.py` & `agenius-4.0.2/agenius/class_types/base.py`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/agenius/class_types/song.py` & `agenius-4.0.2/agenius/class_types/song.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Copyright (c) 2018, 2020, 2021 John W. Miller
+Copyright (c) 2023 John W. Miller
 Originally part of LyricsGenius, licensed under the MIT License.
 
-Copyright (C) 2022 dopebnan
+Copyright (C) 2024 dopebnan
 This file is part of AGenius.py.
 You should have received a copy of the GNU Lesser General Public License along with AGenius.py.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 import json
 from filecmp import cmp
@@ -47,10 +47,12 @@
         lyr = self.lyrics[:100]
         if len(self.lyrics) > 100:
             lyr += "…"
         lyr.replace('\n', '\n    ')
         return f"{self.title} by {self.artist}:\n    {lyr}"
 
     def __cmp__(self, other):
-        return (cmp(self.title, other.title)
-                and cmp(self.artist, other.artist)
-                and cmp(self.lyrics, other.lyrics))
+        return (
+            cmp(self.title, other.title) and
+            cmp(self.artist, other.artist) and
+            cmp(self.lyrics, other.lyrics)
+        )
```

### Comparing `agenius-4.0.1.post1/agenius/main.py` & `agenius-4.0.2/agenius/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-Copyright (c) 2018, 2020, 2021 John W. Miller
+Copyright (c) 2023 John W. Miller
 Originally part of LyricsGenius, licensed under the MIT License.
 
 
-Copyright (C) 2022 dopebnan
+Copyright (C) 2024 dopebnan
 This file is part of AGenius.py.
 
 AGenius.py is free software: you can redistribute it and/or modify it under the terms of
 the GNU Lesser General Public License as published by the Free Software Foundation,
 either version 3 of the License, or any later version.
 
 AGenius.py is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
@@ -42,16 +42,18 @@
         return title_is_match
     result_artist = unicodedata.normalize("NFKD", result["primary_artist"]["name"])
     return title_is_match and result_artist == unicodedata.normalize("NFKD", artist)
 
 
 class Genius(API):
     """Main class that makes the requests. Inherits from the API class."""
-    default_ex_terms = [r"track\s?list", "album art(work)?", "liner notes", "booklet", "credits", "interview", "skit",
-                        "instrumental", "setlist"]
+    default_ex_terms = [
+        r"track\s?list", "album art(work)?", "liner notes", "booklet", "credits",
+        "interview", "skit", "instrumental", "setlist"
+    ]
 
     def __init__(self, access_token, verbose=True, retries=0):
         """
         User-level interface with the Genius.com API.
 
         :param access_token: str, API key provided by Genius
         :param verbose: bool, turn logs on/off
@@ -132,23 +134,23 @@
         response = await self._make_request_web(song_url)
         html = BeautifulSoup(
             response.replace('<br/>', '\n'),
             "html.parser"
         )
 
         # Determine the class of the div
-        div = html.find("div", class_=re.compile("^lyrics$|Lyrics__Root"))
-        if div is None:
+        divs = html.find_all("div", class_=re.compile("^lyrics$|Lyrics__Container"))
+        if divs is None or len(divs) <= 0:
             if self.verbose:
                 print("Couldn't find the lyrics section. "
                       "Please report this if the song has lyrics.\n"
                       f"Song URL: {song_url}")
             return None
 
-        lyrics = div.get_text()
+        lyrics = "\n".join([div.get_text() for div in divs])
         return lyrics.strip("\n")
 
     async def search_song(self, title=None, artist="", song_id=None):
         """
         Searches for a specific song.
 
         You must pass either the title or song id.
```

### Comparing `agenius-4.0.1.post1/agenius.egg-info/PKG-INFO` & `agenius-4.0.2/agenius.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: agenius
-Version: 4.0.1.post1
+Version: 4.0.2
 Summary: A LyricsGenius fork with async ready features.
 Home-page: https://github.com/dopebnan/AGenius.py
 Author: dopebnan
 Author-email: 82271322+dopebnan@users.noreply.github.com
-License: LGPLv3
+License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/dopebnan/AGenius.py/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Software Development :: Libraries
@@ -18,14 +18,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING
 License-File: COPYING.LESSER
 License-File: COPYING.ORIGINAL.txt
+Requires-Dist: beautifulsoup4>=4.6.0
+Requires-Dist: aiohttp<4,>=3.6.0
 
 <div align="center">
 
 # AGenius.py
 
 [![Latest Release](https://img.shields.io/pypi/v/agenius?color=brightgreen&label=%20)](https://github.com/dopebnan/AGenius.py/releases "Releases")
 ![Python Version](https://img.shields.io/pypi/pyversions/agenius)
```

### Comparing `agenius-4.0.1.post1/agenius.egg-info/SOURCES.txt` & `agenius-4.0.2/agenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agenius-4.0.1.post1/setup.py` & `agenius-4.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="agenius",
-    version="4.0.1.rev1",
+    version="4.0.2",
     description="A LyricsGenius fork with async ready features.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dopebnan/AGenius.py",
     project_urls={
         "Bug Tracker": "https://github.com/dopebnan/AGenius.py/issues"
     },
     author="dopebnan",
     author_email="82271322+dopebnan@users.noreply.github.com",
-    license="LGPLv3",
+    license="LGPLv3+",
     packages=["agenius", "agenius.api_calls", "agenius.class_types"],
     python_requires=">=3.7",
     install_requires=[
         "beautifulsoup4>=4.6.0",
         "aiohttp>=3.6.0,<4",
     ],
     classifiers=[
```

