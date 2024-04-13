# Comparing `tmp/pyhtml_enhanced-2.0.1.tar.gz` & `tmp/pyhtml_enhanced-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtml_enhanced-2.0.1.tar", max compression
+gzip compressed data, was "pyhtml_enhanced-2.0.2.tar", max compression
```

## Comparing `pyhtml_enhanced-2.0.1.tar` & `pyhtml_enhanced-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1090 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/LICENSE.md
--rw-r--r--   0        0        0    14277 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/LICENSE_DOCS.md
--rw-r--r--   0        0        0     6407 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/README.md
--rw-r--r--   0        0        0     9284 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__init__.py
--rw-r--r--   0        0        0     4565 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tag_base.py
--rw-r--r--   0        0        0     3111 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/__init__.py
--rw-r--r--   0        0        0     1261 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/comment.py
--rw-r--r--   0        0        0     1543 2024-04-03 02:29:02.690998 pyhtml_enhanced-2.0.1/pyhtml/__tags/dangerous_raw_html.py
--rw-r--r--   0        0        0   205360 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/generated.py
--rw-r--r--   0        0        0    16608 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/input.py
--rw-r--r--   0        0        0      441 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__tags/renames.py
--rw-r--r--   0        0        0     1231 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__types.py
--rw-r--r--   0        0        0     4055 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/__util.py
--rw-r--r--   0        0        0        0 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyhtml/py.typed
--rw-r--r--   0        0        0     1907 2024-04-03 02:29:02.694998 pyhtml_enhanced-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 pyhtml_enhanced-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-13 06:38:50.933550 pyhtml_enhanced-2.0.2/LICENSE.md
+-rw-r--r--   0        0        0    14277 2024-04-13 06:38:50.933550 pyhtml_enhanced-2.0.2/LICENSE_DOCS.md
+-rw-r--r--   0        0        0     6407 2024-04-13 06:38:50.933550 pyhtml_enhanced-2.0.2/README.md
+-rw-r--r--   0        0        0     9284 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__init__.py
+-rw-r--r--   0        0        0     4565 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tag_base.py
+-rw-r--r--   0        0        0     3111 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/comment.py
+-rw-r--r--   0        0        0     1543 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/dangerous_raw_html.py
+-rw-r--r--   0        0        0   205360 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/generated.py
+-rw-r--r--   0        0        0    16608 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/input.py
+-rw-r--r--   0        0        0      441 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__tags/renames.py
+-rw-r--r--   0        0        0     1245 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__types.py
+-rw-r--r--   0        0        0     4206 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/__util.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyhtml/py.typed
+-rw-r--r--   0        0        0     1868 2024-04-13 06:38:50.937550 pyhtml_enhanced-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 pyhtml_enhanced-2.0.2/PKG-INFO
```

### Comparing `pyhtml_enhanced-2.0.1/LICENSE.md` & `pyhtml_enhanced-2.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/LICENSE_DOCS.md` & `pyhtml_enhanced-2.0.2/LICENSE_DOCS.md`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/README.md` & `pyhtml_enhanced-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__init__.py` & `pyhtml_enhanced-2.0.2/pyhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tag_base.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tag_base.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tags/__init__.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tags/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tags/comment.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tags/comment.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tags/dangerous_raw_html.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tags/dangerous_raw_html.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tags/generated.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tags/generated.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__tags/input.py` & `pyhtml_enhanced-2.0.2/pyhtml/__tags/input.py`

 * *Files identical despite different names*

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__types.py` & `pyhtml_enhanced-2.0.2/pyhtml/__types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 # Pyhtml / Types
 
 Type definitions
 """
 from typing import Union, TYPE_CHECKING
-from collections.abc import Generator
+from collections.abc import Generator, Sequence
 
 
 if TYPE_CHECKING:
     from .__tag_base import Tag
 
 
 AttributeType = Union[str, bool, None]
@@ -29,15 +29,15 @@
 While more types can technically work (such as `int`, `bool` and `float`),
 these aren't allowed in order to encourage proper use of string formatting.
 """
 
 
 ChildrenType = Union[
     ChildElementType,
-    list[ChildElementType],
+    Sequence[ChildElementType],
     'Generator[ChildElementType, None, None]',
     # TODO: Would an `Any` type for the generator return be better, even though
     # it would be discarded?
 ]
 """
 Objects that are valid when passed to a `Tag` for use as children.
```

### Comparing `pyhtml_enhanced-2.0.1/pyhtml/__util.py` & `pyhtml_enhanced-2.0.2/pyhtml/__util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 # PyHTML Enhanced / Util
 
 Random helpful functions used elsewhere
 """
 from typing import Any, TypeVar
-from collections.abc import Generator
+from collections.abc import Generator, Sequence
 from .__types import ChildrenType, ChildElementType
 
 
 T = TypeVar('T')
 K = TypeVar('K')
 V = TypeVar('V')
 
@@ -139,14 +139,18 @@
     """
     result: list[ChildElementType] = []
     for item in the_list:
         if isinstance(item, list):
             result.extend(item)
         elif isinstance(item, Generator):
             result.extend(item)
+        elif isinstance(item, str):
+            result.append(item)
+        elif isinstance(item, Sequence):
+            result.extend(item)
         else:
             result.append(item)
     return result
 
 
 def dict_union(base: dict[K, V], additions: dict[K, V]) -> dict[K, V]:
     """
```

### Comparing `pyhtml_enhanced-2.0.1/pyproject.toml` & `pyhtml_enhanced-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 [tool.poetry]
 name = "pyhtml-enhanced"
-version = "2.0.1"
+version = "2.0.2"
 description = "A library for building HTML documents with a simple and learnable syntax"
 authors = ["Miguel Guthridge <miguel.guthridge@unsw.edu.au>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "pyhtml"}]
+packages = [{ include = "pyhtml" }]
 
 repository = "https://github.com/COMP1010UNSW/pyhtml-enhanced"
 documentation = "https://github.com/COMP1010UNSW/pyhtml-enhanced#README"
 
-keywords = [
-    'html',
-    'template',
-    'pyhtml',
-    'markup',
-    'documentation',
-]
+keywords = ['html', 'template', 'pyhtml', 'markup', 'documentation']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
@@ -52,23 +46,18 @@
 pytest-mypy-plugins = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
-exclude = [
-    'meta/templates/*',
-]
+exclude = ['meta/templates/*']
 
 [tool.flake8]
-exclude = [
-    'meta/templates',
-    'pyhtml/__tags/generated.py',
-]
+exclude = ['meta/templates', 'pyhtml/__tags/generated.py']
 per-file-ignores = [
     "pyhtml/__tags/input.py:E501",
     "pyhtml/__tags/geberated.py:E501",
 ]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-glob README.md"
```

### Comparing `pyhtml_enhanced-2.0.1/PKG-INFO` & `pyhtml_enhanced-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtml-enhanced
-Version: 2.0.1
+Version: 2.0.2
 Summary: A library for building HTML documents with a simple and learnable syntax
 Home-page: https://github.com/COMP1010UNSW/pyhtml-enhanced
 License: MIT
 Keywords: html,template,pyhtml,markup,documentation
 Author: Miguel Guthridge
 Author-email: miguel.guthridge@unsw.edu.au
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_vdpeh45j_/tmpdnts0_kx_TarContainer/0/15", line 282, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyhtml-enhanced Version: 2.0.1 Summary: A library
+Metadata-Version: 2.1 Name: pyhtml-enhanced Version: 2.0.2 Summary: A library
 for building HTML documents with a simple and learnable syntax Home-page:
 https://github.com/COMP1010UNSW/pyhtml-enhanced License: MIT Keywords:
 html,template,pyhtml,markup,documentation Author: Miguel Guthridge Author-
 email: miguel.guthridge@unsw.edu.au Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

