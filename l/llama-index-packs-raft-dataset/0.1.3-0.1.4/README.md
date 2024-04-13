# Comparing `tmp/llama_index_packs_raft_dataset-0.1.3.tar.gz` & `tmp/llama_index_packs_raft_dataset-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_raft_dataset-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_raft_dataset-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_raft_dataset-0.1.3.tar` & `llama_index_packs_raft_dataset-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2896 2024-03-26 13:15:48.767669 llama_index_packs_raft_dataset-0.1.3/README.md
--rw-r--r--   0        0        0       95 2024-03-26 13:15:48.767669 llama_index_packs_raft_dataset-0.1.3/llama_index/packs/raft_dataset/__init__.py
--rw-r--r--   0        0        0     8555 2024-03-26 13:15:48.767669 llama_index_packs_raft_dataset-0.1.3/llama_index/packs/raft_dataset/base.py
--rw-r--r--   0        0        0     1567 2024-03-26 13:15:48.767669 llama_index_packs_raft_dataset-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2896 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/README.md
+-rw-r--r--   0        0        0       95 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/__init__.py
+-rw-r--r--   0        0        0     8458 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/base.py
+-rw-r--r--   0        0        0     1567 2024-04-13 04:42:59.761415 llama_index_packs_raft_dataset-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 llama_index_packs_raft_dataset-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_raft_dataset-0.1.3/README.md` & `llama_index_packs_raft_dataset-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_raft_dataset-0.1.3/llama_index/packs/raft_dataset/base.py` & `llama_index_packs_raft_dataset-0.1.4/llama_index/packs/raft_dataset/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,21 +96,17 @@
         """
         Generates `x` questions / use cases for `chunk`. Used when the input document is of general types
         `pdf`, `json`, or `txt`.
         """
         messages = [
             ChatMessage(
                 role="system",
-                content="You are a synthetic question-answer pair generator. Given a chunk of context about some topic(s), generate %s example questions a user could ask and would be answered using information from the chunk. For example, if the given context was a Wikipedia paragraph about the United States, an example question could be 'How many states are in the United States?'"
+                content="You are a synthetic question-answer pair generator. Given a chunk of context about some topic(s), generate %s example questions a user could ask and would be answered using information from the chunk. For example, if the given context was a Wikipedia paragraph about the United States, an example question could be 'How many states are in the United States?'. The questions should be able to be answered in a few words or less."
                 % (x),
             ),
-            ChatMessage(
-                role="system",
-                content="The questions should be able to be answered in a few words or less.",
-            ),
             ChatMessage(role="user", content=str(chunk)),
         ]
 
         queries = str(self.llm.chat(messages)).split("\n")
         queries = [self.strip_str(q) for q in queries]
         return [q for q in queries if any(c.isalpha() for c in q)]
```

### Comparing `llama_index_packs_raft_dataset-0.1.3/pyproject.toml` & `llama_index_packs_raft_dataset-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index packs RAFT Dataset paper implementation"
 exclude = ["**/BUILD"]
 keywords = ["finetuning", "raft", "raft_dataset"]
 license = "MIT"
 maintainers = ["ravi-theja"]
 name = "llama-index-packs-raft-dataset"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 datasets = "^2.18.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_packs_raft_dataset-0.1.3/PKG-INFO` & `llama_index_packs_raft_dataset-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-raft-dataset
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index packs RAFT Dataset paper implementation
 License: MIT
 Keywords: finetuning,raft,raft_dataset
 Author: Ravi Theja
 Author-email: ravi03071991@gmail.com
 Maintainer: ravi-theja
 Requires-Python: >=3.8.1,<4.0
```

