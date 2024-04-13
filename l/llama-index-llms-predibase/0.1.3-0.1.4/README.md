# Comparing `tmp/llama_index_llms_predibase-0.1.3.tar.gz` & `tmp/llama_index_llms_predibase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_predibase-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_predibase-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_predibase-0.1.3.tar` & `llama_index_llms_predibase-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/README.md
--rw-r--r--   0        0        0       85 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/llama_index/llms/predibase/__init__.py
--rw-r--r--   0        0        0     6739 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/llama_index/llms/predibase/base.py
--rw-r--r--   0        0        0     1436 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 llama_index_llms_predibase-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-13 04:04:38.487162 llama_index_llms_predibase-0.1.4/README.md
+-rw-r--r--   0        0        0       85 2024-04-13 04:04:38.487162 llama_index_llms_predibase-0.1.4/llama_index/llms/predibase/__init__.py
+-rw-r--r--   0        0        0     7912 2024-04-13 04:04:38.487162 llama_index_llms_predibase-0.1.4/llama_index/llms/predibase/base.py
+-rw-r--r--   0        0        0     1436 2024-04-13 04:04:38.487162 llama_index_llms_predibase-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 llama_index_llms_predibase-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_predibase-0.1.3/llama_index/llms/predibase/base.py` & `llama_index_llms_predibase-0.1.4/llama_index/llms/predibase/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,44 +25,51 @@
 
     To use, you should have the ``predibase`` python package installed,
     and have your Predibase API key.
 
     The `model_name` parameter is the Predibase "serverless" base_model ID
     (see https://docs.predibase.com/user-guide/inference/models for the catalog).
 
-    An optional `adapter_id` parameter is the HuggingFace ID of a fine-tuned LLM
-    adapter, whose base model is the `model` parameter; the fine-tuned adapter
-    must be compatible with its base model; otherwise, an error is raised.
+    An optional `adapter_id` parameter is the Predibase ID or the HuggingFace ID
+    of a fine-tuned LLM adapter, whose base model is the `model` parameter; the
+    fine-tuned adapter must be compatible with its base model; otherwise, an
+    error is raised.  If the fine-tuned adapter is hosted at Predibase,
+    `adapter_version` can be specified (omitting it gives the latest version).
 
     Examples:
         `pip install llama-index-llms-predibase`
 
         ```python
         import os
 
         os.environ["PREDIBASE_API_TOKEN"] = "{PREDIBASE_API_TOKEN}"
 
         from llama_index.llms.predibase import PredibaseLLM
 
         llm = PredibaseLLM(
             model_name="mistral-7b",
-            adapter_id="my-repo/my-adapter",  # optional parameter
+            adapter_id="my-adapter-id",  # optional parameter
+            adapter_version=3,  # optional parameter (applies to Predibase only)
             temperature=0.3,
             max_new_tokens=512,
         )
         response = llm.complete("Hello World!")
         print(str(response))
         ```
     """
 
     model_name: str = Field(description="The Predibase base model to use.")
     predibase_api_key: str = Field(description="The Predibase API key to use.")
     adapter_id: str = Field(
         default=None,
-        description="The optional HuggingFace ID of a fine-tuned adapter to use.",
+        description="The optional Predibase ID or HuggingFace ID of a fine-tuned adapter to use.",
+    )
+    adapter_version: str = Field(
+        default=None,
+        description="The optional version number of fine-tuned adapter use (applies to Predibase only).",
     )
     max_new_tokens: int = Field(
         default=DEFAULT_NUM_OUTPUTS,
         description="The number of tokens to generate.",
         gt=0,
     )
     temperature: float = Field(
@@ -80,14 +87,15 @@
     _client: Any = PrivateAttr()
 
     def __init__(
         self,
         model_name: str,
         predibase_api_key: Optional[str] = None,
         adapter_id: Optional[str] = None,
+        adapter_version: Optional[int] = None,
         max_new_tokens: int = DEFAULT_NUM_OUTPUTS,
         temperature: float = DEFAULT_TEMPERATURE,
         context_window: int = DEFAULT_CONTEXT_WINDOW,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
@@ -100,14 +108,15 @@
             else os.environ.get("PREDIBASE_API_TOKEN")
         )
         assert predibase_api_key is not None
 
         super().__init__(
             model_name=model_name,
             adapter_id=adapter_id,
+            adapter_version=adapter_version,
             predibase_api_key=predibase_api_key,
             max_new_tokens=max_new_tokens,
             temperature=temperature,
             context_window=context_window,
             callback_manager=callback_manager,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
@@ -152,19 +161,21 @@
             model_name=self.model_name,
         )
 
     @llm_completion_callback()
     def complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> "CompletionResponse":
+        from predibase.pql.api import ServerResponseError
         from predibase.resource.llm.interface import (
             HuggingFaceLLM,
             LLMDeployment,
         )
         from predibase.resource.llm.response import GeneratedResponse
+        from predibase.resource.model import Model
 
         base_llm_deployment: LLMDeployment = self._client.LLM(
             uri=f"pb://deployments/{self.model_name}"
         )
 
         options: Dict[str, Union[str, float]] = copy.deepcopy(kwargs)
         options.update(
@@ -172,17 +183,28 @@
                 "max_new_tokens": self.max_new_tokens,
                 "temperature": self.temperature,
             }
         )
 
         result: GeneratedResponse
         if self.adapter_id:
-            adapter_model: HuggingFaceLLM = self._client.LLM(
-                uri=f"hf://{self.adapter_id}"
-            )
+            """
+            Attempt to retrieve the fine-tuned adapter from a Predibase repository.
+            If absent, then load the fine-tuned adapter from a HuggingFace repository.
+            """
+            adapter_model: Union[Model, HuggingFaceLLM]
+            try:
+                adapter_model = self._client.get_model(
+                    name=self.adapter_id,
+                    version=self.adapter_version,
+                    model_id=None,
+                )
+            except ServerResponseError:
+                # Predibase does not recognize the adapter ID (query HuggingFace).
+                adapter_model = self._client.LLM(uri=f"hf://{self.adapter_id}")
             result = base_llm_deployment.with_adapter(model=adapter_model).generate(
                 prompt=prompt,
                 options=options,
             )
         else:
             result = base_llm_deployment.generate(
                 prompt=prompt,
```

### Comparing `llama_index_llms_predibase-0.1.3/pyproject.toml` & `llama_index_llms_predibase-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms predibase integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-predibase"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_predibase-0.1.3/PKG-INFO` & `llama_index_llms_predibase-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-predibase
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms predibase integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

