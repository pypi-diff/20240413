# Comparing `tmp/faster_translate-0.1.1.tar.gz` & `tmp/faster_translate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.1.tar", last modified: Sat Apr 13 11:45:21 2024, max compression
+gzip compressed data, was "faster_translate-0.1.2.tar", last modified: Sat Apr 13 12:27:19 2024, max compression
```

## Comparing `faster_translate-0.1.1.tar` & `faster_translate-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/
--rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.1/LICENSE
--rw-r--r--   0 azureuser  (1000) users      (100)     4741 2024-04-13 11:45:21.385757 faster_translate-0.1.1/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.1/README.md
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/faster_translate/
--rw-------   0 azureuser  (1000) users      (100)       33 2024-04-13 06:57:04.000000 faster_translate-0.1.1/faster_translate/__init__.py
--rw-------   0 azureuser  (1000) users      (100)     5978 2024-04-13 10:53:09.000000 faster_translate-0.1.1/faster_translate/model.py
--rw-------   0 azureuser  (1000) users      (100)     2198 2024-04-13 11:23:46.000000 faster_translate-0.1.1/faster_translate/utils.py
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 11:45:21.385757 faster_translate-0.1.1/faster_translate.egg-info/
--rw-r--r--   0 azureuser  (1000) users      (100)     4741 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/SOURCES.txt
--rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/dependency_links.txt
--rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/requires.txt
--rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 11:45:21.000000 faster_translate-0.1.1/faster_translate.egg-info/top_level.txt
--rw-------   0 azureuser  (1000) users      (100)      637 2024-04-13 11:45:15.000000 faster_translate-0.1.1/pyproject.toml
--rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 11:45:21.385757 faster_translate-0.1.1/setup.cfg
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/
+-rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.2/LICENSE
+-rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:27:19.210276 faster_translate-0.1.2/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.2/README.md
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/faster_translate/
+-rw-------   0 azureuser  (1000) users      (100)       75 2024-04-13 12:27:12.000000 faster_translate-0.1.2/faster_translate/__init__.py
+-rw-------   0 azureuser  (1000) users      (100)     6172 2024-04-13 12:25:14.000000 faster_translate-0.1.2/faster_translate/model.py
+-rw-------   0 azureuser  (1000) users      (100)     2198 2024-04-13 11:23:46.000000 faster_translate-0.1.2/faster_translate/utils.py
+drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:27:19.210276 faster_translate-0.1.2/faster_translate.egg-info/
+-rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/PKG-INFO
+-rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/SOURCES.txt
+-rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/dependency_links.txt
+-rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/requires.txt
+-rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 12:27:19.000000 faster_translate-0.1.2/faster_translate.egg-info/top_level.txt
+-rw-------   0 azureuser  (1000) users      (100)      640 2024-04-13 12:26:41.000000 faster_translate-0.1.2/pyproject.toml
+-rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 12:27:19.210276 faster_translate-0.1.2/setup.cfg
```

### Comparing `faster_translate-0.1.1/LICENSE` & `faster_translate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.1/PKG-INFO` & `faster_translate-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple translation utility using Hugging Face models.
-Author-email: Your Name <your.email@example.com>
+Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `faster_translate-0.1.1/README.md` & `faster_translate-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.1/faster_translate/model.py` & `faster_translate-0.1.2/faster_translate/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,19 @@
     def source_tokenize_batch(self, text_batch):
         tokenized_batch = [encoded.tokens for encoded in self.source_tokenizer.encode_batch(text_batch)]
         return tokenized_batch
     
     
     def get_text_normalizer(self, normalizer_func_name):
         if normalizer_func_name == "buetnlpnormalizer":
-            from normalizer import normalize
+            try:
+                from normalizer import normalize
+            except:
+                raise Exception("BUETCSEnlp not installed, please install with `pip install git+https://github.com/csebuetnlp/normalizer`")
+            
             normalizer_func = lambda texts: [normalize(text) for text in texts]
         else:
             raise Exception(f"{normalizer_func_name} not supported yet.")
         return normalizer_func
         
         
     def detokenize_single(self, tokens):
```

### Comparing `faster_translate-0.1.1/faster_translate/utils.py` & `faster_translate-0.1.2/faster_translate/utils.py`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.1/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.2/faster_translate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple translation utility using Hugging Face models.
-Author-email: Your Name <your.email@example.com>
+Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `faster_translate-0.1.1/pyproject.toml` & `faster_translate-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
-authors = [{name = "Your Name", email = "your.email@example.com"}]
+authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "huggingface_hub>=0.0.12",
     "ctranslate2>=4.1.0",
     "tokenizers>=0.15.2",
-]
+]
+
```

