# Comparing `tmp/dialog_lib-0.0.1.1.tar.gz` & `tmp/dialog_lib-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_lib-0.0.1.1.tar", max compression
+gzip compressed data, was "dialog_lib-0.0.1.3.tar", max compression
```

## Comparing `dialog_lib-0.0.1.1.tar` & `dialog_lib-0.0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       98 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/agents/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/agents/abstract.py
--rw-r--r--   0        0        0      117 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/db/__init__.py
--rw-r--r--   0        0        0     2642 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/db/memory.py
--rw-r--r--   0        0        0     1325 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/db/models.py
--rw-r--r--   0        0        0      398 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/db/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/embeddings/__init__.py
--rw-r--r--   0        0        0     1427 2024-04-12 01:44:50.512333 dialog_lib-0.0.1.1/dialog_lib/embeddings/generate.py
--rw-r--r--   0        0        0      148 2024-04-12 01:44:50.516333 dialog_lib-0.0.1.1/dialog_lib/main.py
--rw-r--r--   0        0        0      629 2024-04-12 01:44:50.516333 dialog_lib-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       98 2024-04-12 00:39:12.358734 dialog_lib-0.0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 00:17:13.466371 dialog_lib-0.0.1.3/dialog_lib/agents/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-12 00:26:30.131591 dialog_lib-0.0.1.3/dialog_lib/agents/abstract.py
+-rw-r--r--   0        0        0      117 2024-04-12 00:34:49.628803 dialog_lib-0.0.1.3/dialog_lib/db/__init__.py
+-rw-r--r--   0        0        0     2604 2024-04-12 18:11:08.688869 dialog_lib-0.0.1.3/dialog_lib/db/memory.py
+-rw-r--r--   0        0        0     1325 2024-04-12 00:16:35.393721 dialog_lib-0.0.1.3/dialog_lib/db/models.py
+-rw-r--r--   0        0        0      389 2024-04-12 18:11:15.544813 dialog_lib-0.0.1.3/dialog_lib/db/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 00:27:53.398079 dialog_lib-0.0.1.3/dialog_lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     1427 2024-04-12 01:39:27.537029 dialog_lib-0.0.1.3/dialog_lib/embeddings/generate.py
+-rw-r--r--   0        0        0      148 2024-04-12 00:08:12.155498 dialog_lib-0.0.1.3/dialog_lib/main.py
+-rw-r--r--   0        0        0      629 2024-04-12 18:18:20.791824 dialog_lib-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 dialog_lib-0.0.1.3/PKG-INFO
```

### Comparing `dialog_lib-0.0.1.1/dialog_lib/agents/abstract.py` & `dialog_lib-0.0.1.3/dialog_lib/agents/abstract.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.1/dialog_lib/db/memory.py` & `dialog_lib-0.0.1.3/dialog_lib/db/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from langchain.memory import PostgresChatMessageHistory
 from langchain.schema.messages import BaseMessage, _message_to_dict
 
-from dialog.db.models import Chat, ChatMessages
-from dialog.settings import Settings
+from .models import Chat, ChatMessages
 
 
 class CustomPostgresChatMessageHistory(PostgresChatMessageHistory):
     """
     Custom chat message history for LLM
     """
 
@@ -43,21 +42,21 @@
         )
         if self.parent_session_id:
             message.parent = self.parent_session_id
         self.dbsession.add(message)
         self.dbsession.commit()
 
 
-def generate_memory_instance(session_id, parent_session_id=None, dbsession=None):
+def generate_memory_instance(session_id, parent_session_id=None, dbsession=None, database_url=None):
     """
     Generate a memory instance for a given session_id
     """
 
     return CustomPostgresChatMessageHistory(
-        connection_string=Settings().DATABASE_URL,
+        connection_string=database_url,
         session_id=session_id,
         parent_session_id=parent_session_id,
         table_name="chat_messages",
         dbsession=dbsession
     )
```

### Comparing `dialog_lib-0.0.1.1/dialog_lib/db/models.py` & `dialog_lib-0.0.1.3/dialog_lib/db/models.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.1/dialog_lib/embeddings/generate.py` & `dialog_lib-0.0.1.3/dialog_lib/embeddings/generate.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.1.1/pyproject.toml` & `dialog_lib-0.0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialog-lib"
-version = "0.0.1.1"
+version = "0.0.1.3"
 description = ""
 authors = ["Talkd.AI <foss@talkd.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dialog_lib-0.0.1.1/PKG-INFO` & `dialog_lib-0.0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-lib
-Version: 0.0.1.1
+Version: 0.0.1.3
 Summary: 
 License: MIT
 Author: Talkd.AI
 Author-email: foss@talkd.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

