# Comparing `tmp/xiaogpt-2.31.tar.gz` & `tmp/xiaogpt-2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.31.tar", last modified: Fri Apr 12 15:05:11 2024, max compression
+gzip compressed data, was "xiaogpt-2.32.tar", last modified: Fri Apr 12 15:37:09 2024, max compression
```

## Comparing `xiaogpt-2.31.tar` & `xiaogpt-2.32.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1063 2024-04-12 15:05:01.292487 xiaogpt-2.31/LICENSE
--rw-r--r--   0        0        0    23688 2024-04-12 15:05:01.292487 xiaogpt-2.31/README.md
--rw-r--r--   0        0        0     1280 2024-04-12 15:05:11.808405 xiaogpt-2.31/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1073 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      840 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/bard_bot.py
--rw-r--r--   0        0        0     1467 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     2781 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1944 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     5506 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/cli.py
--rw-r--r--   0        0        0     6703 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      220 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     3978 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/azure.py
--rw-r--r--   0        0        0     4923 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     2072 2024-04-12 15:05:01.292487 xiaogpt-2.31/xiaogpt/utils.py
--rw-r--r--   0        0        0    15400 2024-04-12 15:05:01.296487 xiaogpt-2.31/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    24695 1970-01-01 00:00:00.000000 xiaogpt-2.31/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 15:37:05.944039 xiaogpt-2.32/LICENSE
+-rw-r--r--   0        0        0    23688 2024-04-12 15:37:05.948039 xiaogpt-2.32/README.md
+-rw-r--r--   0        0        0     1280 2024-04-12 15:37:09.308037 xiaogpt-2.32/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1073 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      840 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/bard_bot.py
+-rw-r--r--   0        0        0     1467 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     2781 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     5375 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6533 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      220 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     3978 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/azure.py
+-rw-r--r--   0        0        0     4923 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1172 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/edge.py
+-rw-r--r--   0        0        0     1096 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1533 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/tts/openai.py
+-rw-r--r--   0        0        0     2072 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15400 2024-04-12 15:37:05.948039 xiaogpt-2.32/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    24695 1970-01-01 00:00:00.000000 xiaogpt-2.32/PKG-INFO
```

### Comparing `xiaogpt-2.31/LICENSE` & `xiaogpt-2.32/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/README.md` & `xiaogpt-2.32/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/pyproject.toml` & `xiaogpt-2.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "numexpr>=2.8.6",
     "dashscope==1.10.0",
     "httpcore==0.15.0",
     "idna==3.7",
     "azure-cognitiveservices-speech>=1.37.0",
 ]
 dynamic = []
-version = "2.31"
+version = "2.32"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.31/xiaogpt/bot/__init__.py` & `xiaogpt-2.32/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/bard_bot.py` & `xiaogpt-2.32/xiaogpt/bot/bard_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/base_bot.py` & `xiaogpt-2.32/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.32/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.32/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.32/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-2.32/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.32/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.32/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.32/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/cli.py` & `xiaogpt-2.32/xiaogpt/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,14 @@
         dest="deployment_id",
         help="specify deployment id, only used when api_base points to azure",
     )
 
     options = parser.parse_args()
     if options.bot in ["bard"] and options.stream:
         raise Exception("For now Bard do not support stream")
-    if options.tts in ["edge", "openai", "azure"]:
-        print("Will close stream to better tts")
-        options.stream = False
     config = Config.from_options(options)
 
     miboy = MiGPT(config)
     loop = asyncio.get_event_loop()
     loop.run_until_complete(miboy.run_forever())
```

### Comparing `xiaogpt-2.31/xiaogpt/config.py` & `xiaogpt-2.32/xiaogpt/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,17 +110,14 @@
         if self.bot in ["chatgptapi", "gpt3"]:
             if not self.openai_key:
                 raise Exception(
                     "Using GPT api needs openai API key, please google how to"
                 )
         if self.tts == "azure" and not self.azure_tts_speech_key:
             raise Exception("Using Azure TTS needs azure speech key")
-        if self.tts in ["azure", "edge", "openai"]:
-            print("Will close stream when use tts: {self.tts} for better experience")
-            self.stream = False
 
     @property
     def tts_command(self) -> str:
         return HARDWARE_COMMAND_DICT.get(self.hardware, DEFAULT_COMMAND)[0]
 
     @property
     def wakeup_command(self) -> str:
```

### Comparing `xiaogpt-2.31/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.32/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/langchain/chain.py` & `xiaogpt-2.32/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.32/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.32/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/tts/azure.py` & `xiaogpt-2.32/xiaogpt/tts/azure.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/tts/base.py` & `xiaogpt-2.32/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/tts/edge.py` & `xiaogpt-2.32/xiaogpt/tts/edge.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/tts/mi.py` & `xiaogpt-2.32/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/tts/openai.py` & `xiaogpt-2.32/xiaogpt/tts/openai.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/utils.py` & `xiaogpt-2.32/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/xiaogpt/xiaogpt.py` & `xiaogpt-2.32/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.31/PKG-INFO` & `xiaogpt-2.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.31
+Version: 2.32
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

