# Comparing `tmp/faster_translate-0.1.3.tar.gz` & `tmp/faster_translate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.3.tar", last modified: Sat Apr 13 12:38:59 2024, max compression
+gzip compressed data, was "faster_translate-0.1.4.tar", last modified: Sat Apr 13 21:15:23 2024, max compression
```

## Comparing `faster_translate-0.1.3.tar` & `faster_translate-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.283745 faster_translate-0.1.3/
--rw-------   0 azureuser  (1000) users      (100)     1069 2024-04-13 07:01:03.000000 faster_translate-0.1.3/LICENSE
--rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:38:59.283745 faster_translate-0.1.3/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)     2974 2024-04-13 11:20:57.000000 faster_translate-0.1.3/README.md
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.279745 faster_translate-0.1.3/faster_translate/
--rw-------   0 azureuser  (1000) users      (100)       75 2024-04-13 12:27:12.000000 faster_translate-0.1.3/faster_translate/__init__.py
--rw-------   0 azureuser  (1000) users      (100)     6597 2024-04-13 12:37:57.000000 faster_translate-0.1.3/faster_translate/model.py
--rw-------   0 azureuser  (1000) users      (100)     2057 2024-04-13 12:38:30.000000 faster_translate-0.1.3/faster_translate/utils.py
-drwx------   0 azureuser  (1000) users      (100)        0 2024-04-13 12:38:59.283745 faster_translate-0.1.3/faster_translate.egg-info/
--rw-r--r--   0 azureuser  (1000) users      (100)     4742 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/PKG-INFO
--rw-------   0 azureuser  (1000) users      (100)      312 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/SOURCES.txt
--rw-------   0 azureuser  (1000) users      (100)        1 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/dependency_links.txt
--rw-------   0 azureuser  (1000) users      (100)       62 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/requires.txt
--rw-------   0 azureuser  (1000) users      (100)       17 2024-04-13 12:38:59.000000 faster_translate-0.1.3/faster_translate.egg-info/top_level.txt
--rw-------   0 azureuser  (1000) users      (100)      640 2024-04-13 12:38:52.000000 faster_translate-0.1.3/pyproject.toml
--rw-------   0 azureuser  (1000) users      (100)       38 2024-04-13 12:38:59.283745 faster_translate-0.1.3/setup.cfg
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.4/LICENSE
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:15:23.000898 faster_translate-0.1.4/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.4/README.md
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/faster_translate/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.4/faster_translate/__init__.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     6764 2024-04-13 20:26:22.000000 faster_translate-0.1.4/faster_translate/model.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2057 2024-04-13 18:35:30.000000 faster_translate-0.1.4/faster_translate/utils.py
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/faster_translate.egg-info/
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/SOURCES.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/dependency_links.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/requires.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/top_level.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-13 21:15:16.000000 faster_translate-0.1.4/pyproject.toml
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-13 21:15:23.000898 faster_translate-0.1.4/setup.cfg
```

### Comparing `faster_translate-0.1.3/LICENSE` & `faster_translate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.3/PKG-INFO` & `faster_translate-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: huggingface_hub>=0.0.12
 Requires-Dist: ctranslate2>=4.1.0
 Requires-Dist: tokenizers>=0.15.2
+Requires-Dist: csebuetnlp-normalizer>=1.0.0
 
 
 # Faster Translate
 
 Faster Translate is a high-performance translation library built on top of ctranslate2 and designed for fast and efficient translation. It provides an easy-to-use interface for translating text in various languages with support for pre-trained models from Hugging Face's model hub.
 
 ## Features
```

### Comparing `faster_translate-0.1.3/README.md` & `faster_translate-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.3/faster_translate/model.py` & `faster_translate-0.1.4/faster_translate/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,31 +51,32 @@
     def get_bpe_tokenizer(self, token_list):
         
         # Initialize a tokenizer
         tokenizer = Tokenizer(BPE(unk_token="<unk>"))
         tokenizer.pre_tokenizer = Whitespace()
         
         # Trainer to train the tokenizer
-        trainer = BpeTrainer(special_tokens=token_list)
+        trainer = BpeTrainer(special_tokens=token_list, vocab_size=len(token_list), min_frequency=1)
         tokenizer.train_from_iterator(token_list, trainer=trainer)
         
         return tokenizer
     
     
     def source_tokenize_batch(self, text_batch):
+        text_batch = [f" {text}".replace(" ", "▁") for text in text_batch]
         tokenized_batch = [encoded.tokens for encoded in self.source_tokenizer.encode_batch(text_batch)]
         return tokenized_batch
     
     
     def get_text_normalizer(self, normalizer_func_name):
         if normalizer_func_name == "buetnlpnormalizer":
             try:
                 from normalizer import normalize
             except:
-                raise Exception("BUETCSEnlp not installed, please install with `pip install git+https://github.com/csebuetnlp/normalizer`")
+                raise Exception("Relevant Normalizer not installed, please install with `pip install git+https://github.com/csebuetnlp/normalizer`")
             
             normalizer_func = lambda texts: [normalize(text) for text in texts]
         else:
             raise Exception(f"{normalizer_func_name} not supported yet.")
         return normalizer_func
         
         
@@ -97,14 +98,15 @@
         translated_batch = self.translate_batch(text_batch)
         return translated_batch[0]
 
 
     def translate_batch(self, text_batch):
         normalized_text_batch = self.normalizer_func(text_batch)
         tokenized_text_batch = self.source_tokenize_batch(normalized_text_batch)
+        print(tokenized_text_batch)
         translated_tokens_batch = self.translator.translate_batch(tokenized_text_batch)
         translated_batch = self.detokenize_batch(translated_tokens_batch)
         return translated_batch
     
     
     def translate_bulk(self, text_list, batch_size=1):
         text_batches = [text_list[i:i + batch_size] for i in range(0, len(text_list), batch_size)]
```

### Comparing `faster_translate-0.1.3/faster_translate/utils.py` & `faster_translate-0.1.4/faster_translate/utils.py`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.3/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.4/faster_translate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: huggingface_hub>=0.0.12
 Requires-Dist: ctranslate2>=4.1.0
 Requires-Dist: tokenizers>=0.15.2
+Requires-Dist: csebuetnlp-normalizer>=1.0.0
 
 
 # Faster Translate
 
 Faster Translate is a high-performance translation library built on top of ctranslate2 and designed for fast and efficient translation. It provides an easy-to-use interface for translating text in various languages with support for pre-trained models from Hugging Face's model hub.
 
 ## Features
```

### Comparing `faster_translate-0.1.3/pyproject.toml` & `faster_translate-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
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
+    "csebuetnlp-normalizer>=1.0.0",
 ]
```

