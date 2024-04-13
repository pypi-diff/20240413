# Comparing `tmp/dialog_lib-0.0.1.3.tar.gz` & `tmp/dialog_lib-0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_lib-0.0.1.3.tar", max compression
+gzip compressed data, was "dialog_lib-0.0.1.5.tar", max compression
```

## Comparing `dialog_lib-0.0.1.3.tar` & `dialog_lib-0.0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       98 2024-04-12 00:39:12.358734 dialog_lib-0.0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-12 00:17:13.466371 dialog_lib-0.0.1.3/dialog_lib/agents/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-12 00:26:30.131591 dialog_lib-0.0.1.3/dialog_lib/agents/abstract.py
--rw-r--r--   0        0        0      117 2024-04-12 00:34:49.628803 dialog_lib-0.0.1.3/dialog_lib/db/__init__.py
--rw-r--r--   0        0        0     2604 2024-04-12 18:11:08.688869 dialog_lib-0.0.1.3/dialog_lib/db/memory.py
--rw-r--r--   0        0        0     1325 2024-04-12 00:16:35.393721 dialog_lib-0.0.1.3/dialog_lib/db/models.py
--rw-r--r--   0        0        0      389 2024-04-12 18:11:15.544813 dialog_lib-0.0.1.3/dialog_lib/db/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 00:27:53.398079 dialog_lib-0.0.1.3/dialog_lib/embeddings/__init__.py
--rw-r--r--   0        0        0     1427 2024-04-12 01:39:27.537029 dialog_lib-0.0.1.3/dialog_lib/embeddings/generate.py
--rw-r--r--   0        0        0      148 2024-04-12 00:08:12.155498 dialog_lib-0.0.1.3/dialog_lib/main.py
--rw-r--r--   0        0        0      629 2024-04-12 18:18:20.791824 dialog_lib-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       98 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/agents/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/agents/abstract.py
+-rw-r--r--   0        0        0      117 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/db/__init__.py
+-rw-r--r--   0        0        0     2604 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/db/memory.py
+-rw-r--r--   0        0        0     1325 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/db/models.py
+-rw-r--r--   0        0        0      389 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/db/utils.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     1426 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/embeddings/generate.py
+-rw-r--r--   0        0        0      148 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/dialog_lib/main.py
+-rw-r--r--   0        0        0      629 2024-04-13 15:42:24.001390 dialog_lib-0.0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.5/PKG-INFO
```

### Comparing `dialog_lib-0.0.1.3/dialog_lib/agents/abstract.py` & `dialog_lib-0.0.1.5/dialog_lib/agents/abstract.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.3/dialog_lib/db/memory.py` & `dialog_lib-0.0.1.5/dialog_lib/db/memory.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.3/dialog_lib/db/models.py` & `dialog_lib-0.0.1.5/dialog_lib/db/models.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.3/dialog_lib/embeddings/generate.py` & `dialog_lib-0.0.1.5/dialog_lib/embeddings/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def get_most_relevant_contents_from_message(
         message,
         top=5,
         dataset=None,
         session=None,
-        cosine_similarity_threshold=0.5,
+        cosine_similarity_threshold=0.5
     ):
     message_embedding = generate_embedding(message)
     filters = [
         CompanyContent.embedding.cosine_distance(message_embedding) < cosine_similarity_threshold,
     ]
 
     if dataset is not None:
```

### Comparing `dialog_lib-0.0.1.3/pyproject.toml` & `dialog_lib-0.0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialog-lib"
-version = "0.0.1.3"
+version = "0.0.1.5"
 description = ""
 authors = ["Talkd.AI <foss@talkd.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dialog_lib-0.0.1.3/PKG-INFO` & `dialog_lib-0.0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-lib
-Version: 0.0.1.3
+Version: 0.0.1.5
 Summary: 
 License: MIT
 Author: Talkd.AI
 Author-email: foss@talkd.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

