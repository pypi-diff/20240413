# Comparing `tmp/llama_index_packs_code_hierarchy-0.1.2.tar.gz` & `tmp/llama_index_packs_code_hierarchy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_packs_code_hierarchy-0.1.3.tar", max compression
```

## Comparing `llama_index_packs_code_hierarchy-0.1.2.tar` & `llama_index_packs_code_hierarchy-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4966 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/README.md
--rw-r--r--   0        0        0       17 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/BUILD
--rw-r--r--   0        0        0      371 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/__init__.py
--rw-r--r--   0        0        0     1473 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/base.py
--rw-r--r--   0        0        0    33375 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/code_hierarchy.py
--rw-r--r--   0        0        0     6099 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/query_engine.py
--rw-r--r--   0        0        0     1438 2024-03-27 21:24:26.873463 llama_index_packs_code_hierarchy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     4966 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/README.md
+-rw-r--r--   0        0        0       17 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/BUILD
+-rw-r--r--   0        0        0      371 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/base.py
+-rw-r--r--   0        0        0    33488 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/code_hierarchy.py
+-rw-r--r--   0        0        0     6099 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/query_engine.py
+-rw-r--r--   0        0        0     1438 2024-04-13 04:11:59.738518 llama_index_packs_code_hierarchy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 llama_index_packs_code_hierarchy-0.1.3/PKG-INFO
```

### Comparing `llama_index_packs_code_hierarchy-0.1.2/README.md` & `llama_index_packs_code_hierarchy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/base.py` & `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/code_hierarchy.py` & `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/code_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,19 +335,23 @@
 
         upstream_children_documents: List[TextNode] = []
         all_documents: List[TextNode] = []
 
         # Capture any whitespace before parent.start_byte
         # Very important for space sensitive languages like python
         start_byte = parent.start_byte
-        while start_byte > 0 and text[start_byte - 1] in (" ", "\t"):
+        text_bytes = bytes(text, "utf-8")
+        while start_byte > 0 and text_bytes[start_byte - 1 : start_byte] in (
+            b" ",
+            b"\t",
+        ):
             start_byte -= 1
 
         # Create this node
-        current_chunk = text[start_byte : parent.end_byte]
+        current_chunk = text_bytes[start_byte : parent.end_byte].decode()
 
         # Return early if the chunk is too small
         if len(current_chunk) < self.min_characters and not _root:
             return _ChunkNodeOutput(
                 this_document=None, all_documents=[], upstream_children_documents=[]
             )
```

### Comparing `llama_index_packs_code_hierarchy-0.1.2/llama_index/packs/code_hierarchy/query_engine.py` & `llama_index_packs_code_hierarchy-0.1.3/llama_index/packs/code_hierarchy/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index_packs_code_hierarchy-0.1.2/pyproject.toml` & `llama_index_packs_code_hierarchy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Ryan Peach <rgpeach10@gmail.com>"]
 description = "A node parser which can create a hierarchy of all code scopes in a directory."
 keywords = ["c", "code", "cpp", "hierarchy", "html", "javascript", "python", "repo", "typescript"]
 license = "MIT"
 maintainers = ["ryanpeach"]
 name = "llama-index-packs-code-hierarchy"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 llama-index-core = "^0.10.1"
 tree-sitter-languages = "^1.8.0"
 tree-sitter = "^0.20.2"
 llama-index-agent-openai = ">=0.1.5"
```

### Comparing `llama_index_packs_code_hierarchy-0.1.2/PKG-INFO` & `llama_index_packs_code_hierarchy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-code-hierarchy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A node parser which can create a hierarchy of all code scopes in a directory.
 License: MIT
 Keywords: c,code,cpp,hierarchy,html,javascript,python,repo,typescript
 Author: Ryan Peach
 Author-email: rgpeach10@gmail.com
 Maintainer: ryanpeach
 Requires-Python: >=3.8.1,<3.12
```

