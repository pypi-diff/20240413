# Comparing `tmp/py-txi-0.5.1.tar.gz` & `tmp/py-txi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-txi-0.5.1.tar", last modified: Sat Apr 13 09:10:16 2024, max compression
+gzip compressed data, was "py-txi-0.6.0.tar", last modified: Sat Apr 13 09:13:39 2024, max compression
```

## Comparing `py-txi-0.5.1.tar` & `py-txi-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 09:10:04.000000 py-txi-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:10:16.663463 py-txi-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-13 09:10:04.000000 py-txi-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/py_txi/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/text_embedding_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/text_generation_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/py_txi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 09:10:04.000000 py-txi-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:10:16.663463 py-txi-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-13 09:10:04.000000 py-txi-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:13:39.691785 py-txi-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 09:13:27.000000 py-txi-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:13:39.691785 py-txi-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-13 09:13:27.000000 py-txi-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:13:39.691785 py-txi-0.6.0/py_txi/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 09:13:27.000000 py-txi-0.6.0/py_txi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-13 09:13:27.000000 py-txi-0.6.0/py_txi/inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 09:13:27.000000 py-txi-0.6.0/py_txi/text_embedding_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-13 09:13:27.000000 py-txi-0.6.0/py_txi/text_generation_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 09:13:27.000000 py-txi-0.6.0/py_txi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:13:39.691785 py-txi-0.6.0/py_txi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:13:39.000000 py-txi-0.6.0/py_txi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-13 09:13:39.000000 py-txi-0.6.0/py_txi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:13:39.000000 py-txi-0.6.0/py_txi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 09:13:39.000000 py-txi-0.6.0/py_txi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 09:13:39.000000 py-txi-0.6.0/py_txi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 09:13:27.000000 py-txi-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:13:39.691785 py-txi-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-13 09:13:27.000000 py-txi-0.6.0/setup.py
```

### Comparing `py-txi-0.5.1/LICENSE` & `py-txi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-txi-0.5.1/PKG-INFO` & `py-txi-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
```

### Comparing `py-txi-0.5.1/README.md` & `py-txi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `py-txi-0.5.1/py_txi/inference_server.py` & `py-txi-0.6.0/py_txi/inference_server.py`

 * *Files identical despite different names*

### Comparing `py-txi-0.5.1/py_txi/text_embedding_inference.py` & `py-txi-0.6.0/py_txi/text_embedding_inference.py`

 * *Files identical despite different names*

### Comparing `py-txi-0.5.1/py_txi/text_generation_inference.py` & `py-txi-0.6.0/py_txi/text_generation_inference.py`

 * *Files identical despite different names*

### Comparing `py-txi-0.5.1/py_txi.egg-info/PKG-INFO` & `py-txi-0.6.0/py_txi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
```

### Comparing `py-txi-0.5.1/setup.py` & `py-txi-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-PY_TXI_VERSION = "0.5.1"
+PY_TXI_VERSION = "0.6.0"
 
 common_setup_kwargs = {
     "author": "Ilyas Moutawwakil",
     "author_email": "ilyas.moutawwakil@gmail.com",
     "description": "A Python wrapper around TGI and TEI servers",
     "keywords": ["tgi", "llm", "tei", "embedding", "huggingface", "docker", "python"],
     "url": "https://github.com/IlyasMoutawwakil/py-txi",
```

