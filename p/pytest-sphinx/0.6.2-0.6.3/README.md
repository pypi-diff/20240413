# Comparing `tmp/pytest-sphinx-0.6.2.tar.gz` & `tmp/pytest_sphinx-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sphinx-0.6.2.tar", last modified: Mon Apr  1 19:02:48 2024, max compression
+gzip compressed data, was "pytest_sphinx-0.6.3.tar", last modified: Sat Apr 13 19:11:47 2024, max compression
```

## Comparing `pytest-sphinx-0.6.2.tar` & `pytest_sphinx-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.475334 pytest-sphinx-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 19:02:48.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20687 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/src/pytest_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:02:48.479334 pytest-sphinx-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_doc2test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_python_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_sphinx_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-01 19:02:42.000000 pytest-sphinx-0.6.2/tests/test_text_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:47.287463 pytest_sphinx-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-13 19:11:47.283463 pytest_sphinx-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 19:11:47.287463 pytest_sphinx-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:47.283463 pytest_sphinx-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:47.283463 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 19:11:47.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20687 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/src/pytest_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:47.283463 pytest_sphinx-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/tests/test_doc2test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/tests/test_python_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/tests/test_sphinx_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-13 19:11:35.000000 pytest_sphinx-0.6.3/tests/test_text_files.py
```

### Comparing `pytest-sphinx-0.6.2/LICENSE` & `pytest_sphinx-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/PKG-INFO` & `pytest_sphinx-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sphinx
-Version: 0.6.2
+Version: 0.6.3
 Summary: Doctest plugin for pytest with support for Sphinx-specific doctest-directives
 Author-email: Thomas Wimmer <thomaswimmer@posteo.com>
 Maintainer-email: Thomas Wimmer <thomaswimmer@posteo.com>
 License: 
         Copyright (c) 2017-2024, Thomas Wimmer
         All rights reserved.
         
@@ -48,15 +48,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pytest>=8.0.0
+Requires-Dist: pytest>=8.1.1
 Provides-Extra: lint
 Requires-Dist: isort>=5; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: black; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 
 =============
```

### Comparing `pytest-sphinx-0.6.2/README.rst` & `pytest_sphinx-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/pyproject.toml` & `pytest_sphinx-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-sphinx"
-version = "0.6.2"
+version = "0.6.3"
 description = "Doctest plugin for pytest with support for Sphinx-specific doctest-directives"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["sphinx", "pytest", "rst"]
 authors = [
     { name="Thomas Wimmer", email="thomaswimmer@posteo.com" }
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
 ]
 
 # Requirements
 dependencies = [
-    "pytest >=8.0.0",
+    "pytest >=8.1.1",
 ]
 
 [project.optional-dependencies]
 lint = [
     "isort >= 5",
     "flake8",
     "black",
```

### Comparing `pytest-sphinx-0.6.2/src/pytest_sphinx.egg-info/PKG-INFO` & `pytest_sphinx-0.6.3/src/pytest_sphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sphinx
-Version: 0.6.2
+Version: 0.6.3
 Summary: Doctest plugin for pytest with support for Sphinx-specific doctest-directives
 Author-email: Thomas Wimmer <thomaswimmer@posteo.com>
 Maintainer-email: Thomas Wimmer <thomaswimmer@posteo.com>
 License: 
         Copyright (c) 2017-2024, Thomas Wimmer
         All rights reserved.
         
@@ -48,15 +48,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: pytest>=8.0.0
+Requires-Dist: pytest>=8.1.1
 Provides-Extra: lint
 Requires-Dist: isort>=5; extra == "lint"
 Requires-Dist: flake8; extra == "lint"
 Requires-Dist: black; extra == "lint"
 Requires-Dist: mypy; extra == "lint"
 
 =============
```

### Comparing `pytest-sphinx-0.6.2/src/pytest_sphinx.py` & `pytest_sphinx-0.6.3/src/pytest_sphinx.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/tests/test_doc2test.py` & `pytest_sphinx-0.6.3/tests/test_doc2test.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/tests/test_options.py` & `pytest_sphinx-0.6.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/tests/test_python_files.py` & `pytest_sphinx-0.6.3/tests/test_python_files.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/tests/test_sphinx_doctest.py` & `pytest_sphinx-0.6.3/tests/test_sphinx_doctest.py`

 * *Files identical despite different names*

### Comparing `pytest-sphinx-0.6.2/tests/test_text_files.py` & `pytest_sphinx-0.6.3/tests/test_text_files.py`

 * *Files identical despite different names*

