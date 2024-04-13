# Comparing `tmp/thepipe_api-0.1.2.tar.gz` & `tmp/thepipe_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.2.tar", last modified: Sat Apr 13 19:22:12 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.3.tar", last modified: Sat Apr 13 19:50:04 2024, max compression
```

## Comparing `thepipe_api-0.1.2.tar` & `thepipe_api-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.238142 thepipe_api-0.1.2/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     9615 2024-04-13 19:22:12.237141 thepipe_api-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8534 2024-04-13 17:32:17.000000 thepipe_api-0.1.2/README.md
--rw-rw-rw-   0        0        0      753 2024-04-13 19:18:49.000000 thepipe_api-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      276 2024-04-13 17:21:22.000000 thepipe_api-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 19:22:12.238142 thepipe_api-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-13 19:19:23.000000 thepipe_api-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.220142 thepipe_api-0.1.2/tests/
--rw-rw-rw-   0        0        0     9511 2024-04-13 18:51:15.000000 thepipe_api-0.1.2/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.237141 thepipe_api-0.1.2/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      256 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.337923 thepipe_api-0.1.3/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     9603 2024-04-13 19:50:04.336924 thepipe_api-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8534 2024-04-13 17:32:17.000000 thepipe_api-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 19:50:04.337923 thepipe_api-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-04-13 19:49:58.000000 thepipe_api-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.313921 thepipe_api-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9511 2024-04-13 18:51:15.000000 thepipe_api-0.1.3/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.317921 thepipe_api-0.1.3/thepipe_api/
+-rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.3/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 18:49:04.000000 thepipe_api-0.1.3/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2835 2024-04-13 18:07:10.000000 thepipe_api-0.1.3/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19468 2024-04-13 18:50:12.000000 thepipe_api-0.1.3/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3504 2024-04-13 19:44:28.000000 thepipe_api-0.1.3/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.335923 thepipe_api-0.1.3/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9603 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      256 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.2/LICENSE` & `thepipe_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.2/PKG-INFO` & `thepipe_api-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.2
-Author-email: Emmett McFarlane <emmett@thepi.pe>
-License: MIT License
-Project-URL: Homepage, https://thepi.pe
-Project-URL: Documentation, https://thepi.pe/docs
-Project-URL: Repository, https://github.com/emcf/thepipe
-Project-URL: Issues, https://github.com/emcf/thepipe/issues
-Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Version: 0.1.3
+Summary: Automate information extraction for multimodal LLMs.
+Home-page: https://github.com/emcf/thepipe
+Author: Emmett McFarlane
+Author-email: emmett@thepi.pe
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.8.3
 Requires-Dist: charset-normalizer<3.0,>=2.0
 Requires-Dist: playwright
 Requires-Dist: docx2txt
 Requires-Dist: python-pptx
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.2 Author-email: Emmett
-McFarlane
-thepi.pe> License: MIT License Project-URL: Homepage, https://thepi.pe Project-
-URL: Documentation, https://thepi.pe/docs Project-URL: Repository, https://
-github.com/emcf/thepipe Project-URL: Issues, https://github.com/emcf/thepipe/
-issues Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.3 Summary: Automate
+information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
+thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
 playwright Requires-Dist: docx2txt Requires-Dist: python-pptx Requires-Dist:
 Pyarrow Requires-Dist: unstructured[all-docs] Requires-Dist: poppler-utils
 Requires-Dist: python-magic Requires-Dist: magika Requires-Dist: pandas
 Requires-Dist: colorama Requires-Dist: requests Requires-Dist: pillow Requires-
 Dist: pytesseract Requires-Dist: cssutils Requires-Dist: beautifulsoup4
```

### Comparing `thepipe_api-0.1.2/README.md` & `thepipe_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.2/tests/test_thepipe.py` & `thepipe_api-0.1.3/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.2/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.3/thepipe_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.2
-Author-email: Emmett McFarlane <emmett@thepi.pe>
-License: MIT License
-Project-URL: Homepage, https://thepi.pe
-Project-URL: Documentation, https://thepi.pe/docs
-Project-URL: Repository, https://github.com/emcf/thepipe
-Project-URL: Issues, https://github.com/emcf/thepipe/issues
-Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Version: 0.1.3
+Summary: Automate information extraction for multimodal LLMs.
+Home-page: https://github.com/emcf/thepipe
+Author: Emmett McFarlane
+Author-email: emmett@thepi.pe
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp==3.8.3
 Requires-Dist: charset-normalizer<3.0,>=2.0
 Requires-Dist: playwright
 Requires-Dist: docx2txt
 Requires-Dist: python-pptx
```

#### html2text {}

```diff
@@ -1,13 +1,12 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.2 Author-email: Emmett
-McFarlane
-thepi.pe> License: MIT License Project-URL: Homepage, https://thepi.pe Project-
-URL: Documentation, https://thepi.pe/docs Project-URL: Repository, https://
-github.com/emcf/thepipe Project-URL: Issues, https://github.com/emcf/thepipe/
-issues Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.3 Summary: Automate
+information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
+thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
 playwright Requires-Dist: docx2txt Requires-Dist: python-pptx Requires-Dist:
 Pyarrow Requires-Dist: unstructured[all-docs] Requires-Dist: poppler-utils
 Requires-Dist: python-magic Requires-Dist: magika Requires-Dist: pandas
 Requires-Dist: colorama Requires-Dist: requests Requires-Dist: pillow Requires-
 Dist: pytesseract Requires-Dist: cssutils Requires-Dist: beautifulsoup4
```

