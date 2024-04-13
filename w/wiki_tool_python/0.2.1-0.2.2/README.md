# Comparing `tmp/wiki_tool_python-0.2.1.tar.gz` & `tmp/wiki_tool_python-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiki_tool_python-0.2.1.tar", max compression
+gzip compressed data, was "wiki_tool_python-0.2.2.tar", max compression
```

## Comparing `wiki_tool_python-0.2.1.tar` & `wiki_tool_python-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2018-11-25 15:02:40.055600 wiki_tool_python-0.2.1/LICENSE
--rw-r--r--   0        0        0    23180 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/README.md
--rw-r--r--   0        0        0      971 2024-03-30 19:03:31.287156 wiki_tool_python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4342 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/wiki_tool_python/mediawiki.py
--rw-r--r--   0        0        0    12290 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/wiki_tool_python/mediawiki_1_19.py
--rw-r--r--   0        0        0    14976 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/wiki_tool_python/mediawiki_1_31.py
--rw-r--r--   0        0        0      713 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/wiki_tool_python/requests_wrapper.py
--rw-r--r--   0        0        0    39633 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.1/wiki_tool_python/wikitool.py
--rw-r--r--   0        0        0    24191 1970-01-01 00:00:00.000000 wiki_tool_python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2018-11-25 15:02:40.055600 wiki_tool_python-0.2.2/LICENSE
+-rw-r--r--   0        0        0    23180 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/README.md
+-rw-r--r--   0        0        0      947 2024-04-13 06:36:21.526255 wiki_tool_python-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4342 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/wiki_tool_python/mediawiki.py
+-rw-r--r--   0        0        0    12290 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/wiki_tool_python/mediawiki_1_19.py
+-rw-r--r--   0        0        0    14976 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/wiki_tool_python/mediawiki_1_31.py
+-rw-r--r--   0        0        0      713 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/wiki_tool_python/requests_wrapper.py
+-rw-r--r--   0        0        0    39633 2023-03-31 06:15:57.157152 wiki_tool_python-0.2.2/wiki_tool_python/wikitool.py
+-rw-r--r--   0        0        0    24146 1970-01-01 00:00:00.000000 wiki_tool_python-0.2.2/PKG-INFO
```

### Comparing `wiki_tool_python-0.2.1/LICENSE` & `wiki_tool_python-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/README.md` & `wiki_tool_python-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/pyproject.toml` & `wiki_tool_python-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wiki_tool_python"
-version = "0.2.1"
+version = "0.2.2"
 description = "Script to perform tasks with websites on MediaWiki engine using API"
 authors = ["Artiom Khandamirov <t9max@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ArtUshak/wiki_tool_python/"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -13,15 +13,14 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.7"
 requests = "^2.31.0"
 requests-toolbelt = "^1.0.0"
-flake8-print = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.4"
 mypy = "^1.5.1"
 flake8 = "^6.1.0"
 flake8-bandit = "^4.1.1"
 flake8-pydocstyle = "^0.2.2"
```

### Comparing `wiki_tool_python-0.2.1/wiki_tool_python/mediawiki.py` & `wiki_tool_python-0.2.2/wiki_tool_python/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/wiki_tool_python/mediawiki_1_19.py` & `wiki_tool_python-0.2.2/wiki_tool_python/mediawiki_1_19.py`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/wiki_tool_python/mediawiki_1_31.py` & `wiki_tool_python-0.2.2/wiki_tool_python/mediawiki_1_31.py`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/wiki_tool_python/requests_wrapper.py` & `wiki_tool_python-0.2.2/wiki_tool_python/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/wiki_tool_python/wikitool.py` & `wiki_tool_python-0.2.2/wiki_tool_python/wikitool.py`

 * *Files identical despite different names*

### Comparing `wiki_tool_python-0.2.1/PKG-INFO` & `wiki_tool_python-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiki_tool_python
-Version: 0.2.1
+Version: 0.2.2
 Summary: Script to perform tasks with websites on MediaWiki engine using API
 Home-page: https://github.com/ArtUshak/wiki_tool_python/
 License: MIT
 Author: Artiom Khandamirov
 Author-email: t9max@yandex.ru
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: flake8-print (>=5.0.0,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/ArtUshak/wiki_tool_python/
 Description-Content-Type: text/markdown
 
 # wiki_tool_python
```

