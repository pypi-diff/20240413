# Comparing `tmp/embed_anything-0.1.4.tar.gz` & `tmp/embed_anything-0.1.5.tar.gz`

## Comparing `embed_anything-0.1.4.tar` & `embed_anything-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,30 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.4/Cargo.toml
--rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1123 2024-04-04 15:11:59.000000 embed_anything-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.4/.gitignore
--rw-r--r--   0        0        0    35823 2024-04-04 15:11:59.000000 embed_anything-0.1.4/LICENSE
--rw-r--r--   0        0        0     1431 2024-04-04 15:11:59.000000 embed_anything-0.1.4/README.md
--rw-r--r--   0        0        0    17016 2024-04-04 13:30:00.000000 embed_anything-0.1.4/embed_anything-0.1.1.tar.gz
--rw-r--r--   0        0        0    50353 2024-04-04 15:51:04.000000 embed_anything-0.1.4/embed_anything-0.1.3.tar.gz
--rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.4/embed_anything.pyi
--rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.4/src/embed.rs
--rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.4/src/file_embed.rs
--rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.4/src/lib.rs
--rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.4/src/pdf_processor.rs
--rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.4/test.py
--rw-r--r--   0        0        0    42778 2024-04-04 15:54:53.000000 embed_anything-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      673 2024-04-04 15:54:44.000000 embed_anything-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 embed_anything-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 embed_anything-0.1.5/Cargo.toml
+-rw-r--r--   0        0        0     3664 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1123 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      758 2024-04-07 14:13:10.000000 embed_anything-0.1.5/.gitignore
+-rw-r--r--   0        0        0    98444 2024-04-07 14:53:23.000000 embed_anything-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0    35823 2024-04-07 14:13:10.000000 embed_anything-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1417 2024-04-07 14:13:10.000000 embed_anything-0.1.5/README.md
+-rw-r--r--   0        0        0    17016 2024-04-07 14:13:10.000000 embed_anything-0.1.5/embed_anything-0.1.1.tar.gz
+-rw-r--r--   0        0        0     1486 2024-04-07 14:53:23.000000 embed_anything-0.1.5/embed_anything.pyi
+-rw-r--r--   0        0        0     1940 2024-04-07 14:53:23.000000 embed_anything-0.1.5/examples/clip.rs
+-rw-r--r--   0        0        0     3429 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/bert.rs
+-rw-r--r--   0        0        0     5735 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/clip.rs
+-rw-r--r--   0        0        0     1767 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/embed.rs
+-rw-r--r--   0        0        0     3507 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/jina.rs
+-rw-r--r--   0        0        0       76 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/mod.rs
+-rw-r--r--   0        0        0     1691 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/embedding_model/openai.rs
+-rw-r--r--   0        0        0     1422 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/file_embed.rs
+-rw-r--r--   0        0        0     4756 2024-04-12 21:15:53.000000 embed_anything-0.1.5/src/lib.rs
+-rw-r--r--   0        0        0     2390 2024-04-07 14:53:23.000000 embed_anything-0.1.5/src/parser.rs
+-rw-r--r--   0        0        0      296 2024-04-07 14:13:10.000000 embed_anything-0.1.5/src/pdf_processor.rs
+-rw-r--r--   0        0        0     1057 2024-04-13 17:08:24.000000 embed_anything-0.1.5/test.py
+-rw-r--r--   0        0        0  2224388 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/cat1.jpg
+-rw-r--r--   0        0        0     5378 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/cat2.jpeg
+-rw-r--r--   0        0        0   121984 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/dog1.jpg
+-rw-r--r--   0        0        0     9979 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/dog2.jpeg
+-rw-r--r--   0        0        0    42380 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/clip/monkey1.jpg
+-rw-r--r--   0        0        0    39440 2024-04-01 22:25:38.000000 embed_anything-0.1.5/test_files/test_paper.pdf
+-rw-r--r--   0        0        0   166289 2024-04-07 14:53:23.000000 embed_anything-0.1.5/test_files/wa4_ethics_written_assignment.pdf
+-rw-r--r--   0        0        0      677 2024-04-07 14:53:23.000000 embed_anything-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 embed_anything-0.1.5/PKG-INFO
```

### Comparing `embed_anything-0.1.4/.github/workflows/CI.yml` & `embed_anything-0.1.5/.github/workflows/CI.yml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-# This file is autogenerated by maturin v1.5.1
-# To update, run
-#
-#    maturin generate-ci github
-#
-name: CI
-
-on:
-  push:
-    branches:
-      - main
-      - master
-    tags:
-      - '*'
-  pull_request:
-  workflow_dispatch:
-
-permissions:
-  contents: read
-
-jobs:
-  linux:
-    runs-on: ${{ matrix.platform.runner }}
-    strategy:
-      matrix:
-        platform:
-          - runner: ubuntu-latest
-            target: x86_64
-          - runner: ubuntu-latest
-            target: x86
-          - runner: ubuntu-latest
-            target: aarch64
-          - runner: ubuntu-latest
-            target: armv7
-          - runner: ubuntu-latest
-            target: s390x
-          - runner: ubuntu-latest
-            target: ppc64le
-    steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v5
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.platform.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-          manylinux: auto
-      - name: Upload wheels
-        uses: actions/upload-artifact@v4
-        with:
-          name: wheels-linux-${{ matrix.platform.target }}
-          path: dist
-
-  windows:
-    runs-on: ${{ matrix.platform.runner }}
-    strategy:
-      matrix:
-        platform:
-          - runner: windows-latest
-            target: x64
-          - runner: windows-latest
-            target: x86
-    steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v5
-        with:
-          python-version: '3.10'
-          architecture: ${{ matrix.platform.target }}
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.platform.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v4
-        with:
-          name: wheels-windows-${{ matrix.platform.target }}
-          path: dist
-
-  macos:
-    runs-on: ${{ matrix.platform.runner }}
-    strategy:
-      matrix:
-        platform:
-          - runner: macos-latest
-            target: x86_64
-          - runner: macos-14
-            target: aarch64
-    steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v5
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.platform.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v4
-        with:
-          name: wheels-macos-${{ matrix.platform.target }}
-          path: dist
-
-  sdist:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-      - name: Build sdist
-        uses: PyO3/maturin-action@v1
-        with:
-          command: sdist
-          args: --out dist
-      - name: Upload sdist
-        uses: actions/upload-artifact@v4
-        with:
-          name: wheels-sdist
-          path: dist
-
-  release:
-    name: Release
-    runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
-    steps:
-      - uses: actions/download-artifact@v4
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --non-interactive --skip-existing wheels-*/*
+# This file is autogenerated by maturin v1.5.1
+# To update, run
+#
+#    maturin generate-ci github
+#
+name: CI
+
+on:
+  push:
+    branches:
+      - main
+      - master
+    tags:
+      - '*'
+  pull_request:
+  workflow_dispatch:
+
+permissions:
+  contents: read
+
+jobs:
+  linux:
+    runs-on: ${{ matrix.platform.runner }}
+    strategy:
+      matrix:
+        platform:
+          - runner: ubuntu-latest
+            target: x86_64
+          - runner: ubuntu-latest
+            target: x86
+          - runner: ubuntu-latest
+            target: aarch64
+          - runner: ubuntu-latest
+            target: armv7
+          - runner: ubuntu-latest
+            target: s390x
+          - runner: ubuntu-latest
+            target: ppc64le
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.platform.target }}
+          args: --release --out dist --find-interpreter
+          sccache: 'true'
+          manylinux: auto
+      - name: Upload wheels
+        uses: actions/upload-artifact@v4
+        with:
+          name: wheels-linux-${{ matrix.platform.target }}
+          path: dist
+
+  windows:
+    runs-on: ${{ matrix.platform.runner }}
+    strategy:
+      matrix:
+        platform:
+          - runner: windows-latest
+            target: x64
+          - runner: windows-latest
+            target: x86
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+          architecture: ${{ matrix.platform.target }}
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.platform.target }}
+          args: --release --out dist --find-interpreter
+          sccache: 'true'
+      - name: Upload wheels
+        uses: actions/upload-artifact@v4
+        with:
+          name: wheels-windows-${{ matrix.platform.target }}
+          path: dist
+
+  macos:
+    runs-on: ${{ matrix.platform.runner }}
+    strategy:
+      matrix:
+        platform:
+          - runner: macos-latest
+            target: x86_64
+          - runner: macos-14
+            target: aarch64
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+      - name: Build wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          target: ${{ matrix.platform.target }}
+          args: --release --out dist --find-interpreter
+          sccache: 'true'
+      - name: Upload wheels
+        uses: actions/upload-artifact@v4
+        with:
+          name: wheels-macos-${{ matrix.platform.target }}
+          path: dist
+
+  sdist:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - name: Build sdist
+        uses: PyO3/maturin-action@v1
+        with:
+          command: sdist
+          args: --out dist
+      - name: Upload sdist
+        uses: actions/upload-artifact@v4
+        with:
+          name: wheels-sdist
+          path: dist
+
+  release:
+    name: Release
+    runs-on: ubuntu-latest
+    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [linux, windows, macos, sdist]
+    steps:
+      - uses: actions/download-artifact@v4
+      - name: Publish to PyPI
+        uses: PyO3/maturin-action@v1
+        env:
+          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
+        with:
+          command: upload
+          args: --non-interactive --skip-existing wheels-*/*
```

### Comparing `embed_anything-0.1.4/.github/workflows/python-publish.yml` & `embed_anything-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.4/.gitignore` & `embed_anything-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.4/LICENSE` & `embed_anything-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.4/README.md` & `embed_anything-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 ##Script:
 
 ```python
 import embed_anything
 from embed_anything import EmbedData
 data = embed_anything.embed_file("filename.pdf")
-print(data[0])```
+```
```

### Comparing `embed_anything-0.1.4/embed_anything-0.1.1.tar.gz` & `embed_anything-0.1.5/embed_anything-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.4/src/embed.rs` & `embed_anything-0.1.5/src/embedding_model/openai.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,28 @@
 use reqwest::Client;
 use serde::Deserialize;
 use serde_json::json;
-use std::collections::HashMap;
-use pyo3::prelude::*;
-
-#[derive(Deserialize, Debug)]
-pub struct EmbedResponse {
-    // object: String,
-    pub data: Vec<EmbedData>,
-    // model: String,
-    usage: HashMap<String, usize>,
-}
-#[pyclass]
-#[derive(Deserialize, Debug)]
-pub struct EmbedData {
-    #[pyo3(get, set)]
-    pub embedding: Vec<f32>,
-    #[pyo3(get, set)]
-    pub text: Option<String>,
-}
-
-#[pymethods]
-impl EmbedData {
-
-    #[new]
-    pub fn new(embedding: Vec<f32>, text: Option<String>) -> Self {
-        Self {
-            embedding,
-            text,
-        }
-    }
-
-    pub fn __str__(&self) -> String {
-        format!("EmbedData(embedding: {:?}, text: {:?})", self.embedding, self.text)
-    }
-
-}
-
-pub enum Embeder {
-    OpenAI(OpenAIEmbeder),
-    // AllMiniLmL12V2(AllMiniLmL12V2Embeder),
-}
 
+use crate::embedding_model::embed::{EmbedData, EmbedResponse};
 
-impl Embeder {
-    pub async fn embed(&self, text_batch: &[String]) ->Result<Vec<EmbedData>, reqwest::Error> {
-        match self {
-            Embeder::OpenAI(embeder) => embeder.embed(text_batch).await,
-            // Embeder::AllMiniLmL12V2(embeder) => embeder.embed(text_batch).await,
-        }
-    }
-
-}
-
+use super::embed::Embed;
 
 /// Represents an OpenAIEmbeder struct that contains the URL and API key for making requests to the OpenAI API.
 #[derive(Deserialize, Debug)]
 pub struct OpenAIEmbeder {
     url: String,
     api_key: String,
 }
 
 impl Default for OpenAIEmbeder {
     fn default() -> Self {
         Self::new(None)
     }
 }
 
-
-
-pub trait Embed {
-   fn embed(&self, text_batch: &[String]) -> impl std::future::Future<Output = Result<Vec<EmbedData>, reqwest::Error>> ;
-}
-
-
-
 impl Embed for OpenAIEmbeder {
     async fn embed(&self, text_batch: &[String]) -> Result<Vec<EmbedData>, reqwest::Error> {
         let client = Client::new();
 
         let response = client
             .post(&self.url)
             .header("Content-Type", "application/json")
@@ -88,19 +32,25 @@
                 "model": "text-embedding-3-small",
             }))
             .send()
             .await?;
 
         let data = response.json::<EmbedResponse>().await?;
         println!("{:?}", data.usage);
-        
-        let emb_data = data.data.iter().zip(text_batch).map( move |(data, text)| EmbedData::new(data.embedding.clone(), Some(text.clone()))).collect::<Vec<_>>();
+
+        let emb_data = data
+            .data
+            .iter()
+            .zip(text_batch)
+            .map(move |(data, text)| EmbedData::new(data.embedding.clone(), Some(text.clone())))
+            .collect::<Vec<_>>();
 
         Ok(emb_data)
     }
+    
 }
 
 impl OpenAIEmbeder {
     pub fn new(api_key: Option<String>) -> Self {
         let api_key = api_key.unwrap_or_else(|| std::env::var("OPENAI_API_KEY").unwrap());
 
         Self {
```

### Comparing `embed_anything-0.1.4/src/file_embed.rs` & `embed_anything-0.1.5/src/file_embed.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use std::fmt::Debug;
 use std::io::Error;
-use std::sync::Arc;
 
-use crate::embed::{EmbedData, Embeder};
+use crate::embedding_model::embed::{EmbedData, Embeder};
 
 use super::pdf_processor::PdfProcessor;
 
 #[derive(Debug)]
 pub struct FileEmbeder {
     pub file: String,
     pub chunks: Vec<String>,
@@ -39,16 +38,14 @@
                 chunk.clear();
             }
         }
     }
 
     pub async fn embed(&mut self, embeder:&Embeder) -> Result<(), reqwest::Error> {
         self.embeddings = embeder.embed(&self.chunks).await?;
-        // self.embeddings
-        //     .extend(embeddings.iter().map(|i| i.embedding.clone()));
         Ok(())
     }
 
     pub fn extract_text(&self) -> Result<String, Error> {
         PdfProcessor::extract_text(&self.file)
     }
 }
```

### Comparing `embed_anything-0.1.4/pyproject.toml` & `embed_anything-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 description = "Embed anything at lightning speed"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
+
 ]
 dynamic = ["version"]
+license = {file = "LICENSE"}
+
 [tool.maturin]
 features = ["pyo3/extension-module"]
-license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/StarlightSearch/EmbedAnything/tree/main"
```

### Comparing `embed_anything-0.1.4/PKG-INFO` & `embed_anything-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: embed_anything
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
 Summary: Embed anything at lightning speed
 Requires-Python: >=3.8
@@ -40,10 +40,10 @@
 
 ##Script:
 
 ```python
 import embed_anything
 from embed_anything import EmbedData
 data = embed_anything.embed_file("filename.pdf")
-print(data[0])```
+```
```

