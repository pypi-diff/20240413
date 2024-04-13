# Comparing `tmp/codelinker-0.1.0.tar.gz` & `tmp/codelinker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codelinker-0.1.0.tar", max compression
+gzip compressed data, was "codelinker-0.1.1.tar", max compression
```

## Comparing `codelinker-0.1.0.tar` & `codelinker-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1967 2024-04-12 07:51:00.481447 codelinker-0.1.0/README.md
--rw-r--r--   0        0        0     1584 2024-04-12 07:47:18.761466 codelinker-0.1.0/codelinker/__init__.py
--rw-r--r--   0        0        0     3249 2024-04-12 07:32:04.111573 codelinker-0.1.0/codelinker/config.py
--rw-r--r--   0        0        0     8283 2024-04-12 07:58:38.711392 codelinker-0.1.0/codelinker/linker.py
--rw-r--r--   0        0        0       64 2024-04-10 09:33:27.450556 codelinker-0.1.0/codelinker/models/__init__.py
--rw-r--r--   0        0        0      273 2024-04-10 09:33:27.450556 codelinker-0.1.0/codelinker/models/labels.py
--rw-r--r--   0        0        0      308 2024-04-10 08:45:20.740321 codelinker-0.1.0/codelinker/models/structuredRet.py
--rw-r--r--   0        0        0       32 2024-04-10 08:52:51.480358 codelinker-0.1.0/codelinker/request/__init__.py
--rw-r--r--   0        0        0    11665 2024-04-12 07:32:04.111573 codelinker-0.1.0/codelinker/request/objGen.py
--rw-r--r--   0        0        0     5086 2024-04-12 07:32:04.111573 codelinker-0.1.0/codelinker/request/openai.py
--rw-r--r--   0        0        0     1510 2024-04-10 09:35:49.040568 codelinker-0.1.0/codelinker/utils.py
--rw-r--r--   0        0        0      359 2024-04-10 09:36:02.540569 codelinker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 codelinker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-13 16:22:33.640349 codelinker-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1968 2024-04-13 16:22:33.640349 codelinker-0.1.1/README.md
+-rw-r--r--   0        0        0     1584 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/__init__.py
+-rw-r--r--   0        0        0     3249 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/config.py
+-rw-r--r--   0        0        0     8283 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/linker.py
+-rw-r--r--   0        0        0       64 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/models/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/models/labels.py
+-rw-r--r--   0        0        0      308 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/models/structuredRet.py
+-rw-r--r--   0        0        0       32 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/request/__init__.py
+-rw-r--r--   0        0        0    11665 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/request/objGen.py
+-rw-r--r--   0        0        0     5086 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/request/openai.py
+-rw-r--r--   0        0        0     1510 2024-04-13 16:22:33.640349 codelinker-0.1.1/codelinker/utils.py
+-rw-r--r--   0        0        0      359 2024-04-13 16:22:33.640349 codelinker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 codelinker-0.1.1/PKG-INFO
```

### Comparing `codelinker-0.1.0/README.md` & `codelinker-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CodeLinker: Link your code with Language Models
+# CodeLinker : Link your code with Language Models
 
 CodeLinker aims to provide functions to link your code with language models.
 It builds on top of the Pydatic library and Tool Calling abilities introduced by [OpenAI](https://platform.openai.com/docs/guides/function-calling), which enabling models to generate content according to [Json Schema](https://json-schema.org/).
 
 ## Usage
 The core concept of this package is to treat language models as a function handler.
 By defining a schema for return value of the function, we can call the function and let the model generate the return value.
```

### Comparing `codelinker-0.1.0/codelinker/__init__.py` & `codelinker-0.1.1/codelinker/__init__.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/codelinker/config.py` & `codelinker-0.1.1/codelinker/config.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/codelinker/linker.py` & `codelinker-0.1.1/codelinker/linker.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/codelinker/request/objGen.py` & `codelinker-0.1.1/codelinker/request/objGen.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/codelinker/request/openai.py` & `codelinker-0.1.1/codelinker/request/openai.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/codelinker/utils.py` & `codelinker-0.1.1/codelinker/utils.py`

 * *Files identical despite different names*

### Comparing `codelinker-0.1.0/PKG-INFO` & `codelinker-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codelinker
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: luyaxi
 Author-email: luyaxi@live.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,15 @@
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: openai (>=1.16.2,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
-# CodeLinker: Link your code with Language Models
+# CodeLinker : Link your code with Language Models
 
 CodeLinker aims to provide functions to link your code with language models.
 It builds on top of the Pydatic library and Tool Calling abilities introduced by [OpenAI](https://platform.openai.com/docs/guides/function-calling), which enabling models to generate content according to [Json Schema](https://json-schema.org/).
 
 ## Usage
 The core concept of this package is to treat language models as a function handler.
 By defining a schema for return value of the function, we can call the function and let the model generate the return value.
```

