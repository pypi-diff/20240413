# Comparing `tmp/llama_index_readers_astra_db-0.1.4.tar.gz` & `tmp/llama_index_readers_astra_db-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_astra_db-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_readers_astra_db-0.1.5.tar", max compression
```

## Comparing `llama_index_readers_astra_db-0.1.4.tar` & `llama_index_readers_astra_db-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1565 2024-02-16 00:43:37.895451 llama_index_readers_astra_db-0.1.4/README.md
--rw-r--r--   0        0        0       89 2024-02-16 00:43:37.895451 llama_index_readers_astra_db-0.1.4/llama_index/readers/astra_db/__init__.py
--rw-r--r--   0        0        0     2945 2024-02-26 18:26:06.598583 llama_index_readers_astra_db-0.1.4/llama_index/readers/astra_db/base.py
--rw-r--r--   0        0        0     1486 2024-02-26 18:51:58.270108 llama_index_readers_astra_db-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 llama_index_readers_astra_db-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/README.md
+-rw-r--r--   0        0        0       89 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/__init__.py
+-rw-r--r--   0        0        0     2945 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/base.py
+-rw-r--r--   0        0        0     1491 2024-04-13 04:40:50.559179 llama_index_readers_astra_db-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2198 1970-01-01 00:00:00.000000 llama_index_readers_astra_db-0.1.5/PKG-INFO
```

### Comparing `llama_index_readers_astra_db-0.1.4/README.md` & `llama_index_readers_astra_db-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Astra DB Loader
 
+```bash
+pip install llama-index-readers-astra-db
+```
+
 The Astra DB Loader returns a set of documents retrieved from Astra DB.
 The user initializes the loader with an Astra DB index. They then pass in a vector.
 
 ## Usage
 
 Here's an example usage of the AstraDBReader.
 
 ```python
 from openai import OpenAI
 
-from llama_index import download_loader
-
 
 # Get the credentials for Astra DB
 api_endpoint = "https://324<...>f1c.astra.datastax.com"
 token = "AstraCS:<...>"
 
 # EXAMPLE: OpenAI embeddings
 client = OpenAI(api_key="sk-<...>")
@@ -25,15 +27,15 @@
     input="Your text string goes here", model="text-embedding-ada-002"
 )
 
 # Get the embedding
 query_vector = response.data[0].embedding
 
 # Initialize the Reader object
-AstraDBReader = download_loader("AstraDBReader")
+from llama_index.readers.astra_db import AstraDBReader
 
 # Your Astra DB Account will provide you with the endpoint URL and Token
 reader = AstraDBReader(
     collection_name="astra_v_table",
     token=token,
     api_endpoint=api_endpoint,
     embedding_dimension=len(query_vector),
```

### Comparing `llama_index_readers_astra_db-0.1.4/llama_index/readers/astra_db/base.py` & `llama_index_readers_astra_db-0.1.5/llama_index/readers/astra_db/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_astra_db-0.1.4/pyproject.toml` & `llama_index_readers_astra_db-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers astra_db integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["erichare"]
 name = "llama-index-readers-astra-db"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-astrapy = "^0.7.5"
+astrapy = ">=0.7.7, <2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_readers_astra_db-0.1.4/PKG-INFO` & `llama_index_readers_astra_db-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-astra-db
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index readers astra_db integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: erichare
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astrapy (>=0.7.5,<0.8.0)
+Requires-Dist: astrapy (>=0.7.7,<2)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Astra DB Loader
 
+```bash
+pip install llama-index-readers-astra-db
+```
+
 The Astra DB Loader returns a set of documents retrieved from Astra DB.
 The user initializes the loader with an Astra DB index. They then pass in a vector.
 
 ## Usage
 
 Here's an example usage of the AstraDBReader.
 
 ```python
 from openai import OpenAI
 
-from llama_index import download_loader
-
 
 # Get the credentials for Astra DB
 api_endpoint = "https://324<...>f1c.astra.datastax.com"
 token = "AstraCS:<...>"
 
 # EXAMPLE: OpenAI embeddings
 client = OpenAI(api_key="sk-<...>")
@@ -44,15 +45,15 @@
     input="Your text string goes here", model="text-embedding-ada-002"
 )
 
 # Get the embedding
 query_vector = response.data[0].embedding
 
 # Initialize the Reader object
-AstraDBReader = download_loader("AstraDBReader")
+from llama_index.readers.astra_db import AstraDBReader
 
 # Your Astra DB Account will provide you with the endpoint URL and Token
 reader = AstraDBReader(
     collection_name="astra_v_table",
     token=token,
     api_endpoint=api_endpoint,
     embedding_dimension=len(query_vector),
```

