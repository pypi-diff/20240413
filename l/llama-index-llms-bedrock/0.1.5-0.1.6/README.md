# Comparing `tmp/llama_index_llms_bedrock-0.1.5.tar.gz` & `tmp/llama_index_llms_bedrock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_bedrock-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_bedrock-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_bedrock-0.1.5.tar` & `llama_index_llms_bedrock-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       39 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/README.md
--rw-r--r--   0        0        0      216 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/__init__.py
--rw-r--r--   0        0        0    11323 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/base.py
--rw-r--r--   0        0        0     2248 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/llama_utils.py
--rw-r--r--   0        0        0     8224 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/utils.py
--rw-r--r--   0        0        0     1482 2024-03-19 15:27:11.985205 llama_index_llms_bedrock-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 llama_index_llms_bedrock-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/README.md
+-rw-r--r--   0        0        0      216 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/__init__.py
+-rw-r--r--   0        0        0    11896 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/base.py
+-rw-r--r--   0        0        0     2248 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/llama_utils.py
+-rw-r--r--   0        0        0     8309 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/utils.py
+-rw-r--r--   0        0        0     1482 2024-04-13 04:32:09.066916 llama_index_llms_bedrock-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 llama_index_llms_bedrock-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/base.py` & `llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,35 @@
     Provider,
     completion_with_retry,
     get_provider,
 )
 
 
 class Bedrock(LLM):
+    """Bedrock LLM.
+
+    Examples:
+        `pip install llama-index-llms-bedrock`
+
+        ```python
+        from llama_index.llms.bedrock import Bedrock
+
+        llm = Bedrock(
+            model="amazon.titan-text-express-v1",
+            aws_access_key_id="AWS Access Key ID to use",
+            aws_secret_access_key="AWS Secret Access Key to use",
+            aws_session_token="AWS Session Token to use",
+            aws_region_name="AWS Region to use, eg. us-east-1",
+        )
+
+        resp = llm.complete("Paul Graham is ")
+        print(resp)
+        ```
+    """
+
     model: str = Field(description="The modelId of the Bedrock model to use.")
     temperature: float = Field(description="The temperature to use for sampling.")
     max_tokens: int = Field(description="The maximum number of tokens to generate.")
     context_size: int = Field("The maximum number of tokens available for input.")
     profile_name: Optional[str] = Field(
         description="The name of aws profile to use. If not given, then the default profile is used."
     )
```

### Comparing `llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/llama_utils.py` & `llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/llama_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_bedrock-0.1.5/llama_index/llms/bedrock/utils.py` & `llama_index_llms_bedrock-0.1.6/llama_index/llms/bedrock/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "anthropic.claude-v2:1": 200000,
     "anthropic.claude-3-sonnet-20240229-v1:0": 200000,
     "anthropic.claude-3-haiku-20240307-v1:0": 200000,
     "meta.llama2-13b-chat-v1": 2048,
     "meta.llama2-70b-chat-v1": 4096,
     "mistral.mistral-7b-instruct-v0:2": 32000,
     "mistral.mixtral-8x7b-instruct-v0:1": 32000,
+    "mistral.mistral-large-2402-v1:0": 32000,
 }
 BEDROCK_FOUNDATION_LLMS = {**COMPLETION_MODELS, **CHAT_ONLY_MODELS}
 
 # Only the following models support streaming as
 # per result of Bedrock.Client.list_foundation_models
 # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_foundation_models.html
 STREAMING_MODELS = {
@@ -64,14 +65,15 @@
     "anthropic.claude-v2",
     "anthropic.claude-v2:1",
     "anthropic.claude-3-sonnet-20240229-v1:0",
     "anthropic.claude-3-haiku-20240307-v1:0",
     "meta.llama2-13b-chat-v1",
     "mistral.mistral-7b-instruct-v0:2",
     "mistral.mixtral-8x7b-instruct-v0:1",
+    "mistral.mistral-large-2402-v1:0",
 }
 
 
 class Provider(ABC):
     @property
     @abstractmethod
     def max_tokens_key(self) -> str:
```

### Comparing `llama_index_llms_bedrock-0.1.5/pyproject.toml` & `llama_index_llms_bedrock-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms bedrock integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-bedrock"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-anthropic = "^0.1.7"
 boto3 = "^1.34.26"
```

### Comparing `llama_index_llms_bedrock-0.1.5/PKG-INFO` & `llama_index_llms_bedrock-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-bedrock
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms bedrock integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

