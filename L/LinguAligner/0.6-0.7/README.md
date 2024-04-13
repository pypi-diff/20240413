# Comparing `tmp/lingualigner-0.6.tar.gz` & `tmp/lingualigner-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingualigner-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lingualigner-0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lingualigner-0.6.tar` & `lingualigner-0.7.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.6/LICENSE
--rw-r--r--   0        0        0     2507 2024-04-13 00:31:32.683476 lingualigner-0.6/LinguAligner/__init__.py
--rw-r--r--   0        0        0     6324 2024-04-13 00:17:53.246358 lingualigner-0.6/LinguAligner/aligners.py
--rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.6/LinguAligner/multiple_translations.py
--rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.6/LinguAligner/translation.py
--rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.6/LinguAligner/utils.py
--rw-r--r--   0        0        0     4904 2024-04-13 00:31:16.795299 lingualigner-0.6/README.md
--rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.6/pyproject.toml
--rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 lingualigner-0.6/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-13 00:41:40.164099 lingualigner-0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.7/LICENSE
+-rw-r--r--   0        0        0     2507 2024-04-13 00:40:06.591186 lingualigner-0.7/LinguAligner/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-13 00:17:53.246358 lingualigner-0.7/LinguAligner/aligners.py
+-rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.7/LinguAligner/multiple_translations.py
+-rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.7/LinguAligner/translation.py
+-rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.7/LinguAligner/utils.py
+-rw-r--r--   0        0        0     4904 2024-04-13 00:31:16.795299 lingualigner-0.7/README.md
+-rw-r--r--   0        0        0   101207 2024-02-08 00:36:31.515866 lingualigner-0.7/img/eval_EE.png
+-rw-r--r--   0        0        0    88477 2024-02-08 00:35:58.477683 lingualigner-0.7/img/eval_by_comp.png
+-rw-r--r--   0        0        0      454 2024-04-13 00:39:51.431876 lingualigner-0.7/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-12 13:43:59.759184 lingualigner-0.7/resources/resource.json
+-rw-r--r--   0        0        0     4782 2024-04-13 00:29:23.803830 lingualigner-0.7/teste.ipynb
+-rw-r--r--   0        0        0     5386 1970-01-01 00:00:00.000000 lingualigner-0.7/PKG-INFO
```

### Comparing `lingualigner-0.6/LICENSE` & `lingualigner-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/LinguAligner/__init__.py` & `lingualigner-0.7/LinguAligner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. """
-__version__ = "0.6"
+__version__ = "0.7"
 
 
 from . import aligners
 import spacy
 from . import translation
 from transformers import BertTokenizer, BertModel, logging
 logging.set_verbosity_error()
```

### Comparing `lingualigner-0.6/LinguAligner/aligners.py` & `lingualigner-0.7/LinguAligner/aligners.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/LinguAligner/multiple_translations.py` & `lingualigner-0.7/LinguAligner/multiple_translations.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/LinguAligner/translation.py` & `lingualigner-0.7/LinguAligner/translation.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/LinguAligner/utils.py` & `lingualigner-0.7/LinguAligner/utils.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/README.md` & `lingualigner-0.7/README.md`

 * *Files identical despite different names*

### Comparing `lingualigner-0.6/PKG-INFO` & `lingualigner-0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: LinguAligner
-Version: 0.6
+Version: 0.7
 Summary: LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. 
 Author-email: lfc <lfc@di.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Project-URL: Homepage, https://github.com/lfcc1/LinguAligner
+Project-URL: Issues, https://github.com/lfcc1/LinguAligner/issues
 
 # LinguAligner
 LinguALigner is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALigner has since been adapted into a versatile package for effortless translation of other corpora.
 
 It is composed of two main components: 
 
 - Text translation: We support DeepL Translator, Google Translator and Microsoft Translators APIs.
```

