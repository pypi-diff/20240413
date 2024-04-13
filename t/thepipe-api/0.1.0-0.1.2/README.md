# Comparing `tmp/thepipe_api-0.1.0.tar.gz` & `tmp/thepipe_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.0.tar", last modified: Sat Apr 13 17:40:50 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.2.tar", last modified: Sat Apr 13 19:22:12 2024, max compression
```

## Comparing `thepipe_api-0.1.0.tar` & `thepipe_api-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:40:50.682737 thepipe_api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 17:40:43.000000 thepipe_api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-13 17:40:50.682737 thepipe_api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-13 17:40:43.000000 thepipe_api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-13 17:40:43.000000 thepipe_api-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-13 17:40:43.000000 thepipe_api-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:40:50.682737 thepipe_api-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:40:50.682737 thepipe_api-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-04-13 17:40:43.000000 thepipe_api-0.1.0/tests/test_thepipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:40:50.682737 thepipe_api-0.1.0/thepipe_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:40:50.000000 thepipe_api-0.1.0/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.238142 thepipe_api-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     9615 2024-04-13 19:22:12.237141 thepipe_api-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8534 2024-04-13 17:32:17.000000 thepipe_api-0.1.2/README.md
+-rw-rw-rw-   0        0        0      753 2024-04-13 19:18:49.000000 thepipe_api-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      276 2024-04-13 17:21:22.000000 thepipe_api-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 19:22:12.238142 thepipe_api-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-13 19:19:23.000000 thepipe_api-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.220142 thepipe_api-0.1.2/tests/
+-rw-rw-rw-   0        0        0     9511 2024-04-13 18:51:15.000000 thepipe_api-0.1.2/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:22:12.237141 thepipe_api-0.1.2/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      256 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 19:22:12.000000 thepipe_api-0.1.2/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.0/LICENSE` & `thepipe_api-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Emmett McFarlane
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Emmett McFarlane
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `thepipe_api-0.1.0/PKG-INFO` & `thepipe_api-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-Metadata-Version: 2.1
-Name: thepipe_api
-Version: 0.1.0
-Author-email: Emmett McFarlane <emmett@thepi.pe>
-License: MIT License
-Project-URL: Homepage, https://thepi.pe
-Project-URL: Documentation, https://thepi.pe/docs
-Project-URL: Repository, https://github.com/emcf/thepipe
-Project-URL: Issues, https://github.com/emcf/thepipe/issues
-Project-URL: Changelog, https://github.com/emcf/thepipe/releases
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.8.3
-Requires-Dist: charset-normalizer<3.0,>=2.0
-Requires-Dist: playwright
-Requires-Dist: docx2txt
-Requires-Dist: python-pptx
-Requires-Dist: Pyarrow
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: poppler-utils
-Requires-Dist: python-magic
-Requires-Dist: magika
-Requires-Dist: pandas
-Requires-Dist: colorama
-Requires-Dist: requests
-Requires-Dist: pillow
-Requires-Dist: pytesseract
-Requires-Dist: cssutils
-Requires-Dist: beautifulsoup4
-Requires-Dist: torch
-Requires-Dist: llmlingua
-Requires-Dist: PyMuPDF
-Requires-Dist: pdf2image
-Requires-Dist: python-magic
-
-# <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
-
-### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
-
-The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
-
-## Getting Started 🚀
-
-First, install thepipe:
-```bash
-pip install thepipe_api
-```
-Now you can extract comprehensive text and visuals from any file:
-```python
-from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf")
-```
-Or any website:
-```python
-chunks = thepipe.extract("https://example.com")
-```
-Then feed it into GPT-4-Vision:
-```python
-response = client.chat.completions.create(
-    model="gpt-4-vision-preview",
-    messages = chunks,
-)
-```
-The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
-
-## Features 🌟
-
-- Extracts text and visuals from any file or web page 📚
-- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
-- Can interpret complex PDFs, web apps, markdown, etc 🧠
-- Auto-compress prompts exceeding your chosen token limit 📦
-- Works with missing file extensions, in-memory data streams 💾
-- Works with codebases, URL, git repos, and more 🌐
-- Multi-threaded ⚡️
-
-##  How it works 🛠️
-
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
-
-## Supported File Types 📚
-
-| Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
-|---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
-| Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
-| Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
-| Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
-| PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
-| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
-| Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
-| Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
-| Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
-| Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
-| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
-| ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
-
-## Installation 📦
-
-## Local Installation 🛠️
-
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
-
-```bash
-git clone https://github.com/emcf/thepipe
-pip install -r requirements.txt
-```
-
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
-
-Now you can use The Pipe:
-```bash
-python thepipe.py path/to/directory
-```
-
-This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
-
-Arguments are:
-- The input source (required): can be a file path, a URL, or a directory path.
-- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
-- `--match` (optional): Regex pattern to match files in the directory.
-- `--ignore` (optional): Regex pattern to ignore files in the directory.
-- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
-- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
-- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
-
-![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
-
+Metadata-Version: 2.1
+Name: thepipe_api
+Version: 0.1.2
+Author-email: Emmett McFarlane <emmett@thepi.pe>
+License: MIT License
+Project-URL: Homepage, https://thepi.pe
+Project-URL: Documentation, https://thepi.pe/docs
+Project-URL: Repository, https://github.com/emcf/thepipe
+Project-URL: Issues, https://github.com/emcf/thepipe/issues
+Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.8.3
+Requires-Dist: charset-normalizer<3.0,>=2.0
+Requires-Dist: playwright
+Requires-Dist: docx2txt
+Requires-Dist: python-pptx
+Requires-Dist: Pyarrow
+Requires-Dist: unstructured[all-docs]
+Requires-Dist: poppler-utils
+Requires-Dist: python-magic
+Requires-Dist: magika
+Requires-Dist: pandas
+Requires-Dist: colorama
+Requires-Dist: requests
+Requires-Dist: pillow
+Requires-Dist: pytesseract
+Requires-Dist: cssutils
+Requires-Dist: beautifulsoup4
+Requires-Dist: torch
+Requires-Dist: llmlingua
+Requires-Dist: PyMuPDF
+Requires-Dist: pdf2image
+Requires-Dist: python-magic
+
+# <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
+
+### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
+
+The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
+
+## Getting Started 🚀
+
+First, install thepipe:
+```bash
+pip install thepipe_api
+```
+Now you can extract comprehensive text and visuals from any file:
+```python
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf")
+```
+Or any website:
+```python
+chunks = thepipe.extract("https://example.com")
+```
+Then feed it into GPT-4-Vision:
+```python
+response = client.chat.completions.create(
+    model="gpt-4-vision-preview",
+    messages = chunks,
+)
+```
+The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
+
+## Features 🌟
+
+- Extracts text and visuals from any file or web page 📚
+- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
+- Can interpret complex PDFs, web apps, markdown, etc 🧠
+- Auto-compress prompts exceeding your chosen token limit 📦
+- Works with missing file extensions, in-memory data streams 💾
+- Works with codebases, URL, git repos, and more 🌐
+- Multi-threaded ⚡️
+
+##  How it works 🛠️
+
+The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+
+## Supported File Types 📚
+
+| Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
+|---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
+| Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
+| Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
+| Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
+| PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
+| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
+| Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
+| Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
+| Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
+| Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
+| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
+
+## Installation 📦
+
+## Local Installation 🛠️
+
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
+
+```bash
+git clone https://github.com/emcf/thepipe
+pip install -r requirements.txt
+```
+
+Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
+
+Now you can use The Pipe:
+```bash
+python thepipe.py path/to/directory
+```
+
+This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
+
+Arguments are:
+- The input source (required): can be a file path, a URL, or a directory path.
+- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
+- `--match` (optional): Regex pattern to match files in the directory.
+- `--ignore` (optional): Regex pattern to ignore files in the directory.
+- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
+- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
+
+![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.0 Author-email: Emmett
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.2 Author-email: Emmett
 McFarlane
 thepi.pe> License: MIT License Project-URL: Homepage, https://thepi.pe Project-
 URL: Documentation, https://thepi.pe/docs Project-URL: Repository, https://
 github.com/emcf/thepipe Project-URL: Issues, https://github.com/emcf/thepipe/
 issues Project-URL: Changelog, https://github.com/emcf/thepipe/releases
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
```

### Comparing `thepipe_api-0.1.0/README.md` & `thepipe_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.0/tests/test_thepipe.py` & `thepipe_api-0.1.2/tests/test_thepipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import base64
 import unittest
 import os
 import sys
 sys.path.append('..')
-import thepipe
-import core
-import extractor
-import compressor
+from thepipe_api import thepipe
+from thepipe_api import core
+from thepipe_api import extractor
+from thepipe_api import compressor
 from PIL import Image
 from io import BytesIO
 
 class test_thepipe(unittest.TestCase):
     def setUp(self):
         self.files_directory = os.path.join(os.path.dirname(__file__), 'files')
         self.outputs_directory = 'outputs'
```

### Comparing `thepipe_api-0.1.0/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.2/thepipe_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-Metadata-Version: 2.1
-Name: thepipe_api
-Version: 0.1.0
-Author-email: Emmett McFarlane <emmett@thepi.pe>
-License: MIT License
-Project-URL: Homepage, https://thepi.pe
-Project-URL: Documentation, https://thepi.pe/docs
-Project-URL: Repository, https://github.com/emcf/thepipe
-Project-URL: Issues, https://github.com/emcf/thepipe/issues
-Project-URL: Changelog, https://github.com/emcf/thepipe/releases
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.8.3
-Requires-Dist: charset-normalizer<3.0,>=2.0
-Requires-Dist: playwright
-Requires-Dist: docx2txt
-Requires-Dist: python-pptx
-Requires-Dist: Pyarrow
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: poppler-utils
-Requires-Dist: python-magic
-Requires-Dist: magika
-Requires-Dist: pandas
-Requires-Dist: colorama
-Requires-Dist: requests
-Requires-Dist: pillow
-Requires-Dist: pytesseract
-Requires-Dist: cssutils
-Requires-Dist: beautifulsoup4
-Requires-Dist: torch
-Requires-Dist: llmlingua
-Requires-Dist: PyMuPDF
-Requires-Dist: pdf2image
-Requires-Dist: python-magic
-
-# <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
-
-### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
-
-The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
-
-## Getting Started 🚀
-
-First, install thepipe:
-```bash
-pip install thepipe_api
-```
-Now you can extract comprehensive text and visuals from any file:
-```python
-from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf")
-```
-Or any website:
-```python
-chunks = thepipe.extract("https://example.com")
-```
-Then feed it into GPT-4-Vision:
-```python
-response = client.chat.completions.create(
-    model="gpt-4-vision-preview",
-    messages = chunks,
-)
-```
-The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
-
-## Features 🌟
-
-- Extracts text and visuals from any file or web page 📚
-- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
-- Can interpret complex PDFs, web apps, markdown, etc 🧠
-- Auto-compress prompts exceeding your chosen token limit 📦
-- Works with missing file extensions, in-memory data streams 💾
-- Works with codebases, URL, git repos, and more 🌐
-- Multi-threaded ⚡️
-
-##  How it works 🛠️
-
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
-
-## Supported File Types 📚
-
-| Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
-|---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
-| Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
-| Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
-| Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
-| PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
-| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
-| Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
-| Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
-| Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
-| Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
-| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
-| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
-| ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
-
-## Installation 📦
-
-## Local Installation 🛠️
-
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
-
-```bash
-git clone https://github.com/emcf/thepipe
-pip install -r requirements.txt
-```
-
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
-
-Now you can use The Pipe:
-```bash
-python thepipe.py path/to/directory
-```
-
-This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
-
-Arguments are:
-- The input source (required): can be a file path, a URL, or a directory path.
-- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
-- `--match` (optional): Regex pattern to match files in the directory.
-- `--ignore` (optional): Regex pattern to ignore files in the directory.
-- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
-- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
-- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
-
-![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
-
+Metadata-Version: 2.1
+Name: thepipe_api
+Version: 0.1.2
+Author-email: Emmett McFarlane <emmett@thepi.pe>
+License: MIT License
+Project-URL: Homepage, https://thepi.pe
+Project-URL: Documentation, https://thepi.pe/docs
+Project-URL: Repository, https://github.com/emcf/thepipe
+Project-URL: Issues, https://github.com/emcf/thepipe/issues
+Project-URL: Changelog, https://github.com/emcf/thepipe/releases
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp==3.8.3
+Requires-Dist: charset-normalizer<3.0,>=2.0
+Requires-Dist: playwright
+Requires-Dist: docx2txt
+Requires-Dist: python-pptx
+Requires-Dist: Pyarrow
+Requires-Dist: unstructured[all-docs]
+Requires-Dist: poppler-utils
+Requires-Dist: python-magic
+Requires-Dist: magika
+Requires-Dist: pandas
+Requires-Dist: colorama
+Requires-Dist: requests
+Requires-Dist: pillow
+Requires-Dist: pytesseract
+Requires-Dist: cssutils
+Requires-Dist: beautifulsoup4
+Requires-Dist: torch
+Requires-Dist: llmlingua
+Requires-Dist: PyMuPDF
+Requires-Dist: pdf2image
+Requires-Dist: python-magic
+
+# <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
+
+### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
+
+The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
+
+## Getting Started 🚀
+
+First, install thepipe:
+```bash
+pip install thepipe_api
+```
+Now you can extract comprehensive text and visuals from any file:
+```python
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf")
+```
+Or any website:
+```python
+chunks = thepipe.extract("https://example.com")
+```
+Then feed it into GPT-4-Vision:
+```python
+response = client.chat.completions.create(
+    model="gpt-4-vision-preview",
+    messages = chunks,
+)
+```
+The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
+
+## Features 🌟
+
+- Extracts text and visuals from any file or web page 📚
+- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
+- Can interpret complex PDFs, web apps, markdown, etc 🧠
+- Auto-compress prompts exceeding your chosen token limit 📦
+- Works with missing file extensions, in-memory data streams 💾
+- Works with codebases, URL, git repos, and more 🌐
+- Multi-threaded ⚡️
+
+##  How it works 🛠️
+
+The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+
+## Supported File Types 📚
+
+| Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
+|---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
+| Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
+| Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
+| Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
+| PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
+| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
+| Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
+| Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
+| Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
+| Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
+| Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
+| GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
+| ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
+
+## Installation 📦
+
+## Local Installation 🛠️
+
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
+
+```bash
+git clone https://github.com/emcf/thepipe
+pip install -r requirements.txt
+```
+
+Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
+
+Now you can use The Pipe:
+```bash
+python thepipe.py path/to/directory
+```
+
+This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
+
+Arguments are:
+- The input source (required): can be a file path, a URL, or a directory path.
+- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
+- `--match` (optional): Regex pattern to match files in the directory.
+- `--ignore` (optional): Regex pattern to ignore files in the directory.
+- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
+- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
+
+![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.0 Author-email: Emmett
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.2 Author-email: Emmett
 McFarlane
 thepi.pe> License: MIT License Project-URL: Homepage, https://thepi.pe Project-
 URL: Documentation, https://thepi.pe/docs Project-URL: Repository, https://
 github.com/emcf/thepipe Project-URL: Issues, https://github.com/emcf/thepipe/
 issues Project-URL: Changelog, https://github.com/emcf/thepipe/releases
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
```

