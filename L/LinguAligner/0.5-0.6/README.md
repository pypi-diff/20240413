# Comparing `tmp/lingualigner-0.5.tar.gz` & `tmp/lingualigner-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingualigner-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lingualigner-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lingualigner-0.5.tar` & `lingualigner-0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.5/LICENSE
--rw-r--r--   0        0        0     2418 2024-04-12 23:49:45.394457 lingualigner-0.5/LinguAligner/__init__.py
--rw-r--r--   0        0        0     6267 2024-04-12 18:43:15.944779 lingualigner-0.5/LinguAligner/aligners.py
--rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.5/LinguAligner/multiple_translations.py
--rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.5/LinguAligner/translation.py
--rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.5/LinguAligner/utils.py
--rw-r--r--   0        0        0     2596 2024-04-12 23:48:20.599363 lingualigner-0.5/README.md
--rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.5/pyproject.toml
--rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 lingualigner-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-04-12 15:55:09.589586 lingualigner-0.6/LICENSE
+-rw-r--r--   0        0        0     2507 2024-04-13 00:31:32.683476 lingualigner-0.6/LinguAligner/__init__.py
+-rw-r--r--   0        0        0     6324 2024-04-13 00:17:53.246358 lingualigner-0.6/LinguAligner/aligners.py
+-rw-r--r--   0        0        0     1359 2024-04-12 19:03:23.712783 lingualigner-0.6/LinguAligner/multiple_translations.py
+-rw-r--r--   0        0        0     4529 2024-04-12 18:55:33.013673 lingualigner-0.6/LinguAligner/translation.py
+-rw-r--r--   0        0        0     2398 2023-07-05 13:10:41.000000 lingualigner-0.6/LinguAligner/utils.py
+-rw-r--r--   0        0        0     4904 2024-04-13 00:31:16.795299 lingualigner-0.6/README.md
+-rw-r--r--   0        0        0      327 2024-04-12 23:45:31.966723 lingualigner-0.6/pyproject.toml
+-rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 lingualigner-0.6/PKG-INFO
```

### Comparing `lingualigner-0.5/LICENSE` & `lingualigner-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lingualigner-0.5/LinguAligner/__init__.py` & `lingualigner-0.6/LinguAligner/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """LinguAligner is a Python library for aligning annotations in parallel corpora. It is designed to be used in the context of parallel corpora annotation alignment, where the goal is to align annotations in the source language with annotations in the target language. """
-
-__version__ = "0.5"
+__version__ = "0.6"
 
 
 from . import aligners
 import spacy
 from . import translation
 from transformers import BertTokenizer, BertModel, logging
 logging.set_verbosity_error()
@@ -23,28 +22,31 @@
             print("Model loaded")
 
     def align_annotation(self, src_sent,src_ann, tgt_sent, trans_ann, lookupTable=None):
         pipeline = self.config["pipeline"]
         nlp = self.nlp
         res = aligners.regex_string_match(tgt_sent,trans_ann) 
         if not res:
-            
-            for method in pipeline:
-                print(res, method)
-                if not res and method == 'lemma':
+            i = 0
+            while i < len(pipeline) and not res:
+                method = pipeline[i]
+                if method == 'lemma':
                     res = aligners.lemma_match(tgt_sent,trans_ann,nlp)
-                elif not res and method == 'external_resource' and lookupTable: # Mtrans is combined with lemma method since we also calculate the lemma of the translations
-                    res = aligners.resource_match(tgt_sent,src_ann,nlp,lookupTable)
-                elif not res and method == 'word_aligner':
+                elif method == 'M_Trans': # Mtrans is combined with lemma method since we also calculate the lemma of the translations
+                    if lookupTable:
+                        res = aligners.resource_match(tgt_sent,src_ann,nlp,lookupTable)
+                    else: print("Lookup table not provided for M_Trans method. (skipped)")
+                elif method == 'word_aligner':
                     res = aligners.wordAligner(src_sent,tgt_sent,src_ann,nlp, self.tokenizer, self.model)
-                elif not res and method == 'gestalt':
+                elif method == 'gestalt':
                     res = aligners.gestalt_match(src_ann,tgt_sent,nlp)
-                elif not res and method == 'leveinstein':
+                elif method == 'leveinstein':
                     res = aligners.leveinstein_match(src_ann,tgt_sent,nlp)
                 else:
                     print(f"Invalid alignment method: {method}")
+                i += 1
         return res
     
 
 
 #res = align_annotation("The ship land on the shore","O barco desembarcou na costa","land","terra",nlp) # Expected output: "teste
 #print(res)
```

### Comparing `lingualigner-0.5/LinguAligner/aligners.py` & `lingualigner-0.6/LinguAligner/aligners.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         if ann_span:
             start, end = ann_span
             return ''.join([token.text_with_ws for token in sent_doc][start:end+1]).strip()
     return None
 
 
 def resource_match(tgt_sent, src_ann,nlp,lookupTable):
+    if src_ann not in lookupTable:
+        return None
     src_translations = lookupTable[src_ann]
     i = 0
     res = None
     while i < len(src_translations) and res == None:
         src_trans = src_translations[i]
         
         if regex_string_match(tgt_sent,src_trans):
```

### Comparing `lingualigner-0.5/LinguAligner/multiple_translations.py` & `lingualigner-0.6/LinguAligner/multiple_translations.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.5/LinguAligner/translation.py` & `lingualigner-0.6/LinguAligner/translation.py`

 * *Files identical despite different names*

### Comparing `lingualigner-0.5/LinguAligner/utils.py` & `lingualigner-0.6/LinguAligner/utils.py`

 * *Files identical despite different names*

