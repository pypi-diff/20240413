# Comparing `tmp/kimchima-0.3.1.tar.gz` & `tmp/kimchima-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.3.1.tar", max compression
+gzip compressed data, was "kimchima-0.4.1.tar", max compression
```

## Comparing `kimchima-0.3.1.tar` & `kimchima-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0    11343 2024-04-08 12:45:03.927963 kimchima-0.3.1/LICENSE
--rw-r--r--   0        0        0      908 2024-04-08 12:45:03.927963 kimchima-0.3.1/README.md
--rw-r--r--   0        0        0     2576 2024-04-08 12:45:03.931963 kimchima-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1027 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1558 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0      674 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     2004 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1072 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3233 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/download_hub.py
--rw-r--r--   0        0        0     3222 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4727 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1838 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3558 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1818 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     2032 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     1992 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kimchima-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-13 03:02:35.397894 kimchima-0.4.1/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-13 03:02:35.397894 kimchima-0.4.1/README.md
+-rw-r--r--   0        0        0     2576 2024-04-13 03:02:35.401894 kimchima-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1108 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/chat_template/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/chat_template/chat_template_factory.py
+-rw-r--r--   0        0        0        0 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     3537 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1072 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3233 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/download_hub.py
+-rw-r--r--   0        0        0     3222 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4727 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1838 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3558 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1818 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     2032 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     3041 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-13 03:02:35.401894 kimchima-0.4.1/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kimchima-0.4.1/PKG-INFO
```

### Comparing `kimchima-0.3.1/LICENSE` & `kimchima-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/README.md` & `kimchima-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/pyproject.toml` & `kimchima-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.3.1"
+version = "0.4.1"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.3.1/src/kimchima/__init__.py` & `kimchima-0.4.1/src/kimchima/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,18 +21,19 @@
     QuantizationFactory,
     StreamerFactory,
     Devices,
     DownloadHub
     )
 
 from kimchima.pipelines import PipelinesFactory
-
+from kimchima.chat_template import ChatTemplateFactory
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'Devices',
     'PipelinesFactory',
+    'ChatTemplateFactory',
     'DownloadHub'
     ]
```

### Comparing `kimchima-0.3.1/src/kimchima/cmds/auto_cli.py` & `kimchima-0.4.1/src/kimchima/cmds/auto_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,10 @@
 
         Args:
             args (argparse.Namespace): The arguments.
 
         Returns:
             torch.tensor: The embeddings of text.
         """
-        model = ModelFactory.auto_model(pretrained_model_name_or_path=args.model_name)
+        model = ModelFactory.auto_model(pretrained_model_name_or_path=args.model_name_or_path)
         print(model.config)
```

### Comparing `kimchima-0.3.1/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.4.1/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pipelines/__init__.py` & `kimchima-0.4.1/src/kimchima/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pipelines/pipelines_factory.py` & `kimchima-0.4.1/src/kimchima/chat_template/chat_template_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,52 +12,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from kimchima.pkg import logging
 
-from transformers import pipeline
+from transformers import AutoTokenizer
 
 logger=logging.get_logger(__name__)
 
-
-class PipelinesFactory:
+class ChatTemplateFactory:
     r"""
-    A factory class for creating Huggingface Transformers pipelines for different ML tasks.
+    A factory class for creating prompt from chat Template for different ML tasks.
     """
 
     def __init__(self):
         raise EnvironmentError(
-            "Pipelines is designed to be instantiated "
-            "using the `Pipelines.from_pretrained(pretrained_model_name_or_path)` method."
+            "Chat Template is designed to be instantiated "
+            "using the `AutoTokenizer.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
     @classmethod
-    def text_generation(cls, *args,**kwargs)-> pipeline:
+    def prompt_generation(cls, *args,**kwargs)-> list[int]:
         r"""
-        Create a text generation pipeline using the Huggingface Transformers library.
+        Create prompt by using the Huggingface Transformers library.
         """
-        
         model=kwargs.pop("model", None)
         if model is None:
             raise ValueError("model is required")
-        tokenizer=kwargs.pop("tokenizer", None)
-        if tokenizer is None:
-            raise ValueError("tokenizer is required")
-        streamer=kwargs.pop("text_streamer", None)
-        max_new_tokens=kwargs.pop("max_new_tokens", 20)
-        
-        #
-        pipe=pipeline(
-            task="text-generation",
-            model=model,
-            tokenizer=tokenizer,
-            streamer=streamer,
-            max_new_tokens=max_new_tokens,
-            device_map='auto',
-            **kwargs
-        )
+        messages=kwargs.pop("messages", None)
+        if messages is None:
+            raise ValueError("messages is required")
+
+        tokenize=kwargs.pop("tokenize", False)
+        add_generation_prompt=kwargs.pop("add_generation_prompt", False)
+
+        tokenizer = AutoTokenizer.from_pretrained(model)
 
-        logger.debug(f"The text generation pipeline device is {pipe.device}")
+        tokenized_chat  = tokenizer.apply_chat_template(messages, tokenize=tokenize, add_generation_prompt=add_generation_prompt)
 
-        return pipe
+        return tokenized_chat
```

### Comparing `kimchima-0.3.1/src/kimchima/pkg/__init__.py` & `kimchima-0.4.1/src/kimchima/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/devices.py` & `kimchima-0.4.1/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/download_hub.py` & `kimchima-0.4.1/src/kimchima/pkg/download_hub.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.4.1/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/logging.py` & `kimchima-0.4.1/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/model_factory.py` & `kimchima-0.4.1/src/kimchima/pkg/model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.4.1/src/kimchima/pkg/quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.4.1/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.4.1/src/kimchima/pkg/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/tests/test_devices.py` & `kimchima-0.4.1/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.4.1/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.4.1/src/kimchima/tests/test_pipelines_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,7 +56,39 @@
                 tokenizer=self.tokenizer,
                 text_streamer=self.streamer,
                 quantization_config=self.quantization_config
                 )
     
             self.assertIsNotNone(pipe)
             self.assertEqual(pipe.task, 'text-generation')
+
+        def test_customized_pipe(self):
+            """
+            Test customized_pipe method
+            """
+    
+            pipe = PipelinesFactory.customized_pipe(
+                task="text-generation",
+                model=self.model,
+                tokenizer=self.tokenizer,
+                streamer=self.streamer,
+                max_new_tokens=20,
+                device_map='auto'
+                )
+    
+            self.assertIsNotNone(pipe)
+            self.assertEqual(pipe.task, 'text-generation')
+
+        def test_chat_response(self):
+            """
+            Test chat_response method
+            """
+            msg = "why Melbourne is a good place to travel?"
+            prompt = "Melbourne is often considered one of the most livable cities globally, offering a high quality of life."
+            
+            res = PipelinesFactory.chat_response(
+                conversation_model=self.model_name,
+                messages=msg,
+                prompt=prompt
+                )
+    
+            self.assertIsNotNone(res)
```

### Comparing `kimchima-0.3.1/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.4.1/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.1/PKG-INFO` & `kimchima-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.3.1
+Version: 0.4.1
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

