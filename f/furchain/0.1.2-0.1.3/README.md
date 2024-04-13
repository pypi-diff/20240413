# Comparing `tmp/furchain-0.1.2.tar.gz` & `tmp/furchain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furchain-0.1.2.tar", max compression
+gzip compressed data, was "furchain-0.1.3.tar", max compression
```

## Comparing `furchain-0.1.2.tar` & `furchain-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,45 @@
--rw-r--r--   0        0        0     3207 2024-03-11 07:09:50.381374 furchain-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/conversion/__init__.py
--rw-r--r--   0        0        0     3243 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/conversion/rvc.py
--rw-r--r--   0        0        0     1047 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/conversion/sovits.py
--rw-r--r--   0        0        0     3330 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/schema.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/speech/__init__.py
--rw-r--r--   0        0        0     3648 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/speech/gpt_sovits.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/transcriptions/__init__.py
--rw-r--r--   0        0        0    10542 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/transcriptions/funasr.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/__init__.py
--rw-r--r--   0        0        0     3141 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/audio_editor.py
--rw-r--r--   0        0        0     3872 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/audio_iterator.py
--rw-r--r--   0        0        0     3097 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/audio_separator.py
--rw-r--r--   0        0        0     2934 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/convert.py
--rw-r--r--   0        0        0      897 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/get_format.py
--rw-r--r--   0        0        0     3557 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/microphone.py
--rw-r--r--   0        0        0     2136 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/audio/utils/play.py
--rw-r--r--   0        0        0     1846 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/config.py
--rw-r--r--   0        0        0     2796 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/logger.py
--rw-r--r--   0        0        0      101 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/__init__.py
--rw-r--r--   0        0        0     2706 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/callbacks.py
--rw-r--r--   0        0        0    12516 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/chat_format.py
--rw-r--r--   0        0        0     7003 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/chat_message_history.py
--rw-r--r--   0        0        0     4523 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/chat_prompt_templates.py
--rw-r--r--   0        0        0      617 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/grammars.py
--rw-r--r--   0        0        0     4297 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/llama_cpp_client.py
--rw-r--r--   0        0        0     2779 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/output_parsers.py
--rw-r--r--   0        0        0    50286 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/text/schema.py
--rw-r--r--   0        0        0        0 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/utils/__init__.py
--rw-r--r--   0        0        0     3208 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/utils/broadcaster.py
--rw-r--r--   0        0        0     1997 2024-03-11 07:09:50.385374 furchain-0.1.2/furchain/utils/iterator.py
--rw-r--r--   0        0        0      990 2024-03-11 07:09:50.385374 furchain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 furchain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3207 2024-04-13 05:23:28.617788 furchain-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/__init__.py
+-rw-r--r--   0        0        0      751 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/gpt_sovits_vc.py
+-rw-r--r--   0        0        0     3282 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/rvc.py
+-rw-r--r--   0        0        0     1047 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/sovits.py
+-rw-r--r--   0        0        0     3943 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/schema.py
+-rw-r--r--   0        0        0       34 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/speech/__init__.py
+-rw-r--r--   0        0        0     3716 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/speech/gpt_sovits.py
+-rw-r--r--   0        0        0       27 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/transcriptions/__init__.py
+-rw-r--r--   0        0        0    10530 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/transcriptions/funasr.py
+-rw-r--r--   0        0        0      230 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_editor.py
+-rw-r--r--   0        0        0     3872 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_iterator.py
+-rw-r--r--   0        0        0     3097 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_separator.py
+-rw-r--r--   0        0        0     2934 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/convert.py
+-rw-r--r--   0        0        0      897 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/get_format.py
+-rw-r--r--   0        0        0     3557 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/microphone.py
+-rw-r--r--   0        0        0     2136 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/play.py
+-rw-r--r--   0        0        0     2009 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/config.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/image/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/image/captions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/generation/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/generation/stable_diffusion_webui.py
+-rw-r--r--   0        0        0      127 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/schema.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/__init__.py
+-rw-r--r--   0        0        0     6710 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/actions.py
+-rw-r--r--   0        0        0     1647 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/schema.py
+-rw-r--r--   0        0        0     3171 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/tools.py
+-rw-r--r--   0        0        0     2796 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/logger.py
+-rw-r--r--   0        0        0      101 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/__init__.py
+-rw-r--r--   0        0        0     2314 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/callbacks.py
+-rw-r--r--   0        0        0    14081 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_format.py
+-rw-r--r--   0        0        0     7241 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_message_history.py
+-rw-r--r--   0        0        0     6789 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_prompt_templates.py
+-rw-r--r--   0        0        0      615 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/grammars.py
+-rw-r--r--   0        0        0     4297 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/llama_cpp_client.py
+-rw-r--r--   0        0        0     2779 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/output_parsers.py
+-rw-r--r--   0        0        0    53992 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/schema.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/__init__.py
+-rw-r--r--   0        0        0     3208 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/broadcaster.py
+-rw-r--r--   0        0        0     1998 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/iterator.py
+-rw-r--r--   0        0        0     1029 2024-04-13 05:23:28.621788 furchain-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 furchain-0.1.3/PKG-INFO
```

### Comparing `furchain-0.1.2/README.md` & `furchain-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/conversion/rvc.py` & `furchain-0.1.3/furchain/audio/conversion/rvc.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.resample_sr = resample_sr
         self.rms_mix_rate = rms_mix_rate
         self.protect = protect
         if api is None:
             api = AudioConfig.get_rvc_api()
         self.api = api
 
-    def run(self, audio_bytes: bytes) -> bytes:
+    def run(self, audio_bytes: bytes, **kwargs) -> bytes:
         """
         This method sends a POST request to the RVC API with the necessary parameters and the audio file.
         It then returns the response content which is the converted audio.
 
         Args:
             audio_bytes (bytes): The audio file in bytes.
 
@@ -66,18 +66,19 @@
             "device": self.device,
             "is_half": self.is_half,
             "filter_radius": self.filter_radius,
             "resample_sr": self.resample_sr,
             "rms_mix_rate": self.rms_mix_rate,
             "protect": self.protect,
         }
+        data.update(kwargs)
         files = {
             "input_file": audio_bytes,
         }
 
         response = requests.post(self.api, params=data, files=files)
         return response.content
 
 
 __all__ = [
     "RVC"
-]
+]
```

### Comparing `furchain-0.1.2/furchain/audio/conversion/sovits.py` & `furchain-0.1.3/furchain/audio/conversion/sovits.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/schema.py` & `furchain-0.1.3/furchain/audio/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 
 class TTS(Runnable, metaclass=abc.ABCMeta):
     """
     The TTS class is an abstract base class that represents a Text-to-Speech (TTS) service.
     It inherits from the Runnable class and uses the ABCMeta metaclass to enforce the implementation
     of the abstract methods in any concrete subclass.
     """
-    ...
+
+    def run(self, text: str, *args, **kwargs):
+        raise NotImplementedError
+
+    def invoke(self, input: dict | str, config: Optional[RunnableConfig] = None) -> Output:
+        if isinstance(input, str):
+            input = {"text": input}
+        return self.run(**input)
 
 
 class VC(Runnable, metaclass=abc.ABCMeta):
     """
     The VC class is an abstract base class that represents a Voice Conversion (VC) service.
     It inherits from the Runnable class and uses the ABCMeta metaclass to enforce the implementation
     of the abstract methods in any concrete subclass.
@@ -74,7 +81,16 @@
 class STT(Runnable, metaclass=abc.ABCMeta):
     """
     The STT class is an abstract base class that represents a Speech-to-Text (STT) service.
     It inherits from the Runnable class and uses the ABCMeta metaclass to enforce the implementation
     of the abstract methods in any concrete subclass.
     """
     ...
+
+
+class FeatureExtraction(Runnable, metaclass=abc.ABCMeta):
+    """
+    The FeatureExtraction class is an abstract base class that represents a feature extraction service.
+    It inherits from the Runnable class and uses the ABCMeta metaclass to enforce the implementation
+    of the abstract methods in any concrete subclass.
+    """
+    ...
```

### Comparing `furchain-0.1.2/furchain/audio/speech/gpt_sovits.py` & `furchain-0.1.3/furchain/audio/speech/gpt_sovits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Optional
+from urllib.parse import urljoin
 
 import requests
-from langchain_core.runnables import RunnableConfig
 
 from furchain.audio.schema import TTS
 from furchain.config import AudioConfig
 
 
 class GPTSovitsClient:
     """
@@ -15,15 +14,15 @@
     Attributes:
         api_base (str): The base URL of the GPT-Sovits API.
         refer_wav_path (str): The path to the reference WAV file.
         prompt_text (str): The prompt text.
         prompt_language (str): The language of the prompt text.
     """
 
-    def __init__(self, api_base: str, refer_wav_path: str = None, prompt_text: str = None, prompt_language: str = None):
+    def __init__(self, api_base: str, refer_wav_path: str = None, prompt_text: str = None, prompt_language: str = 'auto'):
         self.api_base = api_base
         self.refer_wav_path = refer_wav_path
         self.prompt_text = prompt_text
         self.prompt_language = prompt_language
 
     def change_refer(self, refer_wav_path: str, prompt_text: str):
         """
@@ -53,56 +52,61 @@
             'prompt_text': self.prompt_text,
             'prompt_language': self.prompt_language,
             'refer_wav_path': self.refer_wav_path
         }
         response = requests.post(self.api_base, json=payload)
         return response.content
 
+    def vc(self, refer_wav:bytes, prompt_wav: bytes, prompt_text:str, noise_scale: float = 0.5):
+        params = {
+            'noise_scale': noise_scale,
+            'prompt_text': prompt_text,
+            'prompt_language': self.prompt_language,
+
+        }
+        file = {
+            'prompt_wav': prompt_wav,
+            'refer_wav': refer_wav
+        }
+        response = requests.post(urljoin(self.api_base, "vc"), params=params, files=file)
+        return response.content
+
+
 
 class GPTSovits(TTS):
     """
     This class is a subclass of TTS and represents the GPT-Sovits Text-to-Speech (TTS) model.
     It is used to convert text to speech.
 
     Attributes:
         client (GPTSovitsClient): The client for the GPT-Sovits API.
     """
 
     def __init__(self, api_base: str = None, refer_wav_path: str = None, prompt_text: str = None,
-                 prompt_language: str = None):
+                 prompt_language: str = None, text_language=None):
         super().__init__()
         if api_base is None:
             api_base = AudioConfig.get_gpt_sovits_api_base()
+        self.text_language = text_language
         self.client = GPTSovitsClient(api_base, refer_wav_path, prompt_text, prompt_language)
 
-    def run(self, text: str, text_language: str) -> bytes:
+    def run(self, text: str, text_language: str = None) -> bytes:
         """
         This method converts the given text to speech by calling the infer method of the client.
 
         Args:
             text (str): The text to be converted to speech.
             text_language (str): The language of the text.
 
         Returns:
             bytes: The speech in bytes.
         """
+        if text_language is None:
+            text_language = self.text_language
         return self.client.infer(text, text_language)
 
-    def invoke(
-            self, input: dict, config: Optional[RunnableConfig] = None
-    ) -> bytes:
-        """
-        This method is a wrapper for the run method. It takes a dictionary as input and unpacks it to call the run method.
-
-        Args:
-            input (dict): The input parameters for the run method.
-            config (Optional[RunnableConfig]): The configuration for the runnable. Default is None.
 
-        Returns:
-            bytes: The speech in bytes.
-        """
-        return self.run(**input)
 
 
 __all__ = [
     "GPTSovits"
 ]
```

### Comparing `furchain-0.1.2/furchain/audio/transcriptions/funasr.py` & `furchain-0.1.3/furchain/audio/transcriptions/funasr.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from furchain.audio.utils.get_format import get_format_from_magic_bytes
 from furchain.config import AudioConfig
 from furchain.logger import logger
 from furchain.utils.iterator import BufferIterator
 
 END_MESSAGE = json.dumps({"is_speaking": False})
 
+
 class FunASRSession:
     """
     This class represents a session with the FunASR API.
     It is used to send and receive messages to and from the API.
 
     Attributes:
         api (str): The URL of the FunASR API.
@@ -250,15 +251,15 @@
         kwargs['mode'] = 'offline'
         i = None
         for i in self.stream(input, **kwargs):
             result += i['text']
         if i is None:
             raise RuntimeError("FunASR failed to return a valid result.")
         if result == '':
-            if audio_format := get_format_from_magic_bytes(input) != 'unknown':
+            if audio_format := get_format_from_magic_bytes(input):
                 warnings.warn(
                     f"You need to convert `{audio_format}` into PCM format with `furchain.audio.utils.convert.convert_to_pcm`.")
 
         i['text'] = result
         return i
 
     def stream(
```

### Comparing `furchain-0.1.2/furchain/audio/utils/audio_editor.py` & `furchain-0.1.3/furchain/audio/utils/audio_editor.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/audio_iterator.py` & `furchain-0.1.3/furchain/audio/utils/audio_iterator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/audio_separator.py` & `furchain-0.1.3/furchain/audio/utils/audio_separator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/convert.py` & `furchain-0.1.3/furchain/audio/utils/convert.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/get_format.py` & `furchain-0.1.3/furchain/audio/utils/get_format.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/microphone.py` & `furchain-0.1.3/furchain/audio/utils/microphone.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/audio/utils/play.py` & `furchain-0.1.3/furchain/audio/utils/play.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/config.py` & `furchain-0.1.3/furchain/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,7 +69,13 @@
     @staticmethod
     def get_azure_region():
         return os.environ['FURCHAIN_AUDIO_AZURE_REGION']
 
     @staticmethod
     def get_funasr_api():
         return os.environ['FURCHAIN_AUDIO_FUNASR_API']
+
+class ImageConfig:
+
+    @classmethod
+    def get_stable_diffusion_webui_api_base(cls):
+        return os.environ['FURCHAIN_IMAGE_STABLE_DIFFUSION_WEBUI_API_BASE']
```

### Comparing `furchain-0.1.2/furchain/logger.py` & `furchain-0.1.3/furchain/logger.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/text/callbacks.py` & `furchain-0.1.3/furchain/text/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,29 @@
     """
     This class provides an iterator over a string iterable, allowing to read the string data in chunks.
 
     Attributes:
         iterable (iter): The iterable to iterate over.
         callbacks (List[Callable]): The list of callback functions to call when the iteration is finished.
         content (str): The content read so far.
-        response_prefix (str): The prefix to add to the first chunk of content. Default is ''.
         skip (tuple): The chunks to skip.
 
     Methods:
         add_callback(callback): Adds a callback function to the list of callbacks.
         __iter__(): Returns the iterator.
         __next__(): Returns the next chunk of string data. If the end of the iterable is reached, calls the callbacks and raises StopIteration.
     """
 
-    def __init__(self, iterable, callbacks: List[Callable], response_prefix='', skip=tuple()):
+    def __init__(self, iterable, callbacks: List[Callable], skip=tuple()):
         """
         Initializes the StrChunkCallbackIterator with the given iterable, callbacks, response prefix, and skip.
         """
         self.iterable = iter(iterable)
         self.callbacks = callbacks
         self.content = ''
-        self.response_prefix = response_prefix
         self.skip = skip
 
     def add_callback(self, callback: Callable):
         """
         Adds a callback function to the list of callbacks.
 
         Args:
@@ -50,23 +48,19 @@
         Returns the next chunk of string data. If the end of the iterable is reached, calls the callbacks and raises StopIteration.
         """
         try:
             chunk = next(self.iterable)
             if isinstance(chunk, str):
                 if chunk in self.skip:
                     return self.__next__()
-                if self.content == '':
-                    chunk = (self.response_prefix + chunk).lstrip()
                 self.content += chunk
                 return chunk
             else:
                 if chunk.content in self.skip:
                     return self.__next__()
-                if self.content == '':
-                    chunk.content = (self.response_prefix + chunk.content).lstrip()
                 self.content += chunk.content
                 return chunk.content
         except StopIteration as e:
             for callback in self.callbacks:
                 callback(self.content)
             logger.debug(f"Response: {self.content}")
             raise e
```

### Comparing `furchain-0.1.2/furchain/text/chat_format.py` & `furchain-0.1.3/furchain/text/chat_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,31 +253,32 @@
         Returns:
             str: The parsed chat prompt value.
         """
         prompt = super().parse(chat_prompt_value).removesuffix(
             '### Response:') + '### Response: (length = ' + cls.length + ')\n'
         return prompt
 
+
 class ChatMLChatFormatParser(ChatFormatParser):
     """
     Chat format parser for the ChatML format.
 
     Attributes:
         _sep (str): Separator string used to separate different parts of the chat.
         _human_prefix (str): Prefix for user messages.
         _ai_prefix (str): Prefix for assistant messages.
         stop (list): List of stop words or phrases.
 
     Methods:
         parse(chat_prompt_value: ChatPromptValue): Parses a chat prompt value in the ChatML format.
     """
 
-    _sep = "<|im_""end|>"  # This special token prevents copilot from generating complete response, so I split it into two parts
-    _human_prefix = "<|im_start|>user"
-    _ai_prefix = "<|im_start|>assistant"
+    _sep = "<|im_""end|>\n"  # This special token prevents copilot from generating complete response, so I split it into two parts
+    _human_prefix = "<|im_start|>user\n"
+    _ai_prefix = "<|im_start|>assistant\n"
     stop = ["<|im_""end|>"]
 
     @classmethod
     def parse(self, chat_prompt_value: ChatPromptValue) -> str:
         """
         Parses a chat prompt value in the ChatML format.
 
@@ -289,20 +290,63 @@
 
         The method starts by initializing the prompt with a system message.
         Then it iterates over the messages in the chat prompt value.
         For each message, it checks the type of the message (HumanMessage or AIMessage) and appends the content of the message to the prompt with the appropriate prefix.
         Finally, it appends the AI prefix to the prompt and returns it.
         """
         messages = chat_prompt_value.messages
-        prompt = "<|im_start|>system"
+        prompt = "<|im_start|>system\n"
+        system_message = ''
+        if len(messages) > 0 and isinstance(messages[0], SystemMessage):
+            system_message = messages[0].content
+            messages = messages[1:]
+        prompt = prompt + system_message + self._sep
+        for idx, i in enumerate(messages):
+            if isinstance(i, HumanMessage):
+                prompt += self._human_prefix + i.content + self._sep
+            elif isinstance(i, AIMessage):
+                prompt += self._ai_prefix + i.content + self._sep
+        prompt += self._ai_prefix  # + response_prefix
+        return prompt
+
+
+class QwenChatFormatParser(ChatMLChatFormatParser):
+    """
+    Chat format parser for the Qwen format.
+
+    This class inherits from the ChatMLChatFormatParser and overrides the stop attribute.
+
+    Attributes:
+        stop (list): List of stop words or phrases. In this case, it's the end of text token.
+    """
+    stop = ["<|""endoftext|>"]
+
+    @classmethod
+    def parse(self, chat_prompt_value: ChatPromptValue) -> str:
+        """
+        Parses a chat prompt value in the ChatML format.
+
+        Args:
+            chat_prompt_value (ChatPromptValue): The chat prompt value to parse.
+
+        Returns:
+            str: The parsed chat prompt value.
+
+        The method starts by initializing the prompt with a system message.
+        Then it iterates over the messages in the chat prompt value.
+        For each message, it checks the type of the message (HumanMessage or AIMessage) and appends the content of the message to the prompt with the appropriate prefix.
+        Finally, it appends the AI prefix to the prompt and returns it.
+        """
+        messages = chat_prompt_value.messages
+        prompt = "<|im_start|>system\n"
         system_message = ''
         if len(messages) > 0 and isinstance(messages[0], SystemMessage):
             system_message = messages[0].content
             messages = messages[1:]
-        prompt = system_message + self._sep + prompt
+        prompt = prompt + system_message + self._sep
         for idx, i in enumerate(messages):
             if isinstance(i, HumanMessage):
                 prompt += self._human_prefix + i.content + self._sep
             elif isinstance(i, AIMessage):
                 prompt += self._ai_prefix + i.content + self._sep
         prompt += self._ai_prefix  # + response_prefix
         return prompt
@@ -315,49 +359,43 @@
     Attributes:
         Alpaca (str): Alpaca chat format.
         ExtendedAlpaca (str): Extended Alpaca chat format.
         LimaRPExtendedAlpaca (str): LimaRP Extended Alpaca chat format.
         ChatML (str): ChatML chat format.
         Llama2 (str): Llama2 chat format.
         Vicuna (str): Vicuna chat format.
+        Qwen (str): Qwen chat format.
 
     Methods:
         parser: Returns the appropriate chat format parser for the chat format.
     """
 
     Alpaca = 'Alpaca'
     ExtendedAlpaca = 'ExtendedAlpaca'
     LimaRPExtendedAlpaca = 'LimaRPExtendedAlpaca'
     ChatML = 'ChatML'
     Llama2 = 'Llama2'
     Vicuna = 'Vicuna'
+    Qwen = 'Qwen'
 
     @property
     def parser(self) -> ChatFormatParser:
         """
         Returns the appropriate chat format parser for the chat format.
 
         Returns:
             ChatFormatParser: The chat format parser.
-
-        Raises:
-            NotImplementedError: If the chat format is not supported.
         """
-        if self == ChatFormat.Alpaca:
-            return AlpacaChatFormatParser()
-        elif self == ChatFormat.ExtendedAlpaca:
-            return ExtendedAlpacaChatFormatParser()
-        elif self == ChatFormat.LimaRPExtendedAlpaca:
-            return LimaRPExtendedAlpacaChatFormatParser()
-        elif self == ChatFormat.ChatML:
-            return ChatMLChatFormatParser()
-        elif self == ChatFormat.Llama2:
-            return Llama2ChatFormatParser()
-        elif self == ChatFormat.Vicuna:
-            return VicunaChatFormatParser()
-        else:
-            raise NotImplementedError
+        return {
+            ChatFormat.Alpaca: AlpacaChatFormatParser,
+            ChatFormat.ExtendedAlpaca: ExtendedAlpacaChatFormatParser,
+            ChatFormat.LimaRPExtendedAlpaca: LimaRPExtendedAlpacaChatFormatParser,
+            ChatFormat.ChatML: ChatMLChatFormatParser,
+            ChatFormat.Llama2: Llama2ChatFormatParser,
+            ChatFormat.Vicuna: VicunaChatFormatParser,
+            ChatFormat.Qwen: QwenChatFormatParser
+        }[self]()
 
 
 __all__ = [
     "ChatFormat"
 ]
```

### Comparing `furchain-0.1.2/furchain/text/chat_message_history.py` & `furchain-0.1.3/furchain/text/chat_message_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,22 @@
     def dict(self) -> dict:
         """
         Returns a dictionary representation of the chat message history.
 
         Returns:
             dict: A dictionary representation of the chat message history.
         """
-        return self.collection.find_one({"session_id": self.session_id})
+        return self.collection.find_one({"session_id": self.session_id}) or {
+            "session_id": self.session_id,
+            "npc": self.npc.to_dict(),
+            "player": self.player.to_dict(),
+            "scenario": self.scenario.to_dict(),
+            "chat_history": self.chat_history
+        }
+
 
     def find(self, session_id, collection_name=None):
         """
         Finds a chat message history by session ID.
 
         Args:
             session_id (str): The session ID.
```

### Comparing `furchain-0.1.2/furchain/text/grammars.py` & `furchain-0.1.3/furchain/text/grammars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-JSON_GRAMMAR = r"""root   ::= object
+JSON_GRAMMAR = r"""root ::= object
 value  ::= object | array | string | number | ("true" | "false" | "null") ws
 
 object ::=
   "{" ws (
             string ":" ws value
     ("," ws string ":" ws value)*
   )? "}" ws
```

### Comparing `furchain-0.1.2/furchain/text/llama_cpp_client.py` & `furchain-0.1.3/furchain/text/llama_cpp_client.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/text/output_parsers.py` & `furchain-0.1.3/furchain/text/output_parsers.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/text/schema.py` & `furchain-0.1.3/furchain/text/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+import itertools
 import json
 from typing import Optional, Any, Iterable, Iterator
 
 import requests
 from langchain.output_parsers import PydanticOutputParser
 from langchain_core.messages import HumanMessage, AIMessage
 from langchain_core.messages import SystemMessage, messages_from_dict
 from langchain_core.messages import messages_to_dict
+from langchain_core.prompt_values import ChatPromptValue
 from langchain_core.prompts import AIMessagePromptTemplate, \
     MessagesPlaceholder
 from langchain_core.prompts import ChatPromptTemplate, HumanMessagePromptTemplate, SystemMessagePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel as BaseModel_v1, Field as Field_v1, root_validator
 from langchain_core.runnables import Runnable, RunnableBinding
 from langchain_core.runnables import RunnableConfig
 from langchain_core.runnables import RunnableLambda
 from langchain_core.runnables.utils import Output
-from llama_cpp.llama_grammar import json_schema_to_gbnf
+from llama_cpp.llama_grammar import json_schema_to_gbnf, LlamaGrammar
 from pydantic import BaseModel, Field
 from pymongo import MongoClient
 
 from furchain.config import TextConfig
+from furchain.interaction.tools import ToolSymbol, Tool, ToolCall
 from furchain.text.callbacks import StrChunkCallbackIterator
 from furchain.text.chat_format import ChatFormat
 from furchain.text.chat_message_history import MongoDBChatMessageHistory, logger
-from furchain.text.chat_prompt_templates import ROLEPLAY_CHAT_PROMPT_TEMPLATE, NO_HISTORY_CHAT_PROMPT_TEMPLATE
+from furchain.text.chat_prompt_templates import ROLEPLAY_CHAT_PROMPT_TEMPLATE, NO_HISTORY_CHAT_PROMPT_TEMPLATE, \
+    ROLEPLAY_WITH_TOOLS_CHAT_PROMPT_TEMPLATE
+from furchain.text.grammars import JSON_GRAMMAR
 from furchain.text.llama_cpp_client import LlamaCppClient
 
 CLASS_DICT = {
     'HumanMessagePromptTemplate': HumanMessagePromptTemplate,
     'AIMessagePromptTemplate': AIMessagePromptTemplate,
     'SystemMessagePromptTemplate': SystemMessagePromptTemplate,
     'HumanMessage': HumanMessage,
     'AIMessage': AIMessage,
     'SystemMessage': SystemMessage,
     'MessagesPlaceholder': MessagesPlaceholder
 }
 
+
 class Meta_v2(BaseModel):
     """
     A Pydantic model for meta data.
 
     Attributes:
         tags (list[str]): A list of tags for the meta data.
     """
@@ -224,14 +230,16 @@
         data = data.copy()
 
         return Scenario(
             scenario_name=data['scenario_name'],
             scenario_description=data['scenario_description'],
             meta=Meta_v2(**data['meta'])
         )
+
+
 class _Character_v2(BaseModel):
     """
     A Pydantic model for character data used to generate GBNF grammar.
 
     Attributes:
         character_name (str): The name of the character.
         persona (str): The persona of the character.
@@ -420,14 +428,15 @@
         chat_format (ChatFormat): The chat format.
         model_kwargs (dict): The model keyword arguments.
 
     Methods:
         invoke(input: str | list | dict, config: Optional[RunnableConfig] = None, **kwargs) -> Output: Invokes the LlamaCpp client with the given input and returns the output.
         stream(input: str | list | dict, config: Optional[RunnableConfig] = None, **kwargs: Optional[Any]) -> Iterator[Output]: Streams the LlamaCpp client with the given input and yields the output.
     """
+
     def __init__(self, base_url=None, api_key=None, chat_format: ChatFormat = ChatFormat.Alpaca, **kwargs):
         self.client = LlamaCppClient(base_url, api_key)
         self.chat_format = chat_format
         self.model_kwargs = kwargs
 
     def invoke(self, input: str | list | dict, config: Optional[RunnableConfig] = None, **kwargs) -> Output:
         """
@@ -437,17 +446,21 @@
             input (str | list | dict): The input to invoke the LlamaCpp client with.
             config (Optional[RunnableConfig]): The runnable config. Defaults to None.
             **kwargs: Additional keyword arguments.
 
         Returns:
             Output: The output from the LlamaCpp client.
         """
+        if isinstance(input, ChatPromptValue):
+            input = self.chat_format.parser.parse(input)
         if isinstance(input, (str, list)):
             input = {"prompt": input}
-        return self.client.complete(input, **kwargs, **self.model_kwargs)['content']
+        response = self.client.complete(input, **kwargs, **self.model_kwargs)
+        logger.debug(response)
+        return response['content']
 
     def stream(
             self,
             input: str | list | dict,
             config: Optional[RunnableConfig] = None,
             **kwargs: Optional[Any],
     ) -> Iterator[Output]:
@@ -458,14 +471,16 @@
             input (str | list | dict): The input to stream the LlamaCpp client with.
             config (Optional[RunnableConfig]): The runnable config. Defaults to None.
             **kwargs: Additional keyword arguments.
 
         Yields:
             Output: The output from the LlamaCpp client.
         """
+        if isinstance(input, ChatPromptValue):
+            input = self.chat_format.parser.parse(input)
         if isinstance(input, (str, list)):
             input = {"prompt": input}
         for i in self.client.stream(input, **kwargs, **self.model_kwargs):
             yield i['content']
 
 
 class Session(BaseModel_v1):
@@ -579,15 +594,15 @@
         """
         Returns a dictionary representation of the session.
 
         Returns:
             dict: A dictionary representation of the session.
         """
         result = self.chat_history_proxy.dict()
-        result.pop("_id")
+        result.pop("_id", None)
         return result
 
     @classmethod
     def from_dict(cls, data: dict, session_id=None, collection_name="Session"):
         """
         Creates a session from a dictionary.
 
@@ -675,127 +690,149 @@
         """
         Clears the session's chat history.
 
         Returns:
             None
         """
         self.chat_history_proxy.clear()
+
+
 class Chat(Runnable):
     """
     A class that represents a chat in a role-playing game.
 
     Attributes:
         llm (LlamaCpp | RunnableBinding): The LlamaCpp instance or a RunnableBinding.
         session (Session): The session.
         chat_prompt_template (ChatPromptTemplate): The chat prompt template.
-        response_prefix (str): The response prefix.
         grammar (str): The grammar.
         kwargs (dict): Additional keyword arguments.
 
     Methods:
-        _get_chain_params(query: str, response_prefix: str = None, **kwargs): Gets the chain parameters.
+        _get_chain_params(query: str, **kwargs): Gets the chain parameters.
         invoke(input: dict | str, config: Optional[RunnableConfig] = None, **kwargs: Any) -> Output: Invokes the chat with the given input and returns the output.
         stream(input: dict | str, config: Optional[RunnableConfig] = None, **kwargs: Any) -> Iterable[Output]: Streams the chat with the given input and yields the output.
     """
 
     def __init__(self, llm: LlamaCpp | RunnableBinding,
                  session: Session,
                  chat_prompt_template: ChatPromptTemplate = None,
-                 response_prefix: str = None,
-                 grammar: str = '',
+                 grammar: str = None,
+                 tools: list[Tool] = None,
                  **kwargs):
         super().__init__()
-        if response_prefix is None:
-            response_prefix = session.npc.character_name + ':'
+
+        if grammar is None:
+            self.grammar = r'''root ::= "''' + session.npc.character_name.encode("unicode-escape").decode(
+                "utf-8") + r''':" [\u4E00-\u9FFFA-Za-z0-9\u0021-\u002F\u003A-\u0040\u005B-\u0060\u007B-\u007E\uFF01-\uFF0F\uFF1A-\uFF20\uFF3B-\uFF40\uFF5B-\uFF65\u3002\n ]*'''  # Start with the npc's name, followed by any characters
+        else:
+            self.grammar = grammar
         if isinstance(llm, RunnableBinding):
             model_kwargs = llm.kwargs
             llm = llm.bound
         else:
             model_kwargs = llm.model_kwargs
         chat_format = llm.chat_format
         self.kwargs = kwargs
+        self.tools = tools
         chat_format_parser = chat_format.parser if isinstance(chat_format, ChatFormat) else ChatFormat(
             chat_format).parser
-        self.llm = llm.bind(stop=model_kwargs.get("stop", []) + chat_format_parser.stop, grammar=grammar)
+        if self.tools:
+            root_grammar = f'''root ::= "{session.npc.character_name.encode("unicode-escape").decode("utf-8")}:" ''' + f'''anything+ (tool | anything)+\n''' + f'''tool ::= {" | ".join(i.tool_name + "-root" for i in self.tools)}\n''' + r'''anything ::= [\u4E00-\u9FFFA-Za-z0-9\u0021-\u002F\u003A-\u0040\u005B-\u0060\u007B-\u007E\uFF01-\uFF0F\uFF1A-\uFF20\uFF3B-\uFF40\uFF5B-\uFF65\u3002\n ]'''
+            tool_grammar = '\n'.join([
+                f'''{i.tool_name}-root ::= "{ToolSymbol.TOOL_NAME.value.encode("unicode-escape").decode("utf-8")}" "{i.tool_name}" "{ToolSymbol.TOOL_PARAMETER.value.encode("unicode-escape").decode("utf-8")}" parameter-{i.tool_name}-root "{ToolSymbol.TOOL_OUTPUT.value.encode("unicode-escape").decode("utf-8")}"'''
+                for i in self.tools])
+            json_grammar = "json-" + JSON_GRAMMAR
+            parameter_grammar = '\n'.join([f'parameter-{i.tool_name}-' + i.tool_parameter_grammar for i in self.tools])
+            self.grammar = '\n'.join([
+                root_grammar,
+                tool_grammar,
+                json_grammar,
+                parameter_grammar
+            ])
+        self.llm = llm.bind(stop=model_kwargs.get("stop", []) + chat_format_parser.stop, grammar=self.grammar)
         self.chat_format_parser = chat_format_parser
         self.session = session
-        self.response_prefix = response_prefix
-        self.chat_prompt_template = chat_prompt_template if chat_prompt_template is not None else ROLEPLAY_CHAT_PROMPT_TEMPLATE
+        assert LlamaGrammar.from_string(self.grammar)
+
+        if chat_prompt_template is None:
+            if self.tools:
+                self.chat_prompt_template = ROLEPLAY_WITH_TOOLS_CHAT_PROMPT_TEMPLATE
+            else:
+                self.chat_prompt_template = ROLEPLAY_CHAT_PROMPT_TEMPLATE
+        else:
+            self.chat_prompt_template = chat_prompt_template
 
-    def _get_chain_params(self, query: str, response_prefix: str = None,
+    def _get_chain_params(self, query: str,
                           **kwargs):
         """
         Gets the chain parameters.
 
         Args:
             query (str): The query.
-            response_prefix (str, optional): The response prefix. Defaults to None.
             **kwargs: Additional keyword arguments.
 
         Returns:
             tuple: The chain, parameters, and the function to update the chat history.
         """
-        if response_prefix is None:
-            response_prefix = self.response_prefix
 
         # Define the chain of operations
-        chain = (
+        prompt_template = (
                 RunnableLambda(lambda x: (
                     self.chat_prompt_template.format_prompt(chat_history=messages_from_dict(x.pop('chat_history', [])),
                                                             **x)
                 ))
                 | RunnableLambda(self.chat_format_parser.parse)
-                | RunnableLambda(lambda x: (logger.debug("Prompt: " + x + response_prefix), x + response_prefix)[1])
-                | self.llm
         )
         if "chat_history" in self.chat_prompt_template.input_variables:
             history_messages = self.session.messages
         else:
             history_messages = []
         for i in history_messages:
             if isinstance(i, HumanMessage):
-                i.content = i.content.removeprefix(f"{self.session.player.character_name}: ")
-                i.content = f"{self.session.player.character_name}: {i.content}"
+                i.content = i.content.removeprefix(f"{self.session.player.character_name}:")
+                i.content = f"{self.session.player.character_name}:{i.content}"
             elif isinstance(i, AIMessage):
-                i.content = i.content.removeprefix(f"{self.session.npc.character_name}: ")
-                i.content = f"{self.session.npc.character_name}: {i.content}"
+                i.content = i.content.removeprefix(f"{self.session.npc.character_name}:")
+                i.content = f"{self.session.npc.character_name}:{i.content}"
         chat_history = messages_to_dict(history_messages)
         kwargs['npc_name'] = self.session.npc.character_name
         kwargs['npc_persona'] = self.session.npc.persona.format(
             npc_name=self.session.npc.character_name,
             player_name=self.session.player.character_name)
         kwargs['player_persona'] = self.session.player.persona.format(
             npc_name=self.session.npc.character_name,
             player_name=self.session.player.character_name)
         kwargs['player_name'] = self.session.player.character_name
         kwargs['scenario_description'] = self.session.scenario.scenario_description.format(
             npc_name=self.session.npc.character_name,
             player_name=self.session.player.character_name)
         kwargs['query'] = query
         kwargs['chat_history'] = chat_history
-        kwargs['response_prefix'] = response_prefix
+        if self.tools:
+            kwargs['tools'] = "\n".join([f"{i.tool_name}: {i.tool_description}" for i in self.tools])
 
-        def _update_chat_history(response_with_prefix):
+        def _update_chat_history(response):
             """
             Updates the chat history.
 
             Args:
-                response_with_prefix (str): The response with prefix.
+                response (str): The response from AI.
 
             Returns:
                 None
             """
             human_message = HumanMessage(content=f"{query}")
-            ai_message = AIMessage(content=f"{response_with_prefix}")
+            ai_message = AIMessage(content=f"{response}")
             self.session.add_messages([
                 human_message,
                 ai_message
             ])
 
-        return chain, kwargs, _update_chat_history
+        return prompt_template, kwargs, _update_chat_history
 
     def invoke(
             self, input: dict | str, config: Optional[RunnableConfig] = None, **kwargs: Any
     ) -> Output:
         """
         Invokes the chat with the given input and returns the output.
 
@@ -831,22 +868,56 @@
             Output: The output from the chat.
         """
         params = {}
         if isinstance(input, str):
             input = {'query': input}
         params.update(input)
         params.update(kwargs)
-        chain, params, _update_chat_history = self._get_chain_params(**params)
-        stream = chain.stream(params, config)
+        prompt_template, params, _update_chat_history = self._get_chain_params(**params)
+        prompt_template: ChatPromptTemplate
+        chain = prompt_template | self.llm
+        stream = chain.stream(params)
         logger.debug(f"stream input: {params}")
-        yield from StrChunkCallbackIterator(
-            iterable=stream,
-            callbacks=[_update_chat_history],
-            response_prefix=params['response_prefix'],
-        )
+        if not self.tools:
+            yield from StrChunkCallbackIterator(
+                iterable=stream,
+                callbacks=[_update_chat_history],
+            )
+        else:
+            #
+            def _stream(prompt_value, llm, buffer, content=''):
+                logger.debug(f"stream input: {prompt_value}")
+                new_stream = llm.stream(prompt_value)
+                iterator = StrChunkCallbackIterator(
+                    iterable=itertools.chain(buffer, new_stream),
+                    callbacks=[_update_chat_history]
+                )
+                iterator.content = content
+                for token in iterator:
+                    print(f"{token=}")
+                    yield token
+                    if ToolSymbol.TOOL_OUTPUT.value in token:  # meet a tool call end, then look back to extract
+                        tool_call = ToolCall.from_string(iterator.content)
+                        result = tool_call.execute()
+                        prompt_value += iterator.content + result + ToolSymbol.TOOL_END.value
+                        new_iterator = _stream(prompt_value,
+                                               self.llm.bind(grammar=self.grammar.replace(
+                                                   f'''"{self.session.npc.character_name.encode('unicode-escape').decode('utf-8')}:"''',
+                                                   '', 1)),
+                                               result + ToolSymbol.TOOL_END.value,
+                                               iterator.content)
+                        print(self.grammar.replace(
+                                                   f"{self.session.npc.character_name.encode('unicode-escape').decode('utf-8')}:",
+                                                   '', 1))
+                        del iterator
+                        yield from new_iterator
+                        return
+
+            prompt_value = prompt_template.invoke(params)
+            yield from _stream(prompt_value, self.llm, '')
 
 
 class CreateScenarioByChat:
     format_instructions = PydanticOutputParser(pydantic_object=Scenario).get_format_instructions()
     prompt_template = ChatPromptTemplate.from_messages([
         HumanMessage(content="""a scenario in intimacy"""),
         AIMessage(
@@ -878,22 +949,22 @@
                           scenario=cls.scenario,
                           )
         chat = Chat(
             llm=llm,
             session=session,
             chat_prompt_template=NO_HISTORY_CHAT_PROMPT_TEMPLATE,
             grammar=json_schema_to_gbnf(json.dumps(_Scenario_v2.model_json_schema()).replace("allOf", "oneOf")),
-            response_prefix=''
         )
         result = chat.invoke(description)
         result = json.loads(result)
         result['meta'] = Meta_v2(**result.get('meta', {}))
         result['type'] = 'scenario'
         return Scenario(**result)
 
+
 class CreateCharacterByChat:
     """
     A class that creates a character by chat.
 
     Attributes:
         format_instructions (str): The format instructions for the character.
         prompt_template (ChatPromptTemplate): The chat prompt template.
@@ -950,33 +1021,36 @@
                           scenario=cls.scenario,
                           )
         chat = Chat(
             llm=llm,
             session=session,
             chat_prompt_template=NO_HISTORY_CHAT_PROMPT_TEMPLATE,
             grammar=json_schema_to_gbnf(json.dumps(_Character_v2.model_json_schema()).replace("allOf", "oneOf")),
-            response_prefix=''
         )
         result = chat.invoke(description)
         result = json.loads(result)
         result['meta'] = Meta_v2(**result.get('meta', {}))
         result['type'] = 'character'
         return Character(**result)
+
+
 class _Session_v2(BaseModel):
     """
     A Pydantic model for session data used to generate GBNF grammar.
 
     Attributes:
         npc (_Character_v2): The non-player character (NPC) in the session.
         player (_Character_v2): The player character in the session.
         scenario (_Scenario_v2): The scenario of the session.
     """
     npc: _Character_v2 = Field(description="Characteristics of the npc")
     player: _Character_v2 = Field(description="Characteristics of the player")
     scenario: _Scenario_v2 = Field(description="Characteristics of the scenario")
+
+
 class CreateSessionByChat:
     """
     A class that creates a session by chat.
 
     Attributes:
         _Session (BaseModel_v1): A Pydantic model for session data.
         format_instructions (str): The format instructions for the session.
@@ -1050,15 +1124,14 @@
                           scenario=cls.scenario,
                           )
         chat = Chat(
             llm=llm,
             session=session,
             chat_prompt_template=NO_HISTORY_CHAT_PROMPT_TEMPLATE,
             grammar=json_schema_to_gbnf(json.dumps(_Session_v2.model_json_schema()).replace("allOf", "oneOf")),
-            response_prefix=''
         )
         result = chat.invoke(description)
         result = json.loads(result)
         npc = Character.from_dict(result['npc'])
         player = Character.from_dict(result['player'])
         scenario = Scenario.from_dict(result['scenario'])
         return Session(
```

### Comparing `furchain-0.1.2/furchain/utils/broadcaster.py` & `furchain-0.1.3/furchain/utils/broadcaster.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.2/furchain/utils/iterator.py` & `furchain-0.1.3/furchain/utils/iterator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import queue
 
+
 class BufferIterator:
     """
     A class that provides an iterator interface for a buffer.
 
     Attributes:
         queue (queue.Queue): The queue object to be iterated over.
         stop (Any): The sentinel value that indicates the end of the iteration.
```

### Comparing `furchain-0.1.2/pyproject.toml` & `furchain-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "furchain"
-version = "0.1.2"
+version = "0.1.3"
 description = "FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline."
 authors = ["markyfsun <mark@furchain.xyz>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 websocket-client = "^1.7.0"
 pydantic = "^2.5.3"
 pydub = "^0.25.1"
 soundfile = "^0.12.1"
 requests = "^2.31.0"
 sympy = "^1.12"
-audio-separator = { extras = ["gpu"], version = "^0.13.0" }
+#audio-separator = { extras = ["gpu"], version = "^0.13.0" }
 langchain-core = "^0.1.16"
 langchain-community = "^0.0.16"
 openai = "^1.10.0"
 ffmpeg-python = "^0.2.0"
 langchain = "^0.1.4"
 pymongo = "^4.6.1"
 llama-cpp-python = "^0.2.52"
 python-dotenv = "^1.0.1"
 pyaudio = "^0.2.14"
 websockets = "^12.0"
+webuiapi = "^0.9.9"
+emoji = "^2.10.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `furchain-0.1.2/PKG-INFO` & `furchain-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: furchain
-Version: 0.1.2
+Version: 0.1.3
 Summary: FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline.
 Author: markyfsun
 Author-email: mark@furchain.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: audio-separator[gpu] (>=0.13.0,<0.14.0)
+Requires-Dist: emoji (>=2.10.1,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: langchain (>=0.1.4,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.16,<0.0.17)
 Requires-Dist: langchain-core (>=0.1.16,<0.2.0)
 Requires-Dist: llama-cpp-python (>=0.2.52,<0.3.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: pyaudio (>=0.2.14,<0.3.0)
@@ -22,14 +22,15 @@
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: sympy (>=1.12,<2.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
+Requires-Dist: webuiapi (>=0.9.9,<0.10.0)
 Description-Content-Type: text/markdown
 
 # 🦊🔗 FurChain
 
 🌟 Create Lifelike Digital Personas 🌟
 
 Empower your digital experiences with lifelike characters, complete with their own voices and personalities.
```

