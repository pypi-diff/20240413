# Comparing `tmp/athina_logger-1.2.0.tar.gz` & `tmp/athina_logger-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina_logger-1.2.0.tar", max compression
+gzip compressed data, was "athina_logger-1.2.1.tar", max compression
```

## Comparing `athina_logger-1.2.0.tar` & `athina_logger-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.0/athina_logger/__init__.py
--rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.0/athina_logger/api_key.py
--rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.0/athina_logger/athina_meta.py
--rw-r--r--   0        0        0      346 2024-04-06 02:20:32.526115 athina_logger-1.2.0/athina_logger/constants.py
--rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.0/athina_logger/exception/custom_exception.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.0/athina_logger/feedback/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.0/athina_logger/feedback/user_feedback.py
--rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.0/athina_logger/inference_logger.py
--rw-r--r--   0        0        0    14226 2024-04-02 05:37:10.002663 athina_logger-1.2.0/athina_logger/langchain_handler.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.0/athina_logger/log_stream_inference/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.0/athina_logger/log_stream_inference/log_stream_inference.py
--rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py
--rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.0/athina_logger/log_stream_inference/openai_completion_stream.py
--rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.0/athina_logger/openai_wrapper.py
--rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.0/athina_logger/request_helper.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.0/athina_logger/tracing/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.0/athina_logger/tracing/callback/__init__.py
--rw-r--r--   0        0        0    20259 2024-03-31 23:08:32.644755 athina_logger-1.2.0/athina_logger/tracing/callback/langchain.py
--rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.0/athina_logger/tracing/models.py
--rw-r--r--   0        0        0    14103 2024-04-06 02:19:19.300937 athina_logger-1.2.0/athina_logger/tracing/span.py
--rw-r--r--   0        0        0     6864 2024-04-06 02:19:19.301218 athina_logger-1.2.0/athina_logger/tracing/trace.py
--rw-r--r--   0        0        0      260 2024-03-31 22:30:00.379971 athina_logger-1.2.0/athina_logger/tracing/util.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.0/athina_logger/util/__init__.py
--rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.0/athina_logger/util/extract_model.py
--rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.0/athina_logger/util/token_count_helper.py
--rw-r--r--   0        0        0      465 2024-04-06 02:19:46.556941 athina_logger-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.1/athina_logger/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.1/athina_logger/api_key.py
+-rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.1/athina_logger/athina_meta.py
+-rw-r--r--   0        0        0      346 2024-04-11 21:50:15.997677 athina_logger-1.2.1/athina_logger/constants.py
+-rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.1/athina_logger/exception/custom_exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.1/athina_logger/feedback/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.1/athina_logger/feedback/user_feedback.py
+-rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.1/athina_logger/inference_logger.py
+-rw-r--r--   0        0        0    14226 2024-04-02 05:37:10.002663 athina_logger-1.2.1/athina_logger/langchain_handler.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.1/athina_logger/log_stream_inference/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.1/athina_logger/log_stream_inference/log_stream_inference.py
+-rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.1/athina_logger/log_stream_inference/openai_chat_completion_stream.py
+-rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.1/athina_logger/log_stream_inference/openai_completion_stream.py
+-rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.1/athina_logger/openai_wrapper.py
+-rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.1/athina_logger/request_helper.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.1/athina_logger/tracing/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.1/athina_logger/tracing/callback/__init__.py
+-rw-r--r--   0        0        0    19798 2024-04-13 02:48:04.524470 athina_logger-1.2.1/athina_logger/tracing/callback/langchain.py
+-rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.1/athina_logger/tracing/models.py
+-rw-r--r--   0        0        0    14103 2024-04-06 02:19:19.300937 athina_logger-1.2.1/athina_logger/tracing/span.py
+-rw-r--r--   0        0        0     6864 2024-04-06 02:19:19.301218 athina_logger-1.2.1/athina_logger/tracing/trace.py
+-rw-r--r--   0        0        0      260 2024-03-31 22:30:00.379971 athina_logger-1.2.1/athina_logger/tracing/util.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.1/athina_logger/util/__init__.py
+-rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.1/athina_logger/util/extract_model.py
+-rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.1/athina_logger/util/token_count_helper.py
+-rw-r--r--   0        0        0      465 2024-04-13 02:48:04.524967 athina_logger-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.1/PKG-INFO
```

### Comparing `athina_logger-1.2.0/README.md` & `athina_logger-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/athina_meta.py` & `athina_logger-1.2.1/athina_logger/athina_meta.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/feedback/user_feedback.py` & `athina_logger-1.2.1/athina_logger/feedback/user_feedback.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/inference_logger.py` & `athina_logger-1.2.1/athina_logger/inference_logger.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/langchain_handler.py` & `athina_logger-1.2.1/athina_logger/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/log_stream_inference/log_stream_inference.py` & `athina_logger-1.2.1/athina_logger/log_stream_inference/log_stream_inference.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py` & `athina_logger-1.2.1/athina_logger/log_stream_inference/openai_chat_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/log_stream_inference/openai_completion_stream.py` & `athina_logger-1.2.1/athina_logger/log_stream_inference/openai_completion_stream.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/openai_wrapper.py` & `athina_logger-1.2.1/athina_logger/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/request_helper.py` & `athina_logger-1.2.1/athina_logger/request_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/tracing/callback/langchain.py` & `athina_logger-1.2.1/athina_logger/tracing/callback/langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,31 +16,32 @@
     ChatMessage,
     HumanMessage,
     SystemMessage,
     ToolMessage,
     FunctionMessage,
 )
 from athina_logger.tracing.trace import Trace
+from athina_logger.util.extract_model import _extract_model_name
 
 class LangchainCallbackHandler(
     BaseCallbackHandler, AthinaApiKey
 ):
     next_span_id: Optional[str] = None
 
     def __init__(
         self,
         trace_name: Optional[str] = None,
         version: Optional[str] = None,
     ) -> None: 
         _debug("LangchainCallbackHandler.__init__")
         self.version = version
         self.trace_name = trace_name
+        self.trace_run_id = None
         self.runs = {}
-        self.trace = None 
-        self.root_span = None
+        self.trace: Trace = None 
 
     def setNextSpan(self, id: str):
         self.next_span_id = id
 
     def on_llm_new_token(
         self,
         token: str,
@@ -94,18 +95,16 @@
             tags=tags,
             metadata=metadata,
             version=self.version,
             **kwargs,
         )
         name = self._get_athina_run_name(serialized, **kwargs) 
         if parent_run_id is None:
-            if self.root_span is None:
-                self.runs[run_id] = self.trace.create_span(name=name, input=inputs, version=self.version)
-            else:
-                self.runs[run_id] = self.root_span.create_span(name=name, input=inputs, version=self.version)
+            self.runs[run_id] = self.trace.create_span(name=name, input=inputs, version=self.version)
+
         if parent_run_id is not None:
             self.runs[run_id] = self.runs[parent_run_id].create_span(name=name, input=inputs, version=self.version) 
 
     def on_chain_end(
         self,
         outputs: Dict[str, Any],
         *,
@@ -117,15 +116,16 @@
             _debug(
                 f"on chain end: run_id: {run_id} parent_run_id: {parent_run_id}"
             )
             if run_id not in self.runs:
                 raise Exception("run not found")
             self._update_run(run_id, outputs, None)
             self.runs[run_id].end()
-            self.trace.end()
+            if self.trace_run_id == run_id:
+                self.trace.end()
         except Exception as e:
             _debug(e)
 
     def on_chain_error(
         self,
         error: Union[Exception, KeyboardInterrupt],
         *,
@@ -368,15 +368,15 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         try:
-            self.log.info(
+            _debug(
                 f"on llm start: run_id: {run_id} parent_run_id: {parent_run_id}"
             )
             _debug("metadata:")
             _debug(metadata)
             self._on_llm_action(
                 serialized,
                 run_id,
@@ -406,14 +406,17 @@
             else:
                 generation = response.generations[-1][-1]
                 extracted_response = (
                     self._convert_message_to_dict(generation.message)
                     if isinstance(generation, ChatGeneration)
                     else _extract_raw_esponse(generation)
                 )
+                if isinstance(extracted_response, Dict):
+                    extracted_response = extracted_response.get('content', None)
+
                 llm_usage = (
                     None
                     if response.llm_output is None
                     or not response.llm_output["token_usage"]
                     else response.llm_output["token_usage"]
                 )
                 _debug(self.runs[run_id])
@@ -440,15 +443,15 @@
         except Exception as e:
             _debug(e)
 
     def _on_llm_action(
         self,
         serialized: Dict[str, Any],
         run_id: UUID,
-        prompts: List[str],
+        prompts: List[Any],
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ):
         try:
             self._generate_trace(
@@ -457,40 +460,31 @@
                 run_id=run_id,
                 parent_run_id=parent_run_id,
                 tags=tags,
                 metadata=metadata,
                 version=self.version,
                 kwargs=kwargs,
             ) 
-            # Convert all items in prompts to strings, handling dictionaries specifically
-            prompts_str = []
-            for item in prompts:
-                if isinstance(item, dict):
-                    prompts_str.append(item.get('text', str(item)))
-                else:
-                    prompts_str.append(str(item))
             name = self._get_athina_run_name(serialized, **kwargs)
             attributes = { 
                 'is_chat_model' : metadata.get('is_chat_model', False),
                 'prompt_slug': metadata.get('prompt_slug', None),
                 'user_query': metadata.get('user_query', None),
                 'context': metadata.get('global_context', None),
-                'prompt': {'text': ' '.join(prompts_str)},
+                'prompt': prompts,
                 'session_id': metadata.get('session_id', None),
                 'customer_id': metadata.get('customer_id', None),
                 'customer_user_id': metadata.get('customer_user_id', None),
                 'external_reference_id': metadata.get('external_reference_id', None),
                 'custom_attributes': metadata.get('custom_attributes', None),
-                'language_model_id': kwargs.get('invocation_params').get('model_name')
+                'language_model_id': _extract_model_name(serialized, **kwargs)
             }
             prompt_slug = metadata.get('prompt_slug', None)
             if parent_run_id in self.runs:
                 self.runs[run_id] = self.runs[parent_run_id].create_generation(name=name, attributes=attributes, version=self.version, prompt_slug=prompt_slug)
-            elif self.root_span is not None and parent_run_id is None:
-                self.runs[run_id] = self.root_span.create_generation(name=name, attributes=attributes, version=self.version, prompt_slug=prompt_slug)
             else:
                 self.runs[run_id] = self.trace.create_generation(name=name, attributes=attributes, version=self.version, prompt_slug=prompt_slug)
 
         except Exception as e:
             _debug(e)
 
 
@@ -511,15 +505,15 @@
             if self.trace is None:
                 trace = Trace(
                     name=self.trace_name if self.trace_name is not None else class_name,
                     attributes=metadata,
                     version=self.version,
                 )
                 self.trace = trace 
-
+                self.trace_run_id = run_id
         except Exception as e:
             _debug(e)
 
     def _join_tags_and_metadata(
         self,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
```

### Comparing `athina_logger-1.2.0/athina_logger/tracing/models.py` & `athina_logger-1.2.1/athina_logger/tracing/models.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/tracing/span.py` & `athina_logger-1.2.1/athina_logger/tracing/span.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/tracing/trace.py` & `athina_logger-1.2.1/athina_logger/tracing/trace.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/util/extract_model.py` & `athina_logger-1.2.1/athina_logger/util/extract_model.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/athina_logger/util/token_count_helper.py` & `athina_logger-1.2.1/athina_logger/util/token_count_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.2.0/PKG-INFO` & `athina_logger-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athina-logger
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Author: Akshat Gupta
 Author-email: akshat@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

