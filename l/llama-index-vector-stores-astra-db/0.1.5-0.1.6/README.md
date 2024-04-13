# Comparing `tmp/llama_index_vector_stores_astra_db-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_astra_db-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_astra_db-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_astra_db-0.1.6.tar", max compression
```

## Comparing `llama_index_vector_stores_astra_db-0.1.5.tar` & `llama_index_vector_stores_astra_db-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2024-03-12 15:55:24.823332 llama_index_vector_stores_astra_db-0.1.5/README.md
--rw-r--r--   0        0        0      105 2024-03-12 15:55:24.823332 llama_index_vector_stores_astra_db-0.1.5/llama_index/vector_stores/astra_db/__init__.py
--rw-r--r--   0        0        0    13390 2024-03-12 17:18:01.593304 llama_index_vector_stores_astra_db-0.1.5/llama_index/vector_stores/astra_db/base.py
--rw-r--r--   0        0        0     1479 2024-03-13 22:02:43.943455 llama_index_vector_stores_astra_db-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 llama_index_vector_stores_astra_db-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      944 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/README.md
+-rw-r--r--   0        0        0      105 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/base.py
+-rw-r--r--   0        0        0     1484 2024-04-13 04:40:50.711179 llama_index_vector_stores_astra_db-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 llama_index_vector_stores_astra_db-0.1.6/PKG-INFO
```

### Comparing `llama_index_vector_stores_astra_db-0.1.5/README.md` & `llama_index_vector_stores_astra_db-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_astra_db-0.1.5/llama_index/vector_stores/astra_db/base.py` & `llama_index_vector_stores_astra_db-0.1.6/llama_index/vector_stores/astra_db/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,40 @@
     vector-similarity-search. Documents, and their embeddings, are stored
     in an Astra table and a vector-capable index is used for searches.
     The table does not need to exist beforehand: if necessary it will
     be created behind the scenes.
 
     All Astra operations are done through the astrapy library.
 
+    Visit https://astra.datastax.com/signup to create an account and get an API key.
+
     Args:
         collection_name (str): collection name to use. If not existing, it will be created.
         token (str): The Astra DB Application Token to use.
         api_endpoint (str): The Astra DB JSON API endpoint for your database.
         embedding_dimension (int): length of the embedding vectors in use.
         namespace (Optional[str]): The namespace to use. If not provided, 'default_keyspace'
         ttl_seconds (Optional[int]): expiration time for inserted entries.
             Default is no expiration.
 
+    Examples:
+        `pip install llama-index-vector-stores-astra`
+
+        ```python
+        from llama_index.vector_stores.astra import AstraDBVectorStore
+
+        # Create the Astra DB Vector Store object
+        astra_db_store = AstraDBVectorStore(
+            collection_name="astra_v_table",
+            token=token,
+            api_endpoint=api_endpoint,
+            embedding_dimension=1536,
+        )
+        ```
+
     """
 
     stores_text: bool = True
     flat_metadata: bool = True
 
     _embedding_dimension: int = PrivateAttr()
     _ttl_seconds: Optional[int] = PrivateAttr()
@@ -222,15 +239,15 @@
 
         Args:
             ref_doc_id (str): The id of the document to delete.
 
         """
         _logger.debug("Deleting a document from the Astra table")
 
-        self._astra_db_collection.delete(id=ref_doc_id, **delete_kwargs)
+        self._astra_db_collection.delete_one(id=ref_doc_id, **delete_kwargs)
 
     @property
     def client(self) -> Any:
         """Return the underlying Astra vector table object."""
         return self._astra_db_collection
 
     @staticmethod
```

### Comparing `llama_index_vector_stores_astra_db-0.1.5/pyproject.toml` & `llama_index_vector_stores_astra_db-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores astra integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-astra-db"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-astrapy = "^0.7.7"
+astrapy = ">=0.7.7, <2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_vector_stores_astra_db-0.1.5/PKG-INFO` & `llama_index_vector_stores_astra_db-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-astra-db
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index vector_stores astra integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astrapy (>=0.7.7,<0.8.0)
+Requires-Dist: astrapy (>=0.7.7,<2)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Astra DB Vector Store
 
 A LlamaIndex vector store using Astra DB as the backend.
```

