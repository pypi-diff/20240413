# Comparing `tmp/dpq-0.1.3.tar.gz` & `tmp/dpq-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpq-0.1.3.tar", max compression
+gzip compressed data, was "dpq-0.1.4.tar", max compression
```

## Comparing `dpq-0.1.3.tar` & `dpq-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     3693 2024-04-12 07:53:08.845937 dpq-0.1.3/README.md
--rw-r--r--   0        0        0       23 2024-04-09 07:16:40.852521 dpq-0.1.3/dpq/__init__.py
--rw-r--r--   0        0        0     5117 2024-04-12 16:17:32.082520 dpq-0.1.3/dpq/dpq.py
--rw-r--r--   0        0        0      567 2024-04-09 07:16:40.852979 dpq-0.1.3/dpq/prompts/classify_sentiment.json
--rw-r--r--   0        0        0      428 2024-04-12 16:17:44.054453 dpq-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 dpq-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 16:25:12.165851 dpq-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3730 2024-04-13 20:19:51.498774 dpq-0.1.4/README.md
+-rw-r--r--   0        0        0       23 2024-04-09 07:16:40.852521 dpq-0.1.4/dpq/__init__.py
+-rw-r--r--   0        0        0     5117 2024-04-12 16:17:32.082520 dpq-0.1.4/dpq/dpq.py
+-rw-r--r--   0        0        0      567 2024-04-13 20:19:51.501474 dpq-0.1.4/dpq/prompts/classify_sentiment.json
+-rw-r--r--   0        0        0      575 2024-04-13 20:37:42.785283 dpq-0.1.4/dpq/prompts/translate_to_english.json
+-rw-r--r--   0        0        0      428 2024-04-13 20:38:28.094526 dpq-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 dpq-0.1.4/PKG-INFO
```

### Comparing `dpq-0.1.3/README.md` & `dpq-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # dpq: data. prompt. query.
 
 dpq is a Python library that makes it easy to process data and engineer features using
 generative AI.
 
-![dpq_demo](https://github.com/data-prompt-query/pre-release/assets/15915676/ea08d1ec-bf2d-473d-b521-d1ae9581050a)
+![dpq_demo](https://github.com/data-prompt-query/dpq/assets/15915676/09d4936c-360a-460f-8abe-15e07af14306)
+
+## installation
+```bash
+pip install dpq
+```
 
 ## quick start
 ```python
 import dpq
 
 # Initialize dpq agent with API configuration
 dpq_agent = dpq.Agent(
```

### Comparing `dpq-0.1.3/dpq/dpq.py` & `dpq-0.1.4/dpq/dpq.py`

 * *Files identical despite different names*

### Comparing `dpq-0.1.3/dpq/prompts/classify_sentiment.json` & `dpq-0.1.4/dpq/prompts/classify_sentiment.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {'1': "{'content': 'I like dpq.'}", '3': "{'content': 'I hate dpq.'}"}*

```diff
@@ -1,22 +1,22 @@
 [
     {
         "content": "You are a sentiment classifier. You classify statements as having either positive or negative overall sentiment. You return only one of two words: positive, negative. do not return any other word except for one of these.",
         "role": "system"
     },
     {
-        "content": "I like dpt.",
+        "content": "I like dpq.",
         "role": "user"
     },
     {
         "content": "positive",
         "role": "assistant"
     },
     {
-        "content": "I hate dpt.",
+        "content": "I hate dpq.",
         "role": "user"
     },
     {
         "content": "negative",
         "role": "assistant"
     }
 ]
```

### Comparing `dpq-0.1.3/PKG-INFO` & `dpq-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpq
-Version: 0.1.3
+Version: 0.1.4
 Summary: dpq is an open-source python library that makes prompt-based data processing and feature engineering easy.
 License: Apache-2.0
 Author: dpq
 Author-email: dpq.code@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,20 @@
 Description-Content-Type: text/markdown
 
 # dpq: data. prompt. query.
 
 dpq is a Python library that makes it easy to process data and engineer features using
 generative AI.
 
-![dpq_demo](https://github.com/data-prompt-query/pre-release/assets/15915676/ea08d1ec-bf2d-473d-b521-d1ae9581050a)
+![dpq_demo](https://github.com/data-prompt-query/dpq/assets/15915676/09d4936c-360a-460f-8abe-15e07af14306)
+
+## installation
+```bash
+pip install dpq
+```
 
 ## quick start
 ```python
 import dpq
 
 # Initialize dpq agent with API configuration
 dpq_agent = dpq.Agent(
```

