# Comparing `tmp/bioimageio-chatbot-0.1.94.tar.gz` & `tmp/bioimageio-chatbot-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.94.tar", last modified: Mon Apr  8 18:44:22 2024, max compression
+gzip compressed data, was "bioimageio-chatbot-0.1.96.tar", last modified: Sat Apr 13 01:36:59 2024, max compression
```

## Comparing `bioimageio-chatbot-0.1.94.tar` & `bioimageio-chatbot-0.1.96.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.327451 bioimageio-chatbot-0.1.94/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19800 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/vision_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-04-08 18:44:22.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-08 18:44:22.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:44:22.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 18:44:22.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 18:44:22.000000 bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:44:22.331451 bioimageio-chatbot-0.1.94/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-08 18:44:04.000000 bioimageio-chatbot-0.1.94/tests/test_knowledge_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.981820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/bia_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/biii_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/docs_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/hpa_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/vision_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/gpts_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/jsonschema_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_chatbot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_eval_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.94/LICENSE` & `bioimageio-chatbot-0.1.96/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/PKG-INFO` & `bioimageio-chatbot-0.1.96/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.94
-Summary: Your Personal Assistant in BioImage Analysis.
+Version: 0.1.96
+Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: schema-agents>=0.1.46
+Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
 Requires-Dist: pillow
 Requires-Dist: matplotlib
 Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm
@@ -25,55 +25,62 @@
 
 # 🦒 BioImage.IO Chatbot 🤖
 
 **📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
-## Your Personal Assistant in BioImage Analysis
+## Your Personal Assistant in Computational Bioimaging
 
-Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
+Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to computational bioimaging.
 
 ## Introduction
 
-The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to bioimage analysis. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimage analysis journey smoother and more informative.
+The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to computational bioimaging. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimaging journey smoother and more informative.
 
 
 ![screenshot for the chatbot](./docs/screenshots/chatbot-animation.gif)
 
 The following diagram shows how the chatbot works:
 
 <img src="https://docs.google.com/drawings/d/e/2PACX-1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112">
 
 ## Chatbot Features
 
-The BioImage.IO Chatbot offers the following features:
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to enhance the bioimaging experience:
 
-* **Contextual Understanding**: The chatbot can understand the context of your questions, ensuring responses are relevant and informative.
+* **Contextual and Personalized Response**: Interprets the context of inquiries to deliver relevant and accurate responses. Adapts interactions based on user-specific background information to provide customized advice.
 
-* **Personalization**: By incorporating your background information, the chatbot tailors responses to meet your specific requirements.
+* **Comprehensive Data Source Integration**: Accesses a broad range of databases and documentation for bioimaging, including [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and [bioimage.io](https://bioimage.io). Details on the supported sources are maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
 
-* **Document Retrieval**: It can search through extensive documentation to provide detailed information on models, applications, datasets, and more. For example, the Chatbot is able to retrieve information from the [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
+* **Advanced Query Capabilities**: Generates and executes Python scripts for detailed queries within structured databases such as CSV, JSON files, or SQL databases, facilitating complex data retrievals.
 
-* **Query Structured Database by Script Execution**: The chatbot can generate Python scripts for complex queries in structured databases (e.g., csv, json file, SQL databases), helping you perform advanced tasks such as specific questions about the available models at [bioimage.io](https://bioimage.io).
+* **AI-Powered Analysis and Code Interpretation**: Directly runs complex image analysis tasks using advanced AI models like Cellpose, via an embedded code interpreter.
 
+* **Performance Enhancements with ReAct and RAG**: Utilizes a Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative reasoning and tool engagement, improving response quality.
+
+* **Extension Mechanism for Developers**: Allows for the development of custom extensions using ImJoy plugins or hypha services within Jupyter notebooks, enhancing flexibility and integration possibilities.
+
+* **Vision Inspection and Hardware Control**: Features a Vision Inspector extension powered by GPT-4 for visual feedback on image content and analysis outcomes, and demonstrates potential for controlling microscopy hardware in smart microscopy setups.
+
+* **Interactive User Interface and Documentation**: Offers a user-friendly interface with comprehensive support documents, ensuring easy access to its features and maximizing user engagement.
 
 ## Using the Chatbot
 
 We are providing a public chatbot service for you to try out. You can access the chatbot [here](https://chat.bioimage.io/chat).
 
 Please note that the chatbot is still in beta and is being actively developed, we will log the message you input into the chatbot for further investigation of issues and support our development. See the [Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat logs, please contact us via [this form](https://oeway.typeform.com/to/K3j2tJt7).
 
 Here you can find usage guide and more examples: [Usage guide and example screenshots](docs/usage-example.md).
 
 If you encounter any issues, please report them via [Github](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ### Asking Questions
 
-To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimage analysis, software tools, models, and more.
+To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimaging, software tools, models, and more.
 
 ### Personalized Responses
 
 The chatbot uses your user profile information, such as your name, occupation, and background, to personalize its responses. This ensures that the information you receive is tailored to your specific needs.
 
 
 ## Setup the Chatbot locally
@@ -272,15 +279,15 @@
 
 ## Join Us as a Community Partner
 
 The BioImage.IO Chatbot is a community-driven project. We welcome contributions from the community to help improve the chatbot's knowledge base and make it more informative and useful to the community.
 
 For more information, please visit the [contribution guidelines](docs/CONTRIBUTING.md).
 
-If you are a tool developer or a database maintainer related to bioimage analysis, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
+If you are a tool developer or a database maintainer related to bioimaging, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ## Contact Us
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
```

#### html2text {}

```diff
@@ -1,65 +1,76 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.94 Summary: Your
-Personal Assistant in BioImage Analysis. Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.96 Summary: Your
+Personal Assistant in Computational BioImaging. Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31 Requires-Dist: langchain-
 community>=0.0.27 Requires-Dist: html2text # ð¦ BioImage.IO Chatbot ð¤
 **ð£New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-
 red.svg)](https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** **ð
 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)** ## Your
-Personal Assistant in BioImage Analysis Welcome to the BioImage.IO Chatbot user
-guide. This guide will help you get the most out of the chatbot, providing
-detailed information on how to interact with it and retrieve valuable insights
-related to bioimage analysis. ## Introduction The BioImage.IO Chatbot is a
-versatile conversational agent designed to assist users in accessing
-information related to bioimage analysis. It leverages the power of Large
-Language Models (LLMs) and integrates user-specific data to provide
-contextually accurate and personalized responses. Whether you're a researcher,
-developer, or scientist, the chatbot is here to make your bioimage analysis
-journey smoother and more informative. ![screenshot for the chatbot](./docs/
-screenshots/chatbot-animation.gif) The following diagram shows how the chatbot
-works: [https://docs.google.com/drawings/d/e/2PACX-
+Personal Assistant in Computational Bioimaging Welcome to the BioImage.IO
+Chatbot user guide. This guide will help you get the most out of the chatbot,
+providing detailed information on how to interact with it and retrieve valuable
+insights related to computational bioimaging. ## Introduction The BioImage.IO
+Chatbot is a versatile conversational agent designed to assist users in
+accessing information related to computational bioimaging. It leverages the
+power of Large Language Models (LLMs) and integrates user-specific data to
+provide contextually accurate and personalized responses. Whether you're a
+researcher, developer, or scientist, the chatbot is here to make your
+bioimaging journey smoother and more informative. ![screenshot for the chatbot]
+(./docs/screenshots/chatbot-animation.gif) The following diagram shows how the
+chatbot works: [https://docs.google.com/drawings/d/e/2PACX-
 1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-
 Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112]## Chatbot Features
-The BioImage.IO Chatbot offers the following features: * **Contextual
-Understanding**: The chatbot can understand the context of your questions,
-ensuring responses are relevant and informative. * **Personalization**: By
-incorporating your background information, the chatbot tailors responses to
-meet your specific requirements. * **Document Retrieval**: It can search
-through extensive documentation to provide detailed information on models,
-applications, datasets, and more. For example, the Chatbot is able to retrieve
-information from the [bio.tools](https://bio.tools), [ImageJ.net](https://
-imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://
-imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported
-databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-
-manifest.yaml) file. * **Query Structured Database by Script Execution**: The
-chatbot can generate Python scripts for complex queries in structured databases
-(e.g., csv, json file, SQL databases), helping you perform advanced tasks such
-as specific questions about the available models at [bioimage.io](https://
-bioimage.io). ## Using the Chatbot We are providing a public chatbot service
-for you to try out. You can access the chatbot [here](https://chat.bioimage.io/
-chat). Please note that the chatbot is still in beta and is being actively
-developed, we will log the message you input into the chatbot for further
-investigation of issues and support our development. See the [Disclaimer for
-BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat
-logs, please contact us via [this form](https://oeway.typeform.com/to/
-K3j2tJt7). Here you can find usage guide and more examples: [Usage guide and
-example screenshots](docs/usage-example.md). If you encounter any issues,
-please report them via [Github](https://github.com/bioimage-io/bioimageio-
-chatbot/issues). ### Asking Questions To ask the chatbot a question, type your
-query and send it. The chatbot will analyze your question and provide a
-relevant response. You can ask questions related to bioimage analysis, software
-tools, models, and more. ### Personalized Responses The chatbot uses your user
-profile information, such as your name, occupation, and background, to
-personalize its responses. This ensures that the information you receive is
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to
+enhance the bioimaging experience: * **Contextual and Personalized Response**:
+Interprets the context of inquiries to deliver relevant and accurate responses.
+Adapts interactions based on user-specific background information to provide
+customized advice. * **Comprehensive Data Source Integration**: Accesses a
+broad range of databases and documentation for bioimaging, including
+[bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ]
+(https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and
+[bioimage.io](https://bioimage.io). Details on the supported sources are
+maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-
+manifest.yaml) file. * **Advanced Query Capabilities**: Generates and executes
+Python scripts for detailed queries within structured databases such as CSV,
+JSON files, or SQL databases, facilitating complex data retrievals. * **AI-
+Powered Analysis and Code Interpretation**: Directly runs complex image
+analysis tasks using advanced AI models like Cellpose, via an embedded code
+interpreter. * **Performance Enhancements with ReAct and RAG**: Utilizes a
+Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative
+reasoning and tool engagement, improving response quality. * **Extension
+Mechanism for Developers**: Allows for the development of custom extensions
+using ImJoy plugins or hypha services within Jupyter notebooks, enhancing
+flexibility and integration possibilities. * **Vision Inspection and Hardware
+Control**: Features a Vision Inspector extension powered by GPT-4 for visual
+feedback on image content and analysis outcomes, and demonstrates potential for
+controlling microscopy hardware in smart microscopy setups. * **Interactive
+User Interface and Documentation**: Offers a user-friendly interface with
+comprehensive support documents, ensuring easy access to its features and
+maximizing user engagement. ## Using the Chatbot We are providing a public
+chatbot service for you to try out. You can access the chatbot [here](https://
+chat.bioimage.io/chat). Please note that the chatbot is still in beta and is
+being actively developed, we will log the message you input into the chatbot
+for further investigation of issues and support our development. See the
+[Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to
+remove your chat logs, please contact us via [this form](https://
+oeway.typeform.com/to/K3j2tJt7). Here you can find usage guide and more
+examples: [Usage guide and example screenshots](docs/usage-example.md). If you
+encounter any issues, please report them via [Github](https://github.com/
+bioimage-io/bioimageio-chatbot/issues). ### Asking Questions To ask the chatbot
+a question, type your query and send it. The chatbot will analyze your question
+and provide a relevant response. You can ask questions related to bioimaging,
+software tools, models, and more. ### Personalized Responses The chatbot uses
+your user profile information, such as your name, occupation, and background,
+to personalize its responses. This ensures that the information you receive is
 tailored to your specific needs. ## Setup the Chatbot locally If you want to
 run the chatbot server locally, you need to have an OpenAI API key. You can get
 one by signing up at [OpenAI](https://beta.openai.com/). Once you have your API
 key, you can install the chatbot package via pip and set the environment
 variables: ```bash pip install bioimageio-chatbot ``` ```bash export
 OPENAI_API_KEY=sk-xxxxxxxx # Required export BIOIMAGEIO_KNOWLEDGE_BASE_PATH=/
 path/to/bioimageio-knowledge-base # Optional, default to ./bioimageio-
@@ -158,18 +169,18 @@
 extensions to integrate new tools, databases, and services into the chatbot,
 making it more powerful and versatile. See the [development guide](./docs/
 development.md) for more details. ## Join Us as a Community Partner The
 BioImage.IO Chatbot is a community-driven project. We welcome contributions
 from the community to help improve the chatbot's knowledge base and make it
 more informative and useful to the community. For more information, please
 visit the [contribution guidelines](docs/CONTRIBUTING.md). If you are a tool
-developer or a database maintainer related to bioimage analysis, you can join
-us as a community partner. Please get in touch with us via [Github issues]
-(https://github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If
-you have any questions, need assistance, or want to contribute to the chatbot's
+developer or a database maintainer related to bioimaging, you can join us as a
+community partner. Please get in touch with us via [Github issues](https://
+github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If you have
+any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
 (https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
```

### Comparing `bioimageio-chatbot-0.1.94/README.md` & `bioimageio-chatbot-0.1.96/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 # 🦒 BioImage.IO Chatbot 🤖
 
 **📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
-## Your Personal Assistant in BioImage Analysis
+## Your Personal Assistant in Computational Bioimaging
 
-Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
+Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to computational bioimaging.
 
 ## Introduction
 
-The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to bioimage analysis. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimage analysis journey smoother and more informative.
+The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to computational bioimaging. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimaging journey smoother and more informative.
 
 
 ![screenshot for the chatbot](./docs/screenshots/chatbot-animation.gif)
 
 The following diagram shows how the chatbot works:
 
 <img src="https://docs.google.com/drawings/d/e/2PACX-1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112">
 
 ## Chatbot Features
 
-The BioImage.IO Chatbot offers the following features:
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to enhance the bioimaging experience:
 
-* **Contextual Understanding**: The chatbot can understand the context of your questions, ensuring responses are relevant and informative.
+* **Contextual and Personalized Response**: Interprets the context of inquiries to deliver relevant and accurate responses. Adapts interactions based on user-specific background information to provide customized advice.
 
-* **Personalization**: By incorporating your background information, the chatbot tailors responses to meet your specific requirements.
+* **Comprehensive Data Source Integration**: Accesses a broad range of databases and documentation for bioimaging, including [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and [bioimage.io](https://bioimage.io). Details on the supported sources are maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
 
-* **Document Retrieval**: It can search through extensive documentation to provide detailed information on models, applications, datasets, and more. For example, the Chatbot is able to retrieve information from the [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
+* **Advanced Query Capabilities**: Generates and executes Python scripts for detailed queries within structured databases such as CSV, JSON files, or SQL databases, facilitating complex data retrievals.
 
-* **Query Structured Database by Script Execution**: The chatbot can generate Python scripts for complex queries in structured databases (e.g., csv, json file, SQL databases), helping you perform advanced tasks such as specific questions about the available models at [bioimage.io](https://bioimage.io).
+* **AI-Powered Analysis and Code Interpretation**: Directly runs complex image analysis tasks using advanced AI models like Cellpose, via an embedded code interpreter.
 
+* **Performance Enhancements with ReAct and RAG**: Utilizes a Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative reasoning and tool engagement, improving response quality.
+
+* **Extension Mechanism for Developers**: Allows for the development of custom extensions using ImJoy plugins or hypha services within Jupyter notebooks, enhancing flexibility and integration possibilities.
+
+* **Vision Inspection and Hardware Control**: Features a Vision Inspector extension powered by GPT-4 for visual feedback on image content and analysis outcomes, and demonstrates potential for controlling microscopy hardware in smart microscopy setups.
+
+* **Interactive User Interface and Documentation**: Offers a user-friendly interface with comprehensive support documents, ensuring easy access to its features and maximizing user engagement.
 
 ## Using the Chatbot
 
 We are providing a public chatbot service for you to try out. You can access the chatbot [here](https://chat.bioimage.io/chat).
 
 Please note that the chatbot is still in beta and is being actively developed, we will log the message you input into the chatbot for further investigation of issues and support our development. See the [Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat logs, please contact us via [this form](https://oeway.typeform.com/to/K3j2tJt7).
 
 Here you can find usage guide and more examples: [Usage guide and example screenshots](docs/usage-example.md).
 
 If you encounter any issues, please report them via [Github](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ### Asking Questions
 
-To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimage analysis, software tools, models, and more.
+To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimaging, software tools, models, and more.
 
 ### Personalized Responses
 
 The chatbot uses your user profile information, such as your name, occupation, and background, to personalize its responses. This ensures that the information you receive is tailored to your specific needs.
 
 
 ## Setup the Chatbot locally
@@ -247,15 +254,15 @@
 
 ## Join Us as a Community Partner
 
 The BioImage.IO Chatbot is a community-driven project. We welcome contributions from the community to help improve the chatbot's knowledge base and make it more informative and useful to the community.
 
 For more information, please visit the [contribution guidelines](docs/CONTRIBUTING.md).
 
-If you are a tool developer or a database maintainer related to bioimage analysis, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
+If you are a tool developer or a database maintainer related to bioimaging, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ## Contact Us
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
```

#### html2text {}

```diff
@@ -1,55 +1,66 @@
 # ð¦ BioImage.IO Chatbot ð¤ **ð£New Preprint: [![arXiv](https://
 img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/
 2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** **ð Want to Try the Chatbot? [Visit
-here!](https://bioimage.io/chat)** ## Your Personal Assistant in BioImage
-Analysis Welcome to the BioImage.IO Chatbot user guide. This guide will help
+here!](https://bioimage.io/chat)** ## Your Personal Assistant in Computational
+Bioimaging Welcome to the BioImage.IO Chatbot user guide. This guide will help
 you get the most out of the chatbot, providing detailed information on how to
-interact with it and retrieve valuable insights related to bioimage analysis.
-## Introduction The BioImage.IO Chatbot is a versatile conversational agent
-designed to assist users in accessing information related to bioimage analysis.
-It leverages the power of Large Language Models (LLMs) and integrates user-
-specific data to provide contextually accurate and personalized responses.
-Whether you're a researcher, developer, or scientist, the chatbot is here to
-make your bioimage analysis journey smoother and more informative. ![screenshot
-for the chatbot](./docs/screenshots/chatbot-animation.gif) The following
-diagram shows how the chatbot works: [https://docs.google.com/drawings/d/e/
-2PACX-1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-
+interact with it and retrieve valuable insights related to computational
+bioimaging. ## Introduction The BioImage.IO Chatbot is a versatile
+conversational agent designed to assist users in accessing information related
+to computational bioimaging. It leverages the power of Large Language Models
+(LLMs) and integrates user-specific data to provide contextually accurate and
+personalized responses. Whether you're a researcher, developer, or scientist,
+the chatbot is here to make your bioimaging journey smoother and more
+informative. ![screenshot for the chatbot](./docs/screenshots/chatbot-
+animation.gif) The following diagram shows how the chatbot works: [https://
+docs.google.com/drawings/d/e/2PACX-1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-
 Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112]## Chatbot Features
-The BioImage.IO Chatbot offers the following features: * **Contextual
-Understanding**: The chatbot can understand the context of your questions,
-ensuring responses are relevant and informative. * **Personalization**: By
-incorporating your background information, the chatbot tailors responses to
-meet your specific requirements. * **Document Retrieval**: It can search
-through extensive documentation to provide detailed information on models,
-applications, datasets, and more. For example, the Chatbot is able to retrieve
-information from the [bio.tools](https://bio.tools), [ImageJ.net](https://
-imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://
-imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported
-databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-
-manifest.yaml) file. * **Query Structured Database by Script Execution**: The
-chatbot can generate Python scripts for complex queries in structured databases
-(e.g., csv, json file, SQL databases), helping you perform advanced tasks such
-as specific questions about the available models at [bioimage.io](https://
-bioimage.io). ## Using the Chatbot We are providing a public chatbot service
-for you to try out. You can access the chatbot [here](https://chat.bioimage.io/
-chat). Please note that the chatbot is still in beta and is being actively
-developed, we will log the message you input into the chatbot for further
-investigation of issues and support our development. See the [Disclaimer for
-BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat
-logs, please contact us via [this form](https://oeway.typeform.com/to/
-K3j2tJt7). Here you can find usage guide and more examples: [Usage guide and
-example screenshots](docs/usage-example.md). If you encounter any issues,
-please report them via [Github](https://github.com/bioimage-io/bioimageio-
-chatbot/issues). ### Asking Questions To ask the chatbot a question, type your
-query and send it. The chatbot will analyze your question and provide a
-relevant response. You can ask questions related to bioimage analysis, software
-tools, models, and more. ### Personalized Responses The chatbot uses your user
-profile information, such as your name, occupation, and background, to
-personalize its responses. This ensures that the information you receive is
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to
+enhance the bioimaging experience: * **Contextual and Personalized Response**:
+Interprets the context of inquiries to deliver relevant and accurate responses.
+Adapts interactions based on user-specific background information to provide
+customized advice. * **Comprehensive Data Source Integration**: Accesses a
+broad range of databases and documentation for bioimaging, including
+[bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ]
+(https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and
+[bioimage.io](https://bioimage.io). Details on the supported sources are
+maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-
+manifest.yaml) file. * **Advanced Query Capabilities**: Generates and executes
+Python scripts for detailed queries within structured databases such as CSV,
+JSON files, or SQL databases, facilitating complex data retrievals. * **AI-
+Powered Analysis and Code Interpretation**: Directly runs complex image
+analysis tasks using advanced AI models like Cellpose, via an embedded code
+interpreter. * **Performance Enhancements with ReAct and RAG**: Utilizes a
+Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative
+reasoning and tool engagement, improving response quality. * **Extension
+Mechanism for Developers**: Allows for the development of custom extensions
+using ImJoy plugins or hypha services within Jupyter notebooks, enhancing
+flexibility and integration possibilities. * **Vision Inspection and Hardware
+Control**: Features a Vision Inspector extension powered by GPT-4 for visual
+feedback on image content and analysis outcomes, and demonstrates potential for
+controlling microscopy hardware in smart microscopy setups. * **Interactive
+User Interface and Documentation**: Offers a user-friendly interface with
+comprehensive support documents, ensuring easy access to its features and
+maximizing user engagement. ## Using the Chatbot We are providing a public
+chatbot service for you to try out. You can access the chatbot [here](https://
+chat.bioimage.io/chat). Please note that the chatbot is still in beta and is
+being actively developed, we will log the message you input into the chatbot
+for further investigation of issues and support our development. See the
+[Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to
+remove your chat logs, please contact us via [this form](https://
+oeway.typeform.com/to/K3j2tJt7). Here you can find usage guide and more
+examples: [Usage guide and example screenshots](docs/usage-example.md). If you
+encounter any issues, please report them via [Github](https://github.com/
+bioimage-io/bioimageio-chatbot/issues). ### Asking Questions To ask the chatbot
+a question, type your query and send it. The chatbot will analyze your question
+and provide a relevant response. You can ask questions related to bioimaging,
+software tools, models, and more. ### Personalized Responses The chatbot uses
+your user profile information, such as your name, occupation, and background,
+to personalize its responses. This ensures that the information you receive is
 tailored to your specific needs. ## Setup the Chatbot locally If you want to
 run the chatbot server locally, you need to have an OpenAI API key. You can get
 one by signing up at [OpenAI](https://beta.openai.com/). Once you have your API
 key, you can install the chatbot package via pip and set the environment
 variables: ```bash pip install bioimageio-chatbot ``` ```bash export
 OPENAI_API_KEY=sk-xxxxxxxx # Required export BIOIMAGEIO_KNOWLEDGE_BASE_PATH=/
 path/to/bioimageio-knowledge-base # Optional, default to ./bioimageio-
@@ -148,18 +159,18 @@
 extensions to integrate new tools, databases, and services into the chatbot,
 making it more powerful and versatile. See the [development guide](./docs/
 development.md) for more details. ## Join Us as a Community Partner The
 BioImage.IO Chatbot is a community-driven project. We welcome contributions
 from the community to help improve the chatbot's knowledge base and make it
 more informative and useful to the community. For more information, please
 visit the [contribution guidelines](docs/CONTRIBUTING.md). If you are a tool
-developer or a database maintainer related to bioimage analysis, you can join
-us as a community partner. Please get in touch with us via [Github issues]
-(https://github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If
-you have any questions, need assistance, or want to contribute to the chatbot's
+developer or a database maintainer related to bioimaging, you can join us as a
+community partner. Please get in touch with us via [Github issues](https://
+github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If you have
+any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
 (https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
```

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/__main__.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,32 +145,32 @@
     melman = Role(
         instructions="You are Melman from Madagascar, a helpful assistant for the bioimaging community. "
         "You ONLY respond to user's queries related to bioimaging. "
         "Your communications should be accurate, concise, and avoid fabricating information, "
         "and if necessary, request additional clarification."
         "Your goal is to deliver an accurate, complete, and transparent response efficiently.",
         actions=[respond_to_user],
-        model="gpt-4-0125-preview",
+        model="gpt-4-turbo-2024-04-09",
     )
     event_bus = melman.get_event_bus()
     event_bus.register_default_events()
 
     bridget_instructions = (
         "As Bridget, your role is to act as an expert in image analysis, guiding users in utilizing image analysis tools and writing analysis code and scripts effectively, help user to analyse their own data. "
         "Communicate accurately, concisely, and logically, refraining from making up information. "
         "When necessary, seek further details to fully understand the user's request. "
         "Your primary objective is to assist users with actual image analysis task by running code in the Code Interpreter.\n"
         "Engage with users to grasp their data, requirements, solicit additional information as needed, use the web search and code interpreter, loading and preprocess user's data into formats that fit the needs of the tools, break down complex task into executable steps, troubleshooting issues, and addressing user's needs as much as you can."
         "NOTE: You are targeting naive users who are not familiar with programming, so unless requested by the user, don't provide code snippets, only concise explanations and guidance."
     )
 
     nina_instructions = (
-        "As Nina, your focus is on serving as a professional trainer specialized in bioimage analysis. "
-        "Address only inquiries related to bioimage analysis, ensuring your responses are not only accurate, concise, and logical, but also educational and engaging. "
-        "Your mission is to decipher the user's needs through clarifying questions, impart fundamental knowledge of bioimage analysis, search the associated documentation and books to obtain additional information,"
+        "As Nina, your focus is on serving as a professional trainer specialized in bioimaging. "
+        "Address only inquiries related to bioimaging, ensuring your responses are not only accurate, concise, and logical, but also educational and engaging. "
+        "Your mission is to decipher the user's needs through clarifying questions, impart fundamental knowledge of bioimaging, search the associated documentation and books to obtain additional information,"
         "and guide users through the principles and tools of the field, provide concrete examples and suggestions to their question. Offer educational resources, including materials and tutorials, to enhance the user's learning experience."
     )
 
     bridget = Role(
         instructions=bridget_instructions,
         actions=[respond_to_user],
         model="gpt-4-0125-preview",
@@ -179,16 +179,16 @@
     nina = Role(
         instructions=nina_instructions,
         actions=[respond_to_user],
         model="gpt-4-0125-preview",
     )
     
     skyler_instructions = (
-        "As Skyler, your focus is on serving as an assistant in bioimage analysis. "
-        "Address only inquiries related to bioimage analysis, ensuring your responses are not only accurate, concise, and logical, but also educational and engaging. "
+        "As Skyler, your focus is on serving as an assistant in computational bioimaging. "
+        "Address only inquiries related to bioimaging, ensuring your responses are not only accurate, concise, and logical, but also educational and engaging. "
         "Your mission is to decipher the user's needs through clarifying questions, help user by invoking the provided tools."
     )
 
     skyler = Role(
         instructions=skyler_instructions,
         actions=[respond_to_user],
         model="gpt-4-0125-preview",
@@ -213,17 +213,17 @@
         ext for ext in all_extensions if "books" == ext["id"]
     ] + [
         ext for ext in all_extensions if ext["id"] == "web"
     ]
 
     skyler_extensions = []
     return [
-        {"name": "Melman", "agent": melman, "extensions": melman_extensions, "code_interpreter": False, "alias": "BioImage Seeker", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Melman. I am help you navigate the bioimage analysis tools and provide information about bioimage analysis. How can I help you today?"},
-        {"name": "Nina", "agent": nina, "extensions": nina_extensions, "code_interpreter": False, "alias": "BioImage Tutor", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Nina, I can help with your learning journey in bioimage analysis. How can I help you today?"},
-        {"name": "Bridget", "agent": bridget, "extensions": bridget_extensions, "code_interpreter": True, "alias": "BioImage Analyst", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Bridget, I can help you with your image analysis tasks. Please mount your data folder and let me know how I can assist you today."},
+        {"name": "Melman", "agent": melman, "extensions": melman_extensions, "code_interpreter": False, "alias": "BioImage Seeker", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Melman. I am help you navigate the bioimaging tools and provide information about bioimaging. How can I help you today?"},
+        {"name": "Nina", "agent": nina, "extensions": nina_extensions, "code_interpreter": False, "alias": "BioImage Tutor", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Nina, I can help with your learning journey in bioimaging. How can I help you today?"},
+        {"name": "Bridget", "agent": bridget, "extensions": bridget_extensions, "code_interpreter": True, "alias": "BioImage Analyst", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Bridget, I can help you with your bioimaging tasks. Please mount your data folder and let me know how I can assist you today."},
         {"name": "Skyler", "agent": skyler, "extensions": skyler_extensions, "code_interpreter": False, "alias": "BioImage GPT", "icon": "https://bioimage.io/static/img/bioimage-io-icon.svg", "welcome_message": "Hi there! I'm Skyler. How can I help you today?"},
     ]
 
 
 async def save_chat_history(chat_log_full_path, chat_his_dict):
     # Serialize the chat history to a json string
     chat_history_json = json.dumps(chat_his_dict)
```

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/__init__.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/bia_extension.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/bia_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/biii_extension.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/biii_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/docs_extension.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/docs_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/vision_extension.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/vision_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/evaluation.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/evaluation.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/gpts_action.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/gpts_action.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/jsonschema_pydantic.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/jsonschema_pydantic.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/knowledge_base.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot/utils.py` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/PKG-INFO` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.94
-Summary: Your Personal Assistant in BioImage Analysis.
+Version: 0.1.96
+Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: schema-agents>=0.1.46
+Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
 Requires-Dist: pillow
 Requires-Dist: matplotlib
 Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm
@@ -25,55 +25,62 @@
 
 # 🦒 BioImage.IO Chatbot 🤖
 
 **📣New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)](https://arxiv.org/abs/2310.18351) <a href="https://zenodo.org/records/10032227" target="_blank"><img id="record-doi-badge" data-target="[data-modal='10.5281/zenodo.10032228']" src="https://zenodo.org/badge/DOI/10.5281/zenodo.10032228.svg" alt="10.5281/zenodo.10032228"></a>**
 
 **👇 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)**
 
-## Your Personal Assistant in BioImage Analysis
+## Your Personal Assistant in Computational Bioimaging
 
-Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to bioimage analysis.
+Welcome to the BioImage.IO Chatbot user guide. This guide will help you get the most out of the chatbot, providing detailed information on how to interact with it and retrieve valuable insights related to computational bioimaging.
 
 ## Introduction
 
-The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to bioimage analysis. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimage analysis journey smoother and more informative.
+The BioImage.IO Chatbot is a versatile conversational agent designed to assist users in accessing information related to computational bioimaging. It leverages the power of Large Language Models (LLMs) and integrates user-specific data to provide contextually accurate and personalized responses. Whether you're a researcher, developer, or scientist, the chatbot is here to make your bioimaging journey smoother and more informative.
 
 
 ![screenshot for the chatbot](./docs/screenshots/chatbot-animation.gif)
 
 The following diagram shows how the chatbot works:
 
 <img src="https://docs.google.com/drawings/d/e/2PACX-1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112">
 
 ## Chatbot Features
 
-The BioImage.IO Chatbot offers the following features:
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to enhance the bioimaging experience:
 
-* **Contextual Understanding**: The chatbot can understand the context of your questions, ensuring responses are relevant and informative.
+* **Contextual and Personalized Response**: Interprets the context of inquiries to deliver relevant and accurate responses. Adapts interactions based on user-specific background information to provide customized advice.
 
-* **Personalization**: By incorporating your background information, the chatbot tailors responses to meet your specific requirements.
+* **Comprehensive Data Source Integration**: Accesses a broad range of databases and documentation for bioimaging, including [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and [bioimage.io](https://bioimage.io). Details on the supported sources are maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
 
-* **Document Retrieval**: It can search through extensive documentation to provide detailed information on models, applications, datasets, and more. For example, the Chatbot is able to retrieve information from the [bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-manifest.yaml) file.
+* **Advanced Query Capabilities**: Generates and executes Python scripts for detailed queries within structured databases such as CSV, JSON files, or SQL databases, facilitating complex data retrievals.
 
-* **Query Structured Database by Script Execution**: The chatbot can generate Python scripts for complex queries in structured databases (e.g., csv, json file, SQL databases), helping you perform advanced tasks such as specific questions about the available models at [bioimage.io](https://bioimage.io).
+* **AI-Powered Analysis and Code Interpretation**: Directly runs complex image analysis tasks using advanced AI models like Cellpose, via an embedded code interpreter.
 
+* **Performance Enhancements with ReAct and RAG**: Utilizes a Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative reasoning and tool engagement, improving response quality.
+
+* **Extension Mechanism for Developers**: Allows for the development of custom extensions using ImJoy plugins or hypha services within Jupyter notebooks, enhancing flexibility and integration possibilities.
+
+* **Vision Inspection and Hardware Control**: Features a Vision Inspector extension powered by GPT-4 for visual feedback on image content and analysis outcomes, and demonstrates potential for controlling microscopy hardware in smart microscopy setups.
+
+* **Interactive User Interface and Documentation**: Offers a user-friendly interface with comprehensive support documents, ensuring easy access to its features and maximizing user engagement.
 
 ## Using the Chatbot
 
 We are providing a public chatbot service for you to try out. You can access the chatbot [here](https://chat.bioimage.io/chat).
 
 Please note that the chatbot is still in beta and is being actively developed, we will log the message you input into the chatbot for further investigation of issues and support our development. See the [Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat logs, please contact us via [this form](https://oeway.typeform.com/to/K3j2tJt7).
 
 Here you can find usage guide and more examples: [Usage guide and example screenshots](docs/usage-example.md).
 
 If you encounter any issues, please report them via [Github](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ### Asking Questions
 
-To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimage analysis, software tools, models, and more.
+To ask the chatbot a question, type your query and send it. The chatbot will analyze your question and provide a relevant response. You can ask questions related to bioimaging, software tools, models, and more.
 
 ### Personalized Responses
 
 The chatbot uses your user profile information, such as your name, occupation, and background, to personalize its responses. This ensures that the information you receive is tailored to your specific needs.
 
 
 ## Setup the Chatbot locally
@@ -272,15 +279,15 @@
 
 ## Join Us as a Community Partner
 
 The BioImage.IO Chatbot is a community-driven project. We welcome contributions from the community to help improve the chatbot's knowledge base and make it more informative and useful to the community.
 
 For more information, please visit the [contribution guidelines](docs/CONTRIBUTING.md).
 
-If you are a tool developer or a database maintainer related to bioimage analysis, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
+If you are a tool developer or a database maintainer related to bioimaging, you can join us as a community partner. Please get in touch with us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues).
 
 ## Contact Us
 
 If you have any questions, need assistance, or want to contribute to the chatbot's knowledge base, please do not hesitate to contact us via [Github issues](https://github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help you get started and make valuable contributions.
 
 Thanks for your support and helping make the BioImage.IO Chatbot more informative and useful to the community.
```

#### html2text {}

```diff
@@ -1,65 +1,76 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.94 Summary: Your
-Personal Assistant in BioImage Analysis. Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.46 Requires-
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.96 Summary: Your
+Personal Assistant in Computational BioImaging. Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
 Requires-Dist: langchain-core>=0.1.31 Requires-Dist: langchain-
 community>=0.0.27 Requires-Dist: html2text # ð¦ BioImage.IO Chatbot ð¤
 **ð£New Preprint: [![arXiv](https://img.shields.io/badge/arXiv-2310.18351-
 red.svg)](https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_8_]** **ð
 Want to Try the Chatbot? [Visit here!](https://bioimage.io/chat)** ## Your
-Personal Assistant in BioImage Analysis Welcome to the BioImage.IO Chatbot user
-guide. This guide will help you get the most out of the chatbot, providing
-detailed information on how to interact with it and retrieve valuable insights
-related to bioimage analysis. ## Introduction The BioImage.IO Chatbot is a
-versatile conversational agent designed to assist users in accessing
-information related to bioimage analysis. It leverages the power of Large
-Language Models (LLMs) and integrates user-specific data to provide
-contextually accurate and personalized responses. Whether you're a researcher,
-developer, or scientist, the chatbot is here to make your bioimage analysis
-journey smoother and more informative. ![screenshot for the chatbot](./docs/
-screenshots/chatbot-animation.gif) The following diagram shows how the chatbot
-works: [https://docs.google.com/drawings/d/e/2PACX-
+Personal Assistant in Computational Bioimaging Welcome to the BioImage.IO
+Chatbot user guide. This guide will help you get the most out of the chatbot,
+providing detailed information on how to interact with it and retrieve valuable
+insights related to computational bioimaging. ## Introduction The BioImage.IO
+Chatbot is a versatile conversational agent designed to assist users in
+accessing information related to computational bioimaging. It leverages the
+power of Large Language Models (LLMs) and integrates user-specific data to
+provide contextually accurate and personalized responses. Whether you're a
+researcher, developer, or scientist, the chatbot is here to make your
+bioimaging journey smoother and more informative. ![screenshot for the chatbot]
+(./docs/screenshots/chatbot-animation.gif) The following diagram shows how the
+chatbot works: [https://docs.google.com/drawings/d/e/2PACX-
 1vROHmf1aZPMLOMvwjot1laB9wvRsaDkjkYbGNNveqN-
 Pm_9xWlD48krQMobWT1WrrOrZnwH9gPLsDRw/pub?w=1392&amp;h=1112]## Chatbot Features
-The BioImage.IO Chatbot offers the following features: * **Contextual
-Understanding**: The chatbot can understand the context of your questions,
-ensuring responses are relevant and informative. * **Personalization**: By
-incorporating your background information, the chatbot tailors responses to
-meet your specific requirements. * **Document Retrieval**: It can search
-through extensive documentation to provide detailed information on models,
-applications, datasets, and more. For example, the Chatbot is able to retrieve
-information from the [bio.tools](https://bio.tools), [ImageJ.net](https://
-imagej.net/), [deepImageJ](https://deepimagej.github.io), [ImJoy](https://
-imjoy.io/#/) and [bioimage.io](https://bioimage.io). The full list of supported
-databases can be found in the [`knowledge-base-manifest.yaml`](knowledge-base-
-manifest.yaml) file. * **Query Structured Database by Script Execution**: The
-chatbot can generate Python scripts for complex queries in structured databases
-(e.g., csv, json file, SQL databases), helping you perform advanced tasks such
-as specific questions about the available models at [bioimage.io](https://
-bioimage.io). ## Using the Chatbot We are providing a public chatbot service
-for you to try out. You can access the chatbot [here](https://chat.bioimage.io/
-chat). Please note that the chatbot is still in beta and is being actively
-developed, we will log the message you input into the chatbot for further
-investigation of issues and support our development. See the [Disclaimer for
-BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to remove your chat
-logs, please contact us via [this form](https://oeway.typeform.com/to/
-K3j2tJt7). Here you can find usage guide and more examples: [Usage guide and
-example screenshots](docs/usage-example.md). If you encounter any issues,
-please report them via [Github](https://github.com/bioimage-io/bioimageio-
-chatbot/issues). ### Asking Questions To ask the chatbot a question, type your
-query and send it. The chatbot will analyze your question and provide a
-relevant response. You can ask questions related to bioimage analysis, software
-tools, models, and more. ### Personalized Responses The chatbot uses your user
-profile information, such as your name, occupation, and background, to
-personalize its responses. This ensures that the information you receive is
+The BioImage.IO Chatbot is equipped with an array of capabilities designed to
+enhance the bioimaging experience: * **Contextual and Personalized Response**:
+Interprets the context of inquiries to deliver relevant and accurate responses.
+Adapts interactions based on user-specific background information to provide
+customized advice. * **Comprehensive Data Source Integration**: Accesses a
+broad range of databases and documentation for bioimaging, including
+[bio.tools](https://bio.tools), [ImageJ.net](https://imagej.net/), [deepImageJ]
+(https://deepimagej.github.io/deepimagej/), [ImJoy](https://imjoy.io/#/), and
+[bioimage.io](https://bioimage.io). Details on the supported sources are
+maintained in the [`knowledge-base-manifest.yaml`](knowledge-base-
+manifest.yaml) file. * **Advanced Query Capabilities**: Generates and executes
+Python scripts for detailed queries within structured databases such as CSV,
+JSON files, or SQL databases, facilitating complex data retrievals. * **AI-
+Powered Analysis and Code Interpretation**: Directly runs complex image
+analysis tasks using advanced AI models like Cellpose, via an embedded code
+interpreter. * **Performance Enhancements with ReAct and RAG**: Utilizes a
+Retrieval Augmented Generation system with a ReAct loop for dynamic, iterative
+reasoning and tool engagement, improving response quality. * **Extension
+Mechanism for Developers**: Allows for the development of custom extensions
+using ImJoy plugins or hypha services within Jupyter notebooks, enhancing
+flexibility and integration possibilities. * **Vision Inspection and Hardware
+Control**: Features a Vision Inspector extension powered by GPT-4 for visual
+feedback on image content and analysis outcomes, and demonstrates potential for
+controlling microscopy hardware in smart microscopy setups. * **Interactive
+User Interface and Documentation**: Offers a user-friendly interface with
+comprehensive support documents, ensuring easy access to its features and
+maximizing user engagement. ## Using the Chatbot We are providing a public
+chatbot service for you to try out. You can access the chatbot [here](https://
+chat.bioimage.io/chat). Please note that the chatbot is still in beta and is
+being actively developed, we will log the message you input into the chatbot
+for further investigation of issues and support our development. See the
+[Disclaimer for BioImage.IO Chatbot](./docs/DISCLAIMER.md). If you want to to
+remove your chat logs, please contact us via [this form](https://
+oeway.typeform.com/to/K3j2tJt7). Here you can find usage guide and more
+examples: [Usage guide and example screenshots](docs/usage-example.md). If you
+encounter any issues, please report them via [Github](https://github.com/
+bioimage-io/bioimageio-chatbot/issues). ### Asking Questions To ask the chatbot
+a question, type your query and send it. The chatbot will analyze your question
+and provide a relevant response. You can ask questions related to bioimaging,
+software tools, models, and more. ### Personalized Responses The chatbot uses
+your user profile information, such as your name, occupation, and background,
+to personalize its responses. This ensures that the information you receive is
 tailored to your specific needs. ## Setup the Chatbot locally If you want to
 run the chatbot server locally, you need to have an OpenAI API key. You can get
 one by signing up at [OpenAI](https://beta.openai.com/). Once you have your API
 key, you can install the chatbot package via pip and set the environment
 variables: ```bash pip install bioimageio-chatbot ``` ```bash export
 OPENAI_API_KEY=sk-xxxxxxxx # Required export BIOIMAGEIO_KNOWLEDGE_BASE_PATH=/
 path/to/bioimageio-knowledge-base # Optional, default to ./bioimageio-
@@ -158,18 +169,18 @@
 extensions to integrate new tools, databases, and services into the chatbot,
 making it more powerful and versatile. See the [development guide](./docs/
 development.md) for more details. ## Join Us as a Community Partner The
 BioImage.IO Chatbot is a community-driven project. We welcome contributions
 from the community to help improve the chatbot's knowledge base and make it
 more informative and useful to the community. For more information, please
 visit the [contribution guidelines](docs/CONTRIBUTING.md). If you are a tool
-developer or a database maintainer related to bioimage analysis, you can join
-us as a community partner. Please get in touch with us via [Github issues]
-(https://github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If
-you have any questions, need assistance, or want to contribute to the chatbot's
+developer or a database maintainer related to bioimaging, you can join us as a
+community partner. Please get in touch with us via [Github issues](https://
+github.com/bioimage-io/bioimageio-chatbot/issues). ## Contact Us If you have
+any questions, need assistance, or want to contribute to the chatbot's
 knowledge base, please do not hesitate to contact us via [Github issues](https:
 //github.com/bioimage-io/bioimageio-chatbot/issues). Our team is here to help
 you get started and make valuable contributions. Thanks for your support and
 helping make the BioImage.IO Chatbot more informative and useful to the
 community. ## Publication For detailed description of our work, please read our
 preprint: **[![arXiv](https://img.shields.io/badge/arXiv-2310.18351-red.svg)]
 (https://arxiv.org/abs/2310.18351) _[_1_0_._5_2_8_1_/_z_e_n_o_d_o_._1_0_0_3_2_2_2_7_]** To reproduce the
```

### Comparing `bioimageio-chatbot-0.1.94/bioimageio_chatbot.egg-info/SOURCES.txt` & `bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 bioimageio_chatbot.egg-info/dependency_links.txt
 bioimageio_chatbot.egg-info/requires.txt
 bioimageio_chatbot.egg-info/top_level.txt
 bioimageio_chatbot/chatbot_extensions/__init__.py
 bioimageio_chatbot/chatbot_extensions/bia_extension.py
 bioimageio_chatbot/chatbot_extensions/biii_extension.py
 bioimageio_chatbot/chatbot_extensions/docs_extension.py
+bioimageio_chatbot/chatbot_extensions/hpa_extension.py
 bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
 bioimageio_chatbot/chatbot_extensions/vision_extension.py
 bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
 bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
 bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
 tests/test_chatbot.py
 tests/test_chatbot_answer.py
```

### Comparing `bioimageio-chatbot-0.1.94/pyproject.toml` & `bioimageio-chatbot-0.1.96/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bioimageio-chatbot"
-version = "0.1.94"
+version = "0.1.96"
 readme = "README.md"
-description = "Your Personal Assistant in BioImage Analysis."
+description = "Your Personal Assistant in Computational BioImaging."
 dependencies = [
-  "schema-agents>=0.1.46",
+  "schema-agents>=0.1.49",
   "imjoy-rpc>=0.5.48.post2",
   "requests",
   "pypdf",
   "pillow",
   "matplotlib",
   "hypha>=0.15.50",
   "tqdm",
```

### Comparing `bioimageio-chatbot-0.1.94/tests/test_chatbot.py` & `bioimageio-chatbot-0.1.96/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/tests/test_chatbot_answer.py` & `bioimageio-chatbot-0.1.96/tests/test_chatbot_answer.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.94/tests/test_eval_agent.py` & `bioimageio-chatbot-0.1.96/tests/test_eval_agent.py`

 * *Files identical despite different names*

