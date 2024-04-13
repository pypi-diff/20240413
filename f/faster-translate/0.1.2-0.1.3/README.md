# Comparing `tmp/faster_translate-0.1.2.tar.gz` & `tmp/faster_translate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.2.tar", last modified: Sat Apr 13 12:27:19 2024, max compression
+gzip compressed data, was "faster_translate-0.1.3.tar", last modified: Sat Apr 13 12:38:59 2024, max compression
```

## Comparing `faster_translate-0.1.2.tar` & `faster_translate-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/
--rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.2/LICENSE
--rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:27:19.210276 faster_translate-0.1.2/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.2/README.md
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/faster_translate/
--rw-------   0 azureuser  (1000) users      (100)       75 2024-04-13 12:27:12.000000 faster_translate-0.1.2/faster_translate/__init__.py
--rw-------   0 azureuser  (1000) users      (100)     6172 2024-04-13 12:25:14.000000 faster_translate-0.1.2/faster_translate/model.py
--rw-------   0 azureuser  (1000) users      (100)     2198 2024-04-13 11:23:46.000000 faster_translate-0.1.2/faster_translate/utils.py
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/faster_translate.egg-info/
--rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/SOURCES.txt
--rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/dependency_links.txt
--rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/requires.txt
--rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/top_level.txt
--rw-------   0 azureuser  (1000) users      (100)      640 2024-04-13 12:26:41.000000 faster_translate-0.1.2/pyproject.toml
--rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 12:27:19.210276 faster_translate-0.1.2/setup.cfg
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.283745 faster_translate-0.1.3/
+-rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.3/LICENSE
+-rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:38:59.283745 faster_translate-0.1.3/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.3/README.md
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.279745 faster_translate-0.1.3/faster_translate/
+-rw-------   0 azureuser  (1000) users      (100)       75 2024-04-13 12:27:12.000000 faster_translate-0.1.3/faster_translate/__init__.py
+-rw-------   0 azureuser  (1000) users      (100)     6597 2024-04-13 12:37:57.000000 faster_translate-0.1.3/faster_translate/model.py
+-rw-------   0 azureuser  (1000) users      (100)     2057 2024-04-13 12:38:30.000000 faster_translate-0.1.3/faster_translate/utils.py
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.283745 faster_translate-0.1.3/faster_translate.egg-info/
+-rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/SOURCES.txt
+-rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/dependency_links.txt
+-rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/requires.txt
+-rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/top_level.txt
+-rw-------   0 azureuser  (1000) users      (100)      640 2024-04-13 12:38:52.000000 faster_translate-0.1.3/pyproject.toml
+-rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 12:38:59.283745 faster_translate-0.1.3/setup.cfg
```

### Comparing `faster_translate-0.1.2/LICENSE` & `faster_translate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.2/PKG-INFO` & `faster_translate-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.2/README.md` & `faster_translate-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.2/faster_translate/model.py` & `faster_translate-0.1.3/faster_translate/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 import os
 import json
+import subprocess
 import ctranslate2
 from tqdm.auto import tqdm
 from tokenizers import Tokenizer
 from tokenizers.models import BPE
 from tokenizers.pre_tokenizers import Whitespace
 from tokenizers.trainers import BpeTrainer
 
 from .utils import download_model_hf, _MODELS
 
+
+def is_cuda_available():
+    # Method 1: Check using nvcc
+    try:
+        subprocess.check_output(['nvcc', '--version'])
+        return True
+    except (subprocess.CalledProcessError, FileNotFoundError):
+        pass
+
+    # Method 2: Check CUDA_PATH environment variable
+    if 'CUDA_PATH' in os.environ:
+        return True
+
+    return False
+
+device_name = "cuda" if is_cuda_available() else "cpu"
+
 class TranslateModel:
-    def __init__(self, model_dir, source_token_list = None, normalizer_func=None, device = "cuda"):
+    def __init__(self, model_dir, source_token_list = None, normalizer_func=None, device = device_name):
         self.model_dir = model_dir
         self.translator = ctranslate2.Translator(model_dir, device=device)
         
         if normalizer_func is None:
             self.normalizer_func = lambda x: x
         elif isinstance(normalizer_func, str):
             self.normalizer_func = self.get_text_normalizer(normalizer_func)
```

### Comparing `faster_translate-0.1.2/faster_translate/utils.py` & `faster_translate-0.1.3/faster_translate/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,14 @@
     # Use snapshot_download to download the repository or a specific snapshot of it
     if repo_name in _MODELS:
         model_args = _MODELS[repo_name]
         repo_name = model_args["model_repo"]
 
     downloaded_path = snapshot_download(
         repo_id=repo_name,
-        cache_dir=save_path,  # If None, huggingface_hub uses its default cache directory
+        cache_dir=save_path,  
         revision=revision,
-        use_auth_token=token if token else True  # Pass True to use the token from the HF_HOME or token cache if available
+        token=token if token else None  
     )
     
     print(f"Model downloaded to {downloaded_path}.")
     return downloaded_path
```

### Comparing `faster_translate-0.1.2/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.3/faster_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.2/pyproject.toml` & `faster_translate-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

