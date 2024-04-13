# Comparing `tmp/embed_anything-0.1.5.tar.gz` & `tmp/embed_anything-0.1.6.tar.gz`

## Comparing `embed_anything-0.1.5.tar` & `embed_anything-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 embed_anything-0.1.5/Cargo.toml
--rw-r--r--   0        0        0     3664 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1123 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      758 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.gitignore
--rw-r--r--   0        0        0    98444 2024-04-07 14:53:23.000000 embed_anything-0.1.5/Cargo.lock
--rw-r--r--   0        0        0    35823 2024-04-07 14:13:10.000000 embed_anything-0.1.5/LICENSE
--rw-r--r--   0        0        0     1417 2024-04-07 14:13:10.000000 embed_anything-0.1.5/README.md
--rw-r--r--   0        0        0    17016 2024-04-07 14:13:10.000000 embed_anything-0.1.5/embed_anything-0.1.1.tar.gz
--rw-r--r--   0        0        0     1486 2024-04-07 14:53:23.000000 embed_anything-0.1.5/embed_anything.pyi
--rw-r--r--   0        0        0     1940 2024-04-07 14:53:23.000000 embed_anything-0.1.5/examples/clip.rs
--rw-r--r--   0        0        0     3429 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/bert.rs
--rw-r--r--   0        0        0     5735 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/clip.rs
--rw-r--r--   0        0        0     1767 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/embed.rs
--rw-r--r--   0        0        0     3507 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/jina.rs
--rw-r--r--   0        0        0       76 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/mod.rs
--rw-r--r--   0        0        0     1691 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/openai.rs
--rw-r--r--   0        0        0     1422 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/file_embed.rs
--rw-r--r--   0        0        0     4756 2024-04-12 21:15:53.000000 embed_anything-0.1.5/src/lib.rs
--rw-r--r--   0        0        0     2390 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/parser.rs
--rw-r--r--   0        0        0      296 2024-04-07 14:13:10.000000 embed_anything-0.1.5/src/pdf_processor.rs
--rw-r--r--   0        0        0     1057 2024-04-13 17:08:24.000000 embed_anything-0.1.5/test.py
--rw-r--r--   0        0        0  2224388 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/cat1.jpg
--rw-r--r--   0        0        0     5378 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/cat2.jpeg
--rw-r--r--   0        0        0   121984 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/dog1.jpg
--rw-r--r--   0        0        0     9979 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/dog2.jpeg
--rw-r--r--   0        0        0    42380 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/monkey1.jpg
--rw-r--r--   0        0        0    39440 2024-04-01 22:25:38.000000 embed_anything-0.1.5/test_files/test_paper.pdf
--rw-r--r--   0        0        0   166289 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/wa4_ethics_written_assignment.pdf
--rw-r--r--   0        0        0      677 2024-04-07 14:53:23.000000 embed_anything-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 embed_anything-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 embed_anything-0.1.6/Cargo.toml
+-rw-r--r--   0        0        0     3664 2024-04-07 14:13:10.000000 embed_anything-0.1.6/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1123 2024-04-07 14:13:10.000000 embed_anything-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      758 2024-04-07 14:13:10.000000 embed_anything-0.1.6/.gitignore
+-rw-r--r--   0        0        0    94650 2024-04-13 21:38:43.000000 embed_anything-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0    35823 2024-04-07 14:13:10.000000 embed_anything-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1754 2024-04-13 21:34:20.000000 embed_anything-0.1.6/README.md
+-rw-r--r--   0        0        0    17016 2024-04-07 14:13:10.000000 embed_anything-0.1.6/embed_anything-0.1.1.tar.gz
+-rw-r--r--   0        0        0     1486 2024-04-07 14:53:23.000000 embed_anything-0.1.6/embed_anything.pyi
+-rw-r--r--   0        0        0     1940 2024-04-07 14:53:23.000000 embed_anything-0.1.6/examples/clip.rs
+-rw-r--r--   0        0        0     3429 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/bert.rs
+-rw-r--r--   0        0        0     5735 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/clip.rs
+-rw-r--r--   0        0        0     1767 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/embed.rs
+-rw-r--r--   0        0        0     3507 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/jina.rs
+-rw-r--r--   0        0        0       76 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/mod.rs
+-rw-r--r--   0        0        0     1691 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/embedding_model/openai.rs
+-rw-r--r--   0        0        0     1422 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/file_embed.rs
+-rw-r--r--   0        0        0     4756 2024-04-12 21:15:53.000000 embed_anything-0.1.6/src/lib.rs
+-rw-r--r--   0        0        0     2390 2024-04-07 14:53:23.000000 embed_anything-0.1.6/src/parser.rs
+-rw-r--r--   0        0        0      296 2024-04-07 14:13:10.000000 embed_anything-0.1.6/src/pdf_processor.rs
+-rw-r--r--   0        0        0     1057 2024-04-13 17:08:24.000000 embed_anything-0.1.6/test.py
+-rw-r--r--   0        0        0  2224388 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/clip/cat1.jpg
+-rw-r--r--   0        0        0     5378 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/clip/cat2.jpeg
+-rw-r--r--   0        0        0   121984 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/clip/dog1.jpg
+-rw-r--r--   0        0        0     9979 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/clip/dog2.jpeg
+-rw-r--r--   0        0        0    42380 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/clip/monkey1.jpg
+-rw-r--r--   0        0        0    39440 2024-04-01 22:25:38.000000 embed_anything-0.1.6/test_files/test_paper.pdf
+-rw-r--r--   0        0        0   166289 2024-04-07 14:53:23.000000 embed_anything-0.1.6/test_files/wa4_ethics_written_assignment.pdf
+-rw-r--r--   0        0        0      677 2024-04-07 14:53:23.000000 embed_anything-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 embed_anything-0.1.6/PKG-INFO
```

### Comparing `embed_anything-0.1.5/Cargo.toml` & `embed_anything-0.1.6/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "embed_anything"
-version = "0.1.5"
+version = "0.1.6"
 edition = "2021"
 
 
 
 [dependencies]
 pyo3 = { version = "0.20", features = ["extension-module"] }
 pyo3-asyncio = { version = "0.20", features = ["tokio-runtime"] }
```

### Comparing `embed_anything-0.1.5/.github/workflows/CI.yml` & `embed_anything-0.1.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/.github/workflows/python-publish.yml` & `embed_anything-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/.gitignore` & `embed_anything-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/LICENSE` & `embed_anything-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/README.md` & `embed_anything-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.3
+Name: embed_anything
+Version: 0.1.6
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+License-File: LICENSE
+Summary: Embed anything at lightning speed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/StarlightSearch/EmbedAnything/tree/main
+
 # EmbedAnything
 
 
 EmbedAnything is a powerful library designed to streamline the creation and management of embedding pipelines. Whether you're working with text, images, audio, or any other type of data[Multimodality to be added], EmbedAnything makes it easy to generate embeddings from multiple sources and store them efficiently in a vector database.
 
 ## Key Features
 
@@ -18,18 +31,36 @@
 
 `
 pip install embed-anything`
 
 
 Requirements:
 
-Please check if you already have the OpenAI key in the Environment variable. We have only released the OpenAI embedder library so far. Please stay tuned for updates for the local embeddings as well.
 
 
-##Script:
 
+## Script:
+
+**Do not forget to check out test.py on Github**
+
+### PDFs texts with OpenAI, make sure you have openai key in the environment variable.
 ```python
 import embed_anything
 from embed_anything import EmbedData
 data = embed_anything.embed_file("filename.pdf")
 ```
 
+### Local Embedding for files,
+
+```python
+data:list[EmbedData] = embed_anything.embed_file("test_paper.pdf", embeder= "Bert")
+embeddings = np.array([data.embedding for data in data])
+```
+
+### Create Image Embeddings
+
+```python
+data:list[EmbedData] = embed_anything.embed_directory("directory/images", embeder= "Clip")
+embeddings = np.array([data.embedding for data in data])
+```
+
+
```

### Comparing `embed_anything-0.1.5/embed_anything-0.1.1.tar.gz` & `embed_anything-0.1.6/embed_anything-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/embed_anything.pyi` & `embed_anything-0.1.6/embed_anything.pyi`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/examples/clip.rs` & `embed_anything-0.1.6/examples/clip.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/embedding_model/bert.rs` & `embed_anything-0.1.6/src/embedding_model/bert.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/embedding_model/clip.rs` & `embed_anything-0.1.6/src/embedding_model/clip.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/embedding_model/embed.rs` & `embed_anything-0.1.6/src/embedding_model/embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/embedding_model/jina.rs` & `embed_anything-0.1.6/src/embedding_model/jina.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/embedding_model/openai.rs` & `embed_anything-0.1.6/src/embedding_model/openai.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/file_embed.rs` & `embed_anything-0.1.6/src/file_embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/lib.rs` & `embed_anything-0.1.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/src/parser.rs` & `embed_anything-0.1.6/src/parser.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test.py` & `embed_anything-0.1.6/test.py`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/clip/cat1.jpg` & `embed_anything-0.1.6/test_files/clip/cat1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/clip/cat2.jpeg` & `embed_anything-0.1.6/test_files/clip/cat2.jpeg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/clip/dog1.jpg` & `embed_anything-0.1.6/test_files/clip/dog1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/clip/dog2.jpeg` & `embed_anything-0.1.6/test_files/clip/dog2.jpeg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/clip/monkey1.jpg` & `embed_anything-0.1.6/test_files/clip/monkey1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/test_paper.pdf` & `embed_anything-0.1.6/test_files/test_paper.pdf`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/test_files/wa4_ethics_written_assignment.pdf` & `embed_anything-0.1.6/test_files/wa4_ethics_written_assignment.pdf`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.5/pyproject.toml` & `embed_anything-0.1.6/pyproject.toml`

 * *Files identical despite different names*

