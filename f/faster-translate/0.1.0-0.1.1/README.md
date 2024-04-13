# Comparing `tmp/faster_translate-0.1.0.tar.gz` & `tmp/faster_translate-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.0.tar", last modified: Sat Apr 13 11:04:47 2024, max compression
+gzip compressed data, was "faster_translate-0.1.1.tar", last modified: Sat Apr 13 11:45:21 2024, max compression
```

## Comparing `faster_translate-0.1.0.tar` & `faster_translate-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:04:47.549373 faster_translate-0.1.0/
--rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.0/LICENSE
--rw-r--r--   0 azureuser  (1000) users      (100)     2271 2024-04-13 11:04:47.549373 faster_translate-0.1.0/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)      504 2024-04-13 11:03:20.000000 faster_translate-0.1.0/README.md
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:04:47.549373 faster_translate-0.1.0/faster_translate/
--rw-------   0 azureuser  (1000) users      (100)       33 2024-04-13 06:57:04.000000 faster_translate-0.1.0/faster_translate/__init__.py
--rw-------   0 azureuser  (1000) users      (100)     5978 2024-04-13 10:53:09.000000 faster_translate-0.1.0/faster_translate/model.py
--rw-------   0 azureuser  (1000) users      (100)     2198 2024-04-13 10:54:44.000000 faster_translate-0.1.0/faster_translate/utils.py
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:04:47.549373 faster_translate-0.1.0/faster_translate.egg-info/
--rw-r--r--   0 azureuser  (1000) users      (100)     2271 2024-04-13 11:04:47.000000 faster_translate-0.1.0/faster_translate.egg-info/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 11:04:47.000000 faster_translate-0.1.0/faster_translate.egg-info/SOURCES.txt
--rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 11:04:47.000000 faster_translate-0.1.0/faster_translate.egg-info/dependency_links.txt
--rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 11:04:47.000000 faster_translate-0.1.0/faster_translate.egg-info/requires.txt
--rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 11:04:47.000000 faster_translate-0.1.0/faster_translate.egg-info/top_level.txt
--rw-------   0 azureuser  (1000) users      (100)      637 2024-04-13 07:08:03.000000 faster_translate-0.1.0/pyproject.toml
--rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 11:04:47.549373 faster_translate-0.1.0/setup.cfg
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/
+-rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.1/LICENSE
+-rw-r--r--   0 azureuser  (1000) users      (100)     4741 2024-04-13 11:45:21.385757 faster_translate-0.1.1/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.1/README.md
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/faster_translate/
+-rw-------   0 azureuser  (1000) users      (100)       33 2024-04-13 06:57:04.000000 faster_translate-0.1.1/faster_translate/__init__.py
+-rw-------   0 azureuser  (1000) users      (100)     5978 2024-04-13 10:53:09.000000 faster_translate-0.1.1/faster_translate/model.py
+-rw-------   0 azureuser  (1000) users      (100)     2198 2024-04-13 11:23:46.000000 faster_translate-0.1.1/faster_translate/utils.py
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/faster_translate.egg-info/
+-rw-r--r--   0 azureuser  (1000) users      (100)     4741 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/SOURCES.txt
+-rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/dependency_links.txt
+-rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/requires.txt
+-rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/top_level.txt
+-rw-------   0 azureuser  (1000) users      (100)      637 2024-04-13 11:45:15.000000 faster_translate-0.1.1/pyproject.toml
+-rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 11:45:21.385757 faster_translate-0.1.1/setup.cfg
```

### Comparing `faster_translate-0.1.0/LICENSE` & `faster_translate-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.0/faster_translate/model.py` & `faster_translate-0.1.1/faster_translate/model.py`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.0/faster_translate/utils.py` & `faster_translate-0.1.1/faster_translate/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 _MODELS = {
     "banglanmt_bn2en": {
         "model_repo": "sawradip/faster-translate-banglanmt-bn2en-t5",
         "normalizer_func":"buetnlpnormalizer"
     },
     "banglanmt_en2bn": {
-        "model_repo": "sawradip/faster-translate-banglanmt-bn2en-t5"
+        "model_repo": "sawradip/faster-translate-banglanmt-en2bn-t5"
     }
 }
 def upload_model_hf(repo_name, folder_path, token ):
     """
     Upload all files from a folder to a Hugging Face repository.
 
     Parameters:
```

### Comparing `faster_translate-0.1.0/pyproject.toml` & `faster_translate-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Your Name", email = "your.email@example.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

