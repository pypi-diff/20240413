# Comparing `tmp/imas_tools-0.1.1.tar.gz` & `tmp/imas_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.1.1.tar", max compression
+gzip compressed data, was "imas_tools-0.1.2.tar", max compression
```

## Comparing `imas_tools-0.1.1.tar` & `imas_tools-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.1.1/imas_tools/__init__.py
--rw-r--r--   0        0        0     4124 2024-04-13 08:31:37.334472 imas_tools-0.1.1/imas_tools/recochoku.py
--rw-r--r--   0        0        0      416 2024-04-13 11:39:07.485442 imas_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.1.1/README.md
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 imas_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.1.2/imas_tools/__init__.py
+-rw-r--r--   0        0        0     4137 2024-04-13 12:02:24.253648 imas_tools-0.1.2/imas_tools/recochoku.py
+-rw-r--r--   0        0        0      416 2024-04-13 12:02:40.373424 imas_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 imas_tools-0.1.2/PKG-INFO
```

### Comparing `imas_tools-0.1.1/imas_tools/recochoku.py` & `imas_tools-0.1.2/imas_tools/recochoku.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests, json, re
-from typing import Dict, Any, TypedDict
+from typing import Dict, Any, TypedDict, Union
 from urllib.parse import quote
 from bs4 import BeautifulSoup
 
 class LyricMetadata(TypedDict):
     title: str
     artist: str
     composer: str
@@ -98,15 +98,15 @@
         "composer": composer,
         "lyricist": lyricist,
         "artist": artist,
         "lyrics": lyrics,
     }
 
 
-def get_lyrics_from_words(words: str | None):
+def get_lyrics_from_words(words: Union[str, None]):
     if words is None:
         return ""
     rtn = ""
     for word in json.loads(words):
         rtn += chr(word)
     return rtn
```

### Comparing `imas_tools-0.1.1/PKG-INFO` & `imas_tools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

