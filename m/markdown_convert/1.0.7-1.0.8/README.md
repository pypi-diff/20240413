# Comparing `tmp/markdown_convert-1.0.7.tar.gz` & `tmp/markdown_convert-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.7.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.8.tar", max compression
```

## Comparing `markdown_convert-1.0.7.tar` & `markdown_convert-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.7/LICENSE
--rw-r--r--   0        0        0     1763 2024-04-10 11:53:43.195866 markdown_convert-1.0.7/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.0.7/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.7/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.7/markdown_convert/code.css
--rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.0.7/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.0.7/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.0.7/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5683 2024-04-10 20:52:03.409736 markdown_convert-1.0.7/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.7/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.0.7/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.7/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      659 2024-04-10 20:59:03.557444 markdown_convert-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 markdown_convert-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1763 2024-04-10 11:53:43.195866 markdown_convert-1.0.8/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.0.8/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.8/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.8/markdown_convert/code.css
+-rw-r--r--   0        0        0     5344 2024-04-10 06:55:23.607495 markdown_convert-1.0.8/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.0.8/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.0.8/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5683 2024-04-10 20:52:03.409736 markdown_convert-1.0.8/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.8/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.0.8/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.8/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      680 2024-04-13 08:22:35.712165 markdown_convert-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 markdown_convert-1.0.8/PKG-INFO
```

### Comparing `markdown_convert-1.0.7/LICENSE` & `markdown_convert-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/README.md` & `markdown_convert-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/__main__.py` & `markdown_convert-1.0.8/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/code.css` & `markdown_convert-1.0.8/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/default.css` & `markdown_convert-1.0.8/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/modules/convert.py` & `markdown_convert-1.0.8/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/modules/resources.py` & `markdown_convert-1.0.8/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/modules/utils.py` & `markdown_convert-1.0.8/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/markdown_convert/modules/validate.py` & `markdown_convert-1.0.8/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.7/pyproject.toml` & `markdown_convert-1.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.7"
+version = "1.0.8"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 argsdict = "1.0.0"
 setuptools = ">=46.0.0"
 weasyprint = "^61.2"
 markdown2 = "^2.4.13"
+pygments = "^2.17.2"
 
 [tool.poetry.scripts]
 markdown-convert = "markdown_convert.__main__:main"
```

### Comparing `markdown_convert-1.0.7/PKG-INFO` & `markdown_convert-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.0.7
+Version: 1.0.8
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argsdict (==1.0.0)
 Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
+Requires-Dist: pygments (>=2.17.2,<3.0.0)
 Requires-Dist: setuptools (>=46.0.0)
 Requires-Dist: weasyprint (>=61.2,<62.0)
 Description-Content-Type: text/markdown
 
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
```

