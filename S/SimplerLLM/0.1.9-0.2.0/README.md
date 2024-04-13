# Comparing `tmp/SimplerLLM-0.1.9.tar.gz` & `tmp/SimplerLLM-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimplerLLM-0.1.9.tar", last modified: Fri Mar 29 15:10:44 2024, max compression
+gzip compressed data, was "SimplerLLM-0.2.0.tar", last modified: Sat Apr 13 10:55:59 2024, max compression
```

## Comparing `SimplerLLM-0.1.9.tar` & `SimplerLLM-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.321175 SimplerLLM-0.1.9/
--rw-rw-rw-   0        0        0     6109 2024-03-29 15:10:44.321175 SimplerLLM-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.294176 SimplerLLM-0.1.9/SimplerLLM/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.300174 SimplerLLM-0.1.9/SimplerLLM/image/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/image/__init__.py
--rw-rw-rw-   0        0        0     1194 2024-03-20 13:27:59.000000 SimplerLLM-0.1.9/SimplerLLM/image/img_helper_funcs.py
--rw-rw-rw-   0        0        0     1996 2024-03-20 13:14:02.000000 SimplerLLM-0.1.9/SimplerLLM/image/stability_ai.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.304175 SimplerLLM-0.1.9/SimplerLLM/language/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/language/__init__.py
--rw-rw-rw-   0        0        0    11122 2024-03-29 15:02:16.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm.py
--rw-rw-rw-   0        0        0     2607 2024-03-25 13:07:09.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_addons.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.309174 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     9658 2024-03-29 15:06:07.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/anthropic_llm.py
--rw-rw-rw-   0        0        0    12109 2024-03-29 15:03:43.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/gemini_llm.py
--rw-rw-rw-   0        0        0      184 2024-03-29 14:59:41.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/llm_response_models.py
--rw-rw-rw-   0        0        0     6997 2024-03-29 15:03:33.000000 SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/openai_llm.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.311174 SimplerLLM-0.1.9/SimplerLLM/prompts/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/prompts/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/prompts/prompt_builder.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.320175 SimplerLLM-0.1.9/SimplerLLM/tools/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/tools/__init__.py
--rw-rw-rw-   0        0        0      915 2024-03-19 15:25:28.000000 SimplerLLM-0.1.9/SimplerLLM/tools/file_loader.py
--rw-rw-rw-   0        0        0     6006 2024-03-19 15:25:27.000000 SimplerLLM-0.1.9/SimplerLLM/tools/generic_loader.py
--rw-rw-rw-   0        0        0     4460 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/tools/json_helpers.py
--rw-rw-rw-   0        0        0     4988 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/SimplerLLM/tools/rapid_api.py
--rw-rw-rw-   0        0        0     7138 2024-03-26 11:09:21.000000 SimplerLLM-0.1.9/SimplerLLM/tools/serp.py
--rw-rw-rw-   0        0        0     3821 2024-03-26 10:57:08.000000 SimplerLLM-0.1.9/SimplerLLM/tools/text_chunker.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.298174 SimplerLLM-0.1.9/SimplerLLM.egg-info/
--rw-rw-rw-   0        0        0     6109 2024-03-29 15:10:44.000000 SimplerLLM-0.1.9/SimplerLLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      948 2024-03-29 15:10:44.000000 SimplerLLM-0.1.9/SimplerLLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:10:44.000000 SimplerLLM-0.1.9/SimplerLLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2024-03-29 15:10:44.000000 SimplerLLM-0.1.9/SimplerLLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-29 15:10:44.000000 SimplerLLM-0.1.9/SimplerLLM.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-29 15:10:44.320175 SimplerLLM-0.1.9/my_tests/
--rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.1.9/my_tests/__init__.py
--rw-rw-rw-   0        0        0       42 2024-03-29 15:10:44.322175 SimplerLLM-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1371 2024-03-29 15:10:35.000000 SimplerLLM-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.821885 SimplerLLM-0.2.0/
+-rw-rw-rw-   0        0        0     6134 2024-04-13 10:55:59.820885 SimplerLLM-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.792885 SimplerLLM-0.2.0/SimplerLLM/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.799885 SimplerLLM-0.2.0/SimplerLLM/image/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/image/__init__.py
+-rw-rw-rw-   0        0        0     1194 2024-03-20 13:27:59.000000 SimplerLLM-0.2.0/SimplerLLM/image/img_helper_funcs.py
+-rw-rw-rw-   0        0        0     1996 2024-03-20 13:14:02.000000 SimplerLLM-0.2.0/SimplerLLM/image/stability_ai.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.804885 SimplerLLM-0.2.0/SimplerLLM/language/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/language/__init__.py
+-rw-rw-rw-   0        0        0     8767 2024-04-13 08:48:06.000000 SimplerLLM-0.2.0/SimplerLLM/language/embeddings.py
+-rw-rw-rw-   0        0        0     6422 2024-04-13 08:35:22.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm.py
+-rw-rw-rw-   0        0        0     2607 2024-03-25 13:07:09.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_addons.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.809885 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     5361 2024-04-13 08:36:07.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/anthropic_llm.py
+-rw-rw-rw-   0        0        0     8566 2024-04-13 08:35:54.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/gemini_llm.py
+-rw-rw-rw-   0        0        0      184 2024-03-29 14:59:41.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/llm_response_models.py
+-rw-rw-rw-   0        0        0     6581 2024-04-13 08:40:58.000000 SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/openai_llm.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.811885 SimplerLLM-0.2.0/SimplerLLM/prompts/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/prompts/prompt_builder.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.819885 SimplerLLM-0.2.0/SimplerLLM/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/tools/__init__.py
+-rw-rw-rw-   0        0        0      915 2024-03-19 15:25:28.000000 SimplerLLM-0.2.0/SimplerLLM/tools/file_loader.py
+-rw-rw-rw-   0        0        0     6006 2024-03-19 15:25:27.000000 SimplerLLM-0.2.0/SimplerLLM/tools/generic_loader.py
+-rw-rw-rw-   0        0        0     5414 2024-04-12 17:40:03.000000 SimplerLLM-0.2.0/SimplerLLM/tools/json_helpers.py
+-rw-rw-rw-   0        0        0     4988 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/SimplerLLM/tools/rapid_api.py
+-rw-rw-rw-   0        0        0     7138 2024-03-26 11:09:21.000000 SimplerLLM-0.2.0/SimplerLLM/tools/serp.py
+-rw-rw-rw-   0        0        0     8646 2024-04-13 08:48:36.000000 SimplerLLM-0.2.0/SimplerLLM/tools/text_chunker.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.796885 SimplerLLM-0.2.0/SimplerLLM.egg-info/
+-rw-rw-rw-   0        0        0     6134 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-13 10:55:59.000000 SimplerLLM-0.2.0/SimplerLLM.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 10:55:59.820885 SimplerLLM-0.2.0/my_tests/
+-rw-rw-rw-   0        0        0        0 2024-03-19 13:24:26.000000 SimplerLLM-0.2.0/my_tests/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 10:55:59.821885 SimplerLLM-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2024-04-13 08:21:31.000000 SimplerLLM-0.2.0/setup.py
```

### Comparing `SimplerLLM-0.1.9/PKG-INFO` & `SimplerLLM-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.1.9
+Version: 0.2.0
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,121 +15,118 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-
 # ⚪ SimplerLLM (Beta)
 
 ⚡ Your Easy Pass to Advanced AI ⚡
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-
 ## 🤔 What is SimplerLLM?
 
 SimplerLLM is an open-source Python library designed to simplify interactions with Large Language Models (LLMs) for researchers and beginners. It offers a unified interface for different LLM providers and a suite of tools to enhance language model capabilities and make it Super easy for anyone to develop AI-powered tools and apps.
 
 ## Easy Installation
+
 With pip:
+
 ```bash
 pip install simplerllm
 ```
 
-
 ## Features
 
 - **Unified LLM Interface**: Define an LLM instance in one line for providers like OpenAI and Google Gemini. Future versions will support more APIs and LLM providers.
 - **Generic Text Loader**: Load text from various sources like DOCX, PDF, TXT files, YouTube scripts, or blog posts.
 - **RapidAPI Connector**: Connect with AI services on RapidAPI.
 - **SERP Integration**: Perform searches using DuckDuckGo, with more search engines coming soon.
 - **Prompt Template Builder**: Easily create and manage prompt templates.
-And Much More Coming Soon!
-
+  And Much More Coming Soon!
 
 ### Setting Up Environment Variables
-To use this library, you need to set several API keys in your environment. Start by creating a .env file in the root directory of your project and adding your API keys there. 
+
+To use this library, you need to set several API keys in your environment. Start by creating a .env file in the root directory of your project and adding your API keys there.
 
 🔴 This file should be kept private and not committed to version control to protect your keys.
 
 Here is an example of what your .env file should look like:
 
-``` 
+```
 OPENAI_API_KEY="your_openai_api_key_here"
 GEMENI_API_KEY="your_gemeni_api_key_here"
 CLAUDE_API_KEY="your_claude_api_key_here"
 RAPIDAPI_API_KEY="your_rapidapi_key_here" # for accessing APIs on RapidAPI
 VALUE_SERP_API_KEY="your_value_serp_api_key_here" #for Google search
 SERPER_API_KEY="your_serper_api_key_here" #for Google search
 STABILITY_API_KEY="your_stability_api_key_here" #for image generation
 
 ```
 
-
-
-
 ### Creating an LLM Instance
 
 ```python
 from SimplerLLM.language.llm import LLM, LLMProvider
 
 # For OpenAI
-llm_instance = LLM.create(provider=LLMProvider.OPENAI)
+llm_instance = LLM.create(provider=LLMProvider.OPENAI, model_name="gpt-3.5-turbo")
 
 # For Google Gemini
 #llm_instance = LLM.create(provider=LLMProvider.GEMINI,model_name="gemini-pro")
 
 # For Anthropic Claude 
 #llm_instance = LLM.create(LLMProvider.ANTHROPIC, model_name="claude-3-opus-20240229")
 
-
-response = llm_instance.generate_text(user_prompt="generate a 5 words sentence")
+response = llm_instance.generate_response(prompt="generate a 5 words sentence")
 
 ```
 
 ### Using Tools
 
 #### SERP
+
 ```python
 from SimplerLLM.tools.serp import search_with_serper_api
 
 search_results = search_with_serper_api("your search query", num_results=3)
 
 # use the search results the way you want!
 
 ```
 
 #### Generic Text Loader
+
 ```python
 from SimplerLLM.tools.generic_loader import load_content
 
 text_file = load_content("file.txt")
 
 print(text_file.content)
 
 ```
 
 #### Calling any RapidAPI API
+
 ```python
 from  SimplerLLM.tools.rapid_api import RapidAPIClient
 
 api_url = "https://domain-authority1.p.rapidapi.com/seo/get-domain-info"
 api_params = {
     'domain': 'learnwithhasan.com',
 }
 
 api_client = RapidAPIClient()  # API key read from environment variable
 response = api_client.call_api(api_url, method='GET', params=api_params)
 
 
 ```
 
-
 #### Prompt Template Builder
 
 ```python
 from SimplerLLM.prompts.prompt_builder import create_multi_value_prompts,create_prompt_template
 
 basic_prompt = "Generate 5 titles for a blog about {topic} and {style}"
 
@@ -143,36 +140,39 @@
 ## working with multiple value prompts
 multi_value_prompt_template = """Hello {name}, your next meeting is on {date}.
  and bring a {object} wit you"""
 
 params_list = [
      {"name": "Alice", "date": "January 10th", "object" : "dog"},
      {"name": "Bob", "date": "January 12th", "object" : "bag"},
-     {"name": "Charlie", "date": "January 15th", "object" : "pen"} 
+     {"name": "Charlie", "date": "January 15th", "object" : "pen"}
 ]
 
 
 multi_value_prompt = create_multi_value_prompts(multi_value_prompt_template)
 generated_prompts = multi_value_prompt.generate_prompts(params_list)
 
 print(generated_prompts[0])
 
 ```
 
-
 ## Chunking Functions
+
 We have introduced new functions to help you split texts into manageable chunks based on different criteria. These functions are part of the chunker tool.
 
 ### chunk_by_max_chunk_size
+
 This function splits text into chunks with a maximum size, optionally preserving sentence structure.
 
 ### chunk_by_sentences
+
 This function splits the text into chunks based on sentences.
 
 ### chunk_by_paragraphs
+
 This function splits text into chunks based on paragraphs.
 
 Example
 
 ```python
 from SimplerLLM.tools import text_chunker as chunker
 
@@ -183,17 +183,17 @@
 
 chunks = chunker.chunk_by_max_chunk_size(text, 100, True)
 
 
 
 ```
 
-
 ### Next Updates
+
 - Adding More Tools
 - Interacting With Local LLMs
 - Prompt Optimization
 - Response Evaluation
 - GPT Trainer
 - Document Chunker
 - Advanced Document Loader
-- Integration With More Providers 
+- Integration With More Providers
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM/image/img_helper_funcs.py` & `SimplerLLM-0.2.0/SimplerLLM/image/img_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/image/stability_ai.py` & `SimplerLLM-0.2.0/SimplerLLM/image/stability_ai.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/language/llm.py` & `SimplerLLM-0.2.0/SimplerLLM/language/embeddings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,336 +1,251 @@
-import SimplerLLM.language.llm_providers.openai_llm as openai_llm
-import SimplerLLM.language.llm_providers.gemini_llm as gemini_llm
-import SimplerLLM.language.llm_providers.anthropic_llm as anthropic_llm
-from enum import Enum
-
-
-class LLMProvider(Enum):
-    OPENAI = 1
-    GEMINI = 2
-    ANTHROPIC = 3
-
-
-class LLM:
-    def __init__(
-        self,
-        provider=LLMProvider.OPENAI,
-        model_name="gpt-3.5-turbo",
-        temperature=0.7,
-        top_p=1.0,
-    ):
-        self.provider = provider
-        self.model_name = model_name
-        self.temperature = temperature
-        self.top_p = top_p
-
-    @staticmethod
-    def create(
-        provider=None,
-        model_name=None,
-        temperature=0.7,
-        top_p=1.0,
-    ):
-        if provider == LLMProvider.OPENAI:
-            return OpenAILLM(provider, model_name, temperature, top_p)
-        if provider == LLMProvider.GEMINI:
-            return GeminiLLM(provider, model_name, temperature, top_p)
-        if provider == LLMProvider.ANTHROPIC:
-            return AnthropicLLM(provider, model_name, temperature, top_p)
-        else:
-            return None
-
-    def set_model(self, provider):
-        if not isinstance(provider, LLMProvider):
-            raise ValueError("Provider must be an instance of LLMProvider Enum")
-        self.provider = provider
-
-
-class OpenAILLM(LLM):
-    def __init__(self, model, model_name, temperature, top_p):
-        super().__init__(model, model_name, temperature, top_p)
-
-    def generate_text(
-        self,
-        user_prompt,
-        system_prompt="",
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=500,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return openai_llm.generate_text(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_text_async(
-        self,
-        user_prompt,
-        system_prompt="",
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=500,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await openai_llm.generate_text_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    def generate_full_response(
-        self,
-        user_prompt,
-        system_prompt="",
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=500,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return openai_llm.generate_full_response(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_full_response_async(
-        self,
-        user_prompt,
-        system_prompt="",
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=500,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await openai_llm.generate_full_response_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-
-class GeminiLLM(LLM):
-    def __init__(self, model, model_name, temperature, top_p):
-        super().__init__(model, model_name, temperature, top_p)
-
-    def generate_text(
-        self,
-        user_prompt,
-        system_prompt=None,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return gemini_llm.generate_text(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    def generate_full_response(
-        self,
-        user_prompt,
-        system_prompt,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return gemini_llm.generate_full_response(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_text_async(
-        self,
-        user_prompt,
-        system_prompt=None,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await gemini_llm.generate_text_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_full_response_async(
-        self,
-        user_prompt,
-        system_prompt,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await gemini_llm.generate_full_response_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-
-class AnthropicLLM(LLM):
-    def __init__(self, model, model_name, temperature, top_p):
-        super().__init__(model, model_name, temperature, top_p)
-
-    def generate_text(
-        self,
-        user_prompt,
-        system_prompt=None,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return anthropic_llm.generate_text(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    def generate_full_response(
-        self,
-        user_prompt,
-        system_prompt,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return anthropic_llm.generate_full_response(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_text_async(
-        self,
-        user_prompt,
-        system_prompt=None,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await anthropic_llm.generate_text_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
-
-    async def generate_full_response_async(
-        self,
-        user_prompt,
-        system_prompt,
-        model_name=None,
-        temperature=None,
-        top_p=None,
-        max_tokens=2024,
-    ):
-        # Use instance values as defaults if not provided
-        model_name = model_name if model_name is not None else self.model_name
-        temperature = temperature if temperature is not None else self.temperature
-        top_p = top_p if top_p is not None else self.top_p
-
-        return await anthropic_llm.generate_full_response_async(
-            user_prompt=user_prompt,
-            system_prompt=system_prompt,
-            model_name=model_name,
-            temperature=temperature,
-            top_p=top_p,
-            max_tokens=max_tokens,
-        )
+# import SimplerLLM.language.llm_providers.openai_llm as openai_llm
+# import SimplerLLM.language.llm_providers.gemini_llm as gemini_llm
+# import SimplerLLM.language.llm_providers.anthropic_llm as anthropic_llm
+# from enum import Enum
+
+
+# class EmbeddingsProvider(Enum):
+#     OPENAI = 1
+#     GEMINI = 2
+#     ANTHROPIC = 3
+
+
+# class LLM:
+#     def __init__(
+#         self, provider=EmbeddingsProvider.OPENAI, model_name="text-embedding-3-small"
+#     ):
+#         self.provider = provider
+#         self.model_name = model_name
+
+#     @staticmethod
+#     def create(
+#         provider=None,
+#         model_name=None,
+#     ):
+#         if provider == EmbeddingsProvider.OPENAI:
+#             return OpenAILLM(provider, model_name)
+#         if provider == EmbeddingsProvider.GEMINI:
+#             return GeminiLLM(provider, model_name)
+#         if provider == EmbeddingsProvider.ANTHROPIC:
+#             return AnthropicLLM(provider, model_name)
+#         else:
+#             return None
+
+#     def set_model(self, provider):
+#         if not isinstance(provider, EmbeddingsProvider):
+#             raise ValueError("Provider must be an instance of EmbeddingsProvider Enum")
+#         self.provider = provider
+
+
+# class OpenAILLM(LLM):
+#     def __init__(self, model, model_name):
+#         super().__init__(model, model_name)
+
+#     def generate_embeddings(
+#         self,
+#         user_input,
+#         model_name=None,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return openai_llm.generate_text(
+#             user_input=user_input,
+#             model_name=model_name,
+#         )
+
+
+# class GeminiLLM(LLM):
+#     def __init__(self, model, model_name, temperature, top_p):
+#         super().__init__(model, model_name, temperature, top_p)
+
+#     def generate_text(
+#         self,
+#         user_prompt,
+#         system_prompt=None,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return gemini_llm.generate_text(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     def generate_full_response(
+#         self,
+#         user_prompt,
+#         system_prompt,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return gemini_llm.generate_full_response(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     async def generate_text_async(
+#         self,
+#         user_prompt,
+#         system_prompt=None,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return await gemini_llm.generate_text_async(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     async def generate_full_response_async(
+#         self,
+#         user_prompt,
+#         system_prompt,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return await gemini_llm.generate_full_response_async(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+
+# class AnthropicLLM(LLM):
+#     def __init__(self, model, model_name, temperature, top_p):
+#         super().__init__(model, model_name, temperature, top_p)
+
+#     def generate_text(
+#         self,
+#         user_prompt,
+#         system_prompt=None,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return anthropic_llm.generate_text(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     def generate_full_response(
+#         self,
+#         user_prompt,
+#         system_prompt,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return anthropic_llm.generate_full_response(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     async def generate_text_async(
+#         self,
+#         user_prompt,
+#         system_prompt=None,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return await anthropic_llm.generate_text_async(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
+
+#     async def generate_full_response_async(
+#         self,
+#         user_prompt,
+#         system_prompt,
+#         model_name=None,
+#         temperature=None,
+#         top_p=None,
+#         max_tokens=2024,
+#     ):
+#         # Use instance values as defaults if not provided
+#         model_name = model_name if model_name is not None else self.model_name
+#         temperature = temperature if temperature is not None else self.temperature
+#         top_p = top_p if top_p is not None else self.top_p
+
+#         return await anthropic_llm.generate_full_response_async(
+#             user_prompt=user_prompt,
+#             system_prompt=system_prompt,
+#             model_name=model_name,
+#             temperature=temperature,
+#             top_p=top_p,
+#             max_tokens=max_tokens,
+#         )
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM/language/llm_addons.py` & `SimplerLLM-0.2.0/SimplerLLM/language/llm_addons.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/gemini_llm.py` & `SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/gemini_llm.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,368 +2,213 @@
 import os
 from dotenv import load_dotenv
 import aiohttp
 import asyncio
 import time
 import requests
 from .llm_response_models import LLMFullResponse
+from typing import Optional, Dict, List
 
 # Load environment variables
 load_dotenv()
 
 # Constants
 GEMINI_API_KEY = os.getenv("GEMINI_API_KEY", "")
 MAX_RETRIES = int(os.getenv("MAX_RETRIES", 3))
 RETRY_DELAY = int(os.getenv("RETRY_DELAY", 2))
 
 
-def __call_gemeni(
+def generate_response(
     model_name: str,
-    user_prompt: str,
-    system_prompt: str,
+    prompt: Optional[str] = None,
+    system_prompt: str = "You are a helpful AI Assistant",
+    messages: Optional[List[Dict]] = None,
     temperature: float = 0.7,
-    max_tokens: int = 2024,
-    top_p: float = 0.8,
+    max_tokens: int = 300,
+    top_p: float = 1.0,
+    full_response: bool = False,
 ) -> Optional[Dict]:
+    start_time = time.time()  # Record the start time
     """
-    Makes a POST request to the generativelanguage API to generate content based on the provided text
-    with specified generation configuration settings.
+    Sends a POST request to the generativelanguage API to generate content based on the provided text
+    or a list of messages with specified generation configuration settings.
 
     Parameters:
-    - model_name (str): The name of the model to use for generation.
-    - user_prompt (str): The text prompt for content generation.
-    - system_prompt (str): The system-generated text prompt.
-    - temperature (float): Controls randomness in generation. Higher values mean more random completions.
+    - model_name (str): The name of the model to use for content generation.
+    - prompt (Optional[str]): The single text prompt for content generation. Required if 'messages' is not provided.
+    - system_prompt (str): The default system-generated prompt used if 'prompt' is provided.
+    - messages (Optional[List[Dict]]): A structured list of message parts for complex conversations. Required if 'prompt' is not provided.
+    - temperature (float): Controls randomness in generation. Higher values result in more random completions.
     - max_tokens (int): The maximum number of tokens to generate.
     - top_p (float): Nucleus sampling parameter controlling the size of the probability mass to consider for token generation.
+    - full_response (bool): If True, returns the full response from the API instead of just the generated text.
 
     Returns:
-    - dict: The response from the API.
+    - Optional[Dict]: The generated text or full response depending on the 'full_response' flag.
     """
-    # Define the URL and headers
+
+    retry_attempts = 3
+    retry_delay = 1  # initial delay between retries in seconds
+
     url = f"https://generativelanguage.googleapis.com/v1beta/models/{model_name}:generateContent"
     headers = {"Content-Type": "application/json"}
 
-    # Create the data payload
+    if messages is None:
+        if prompt is None:
+            raise ValueError("Either 'prompt' or 'messages' must be provided.")
+        if system_prompt:
+            contents = [
+                {"role": "user", "parts": [{"text": system_prompt}]},
+                {"role": "model", "parts": [{"text": "ok"}]},
+                {"role": "user", "parts": [{"text": prompt}]},
+            ]
+        else:
+            contents = [{"role": "user", "parts": [{"text": prompt}]}]
+
+    else:
+        if prompt is not None:
+            raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
+        if system_prompt:
+            contents = [
+                {"role": "user", "parts": [{"text": system_prompt}]},
+                {"role": "model", "parts": [{"text": "ok"}]},
+            ]
+            contents.append(messages)
+        else:
+            contents = messages
+
     payload = {
-        "contents": [
-            {"role": "user", "parts": [{"text": system_prompt}]},
-            {"role": "model", "parts": [{"text": "ok"}]},
-            {"role": "user", "parts": [{"text": user_prompt}]},
-        ],
+        "contents": contents,
         "generationConfig": {
             "temperature": temperature,
             "maxOutputTokens": max_tokens,
             "topP": top_p,
         },
     }
 
-    try:
-        response = requests.post(
-            url, headers=headers, json=payload, params={"key": GEMINI_API_KEY}
-        )
-        response.raise_for_status()  # Raises an HTTPError if the HTTP request returned an unsuccessful status code
-        return response.json()
-    except requests.RequestException as e:
-        print(f"An error occurred: {e}")
-        return None
-
-
-def __generate_response(
-    model_name,
-    user_prompt,
-    system_prompt,
-    temperature,
-    max_tokens,
-    top_p,
-    full_response=False,
-):
-
-    start_time = time.time()  # Record the start time
-    """
-    Generates a response from the generative language model.
-
-    Parameters:
-    model_name (str): Name of the model to use for generation.
-    user_prompt (str): The text prompt for content generation.
-    system_prompt (str): The system-generated text prompt.
-    temperature (float): Controls randomness in generation.
-    max_tokens (int): Maximum number of tokens to generate.
-    top_p (float): Nucleus sampling parameter.
-    full_response (bool): If True, returns the full API response, else returns the generated text.
-
-    Returns:
-    str or dict: The generated text or the full response from the API, based on the 'full_response' flag.
-    """
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
-
-    if not system_prompt:
-        system_prompt = "You are a helpful AI Assitant"
-
-    if not model_name or not isinstance(model_name, str):
-        raise ValueError("model must be a non-empty string.")
-
-    for attempt in range(MAX_RETRIES):
+    for attempt in range(retry_attempts):
         try:
-            response = __call_gemeni(
-                model_name=model_name,
-                system_prompt=system_prompt,
-                user_prompt=user_prompt,
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=top_p,
+            response = requests.post(
+                url, headers=headers, json=payload, params={"key": GEMINI_API_KEY}
             )
+            response.raise_for_status()  # Raises HTTPError for bad requests (4XX or 5XX)
 
             if full_response:
-                end_time = time.time()  # Record the end time before returning
-                process_time = end_time - start_time
-
-                full_reponse = LLMFullResponse(
-                    generated_text=response["candidates"][0]["content"]["parts"][0][
-                        "text"
-                    ],
+                return LLMFullResponse(
+                    generated_text=response.json()["candidates"][0]["content"]["parts"][
+                        0
+                    ]["text"],
                     model=model_name,
-                    process_time=process_time,
-                    llm_provider_response=response,
+                    process_time=time.time() - start_time,
+                    llm_provider_response=response.json(),
                 )
 
-                return full_reponse
             else:
-                return response["candidates"][0]["content"]["parts"][0]["text"]
+                return response.json()["candidates"][0]["content"]["parts"][0]["text"]
 
-        except Exception as e:  # Consider catching more specific exceptions
-            if attempt < MAX_RETRIES - 1:
-                delay = RETRY_DELAY * 2**attempt
-                time.sleep(delay)
-            else:
-                end_time = time.time()  # Record the end time in case of failure
-                process_time = end_time - start_time
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts and {process_time} seconds due to: {e}"
-                )
-                return None
+        except requests.RequestException as e:
+            print(f"Attempt {attempt + 1} failed: {e}")
+            time.sleep(retry_delay)
+            retry_delay *= 2  # Double the delay each retry
 
+    print("All retry attempts failed.")
+    return None
 
-def generate_text(
-    model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> str:
-    """
-    Generates using Gemini and returns only the text.
-    """
-    return __generate_response(
-        model_name,
-        user_prompt,
-        system_prompt,
-        temperature,
-        max_tokens,
-        top_p,
-        full_response=False,
-    )
-
-
-def generate_full_response(
-    model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    max_tokens=2000,
-    top_p=1.0,
-    temperature=0.7,
-) -> LLMFullResponse:
-    """
-    Generates the full response from Gemini.
-    """
-    return __generate_response(
-        model_name,
-        user_prompt,
-        system_prompt,
-        temperature,
-        max_tokens,
-        top_p,
-        full_response=True,
-    )
-
-
-async def __call_gemeni_async(
-    model_name,
-    user_prompt,
-    system_prompt,
-    temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-):
+
+async def generate_response_async(
+    model_name: str,
+    prompt: Optional[str] = None,
+    system_prompt: str = "You are a helpful AI Assistant",
+    messages: Optional[List[Dict]] = None,
+    temperature: float = 0.7,
+    max_tokens: int = 300,
+    top_p: float = 1.0,
+    full_response: bool = False,
+) -> Optional[Dict]:
     """
-    Asynchronously makes a POST request to the generativelanguage API to generate content based on the provided text
-    with specified generation configuration settings.
+    Sends a POST request to the generativelanguage API to generate content based on the provided text
+    or a list of messages with specified generation configuration settings.
 
     Parameters:
-    user_prompt (str): The text prompt for content generation.
-    temperature (float): Controls randomness in generation. Higher values mean more random completions.
-    max_output_tokens (int): The maximum number of tokens to generate.
-    top_p (float): Nucleus sampling parameter controlling the size of the probability mass to consider for token generation.
-    top_k (int): Truncates the number of tokens considered based on their probability.
+    - model_name (str): The name of the model to use for content generation.
+    - prompt (Optional[str]): The single text prompt for content generation. Required if 'messages' is not provided.
+    - system_prompt (str): The default system-generated prompt used if 'prompt' is provided.
+    - messages (Optional[List[Dict]]): A structured list of message parts for complex conversations. Required if 'prompt' is not provided.
+    - temperature (float): Controls randomness in generation. Higher values result in more random completions.
+    - max_tokens (int): The maximum number of tokens to generate.
+    - top_p (float): Nucleus sampling parameter controlling the size of the probability mass to consider for token generation.
+    - full_response (bool): If True, returns the full response from the API instead of just the generated text.
 
     Returns:
-    dict: The response from the API.
+    - Optional[Dict]: The generated text or full response depending on the 'full_response' flag.
     """
+
+    start_time = time.time()  # Record the start time
+
+    retry_attempts = 3
+    retry_delay = 1  # initial delay between retries in seconds
+
     url = f"https://generativelanguage.googleapis.com/v1beta/models/{model_name}:generateContent"
     headers = {"Content-Type": "application/json"}
+
+    if messages is None:
+        if prompt is None:
+            raise ValueError("Either 'prompt' or 'messages' must be provided.")
+        if system_prompt:
+            contents = [
+                {"role": "user", "parts": [{"text": system_prompt}]},
+                {"role": "model", "parts": [{"text": "ok"}]},
+                {"role": "user", "parts": [{"text": prompt}]},
+            ]
+        else:
+            contents = [{"role": "user", "parts": [{"text": prompt}]}]
+
+    else:
+        if prompt is not None:
+            raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
+        if system_prompt:
+            contents = [
+                {"role": "user", "parts": [{"text": system_prompt}]},
+                {"role": "model", "parts": [{"text": "ok"}]},
+            ]
+            contents.append(messages)
+        else:
+            contents = messages
+
     payload = {
-        "contents": [
-            {
-                "role": "user",
-                "parts": [{"text": system_prompt}],
-            },
-            {
-                "role": "model",
-                "parts": [{"text": "ok"}],
-            },
-            {
-                "role": "user",
-                "parts": [{"text": user_prompt}],
-            },
-        ],
+        "contents": contents,
         "generationConfig": {
             "temperature": temperature,
             "maxOutputTokens": max_tokens,
             "topP": top_p,
         },
     }
 
     async with aiohttp.ClientSession() as session:
-        try:
-            async with session.post(
-                url, headers=headers, json=payload, params={"key": GEMINI_API_KEY}
-            ) as response:
-                response.raise_for_status()  # Raises an HTTPError if the HTTP request returned an unsuccessful status code
-                return await response.json()
-        except aiohttp.ClientError as e:
-            print(f"An error occurred: {e}")
-            return None
-
-
-async def __generate_response_async(
-    model_name,
-    user_prompt,
-    system_prompt,
-    temperature,
-    max_tokens,
-    top_p,
-    full_response=False,
-):
-    start_time = time.time()  # Record the start time before making the request
-
-    """
-    Generates a response from the generative language model.
-
-    Parameters:
-    model_name (str): Name of the model to use for generation.
-    user_prompt (str): The text prompt for content generation.
-    system_prompt (str): The system-generated text prompt.
-    temperature (float): Controls randomness in generation.
-    max_tokens (int): Maximum number of tokens to generate.
-    top_p (float): Nucleus sampling parameter.
-    full_response (bool): If True, returns the full API response, else returns the generated text.
-
-    Returns:
-    str or dict: The generated text or the full response from the API, based on the 'full_response' flag.
-    """
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
-
-    if not system_prompt:
-        system_prompt = "You are a helpful AI Assitant"
-
-    if not model_name or not isinstance(model_name, str):
-        raise ValueError("model must be a non-empty string.")
-
-    for attempt in range(MAX_RETRIES):
-        try:
-            response = await __call_gemeni_async(
-                model_name=model_name,
-                system_prompt=system_prompt,
-                user_prompt=user_prompt,
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=top_p,
-            )
-
-            if full_response:
-                end_time = time.time()  # Record the end time before returning
-                process_time = end_time - start_time
-
-                full_reponse = LLMFullResponse(
-                    generated_text=response["candidates"][0]["content"]["parts"][0][
-                        "text"
-                    ],
-                    model=model_name,
-                    process_time=process_time,
-                    llm_provider_response=response,
-                )
-
-                return full_reponse
-            else:
-                return response["candidates"][0]["content"]["parts"][0]["text"]
+        for attempt in range(retry_attempts):
+            try:
+                async with session.post(
+                    url, headers=headers, json=payload, params={"key": GEMINI_API_KEY}
+                ) as response:
+
+                    data = await response.json()
+
+                    if full_response:
+                        return LLMFullResponse(
+                            generated_text=data["candidates"][0]["content"]["parts"][0][
+                                "text"
+                            ],
+                            model=model_name,
+                            process_time=time.time() - start_time,
+                            llm_provider_response=data,
+                        )
+
+                    else:
+                        return data["candidates"][0]["content"]["parts"][0]["text"]
+
+            except aiohttp.ClientError as e:
+                print(f"Attempt {attempt + 1} failed: {e}")
+                await asyncio.sleep(retry_delay)
+                retry_delay *= 2  # Double the delay each retry
 
-        except Exception as e:  # Consider catching more specific exceptions
-            if attempt < MAX_RETRIES - 1:
-                await asyncio.sleep(RETRY_DELAY * (2**attempt))
-            else:
-                end_time = time.time()  # Record the end time in case of failure
-                process_time = end_time - start_time
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts and {process_time} seconds due to: {e}"
-                )
-                return None
-
-
-async def generate_text_async(
-    model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> str:
-    """
-    Generates using Gemini and returns only the text.
-    """
-    result = await __generate_response_async(
-        model_name,
-        user_prompt,
-        system_prompt,
-        temperature,
-        max_tokens,
-        top_p,
-        full_response=False,
-    )
-    return result
-
-
-async def generate_full_response_async(
-    model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    max_tokens=2000,
-    top_p=1.0,
-    temperature=0.7,
-) -> LLMFullResponse:
-    """
-    Generates the full response from Gemini.
-    """
-    result = await __generate_response_async(
-        model_name,
-        user_prompt,
-        system_prompt,
-        temperature,
-        max_tokens,
-        top_p,
-        full_response=True,
-    )
-    return result
+    print("All retry attempts failed.")
+    return None
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM/language/llm_providers/openai_llm.py` & `SimplerLLM-0.2.0/SimplerLLM/language/llm_providers/openai_llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,177 +22,178 @@
     openai_client = OpenAI(api_key=OPENAI_API_KEY)
     return async_openai_client, openai_client
 
 
 async_openai_client, openai_client = initialize_openai_clients()
 
 
-def generate_text(
+def generate_response(
     model_name,
-    user_prompt,
+    prompt=None,
+    messages=None,
     system_prompt="You are a helpful AI Assistant",
     temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> str:
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
+    max_tokens=300,
+    top_p=1.0,
+    full_response=False,
+):
+    start_time = time.time() if full_response else None
+
+    # Validate inputs
+    if prompt and messages:
+        raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
+    if not prompt and not messages:
+        raise ValueError("Either 'prompt' or 'messages' must be provided.")
+
+    # Prepare messages based on input type
+    if prompt:
+        messages = [
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": prompt},
+        ]
+
     for attempt in range(MAX_RETRIES):
         try:
             completion = openai_client.chat.completions.create(
                 model=model_name,
-                messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": user_prompt},
-                ],
+                messages=messages,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
             )
-            return [completion.choices[0].message.content][0]
+            generated_text = completion.choices[0].message.content
+
+            if full_response:
+                end_time = time.time()
+                process_time = end_time - start_time
+                return LLMFullResponse(
+                    generated_text=generated_text,
+                    model=model_name,
+                    process_time=process_time,
+                    llm_provider_response=completion,
+                )
+            return generated_text
 
-        except Exception as e:  # Consider catching more specific exceptions
+        except Exception as e:
             if attempt < MAX_RETRIES - 1:
                 time.sleep(RETRY_DELAY * (2**attempt))
             else:
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts due to: {e}"
-                )
+                error_msg = f"Failed after {MAX_RETRIES} attempts"
+                if full_response:
+                    end_time = time.time()
+                    process_time = end_time - start_time
+                    error_msg += f" and {process_time} seconds"
+                error_msg += f" due to: {e}"
+                print(error_msg)
                 return None
 
 
-async def generate_text_async(
+async def generate_response_async(
     model_name,
-    user_prompt,
+    prompt=None,
+    messages=None,
     system_prompt="You are a helpful AI Assistant",
     temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> str:
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
+    max_tokens=300,
+    top_p=1.0,
+    full_response=False,
+):
+    start_time = time.time() if full_response else None
+
+    # Validate inputs
+    if prompt and messages:
+        raise ValueError("Only one of 'prompt' or 'messages' should be provided.")
+    if not prompt and not messages:
+        raise ValueError("Either 'prompt' or 'messages' must be provided.")
+
+    # Prepare messages based on input type
+    if prompt:
+        messages = [
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": prompt},
+        ]
+
     for attempt in range(MAX_RETRIES):
         try:
             completion = await async_openai_client.chat.completions.create(
                 model=model_name,
-                messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": user_prompt},
-                ],
+                messages=messages,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
             )
-            return [completion.choices[0].message.content][0]
+            generated_text = completion.choices[0].message.content
 
-        except Exception as e:  # Consider catching more specific exceptions
+            if full_response:
+                end_time = time.time()
+                process_time = end_time - start_time
+                return LLMFullResponse(
+                    generated_text=generated_text,
+                    model=model_name,
+                    process_time=process_time,
+                    llm_provider_response=completion,
+                )
+            return generated_text
+
+        except Exception as e:
             if attempt < MAX_RETRIES - 1:
                 await asyncio.sleep(RETRY_DELAY * (2**attempt))
             else:
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts due to: {e}"
-                )
+                error_msg = f"Failed after {MAX_RETRIES} attempts"
+                if full_response:
+                    end_time = time.time()
+                    process_time = end_time - start_time
+                    error_msg += f" and {process_time} seconds"
+                error_msg += f" due to: {e}"
+                print(error_msg)
                 return None
 
 
-def generate_full_response(
+def generate_embeddings(
     model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> LLMFullResponse:
+    user_input=None,
+):
 
-    start_time = time.time()  # Record the start time
+    if not user_input:
+        raise ValueError("user_input must be provided.")
+
+    # Prepare messages based on input type
+    if prompt:
+        messages = [
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": prompt},
+        ]
 
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
     for attempt in range(MAX_RETRIES):
         try:
             completion = openai_client.chat.completions.create(
                 model=model_name,
-                messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": user_prompt},
-                ],
+                messages=messages,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
             )
+            generated_text = completion.choices[0].message.content
 
-            end_time = time.time()  # Record the end time before returning
-            process_time = end_time - start_time
-
-            full_reponse = LLMFullResponse(
-                generated_text=[completion.choices[0].message.content][0],
-                model=model_name,
-                process_time=process_time,
-                llm_provider_response=completion,
-            )
-
-            return full_reponse
-
-        except Exception as e:  # Consider catching more specific exceptions
-            if attempt < MAX_RETRIES - 1:
-                time.sleep(RETRY_DELAY * (2**attempt))
-            else:
-
-                end_time = time.time()  # Record the end time in case of failure
+            if full_response:
+                end_time = time.time()
                 process_time = end_time - start_time
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts and {process_time} seconds due to: {e}"
+                return LLMFullResponse(
+                    generated_text=generated_text,
+                    model=model_name,
+                    process_time=process_time,
+                    llm_provider_response=completion,
                 )
-                return None
+            return generated_text
 
-
-async def generate_full_response_async(
-    model_name,
-    user_prompt,
-    system_prompt="You are a helpful AI Assistant",
-    temperature=0.7,
-    max_tokens=2024,
-    top_p=0.8,
-) -> LLMFullResponse:
-    start_time = time.time()  # Record the start time
-
-    if not user_prompt or not isinstance(user_prompt, str):
-        raise ValueError("user_prompt must be a non-empty string.")
-    for attempt in range(MAX_RETRIES):
-        try:
-            completion = await async_openai_client.chat.completions.create(
-                model=model_name,
-                messages=[
-                    {"role": "system", "content": system_prompt},
-                    {"role": "user", "content": user_prompt},
-                ],
-                temperature=temperature,
-                max_tokens=max_tokens,
-                top_p=top_p,
-            )
-
-            end_time = time.time()  # Record the end time before returning
-            process_time = end_time - start_time
-
-            full_reponse = LLMFullResponse(
-                generated_text=[completion.choices[0].message.content][0],
-                model=model_name,
-                process_time=process_time,
-                llm_provider_response=completion,
-            )
-
-            return full_reponse
-
-        except Exception as e:  # Consider catching more specific exceptions
+        except Exception as e:
             if attempt < MAX_RETRIES - 1:
-                await asyncio.sleep(RETRY_DELAY * (2**attempt))
+                time.sleep(RETRY_DELAY * (2**attempt))
             else:
-                end_time = time.time()  # Record the end time in case of failure
-                process_time = end_time - start_time
-                # Log the error or inform the user
-                print(
-                    f"Failed to generate response after {MAX_RETRIES} attempts and {process_time} seconds due to: {e}"
-                )
+                error_msg = f"Failed after {MAX_RETRIES} attempts"
+                if full_response:
+                    end_time = time.time()
+                    process_time = end_time - start_time
+                    error_msg += f" and {process_time} seconds"
+                error_msg += f" due to: {e}"
+                print(error_msg)
                 return None
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM/prompts/prompt_builder.py` & `SimplerLLM-0.2.0/SimplerLLM/prompts/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/tools/file_loader.py` & `SimplerLLM-0.2.0/SimplerLLM/tools/file_loader.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/tools/generic_loader.py` & `SimplerLLM-0.2.0/SimplerLLM/tools/generic_loader.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/tools/json_helpers.py` & `SimplerLLM-0.2.0/SimplerLLM/tools/json_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,48 @@
         model_instance (YourModel): An instance of your Pydantic model.
 
     Returns:
         str: A JSON string representation of the model.
     """
     return model_instance.model_dump_json()
 
+
 def extract_json_from_text(text_response):
+    pattern = r"\{.*?\}"
+    matches = re.finditer(pattern, text_response, re.DOTALL)
+    json_objects = []
+
+    for match in matches:
+        json_str = __json_extend_search(text_response, match.span())
+        try:
+            json_obj = json.loads(json_str)
+            json_objects.append(json_obj)
+        except json.JSONDecodeError:
+            continue
+
+    return json_objects if json_objects else None
+
+
+def __json_extend_search(text, span):
+    start, end = span
+    nest_count = 1  # Starts with 1 since we know '{' is at the start position
+    for i in range(end, len(text)):
+        if text[i] == "{":
+            nest_count += 1
+        elif text[i] == "}":
+            nest_count -= 1
+            if nest_count == 0:
+                return text[start : i + 1]
+    return text[start:end]
+
+
+@DeprecationWarning
+def __extract_json_from_text_deprecated(text_response):
     # This pattern matches a string that starts with '{' and ends with '}'
-    pattern = r'\{[^{}]*\}'
+    pattern = r"\{[^{}]*\}"
 
     matches = re.finditer(pattern, text_response)
     json_objects = []
 
     for match in matches:
         json_str = match.group(0)
         try:
@@ -42,34 +73,37 @@
                 continue
 
     if json_objects:
         return json_objects
     else:
         return None  # Or handle this case as you prefer
 
-def extend_search(text, span):
+
+@DeprecationWarning
+def __extend_search_deprecated(text, span):
     # Extend the search to try to capture nested structures
     start, end = span
     nest_count = 0
     for i in range(start, len(text)):
-        if text[i] == '{':
+        if text[i] == "{":
             nest_count += 1
-        elif text[i] == '}':
+        elif text[i] == "}":
             nest_count -= 1
             if nest_count == 0:
-                return text[start:i+1]
+                return text[start : i + 1]
     return text[start:end]
 
+
 def validate_json_with_pydantic_model(model_class, json_data):
     """
     Validates JSON data against a specified Pydantic model.
 
     Args:
         model_class (BaseModel): The Pydantic model class to validate against.
-        json_data (dict or list): JSON data to validate. Can be a dict for a single JSON object, 
+        json_data (dict or list): JSON data to validate. Can be a dict for a single JSON object,
                                   or a list for multiple JSON objects.
 
     Returns:
         list: A list of validated JSON objects that match the Pydantic model.
         list: A list of errors for JSON objects that do not match the model.
     """
     validated_data = []
@@ -89,22 +123,24 @@
         except ValidationError as e:
             validation_errors.append({"error": str(e), "data": json_data})
     else:
         raise ValueError("Invalid JSON data type. Expected dict or list.")
 
     return validated_data, validation_errors
 
+
 def convert_json_to_pydantic_model(model_class, json_data):
     try:
         model_instance = model_class(**json_data)
         return model_instance
     except ValidationError as e:
         print("Validation error:", e)
         return None
 
+
 # Define a function to provide example values based on type
 def example_value_for_type(field_type: Type):
     if field_type == str:
         return "example_string"
     elif field_type == int:
         return 0
     elif field_type == float:
@@ -114,16 +150,16 @@
     elif field_type == List[str]:
         return ["generated text 1", "generated text 2"]
     elif field_type == List[int]:
         return [1, 2, 3]
     else:
         return "Unsupported type"
 
+
 # Function to generate a JSON example for any Pydantic model
 def generate_json_example_from_pydantic(model_class: Type[BaseModel]) -> str:
     example_data = {}
     for field_name, field_type in get_type_hints(model_class).items():
         example_data[field_name] = example_value_for_type(field_type)
-    
+
     model_instance = model_class(**example_data)
     return model_instance.json()
-
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM/tools/rapid_api.py` & `SimplerLLM-0.2.0/SimplerLLM/tools/rapid_api.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM/tools/serp.py` & `SimplerLLM-0.2.0/SimplerLLM/tools/serp.py`

 * *Files identical despite different names*

### Comparing `SimplerLLM-0.1.9/SimplerLLM.egg-info/PKG-INFO` & `SimplerLLM-0.2.0/SimplerLLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplerLLM
-Version: 0.1.9
+Version: 0.2.0
 Summary: An easy-to-use Library for interacting with language models.
 Home-page: https://github.com/hassancs91/SimplerLLM
 Author: Hasan Aboul Hasan
 Author-email: hasan@learnwithhasan.com
 Keywords: text generation,openai,LLM,RAG
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,121 +15,118 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-
 # ⚪ SimplerLLM (Beta)
 
 ⚡ Your Easy Pass to Advanced AI ⚡
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-
 ## 🤔 What is SimplerLLM?
 
 SimplerLLM is an open-source Python library designed to simplify interactions with Large Language Models (LLMs) for researchers and beginners. It offers a unified interface for different LLM providers and a suite of tools to enhance language model capabilities and make it Super easy for anyone to develop AI-powered tools and apps.
 
 ## Easy Installation
+
 With pip:
+
 ```bash
 pip install simplerllm
 ```
 
-
 ## Features
 
 - **Unified LLM Interface**: Define an LLM instance in one line for providers like OpenAI and Google Gemini. Future versions will support more APIs and LLM providers.
 - **Generic Text Loader**: Load text from various sources like DOCX, PDF, TXT files, YouTube scripts, or blog posts.
 - **RapidAPI Connector**: Connect with AI services on RapidAPI.
 - **SERP Integration**: Perform searches using DuckDuckGo, with more search engines coming soon.
 - **Prompt Template Builder**: Easily create and manage prompt templates.
-And Much More Coming Soon!
-
+  And Much More Coming Soon!
 
 ### Setting Up Environment Variables
-To use this library, you need to set several API keys in your environment. Start by creating a .env file in the root directory of your project and adding your API keys there. 
+
+To use this library, you need to set several API keys in your environment. Start by creating a .env file in the root directory of your project and adding your API keys there.
 
 🔴 This file should be kept private and not committed to version control to protect your keys.
 
 Here is an example of what your .env file should look like:
 
-``` 
+```
 OPENAI_API_KEY="your_openai_api_key_here"
 GEMENI_API_KEY="your_gemeni_api_key_here"
 CLAUDE_API_KEY="your_claude_api_key_here"
 RAPIDAPI_API_KEY="your_rapidapi_key_here" # for accessing APIs on RapidAPI
 VALUE_SERP_API_KEY="your_value_serp_api_key_here" #for Google search
 SERPER_API_KEY="your_serper_api_key_here" #for Google search
 STABILITY_API_KEY="your_stability_api_key_here" #for image generation
 
 ```
 
-
-
-
 ### Creating an LLM Instance
 
 ```python
 from SimplerLLM.language.llm import LLM, LLMProvider
 
 # For OpenAI
-llm_instance = LLM.create(provider=LLMProvider.OPENAI)
+llm_instance = LLM.create(provider=LLMProvider.OPENAI, model_name="gpt-3.5-turbo")
 
 # For Google Gemini
 #llm_instance = LLM.create(provider=LLMProvider.GEMINI,model_name="gemini-pro")
 
 # For Anthropic Claude 
 #llm_instance = LLM.create(LLMProvider.ANTHROPIC, model_name="claude-3-opus-20240229")
 
-
-response = llm_instance.generate_text(user_prompt="generate a 5 words sentence")
+response = llm_instance.generate_response(prompt="generate a 5 words sentence")
 
 ```
 
 ### Using Tools
 
 #### SERP
+
 ```python
 from SimplerLLM.tools.serp import search_with_serper_api
 
 search_results = search_with_serper_api("your search query", num_results=3)
 
 # use the search results the way you want!
 
 ```
 
 #### Generic Text Loader
+
 ```python
 from SimplerLLM.tools.generic_loader import load_content
 
 text_file = load_content("file.txt")
 
 print(text_file.content)
 
 ```
 
 #### Calling any RapidAPI API
+
 ```python
 from  SimplerLLM.tools.rapid_api import RapidAPIClient
 
 api_url = "https://domain-authority1.p.rapidapi.com/seo/get-domain-info"
 api_params = {
     'domain': 'learnwithhasan.com',
 }
 
 api_client = RapidAPIClient()  # API key read from environment variable
 response = api_client.call_api(api_url, method='GET', params=api_params)
 
 
 ```
 
-
 #### Prompt Template Builder
 
 ```python
 from SimplerLLM.prompts.prompt_builder import create_multi_value_prompts,create_prompt_template
 
 basic_prompt = "Generate 5 titles for a blog about {topic} and {style}"
 
@@ -143,36 +140,39 @@
 ## working with multiple value prompts
 multi_value_prompt_template = """Hello {name}, your next meeting is on {date}.
  and bring a {object} wit you"""
 
 params_list = [
      {"name": "Alice", "date": "January 10th", "object" : "dog"},
      {"name": "Bob", "date": "January 12th", "object" : "bag"},
-     {"name": "Charlie", "date": "January 15th", "object" : "pen"} 
+     {"name": "Charlie", "date": "January 15th", "object" : "pen"}
 ]
 
 
 multi_value_prompt = create_multi_value_prompts(multi_value_prompt_template)
 generated_prompts = multi_value_prompt.generate_prompts(params_list)
 
 print(generated_prompts[0])
 
 ```
 
-
 ## Chunking Functions
+
 We have introduced new functions to help you split texts into manageable chunks based on different criteria. These functions are part of the chunker tool.
 
 ### chunk_by_max_chunk_size
+
 This function splits text into chunks with a maximum size, optionally preserving sentence structure.
 
 ### chunk_by_sentences
+
 This function splits the text into chunks based on sentences.
 
 ### chunk_by_paragraphs
+
 This function splits text into chunks based on paragraphs.
 
 Example
 
 ```python
 from SimplerLLM.tools import text_chunker as chunker
 
@@ -183,17 +183,17 @@
 
 chunks = chunker.chunk_by_max_chunk_size(text, 100, True)
 
 
 
 ```
 
-
 ### Next Updates
+
 - Adding More Tools
 - Interacting With Local LLMs
 - Prompt Optimization
 - Response Evaluation
 - GPT Trainer
 - Document Chunker
 - Advanced Document Loader
-- Integration With More Providers 
+- Integration With More Providers
```

### Comparing `SimplerLLM-0.1.9/SimplerLLM.egg-info/SOURCES.txt` & `SimplerLLM-0.2.0/SimplerLLM.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 SimplerLLM.egg-info/dependency_links.txt
 SimplerLLM.egg-info/requires.txt
 SimplerLLM.egg-info/top_level.txt
 SimplerLLM/image/__init__.py
 SimplerLLM/image/img_helper_funcs.py
 SimplerLLM/image/stability_ai.py
 SimplerLLM/language/__init__.py
+SimplerLLM/language/embeddings.py
 SimplerLLM/language/llm.py
 SimplerLLM/language/llm_addons.py
 SimplerLLM/language/llm_providers/__init__.py
 SimplerLLM/language/llm_providers/anthropic_llm.py
 SimplerLLM/language/llm_providers/gemini_llm.py
 SimplerLLM/language/llm_providers/llm_response_models.py
 SimplerLLM/language/llm_providers/openai_llm.py
```

### Comparing `SimplerLLM-0.1.9/setup.py` & `SimplerLLM-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the long description from the README file
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SimplerLLM",
-    version="0.1.9",
+    version="0.2.0",
     author="Hasan Aboul Hasan",
     author_email="hasan@learnwithhasan.com",
     description="An easy-to-use Library for interacting with language models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hassancs91/SimplerLLM",
     packages=find_packages(),
```

