# Comparing `tmp/docprompt-0.2.5.tar.gz` & `tmp/docprompt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.2.5.tar", max compression
+gzip compressed data, was "docprompt-0.2.6.tar", max compression
```

## Comparing `docprompt-0.2.5.tar` & `docprompt-0.2.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.5/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.5/README.md
--rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.5/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.5/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.5/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.5/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.5/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.5/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.5/docprompt/provenance/util.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.5/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9472 2024-04-09 01:41:32.425414 docprompt-0.2.5/docprompt/schema/document.py
--rw-r--r--   0        0        0     6362 2024-04-05 21:39:49.476813 docprompt-0.2.5/docprompt/schema/layout.py
--rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.5/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.5/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.5/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.5/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.5/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.5/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18333 2024-04-05 21:53:48.708070 docprompt-0.2.5/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.5/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.5/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.5/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.5/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.5/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.5/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.5/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.5/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.5/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.5/docprompt/utils/raster.py
--rw-r--r--   0        0        0     4015 2024-04-10 19:57:12.041828 docprompt-0.2.5/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.5/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-10 19:57:24.297921 docprompt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.5/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.5/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.5/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.5/tests/test_date_extraction.py
--rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.5/tests/test_document.py
--rw-r--r--   0        0        0     1240 2024-04-09 01:41:32.425414 docprompt-0.2.5/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.5/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.5/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.5/tests/util.py
--rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.2.6/README.md
+-rw-r--r--   0        0        0      593 2024-03-21 01:44:38.876965 docprompt-0.2.6/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.2.6/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.2.6/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-03-18 23:40:35.967506 docprompt-0.2.6/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.2.6/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.2.6/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.2.6/docprompt/provenance/util.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.2.6/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9570 2024-04-13 03:18:18.262506 docprompt-0.2.6/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.2.6/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     3764 2024-04-05 21:39:58.248888 docprompt-0.2.6/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.2.6/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.2.6/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.2.6/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.2.6/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.2.6/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.2.6/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.2.6/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.2.6/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.2.6/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.2.6/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.2.6/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.2.6/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      351 2024-03-14 21:45:48.927780 docprompt-0.2.6/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.2.6/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.2.6/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-03-18 15:46:16.978297 docprompt-0.2.6/docprompt/utils/raster.py
+-rw-r--r--   0        0        0     4015 2024-04-13 03:01:14.714377 docprompt-0.2.6/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     3994 2024-04-05 21:52:56.007611 docprompt-0.2.6/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-13 03:18:31.630612 docprompt-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.2.6/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.2.6/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.2.6/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.2.6/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     2103 2024-04-09 01:42:25.113812 docprompt-0.2.6/tests/test_document.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.2.6/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-09 01:36:21.595068 docprompt-0.2.6/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.2.6/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.2.6/tests/util.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 docprompt-0.2.6/PKG-INFO
```

### Comparing `docprompt-0.2.5/LICENSE` & `docprompt-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/README.md` & `docprompt-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/__init__.py` & `docprompt-0.2.6/docprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/_exec/ghostscript.py` & `docprompt-0.2.6/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/provenance/search.py` & `docprompt-0.2.6/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/provenance/source.py` & `docprompt-0.2.6/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/provenance/util.py` & `docprompt-0.2.6/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/schema/document.py` & `docprompt-0.2.6/docprompt/schema/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 
         return get_page_count(self.file_bytes)
 
     @property
     def num_pages(self):
         return self.page_count
 
+    @property
+    def bytes_per_page(self):
+        return len(self.file_bytes) / self.num_pages
+
     @computed_field
     @cached_property
     def document_hash(self) -> str:
         from docprompt.utils.util import hash_from_bytes
 
         return hash_from_bytes(self.file_bytes)
```

### Comparing `docprompt-0.2.5/docprompt/schema/layout.py` & `docprompt-0.2.6/docprompt/schema/layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from typing import List, Literal, Optional
+from typing_extensions import Annotated
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, PlainSerializer
 
 SegmentLevels = Literal["word", "line", "block"]
 TextblockSource = Literal["ocr", "derived"]
 DirectionChoices = Literal["UP", "DOWN", "LEFT", "RIGHT"]
 
+RoundedFloat = Annotated[float, PlainSerializer(lambda x: round(x, 5))]
+BoundedFloat = Annotated[
+    RoundedFloat, Field(..., ge=0, le=1, description="A float between 0 and 1")
+]
+
 
 class TextSpan(BaseModel):
     start_index: int
     end_index: int
     level: Literal["page", "document"] = Field(
         default="page", description="The level of the span"
     )
@@ -18,18 +24,18 @@
 class NormBBox(BaseModel):
     """
     Represents a normalized bounding box with each value in the range [0, 1]
 
     Where x1 > x0 and bottom > top
     """
 
-    x0: float
-    top: float
-    x1: float
-    bottom: float
+    x0: BoundedFloat
+    top: BoundedFloat
+    x1: BoundedFloat
+    bottom: BoundedFloat
 
     class Config:
         json_encoders = {float: lambda v: round(v, 5)}  # 1/10,000 increments is plenty
 
     def as_tuple(self):
         return (self.x0, self.top, self.x1, self.bottom)
 
@@ -167,16 +173,16 @@
     """
     Represents a normalized bounding box with each value in the range [0, 1]
     """
 
     class Config:
         json_encoders = {float: lambda v: round(v, 5)}  # 1/10,000 increments is plenty
 
-    x: float
-    y: float
+    x: BoundedFloat
+    y: BoundedFloat
 
 
 class BoundingPoly(BaseModel):
     """
     Represents a normalized bounding poly with each value in the range [0, 1]
 
     Used for higher order shapes like polygons on a page
@@ -186,15 +192,15 @@
 
     def __getitem__(self, index):
         return self.normalized_vertices[index]
 
 
 class TextBlockMetadata(BaseModel):
     direction: Optional[DirectionChoices] = None
-    confidence: Optional[float] = None
+    confidence: Optional[RoundedFloat] = None
     layout_category: Optional[str] = Field(
         default=None, description="The category of the text block"
     )
 
 
 class TextBlock(BaseModel):
     """
```

### Comparing `docprompt-0.2.5/docprompt/schema/pipeline.py` & `docprompt-0.2.6/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/base.py` & `docprompt-0.2.6/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/message.py` & `docprompt-0.2.6/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/ocr/gcp.py` & `docprompt-0.2.6/docprompt/tasks/ocr/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,18 +515,24 @@
         client = self.get_documentai_client()
         processor_name = client.processor_path(
             project=self.project_id,
             location=self.location,
             processor=self.processor_id,
         )
 
+        file_bytes = document.file_bytes
+
+        if document.bytes_per_page > 1024 * 1024 * 2:
+            logger.info("Document has few pages but is large, compressing first")
+            file_bytes = document.to_compressed_bytes()
+
         logger.info("Splitting document into chunks...")
         document_byte_splits = list(
             pdf_split_iter_with_max_bytes(
-                document.get_bytes(),
+                file_bytes,
                 max_page_count=self.max_page_count,
                 max_bytes=self.max_bytes_per_request,
             )
         )
 
         max_workers = min(len(document_byte_splits), self.max_workers)
```

### Comparing `docprompt-0.2.5/docprompt/tasks/ocr/result.py` & `docprompt-0.2.6/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/table_extraction/base.py` & `docprompt-0.2.6/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.2.6/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/tasks/table_extraction/result.py` & `docprompt-0.2.6/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/utils/date_extraction.py` & `docprompt-0.2.6/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/utils/splitter.py` & `docprompt-0.2.6/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/docprompt/utils/util.py` & `docprompt-0.2.6/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/pyproject.toml` & `docprompt-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.2.5"
+version = "0.2.6"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.2.5/tests/fixtures/1.pdf` & `docprompt-0.2.6/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/fixtures/1_ocr.json` & `docprompt-0.2.6/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/test_date_extraction.py` & `docprompt-0.2.6/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/test_document.py` & `docprompt-0.2.6/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/test_layout_models.py` & `docprompt-0.2.6/tests/test_layout_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from docprompt import NormBBox
 from docprompt.schema.layout import BoundingPoly, Point
+import pytest
 
 
 def test_normbbox_utilities():
     bbox = NormBBox(x0=0, top=0, x1=1, bottom=1)
 
     # Test simple properties
     assert bbox[0] == 0
@@ -17,24 +18,29 @@
     assert bbox.centroid == (0.5, 0.5)
     assert bbox.y_center == 0.5
     assert bbox.x_center == 0.5
 
     # Test equality
     assert bbox == NormBBox(x0=0, top=0, x1=1, bottom=1)
 
+    # Test out of bounds
+
+    with pytest.raises(ValueError):
+        NormBBox(x0=0, top=0, x1=1, bottom=2)
+
     # Add two bboxes
 
-    bbox_2 = NormBBox(x0=0.5, top=0.5, x1=1.5, bottom=1.5)
+    bbox_2 = NormBBox(x0=0.5, top=0.5, x1=1, bottom=1.0)
     combined_bbox = bbox + bbox_2
-    assert combined_bbox == NormBBox(x0=0, top=0, x1=1.5, bottom=1.5)
+    assert combined_bbox == NormBBox(x0=0, top=0, x1=1.0, bottom=1.0)
 
     # Add two bboxes via combine
 
     combined_bbox = NormBBox.combine(bbox, bbox_2)
-    assert combined_bbox == NormBBox(x0=0, top=0, x1=1.5, bottom=1.5)
+    assert combined_bbox == NormBBox(x0=0, top=0, x1=1.0, bottom=1.0)
 
     # Test from bounding poly
     bounding_poly = BoundingPoly(
         normalized_vertices=[
             Point(x=0, y=0),
             Point(x=1, y=0),
             Point(x=1, y=1),
```

### Comparing `docprompt-0.2.5/tests/test_search.py` & `docprompt-0.2.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/test_threadpool.py` & `docprompt-0.2.6/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/tests/util.py` & `docprompt-0.2.6/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.2.5/PKG-INFO` & `docprompt-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.2.5
+Version: 0.2.6
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.2.5 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.2.6 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

