# Comparing `tmp/dialog_lib-0.0.1.6.tar.gz` & `tmp/dialog_lib-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_lib-0.0.1.6.tar", max compression
+gzip compressed data, was "dialog_lib-0.0.1.7.tar", max compression
```

## Comparing `dialog_lib-0.0.1.6.tar` & `dialog_lib-0.0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       98 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/agents/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/agents/abstract.py
--rw-r--r--   0        0        0      117 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/db/__init__.py
--rw-r--r--   0        0        0     2604 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/db/memory.py
--rw-r--r--   0        0        0     1325 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/db/models.py
--rw-r--r--   0        0        0      389 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/db/utils.py
--rw-r--r--   0        0        0        0 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/embeddings/__init__.py
--rw-r--r--   0        0        0     1471 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/embeddings/generate.py
--rw-r--r--   0        0        0      148 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/dialog_lib/main.py
--rw-r--r--   0        0        0      629 2024-04-13 15:55:36.189957 dialog_lib-0.0.1.6/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       98 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/agents/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/agents/abstract.py
+-rw-r--r--   0        0        0      117 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/db/__init__.py
+-rw-r--r--   0        0        0     2717 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/db/memory.py
+-rw-r--r--   0        0        0     1325 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/db/models.py
+-rw-r--r--   0        0        0      389 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/db/utils.py
+-rw-r--r--   0        0        0        0 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     1471 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/embeddings/generate.py
+-rw-r--r--   0        0        0      148 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/dialog_lib/main.py
+-rw-r--r--   0        0        0      629 2024-04-13 19:13:20.620397 dialog_lib-0.0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.7/PKG-INFO
```

### Comparing `dialog_lib-0.0.1.6/dialog_lib/agents/abstract.py` & `dialog_lib-0.0.1.7/dialog_lib/agents/abstract.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.6/dialog_lib/db/memory.py` & `dialog_lib-0.0.1.7/dialog_lib/db/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,25 +56,25 @@
         session_id=session_id,
         parent_session_id=parent_session_id,
         table_name="chat_messages",
         dbsession=dbsession
     )
 
 
-def add_user_message_to_message_history(session_id, message, memory=None, dbsession=None):
+def add_user_message_to_message_history(session_id, message, memory=None, dbsession=None, database_url=None):
     """
     Add a user message to the message history and returns the updated
     memory instance
     """
     if not memory:
-        memory = generate_memory_instance(session_id)
+        memory = generate_memory_instance(session_id, dbsession=dbsession, database_url=database_url)
 
     memory.add_user_message(message)
     return memory
 
 
-def get_messages(session_id, dbsession=None):
+def get_messages(session_id, dbsession=None, database_url=None):
     """
     Get all messages for a given session_id
     """
-    memory = generate_memory_instance(session_id, dbsession=dbsession)
+    memory = generate_memory_instance(session_id, dbsession=dbsession, database_url=database_url)
     return memory.messages
```

### Comparing `dialog_lib-0.0.1.6/dialog_lib/db/models.py` & `dialog_lib-0.0.1.7/dialog_lib/db/models.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.6/dialog_lib/embeddings/generate.py` & `dialog_lib-0.0.1.7/dialog_lib/embeddings/generate.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.6/pyproject.toml` & `dialog_lib-0.0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialog-lib"
-version = "0.0.1.6"
+version = "0.0.1.7"
 description = ""
 authors = ["Talkd.AI <foss@talkd.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dialog_lib-0.0.1.6/PKG-INFO` & `dialog_lib-0.0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-lib
-Version: 0.0.1.6
+Version: 0.0.1.7
 Summary: 
 License: MIT
 Author: Talkd.AI
 Author-email: foss@talkd.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

