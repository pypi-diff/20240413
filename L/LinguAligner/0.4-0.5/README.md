# Comparing `tmp/lingualigner-0.4.tar.gz` & `tmp/lingualigner-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingualigner-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lingualigner-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lingualigner-0.4.tar` & `lingualigner-0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.4/LICENSE
--rw-r--r--   0        0        0     2181 2024-04-12 23:48:30.796541 lingualigner-0.4/LinguAligner/__init__.py
--rw-r--r--   0        0        0     6267 2024-04-12 18:43:15.944779 lingualigner-0.4/LinguAligner/aligners.py
--rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.4/LinguAligner/multiple_translations.py
--rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.4/LinguAligner/translation.py
--rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.4/LinguAligner/utils.py
--rw-r--r--   0        0        0     2596 2024-04-12 23:48:20.599363 lingualigner-0.4/README.md
--rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.4/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 lingualigner-0.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.5/LICENSE
+-rw-r--r--   0        0        0     2418 2024-04-12 23:49:45.394457 lingualigner-0.5/LinguAligner/__init__.py
+-rw-r--r--   0        0        0     6267 2024-04-12 18:43:15.944779 lingualigner-0.5/LinguAligner/aligners.py
+-rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.5/LinguAligner/multiple_translations.py
+-rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.5/LinguAligner/translation.py
+-rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.5/LinguAligner/utils.py
+-rw-r--r--   0        0        0     2596 2024-04-12 23:48:20.599363 lingualigner-0.5/README.md
+-rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 lingualigner-0.5/PKG-INFO
```

### Comparing `lingualigner-0.4/LICENSE` & `lingualigner-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/LinguAligner/__init__.py` & `lingualigner-0.5/LinguAligner/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""An amazing sample package!dd"""
+"""LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. """
 
-__version__ = "0.4"
+__version__ = "0.5"
 
 
 from . import aligners
 import spacy
 from . import translation
 from transformers import BertTokenizer, BertModel, logging
 logging.set_verbosity_error()
```

### Comparing `lingualigner-0.4/LinguAligner/aligners.py` & `lingualigner-0.5/LinguAligner/aligners.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/LinguAligner/multiple_translations.py` & `lingualigner-0.5/LinguAligner/multiple_translations.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/LinguAligner/translation.py` & `lingualigner-0.5/LinguAligner/translation.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/LinguAligner/utils.py` & `lingualigner-0.5/LinguAligner/utils.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/README.md` & `lingualigner-0.5/README.md`

 * *Files identical despite different names*

### Comparing `lingualigner-0.4/PKG-INFO` & `lingualigner-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: LinguAligner
-Version: 0.4
-Summary: An amazing sample package!dd
+Version: 0.5
+Summary: LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. 
 Author-email: lfc <lfc@di.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 # LinguAligner
 LinguALigner is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALigner has since been adapted into a versatile package for effortless translation of other corpora.
```

