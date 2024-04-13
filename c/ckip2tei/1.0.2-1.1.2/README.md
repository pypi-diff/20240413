# Comparing `tmp/ckip2tei-1.0.2.tar.gz` & `tmp/ckip2tei-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckip2tei-1.0.2.tar", max compression
+gzip compressed data, was "ckip2tei-1.1.2.tar", max compression
```

## Comparing `ckip2tei-1.0.2.tar` & `ckip2tei-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-03-18 09:02:38.663405 ckip2tei-1.0.2/LICENSE
--rw-r--r--   0        0        0     3725 2023-03-18 09:02:38.663526 ckip2tei-1.0.2/README.md
--rw-r--r--   0        0        0       66 2023-03-18 09:02:38.663662 ckip2tei-1.0.2/ckip2tei/__init__.py
--rw-r--r--   0        0        0       54 2023-03-18 09:02:38.663806 ckip2tei-1.0.2/ckip2tei/ckip/__init__.py
--rw-r--r--   0        0        0       55 2023-03-18 09:02:38.663966 ckip2tei-1.0.2/ckip2tei/ckip/model/__init__.py
--rw-r--r--   0        0        0     1385 2023-03-18 09:02:38.664072 ckip2tei-1.0.2/ckip2tei/ckip/model/ckip.py
--rw-r--r--   0        0        0     1607 2023-03-18 09:02:38.664179 ckip2tei-1.0.2/ckip2tei/ckip/segmenter.py
--rw-r--r--   0        0        0       60 2023-03-18 09:02:38.664319 ckip2tei-1.0.2/ckip2tei/ckip/transformer/__init__.py
--rw-r--r--   0        0        0     1184 2023-03-18 09:02:38.664425 ckip2tei-1.0.2/ckip2tei/ckip/transformer/transformer.py
--rw-r--r--   0        0        0      116 2023-03-18 09:02:38.664560 ckip2tei-1.0.2/ckip2tei/config/__init__.py
--rw-r--r--   0        0        0      506 2023-03-18 09:02:38.664648 ckip2tei-1.0.2/ckip2tei/config/ckip.py
--rw-r--r--   0        0        0       66 2023-03-18 09:02:38.664781 ckip2tei-1.0.2/ckip2tei/tei/__init__.py
--rw-r--r--   0        0        0       67 2023-03-18 09:02:38.664958 ckip2tei-1.0.2/ckip2tei/tei/tags/body/__init__.py
--rw-r--r--   0        0        0     1952 2023-03-18 09:33:56.897986 ckip2tei-1.0.2/ckip2tei/tei/tags/body/body.py
--rw-r--r--   0        0        0      296 2023-03-18 09:02:38.665386 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/__init__.py
--rw-r--r--   0        0        0     1115 2023-03-18 09:02:38.665499 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/base.py
--rw-r--r--   0        0        0      181 2023-03-18 09:02:38.665634 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/cleaners/__init__.py
--rw-r--r--   0        0        0      204 2023-03-18 09:02:38.665728 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/cleaners/base.py
--rw-r--r--   0        0        0     1145 2023-03-18 09:11:37.714396 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/cleaners/cleaners.py
--rw-r--r--   0        0        0     1485 2023-03-18 09:28:23.451033 ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/taggers.py
--rw-r--r--   0        0        0       69 2023-03-18 09:02:38.666064 ckip2tei-1.0.2/ckip2tei/tei/tags/head/__init__.py
--rw-r--r--   0        0        0     1066 2023-03-18 09:02:38.666179 ckip2tei-1.0.2/ckip2tei/tei/tags/head/head.py
--rw-r--r--   0        0        0     1742 2023-03-18 09:02:38.666285 ckip2tei-1.0.2/ckip2tei/tei/tei.py
--rw-r--r--   0        0        0       96 2023-03-18 09:02:38.666408 ckip2tei-1.0.2/ckip2tei/tei/utils/__init__.py
--rw-r--r--   0        0        0     1322 2023-03-18 09:02:38.666493 ckip2tei-1.0.2/ckip2tei/tei/utils/body.py
--rw-r--r--   0        0        0      407 2023-03-18 09:02:38.666569 ckip2tei-1.0.2/ckip2tei/tei/utils/date.py
--rw-r--r--   0        0        0      711 2023-03-18 09:38:01.237682 ckip2tei-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 ckip2tei-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-13 08:20:39.070323 ckip2tei-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3710 2024-04-13 09:34:53.479456 ckip2tei-1.1.2/README.md
+-rw-r--r--   0        0        0       66 2024-04-13 08:20:39.070665 ckip2tei-1.1.2/ckip2tei/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-13 08:20:39.070858 ckip2tei-1.1.2/ckip2tei/ckip/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-13 08:20:39.071035 ckip2tei-1.1.2/ckip2tei/ckip/model/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-13 09:34:53.479770 ckip2tei-1.1.2/ckip2tei/ckip/model/ckip.py
+-rw-r--r--   0        0        0     1607 2024-04-13 08:20:39.071426 ckip2tei-1.1.2/ckip2tei/ckip/segmenter.py
+-rw-r--r--   0        0        0       60 2024-04-13 08:20:39.071646 ckip2tei-1.1.2/ckip2tei/ckip/transformer/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-13 08:20:39.071786 ckip2tei-1.1.2/ckip2tei/ckip/transformer/transformer.py
+-rw-r--r--   0        0        0       54 2024-04-13 09:34:53.480055 ckip2tei-1.1.2/ckip2tei/config/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-13 09:34:53.480317 ckip2tei-1.1.2/ckip2tei/config/environment.py
+-rw-r--r--   0        0        0       66 2024-04-13 08:20:39.072872 ckip2tei-1.1.2/ckip2tei/tei/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-13 08:20:39.073099 ckip2tei-1.1.2/ckip2tei/tei/tags/body/__init__.py
+-rw-r--r--   0        0        0     1952 2024-04-13 08:20:39.073215 ckip2tei-1.1.2/ckip2tei/tei/tags/body/body.py
+-rw-r--r--   0        0        0      296 2024-04-13 08:20:39.073379 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/__init__.py
+-rw-r--r--   0        0        0     1115 2024-04-13 08:20:39.073498 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/base.py
+-rw-r--r--   0        0        0      181 2024-04-13 08:20:39.073669 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/cleaners/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-13 08:20:39.073778 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/cleaners/base.py
+-rw-r--r--   0        0        0     1145 2024-04-13 08:20:39.073909 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/cleaners/cleaners.py
+-rw-r--r--   0        0        0     1485 2024-04-13 08:20:39.074018 ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/taggers.py
+-rw-r--r--   0        0        0       69 2024-04-13 08:20:39.074177 ckip2tei-1.1.2/ckip2tei/tei/tags/head/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-13 08:20:39.074298 ckip2tei-1.1.2/ckip2tei/tei/tags/head/head.py
+-rw-r--r--   0        0        0     1667 2024-04-13 09:34:53.480633 ckip2tei-1.1.2/ckip2tei/tei/tei.py
+-rw-r--r--   0        0        0       96 2024-04-13 08:20:39.074594 ckip2tei-1.1.2/ckip2tei/tei/utils/__init__.py
+-rw-r--r--   0        0        0     1322 2024-04-13 08:20:39.074700 ckip2tei-1.1.2/ckip2tei/tei/utils/body.py
+-rw-r--r--   0        0        0      407 2024-04-13 08:20:39.074805 ckip2tei-1.1.2/ckip2tei/tei/utils/date.py
+-rw-r--r--   0        0        0     3359 2024-04-13 09:36:19.960454 ckip2tei-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 ckip2tei-1.1.2/PKG-INFO
```

### Comparing `ckip2tei-1.0.2/LICENSE` & `ckip2tei-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/README.md` & `ckip2tei-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 - `media`: the source of the data
 
 The `post_data` argument should be in the following format:
 
 ```python
 {
     "board": "Soft_Job",
-    "post_id": "ABCD",
+    "id": "ABCD",
     "date": "1183186255",
     "title": "[請益] 最愛的程式?",
     "author": "Retr0327",
     "body": "這是一篇測試文章\n我喜歡 Python 和 TypeScript",
     "post_vote": {"推 (pos)": 2, "噓 (neg)": 0, "→ (neu)": 0},
     "comments": [
         {
@@ -62,15 +62,15 @@
 
 After filling the arguments, do it as follows:
 
 
 ```python
 post_data = {
     "board": "Soft_Job",
-    "post_id": "ABCD",
+    "id": "ABCD",
     "date": "1183186255",
     "title": "[請益] 最愛的程式?",
     "author": "Retr0327",
     "body": "這是一篇測試文章\n我喜歡 Python 和 TypeScript",
     "post_vote": {"推 (pos)": 2, "噓 (neg)": 0, "→ (neu)": 0},
     "comments": [
         {
@@ -94,15 +94,15 @@
 This prints:
 
 ```xml
 <TEI.2>
    <teiHeader>
       <metadata name="media">ptt</metadata>
       <metadata name="author">Retr0327</metadata>
-      <metadata name="post_id">ABCD</metadata>
+      <metadata name="id">ABCD</metadata>
       <metadata name="year">2007</metadata>
       <metadata name="board">Soft_Job</metadata>
       <metadata name="title">[請益] 最愛的程式?</metadata>
    </teiHeader>
    <text>
       <title author="Retr0327">
          <s>
```

### Comparing `ckip2tei-1.0.2/ckip2tei/ckip/model/ckip.py` & `ckip2tei-1.1.2/ckip2tei/ckip/model/ckip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-from dataclasses import (
-    dataclass,
-    field,
-)
+from dataclasses import dataclass
 from pathlib import Path
 import pickle
 
-from ckip2tei.config import (
-    CKIP_DIR,
-    CKIP_PATH,
-    NLP_MODEL,
-)
+from ckip2tei.config import config
 
 
-@dataclass(frozen=True, slots=True)
+@dataclass
 class CKIPClient:
     """
     The CKIPClient object connects to ckip drivers.
     """
 
-    _ckip_path: str = field(init=False, default=CKIP_PATH)
-    _nlp_model: str = field(init=False, default=NLP_MODEL)
-
     def __post_init__(self) -> None:
         self.on_ready()
 
     def on_ready(self) -> None:
         """The on_ready method initializes and caches the CKIP drivers."""
-        has_path = Path(self._ckip_path).exists()
+        has_path = Path(config.ckip_drivers_path).exists()
 
         if not has_path:
             from ckip_transformers.nlp import (
                 CkipPosTagger,
                 CkipWordSegmenter,
             )
 
-            Path(CKIP_DIR).mkdir(parents=True, exist_ok=True)
+            Path(config.ckip_dir).mkdir(parents=True, exist_ok=True)
             drivers = (
-                CkipWordSegmenter(model=self._nlp_model),
-                CkipPosTagger(model=self._nlp_model),
+                CkipWordSegmenter(model=config.nlp_model),
+                CkipPosTagger(model=config.nlp_model),
             )
 
-            with open(rf"{self._ckip_path}", "wb") as file:
+            with open(rf"{config.ckip_drivers_path}", "wb") as file:
                 pickle.dump(drivers, file)
 
     def connect(self) -> tuple:
         """The connect method connects to the ckip drivers.
 
         Returns:
             a tuple that contains CkipWordSegmenter and CkipPosTagger.
         """
-        with open(self._ckip_path, "rb") as file:
+        with open(config.ckip_drivers_path, "rb") as file:
             return pickle.load(file)
```

### Comparing `ckip2tei-1.0.2/ckip2tei/ckip/segmenter.py` & `ckip2tei-1.1.2/ckip2tei/ckip/segmenter.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/ckip/transformer/transformer.py` & `ckip2tei-1.1.2/ckip2tei/ckip/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tags/body/body.py` & `ckip2tei-1.1.2/ckip2tei/tei/tags/body/body.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/base.py` & `ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/base.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/cleaners/cleaners.py` & `ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/cleaners/cleaners.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tags/body/taggers/taggers.py` & `ckip2tei-1.1.2/ckip2tei/tei/tags/body/taggers/taggers.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tags/head/head.py` & `ckip2tei-1.1.2/ckip2tei/tei/tags/head/head.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/tei.py` & `ckip2tei-1.1.2/ckip2tei/tei/tei.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 import asyncio
-from typing import Literal
 from xml.dom import minidom
 import xml.etree.ElementTree as ET
 
 from .tags.body import create_body_tags
 from .tags.head import create_header_tag
 from .utils import get_year
 
 PostData = dict[str, str | dict[str, int] | list[dict[str, str]]]
-Media = Literal["ptt", "dcard"]
 
 
-async def create_tags(root: ET.Element, post_data: PostData, media: Media) -> None:
+async def create_tags(root: ET.Element, post_data: PostData, media: str) -> None:
     """The create_tags function creates TEI XML tags and add them to the root.
 
     Args:
         root (xml.etree.ElementTree.Element): the root element of the TEI XML tree
         post_data (PostData): the post data
         media (Media): a Taiwan social media name
     """
     meta_data = {
         "media": media,
+        "id": post_data.get("id"),
         "author": post_data.get("author"),
-        "post_id": post_data.get("post_id"),
         "year": get_year(post_data.get("date")),
         "board": post_data.get("board"),
         "title": post_data.get("title"),
     }
     content = (post_data.get("title"), post_data.get("body"), post_data.get("comments"))
 
     task1 = asyncio.create_task(create_header_tag(root, meta_data))
     task2 = asyncio.create_task(create_body_tags(root, content, meta_data["author"]))
     await asyncio.gather(task1, task2)
 
 
-def generate_tei_xml(post_data: PostData, media: Media) -> str:
+def generate_tei_xml(post_data: PostData, media: str) -> str:
     """The generate_tei_xml function generates TEI XML string.
 
     Args:
         post_data (PostData): the post data
-        media (Media): a Taiwan social media name
+        media (str): a Taiwan social media name
     """
 
     if not post_data:
         raise ValueError("post_data cannot be empty")
 
     root = ET.Element("TEI.2")
     asyncio.run(create_tags(root, post_data, media))
```

### Comparing `ckip2tei-1.0.2/ckip2tei/tei/utils/body.py` & `ckip2tei-1.1.2/ckip2tei/tei/utils/body.py`

 * *Files identical despite different names*

### Comparing `ckip2tei-1.0.2/PKG-INFO` & `ckip2tei-1.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ckip2tei
-Version: 1.0.2
+Version: 1.1.2
 Summary: A Python package that asynchronously segments JSON data into TEI XML format.
 Author: Retr0327
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ckip-transformers (>=0.3.2,<0.4.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ckip-transformers (>=0.3.4,<0.4.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # **ckip-2-tei**
 
 This project segments the title, body, and comments from a JSON file and writes them to a TEI XML file, and
 leverages asynchronous programming to achieve high performance and speed.
 
@@ -46,15 +48,15 @@
 - `media`: the source of the data
 
 The `post_data` argument should be in the following format:
 
 ```python
 {
     "board": "Soft_Job",
-    "post_id": "ABCD",
+    "id": "ABCD",
     "date": "1183186255",
     "title": "[請益] 最愛的程式?",
     "author": "Retr0327",
     "body": "這是一篇測試文章\n我喜歡 Python 和 TypeScript",
     "post_vote": {"推 (pos)": 2, "噓 (neg)": 0, "→ (neu)": 0},
     "comments": [
         {
@@ -75,15 +77,15 @@
 
 After filling the arguments, do it as follows:
 
 
 ```python
 post_data = {
     "board": "Soft_Job",
-    "post_id": "ABCD",
+    "id": "ABCD",
     "date": "1183186255",
     "title": "[請益] 最愛的程式?",
     "author": "Retr0327",
     "body": "這是一篇測試文章\n我喜歡 Python 和 TypeScript",
     "post_vote": {"推 (pos)": 2, "噓 (neg)": 0, "→ (neu)": 0},
     "comments": [
         {
@@ -107,15 +109,15 @@
 This prints:
 
 ```xml
 <TEI.2>
    <teiHeader>
       <metadata name="media">ptt</metadata>
       <metadata name="author">Retr0327</metadata>
-      <metadata name="post_id">ABCD</metadata>
+      <metadata name="id">ABCD</metadata>
       <metadata name="year">2007</metadata>
       <metadata name="board">Soft_Job</metadata>
       <metadata name="title">[請益] 最愛的程式?</metadata>
    </teiHeader>
    <text>
       <title author="Retr0327">
          <s>
```

