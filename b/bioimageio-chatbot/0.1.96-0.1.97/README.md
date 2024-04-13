# Comparing `tmp/bioimageio-chatbot-0.1.96.tar.gz` & `tmp/bioimageio-chatbot-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.96.tar", last modified: Sat Apr 13 01:36:59 2024, max compression
+gzip compressed data, was "bioimageio-chatbot-0.1.97.tar", last modified: Sat Apr 13 02:03:51 2024, max compression
```

## Comparing `bioimageio-chatbot-0.1.96.tar` & `bioimageio-chatbot-0.1.97.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.981820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19758 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/hpa_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/vision_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 01:36:59.000000 bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:36:59.985820 bioimageio-chatbot-0.1.96/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 01:36:47.000000 bioimageio-chatbot-0.1.96/tests/test_knowledge_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.502390 bioimageio-chatbot-0.1.97/bioimageio_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19627 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.502390 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/bia_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/biii_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/docs_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/hpa_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/vision_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/gpts_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/jsonschema_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-13 02:03:38.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16067 2024-04-13 02:03:51.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 02:03:51.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 02:03:51.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 02:03:51.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 02:03:51.000000 bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-13 02:03:39.000000 bioimageio-chatbot-0.1.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:03:51.506390 bioimageio-chatbot-0.1.97/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-13 02:03:39.000000 bioimageio-chatbot-0.1.97/tests/test_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-13 02:03:39.000000 bioimageio-chatbot-0.1.97/tests/test_chatbot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-13 02:03:39.000000 bioimageio-chatbot-0.1.97/tests/test_eval_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 02:03:39.000000 bioimageio-chatbot-0.1.97/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.96/LICENSE` & `bioimageio-chatbot-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/PKG-INFO` & `bioimageio-chatbot-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.96
+Version: 0.1.97
 Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.96 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.97 Summary: Your
 Personal Assistant in Computational BioImaging. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.96/README.md` & `bioimageio-chatbot-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/__main__.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 def create_assistants(builtin_extensions):
     # debug = os.environ.get("BIOIMAGEIO_DEBUG") == "true"
 
     async def respond_to_user(
         question_with_history: QuestionWithHistory = None, role: Role = None
     ) -> RichResponse:
-        """Answer the user's question directly or retrieve relevant documents from the documentation, or create a Python Script to get information about details of models."""
+        """Response to the user's query."""
         steps = []
         inputs = (
             [question_with_history.user_profile]
             + list(question_with_history.chat_history)
             + [question_with_history.question]
         )
         assert question_with_history.chatbot_extensions is not None
```

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/__init__.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/bia_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/bia_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     async def search_bioimage_archive(self, 
         query: str = Field(..., description="The search query string."),
         pageSize: int = Field(10, gt=0, description="Number of search results per page."),
         page: int = Field(1, description="Page number of the search results."),
         sortOrder: Optional[str] = Field("descending", description="Sort order: ascending or descending.")
     ) -> Dict[str, Any]:
-        """Search the BioImage Archive for studies, returning simplified search results.  The link format to each study in the results is: https://www.ebi.ac.uk/biostudies/bioimages/studies/{accession}."""
+        """Search the BioImage Archive for studies and image datasets, returning a list of studies.  The link format to each study in the results is: https://www.ebi.ac.uk/biostudies/bioimages/studies/{accession}."""
         url = f"{self._base_url}/bioimages/search"
         params = {
             "query": query,
             "pageSize": pageSize,
             "page": page,
             "sortOrder": sortOrder
         }
@@ -88,15 +88,15 @@
             "search": search_tool.input_model.schema(),
             "read": read_tool.input_model.schema(),
         }
 
     return ChatbotExtension(
         id="bioimage_archive",
         name="Search BioImage Archive",
-        description="A service to search and read studies from the BioImage Archive.",
+        description="Search for biological images related studies in the BioImage Archive, it provide studies and image datasets related to microscopy images and other imaging modalities.",
         get_schema=get_schema, # This is optional, exists only for testing purposes
         tools=dict(
             search=search_tool,
             read=read_tool
         )
     )
```

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/biii_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/biii_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/docs_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/docs_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/hpa_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/hpa_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/vision_extension.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/vision_extension.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/evaluation.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/evaluation.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/gpts_action.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/gpts_action.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/jsonschema_pydantic.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/jsonschema_pydantic.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/knowledge_base.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot/utils.py` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/PKG-INFO` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio-chatbot
-Version: 0.1.96
+Version: 0.1.97
 Summary: Your Personal Assistant in Computational BioImaging.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-agents>=0.1.49
 Requires-Dist: imjoy-rpc>=0.5.48.post2
 Requires-Dist: requests
 Requires-Dist: pypdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.96 Summary: Your
+Metadata-Version: 2.1 Name: bioimageio-chatbot Version: 0.1.97 Summary: Your
 Personal Assistant in Computational BioImaging. Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: schema-agents>=0.1.49 Requires-
 Dist: imjoy-rpc>=0.5.48.post2 Requires-Dist: requests Requires-Dist: pypdf
 Requires-Dist: pillow Requires-Dist: matplotlib Requires-Dist: hypha>=0.15.50
 Requires-Dist: tqdm Requires-Dist: aiofiles Requires-Dist: langchain>=0.1.6
 Requires-Dist: beautifulsoup4 Requires-Dist: pandas Requires-Dist: duckduckgo-
 search>=5.1.0 Requires-Dist: rank-bm25 Requires-Dist: langchain-openai
```

### Comparing `bioimageio-chatbot-0.1.96/bioimageio_chatbot.egg-info/SOURCES.txt` & `bioimageio-chatbot-0.1.97/bioimageio_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/pyproject.toml` & `bioimageio-chatbot-0.1.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bioimageio-chatbot"
-version = "0.1.96"
+version = "0.1.97"
 readme = "README.md"
 description = "Your Personal Assistant in Computational BioImaging."
 dependencies = [
   "schema-agents>=0.1.49",
   "imjoy-rpc>=0.5.48.post2",
   "requests",
   "pypdf",
```

### Comparing `bioimageio-chatbot-0.1.96/tests/test_chatbot.py` & `bioimageio-chatbot-0.1.97/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/tests/test_chatbot_answer.py` & `bioimageio-chatbot-0.1.97/tests/test_chatbot_answer.py`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.96/tests/test_eval_agent.py` & `bioimageio-chatbot-0.1.97/tests/test_eval_agent.py`

 * *Files identical despite different names*

