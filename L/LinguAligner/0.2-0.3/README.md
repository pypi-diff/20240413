# Comparing `tmp/lingualigner-0.2.tar.gz` & `tmp/lingualigner-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingualigner-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lingualigner-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lingualigner-0.2.tar` & `lingualigner-0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.2/LICENSE
--rw-r--r--   0        0        0     2181 2024-04-12 23:46:51.606031 lingualigner-0.2/LinguAligner/__init__.py
--rw-r--r--   0        0        0     6267 2024-04-12 18:43:15.944779 lingualigner-0.2/LinguAligner/aligners.py
--rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.2/LinguAligner/multiple_translations.py
--rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.2/LinguAligner/translation.py
--rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.2/LinguAligner/utils.py
--rw-r--r--   0        0        0     2590 2024-04-12 23:46:19.224753 lingualigner-0.2/README.md
--rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.2/pyproject.toml
--rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 lingualigner-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.3/LICENSE
+-rw-r--r--   0        0        0     2181 2024-04-12 23:47:58.126810 lingualigner-0.3/LinguAligner/__init__.py
+-rw-r--r--   0        0        0     6267 2024-04-12 18:43:15.944779 lingualigner-0.3/LinguAligner/aligners.py
+-rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.3/LinguAligner/multiple_translations.py
+-rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.3/LinguAligner/translation.py
+-rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.3/LinguAligner/utils.py
+-rw-r--r--   0        0        0     2594 2024-04-12 23:47:36.019246 lingualigner-0.3/README.md
+-rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 lingualigner-0.3/PKG-INFO
```

### Comparing `lingualigner-0.2/LICENSE` & `lingualigner-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lingualigner-0.2/LinguAligner/__init__.py` & `lingualigner-0.3/LinguAligner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """An amazing sample package!dd"""
 
-__version__ = "0.2"
+__version__ = "0.3"
 
 
 from . import aligners
 import spacy
 from . import translation
 from transformers import BertTokenizer, BertModel, logging
 logging.set_verbosity_error()
```

### Comparing `lingualigner-0.2/LinguAligner/aligners.py` & `lingualigner-0.3/LinguAligner/aligners.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.2/LinguAligner/multiple_translations.py` & `lingualigner-0.3/LinguAligner/multiple_translations.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.2/LinguAligner/translation.py` & `lingualigner-0.3/LinguAligner/translation.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.2/LinguAligner/utils.py` & `lingualigner-0.3/LinguAligner/utils.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.2/README.md` & `lingualigner-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # LinguAlign
-LinguALign is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALign has since been adapted into a versatile package for effortless translation of other corpora.
+LinguALigner is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALigner has since been adapted into a versatile package for effortless translation of other corpora.
 
 It is composed of two main components: 
 
 - Text translation: We support DeepL Translator, Google Translator and Microsoft Translators APIs. 
 - Annotations alignments: We developed an annotation alignment pipeline that uses several alignment techniques to align the translated annotations within the translated text.
```

### Comparing `lingualigner-0.2/PKG-INFO` & `lingualigner-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: LinguAligner
-Version: 0.2
+Version: 0.3
 Summary: An amazing sample package!dd
 Author-email: lfc <lfc@di.uminho.pt>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 # LinguAlign
-LinguALign is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALign has since been adapted into a versatile package for effortless translation of other corpora.
+LinguALigner is a comprehensive corpus translation and alignment pipeline designed to facilitate the translation of corpora across different languages. It translates corpora using machine translation and aligns the translated annotations with their corresponding translated text. Initially developed for the automatic translation of ACE-2005 into Portuguese, LinguALigner has since been adapted into a versatile package for effortless translation of other corpora.
 
 It is composed of two main components: 
 
 - Text translation: We support DeepL Translator, Google Translator and Microsoft Translators APIs. 
 - Annotations alignments: We developed an annotation alignment pipeline that uses several alignment techniques to align the translated annotations within the translated text.
```

