# Comparing `tmp/llm_steer-1.0.2.tar.gz` & `tmp/llm_steer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_steer-1.0.2.tar", last modified: Wed Jan 24 13:23:06 2024, max compression
+gzip compressed data, was "llm_steer-1.1.0.tar", last modified: Sat Apr 13 18:38:16 2024, max compression
```

## Comparing `llm_steer-1.0.2.tar` & `llm_steer-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-24 13:23:06.254848 llm_steer-1.0.2/
--rw-rw-rw-   0        0        0     1022 2024-01-19 13:37:36.000000 llm_steer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4381 2024-01-24 13:23:06.253700 llm_steer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3998 2024-01-24 13:19:29.000000 llm_steer-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-01-24 13:23:06.251701 llm_steer-1.0.2/llm_steer.egg-info/
--rw-rw-rw-   0        0        0     4381 2024-01-24 13:23:06.000000 llm_steer-1.0.2/llm_steer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-01-24 13:23:06.000000 llm_steer-1.0.2/llm_steer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-24 13:23:06.000000 llm_steer-1.0.2/llm_steer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-24 13:23:06.000000 llm_steer-1.0.2/llm_steer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-24 13:23:06.000000 llm_steer-1.0.2/llm_steer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8879 2024-01-23 07:50:43.000000 llm_steer-1.0.2/llm_steer.py
--rw-rw-rw-   0        0        0       42 2024-01-24 13:23:06.254848 llm_steer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      613 2024-01-24 13:22:55.000000 llm_steer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:38:16.860499 llm_steer-1.1.0/
+-rw-rw-rw-   0        0        0     1022 2024-04-13 18:37:10.000000 llm_steer-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4415 2024-04-13 18:38:16.860499 llm_steer-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4032 2024-04-13 18:37:10.000000 llm_steer-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 18:38:16.858498 llm_steer-1.1.0/llm_steer.egg-info/
+-rw-rw-rw-   0        0        0     4415 2024-04-13 18:38:16.000000 llm_steer-1.1.0/llm_steer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-13 18:38:16.000000 llm_steer-1.1.0/llm_steer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 18:38:16.000000 llm_steer-1.1.0/llm_steer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 18:38:16.000000 llm_steer-1.1.0/llm_steer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-13 18:38:16.000000 llm_steer-1.1.0/llm_steer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7574 2024-04-13 18:37:10.000000 llm_steer-1.1.0/llm_steer.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 18:38:16.861499 llm_steer-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      613 2024-04-13 18:38:11.000000 llm_steer-1.1.0/setup.py
```

### Comparing `llm_steer-1.0.2/LICENSE` & `llm_steer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_steer-1.0.2/PKG-INFO` & `llm_steer-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_steer
-Version: 1.0.2
+Version: 1.1.0
 Summary: Steer LLM outputs towards a certain topic/subject and enhance response capabilities using activation engineering by adding steer vectors
 Home-page: https://github.com/Mihaiii/llm_steer
 Author: Mihai Chirculescu
 Author-email: apropodemine@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,34 +38,47 @@
 
 ## Advanced usage
 The so-called "advanced usage" involves changing the default values of 2 parameters ("try_keep_nr" and "exclude_bos_token"), which, from my experiments - almost always leads to the LLM outputting gibberish. In the very few cases when the LLM outputs text that does make sense, **the basic usage provides higher quality outputs**.
 
 More info will be provided in a separate file.
 
 ## Q / A
-Q: What's the difference between llm-steer and mentioning the response style in the system prompt?
-A: First of all, I see llm-steer as an enhancer. It can be used together with the system prompt.
+Q: What's the difference between llm_steer and mentioning what you want in the system prompt?
 
+A: I see llm_steer as an enhancer. It can be used together with the system prompt.
+
+<br/>
 Q: How to determine the best parameters to be used?
+
 A: I don't have a method; it's all trial and error. I recommend starting with a small coefficient and then slowly increase it.
 
+<br/>
 Q: What models are supported?
+
 A: I tested it on multiple architectures, including LLaMa, Mistral, Phi, StableLM.
-Keep in mind that llm-steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
+Keep in mind that llm_steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
 
+<br/>
 Q: I applied steering vectors, but the LLM outputs gibberish. What should I do?
+
 A: Try a lower coeff value or another layer.
 
+<br/>
 Q: Can I add multiple steering vectors on the same layer? Can I add the same steering vector on multiple layers? Can I add steering vectors with negative coefficients?
+
 A: Yes, and please do. llm_steer is built for experimenting.
 See the Colab for examples: https://colab.research.google.com/github/Mihaiii/llm_steer/blob/main/demo/llm_steer_demo.ipynb
 
+<br/>
 Q: Can I use steer vectors to enhance role-play characteristics (e.g., personas that are more funny or cocky)?
+
 A: I believe this is possible, but I haven't had good results yet. I'm considering doing some more intensive testing and I might write a new notebook for it.
 
+<br/>
 Q: Can I use negative steering vectors to force it not to say "As an AI language model"?
+
 A: Yes.
 
 ## Credits / Thanks
-- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and also [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
+- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
 - Gary Bernhardt for his excellent [Python for programmers](https://www.executeprogram.com/courses/python-for-programmers) course. I needed a course that could help me go through the basics of Python without treating me like a dev noob (like most basic level tutorials treat their audience).
-- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there alrady was a repo for every idea I had. Not when it comes to tools for LLM, though!
+- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there already was a repo for every idea I had. Not when it comes to tools for LLMs, though!
```

### Comparing `llm_steer-1.0.2/README.md` & `llm_steer-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -28,34 +28,47 @@
 
 ## Advanced usage
 The so-called "advanced usage" involves changing the default values of 2 parameters ("try_keep_nr" and "exclude_bos_token"), which, from my experiments - almost always leads to the LLM outputting gibberish. In the very few cases when the LLM outputs text that does make sense, **the basic usage provides higher quality outputs**.
 
 More info will be provided in a separate file.
 
 ## Q / A
-Q: What's the difference between llm-steer and mentioning the response style in the system prompt?
-A: First of all, I see llm-steer as an enhancer. It can be used together with the system prompt.
+Q: What's the difference between llm_steer and mentioning what you want in the system prompt?
 
+A: I see llm_steer as an enhancer. It can be used together with the system prompt.
+
+<br/>
 Q: How to determine the best parameters to be used?
+
 A: I don't have a method; it's all trial and error. I recommend starting with a small coefficient and then slowly increase it.
 
+<br/>
 Q: What models are supported?
+
 A: I tested it on multiple architectures, including LLaMa, Mistral, Phi, StableLM.
-Keep in mind that llm-steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
+Keep in mind that llm_steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
 
+<br/>
 Q: I applied steering vectors, but the LLM outputs gibberish. What should I do?
+
 A: Try a lower coeff value or another layer.
 
+<br/>
 Q: Can I add multiple steering vectors on the same layer? Can I add the same steering vector on multiple layers? Can I add steering vectors with negative coefficients?
+
 A: Yes, and please do. llm_steer is built for experimenting.
 See the Colab for examples: https://colab.research.google.com/github/Mihaiii/llm_steer/blob/main/demo/llm_steer_demo.ipynb
 
+<br/>
 Q: Can I use steer vectors to enhance role-play characteristics (e.g., personas that are more funny or cocky)?
+
 A: I believe this is possible, but I haven't had good results yet. I'm considering doing some more intensive testing and I might write a new notebook for it.
 
+<br/>
 Q: Can I use negative steering vectors to force it not to say "As an AI language model"?
+
 A: Yes.
 
 ## Credits / Thanks
-- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and also [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
+- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
 - Gary Bernhardt for his excellent [Python for programmers](https://www.executeprogram.com/courses/python-for-programmers) course. I needed a course that could help me go through the basics of Python without treating me like a dev noob (like most basic level tutorials treat their audience).
-- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there alrady was a repo for every idea I had. Not when it comes to tools for LLM, though!
+- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there already was a repo for every idea I had. Not when it comes to tools for LLMs, though!
```

### Comparing `llm_steer-1.0.2/llm_steer.egg-info/PKG-INFO` & `llm_steer-1.1.0/llm_steer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-steer
-Version: 1.0.2
+Version: 1.1.0
 Summary: Steer LLM outputs towards a certain topic/subject and enhance response capabilities using activation engineering by adding steer vectors
 Home-page: https://github.com/Mihaiii/llm_steer
 Author: Mihai Chirculescu
 Author-email: apropodemine@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,34 +38,47 @@
 
 ## Advanced usage
 The so-called "advanced usage" involves changing the default values of 2 parameters ("try_keep_nr" and "exclude_bos_token"), which, from my experiments - almost always leads to the LLM outputting gibberish. In the very few cases when the LLM outputs text that does make sense, **the basic usage provides higher quality outputs**.
 
 More info will be provided in a separate file.
 
 ## Q / A
-Q: What's the difference between llm-steer and mentioning the response style in the system prompt?
-A: First of all, I see llm-steer as an enhancer. It can be used together with the system prompt.
+Q: What's the difference between llm_steer and mentioning what you want in the system prompt?
 
+A: I see llm_steer as an enhancer. It can be used together with the system prompt.
+
+<br/>
 Q: How to determine the best parameters to be used?
+
 A: I don't have a method; it's all trial and error. I recommend starting with a small coefficient and then slowly increase it.
 
+<br/>
 Q: What models are supported?
+
 A: I tested it on multiple architectures, including LLaMa, Mistral, Phi, StableLM.
-Keep in mind that llm-steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
+Keep in mind that llm_steer is meant to be used together with HuggingFace's transformers library, so it won't work on GGUF, for example.
 
+<br/>
 Q: I applied steering vectors, but the LLM outputs gibberish. What should I do?
+
 A: Try a lower coeff value or another layer.
 
+<br/>
 Q: Can I add multiple steering vectors on the same layer? Can I add the same steering vector on multiple layers? Can I add steering vectors with negative coefficients?
+
 A: Yes, and please do. llm_steer is built for experimenting.
 See the Colab for examples: https://colab.research.google.com/github/Mihaiii/llm_steer/blob/main/demo/llm_steer_demo.ipynb
 
+<br/>
 Q: Can I use steer vectors to enhance role-play characteristics (e.g., personas that are more funny or cocky)?
+
 A: I believe this is possible, but I haven't had good results yet. I'm considering doing some more intensive testing and I might write a new notebook for it.
 
+<br/>
 Q: Can I use negative steering vectors to force it not to say "As an AI language model"?
+
 A: Yes.
 
 ## Credits / Thanks
-- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and also [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
+- [DL Explorers](https://www.youtube.com/@DLExplorers-lg7dt) for his video on [activation engineer](https://www.youtube.com/watch?v=J2Gx6FFEaRY&t=29s) which goes over [an article](https://www.greaterwrong.com/posts/5spBue2z2tw4JuDCx/steering-gpt-2-xl-by-adding-an-activation-vector) and [a colab he made](https://colab.research.google.com/github/githubpradeep/notebooks/blob/main/activation_engineering.ipynb). The resources mentioned in that video were the starting point of llm_steer.
 - Gary Bernhardt for his excellent [Python for programmers](https://www.executeprogram.com/courses/python-for-programmers) course. I needed a course that could help me go through the basics of Python without treating me like a dev noob (like most basic level tutorials treat their audience).
-- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there alrady was a repo for every idea I had. Not when it comes to tools for LLM, though!
+- Andrej Karpathy for his [State of GPT](https://www.youtube.com/watch?v=bZQun8Y4L2A) video. I always wanted to make an open-source project, but there already was a repo for every idea I had. Not when it comes to tools for LLMs, though!
```

### Comparing `llm_steer-1.0.2/llm_steer.py` & `llm_steer-1.1.0/llm_steer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import deepcopy
 from transformers import PreTrainedModel, PreTrainedTokenizerBase
 from dataclasses import dataclass
-from typing import List
+from typing import List, Callable
 from torch import Tensor, torch
 from enum import Enum
 
 
 class ActivationMode(Enum):
     ORIGINAL = 1
     CAPTURE = 2
@@ -15,15 +15,17 @@
 @dataclass
 class SteerElement:
     text: str
     tensor: Tensor
     coeff: float
     try_keep_nr: int
     exclude_bos_token: bool = False
-    
+    steering_method: Callable = None
+
+
 @dataclass
 class SteerData:
     orig_forward_fn: torch.nn.Module.forward
     layer_idx: int
     steer_vectors: List[SteerElement]
 
 
@@ -95,95 +97,68 @@
                         you could also consider setting it to False and retrying."""
                     raise Exception(
                         f"""Invalid try_keep_nr value. Current value is {elem.try_keep_nr}, 
                     but it has to be less than {elem.tensor.size()[1]} on layer index {layer_idx}. 
                     You could set a lower value for try_keep_nr or provide longer text for steering. {extraText}"""
                     )
 
-                delta = torch.mean(
-                    elem.coeff * elem.tensor[:, elem.try_keep_nr :, :],
-                    dim=1,
-                    keepdim=True,
-                )
+                if elem.steering_method is not None:
+                    delta = elem.steering_method(elem.tensor, elem.coeff, elem.try_keep_nr)
+                else:
+                    delta = torch.mean(
+                        elem.coeff * elem.tensor[:, elem.try_keep_nr :, :],
+                        dim=1,
+                        keepdim=True,
+                    )
 
                 if "hidden_states" in kwargds:
-                    # if user generates with use_cache=True, we receive only the latest row
-                    # otherwise (use_cache=False), we receive the whole matrix, that will keep expanding
                     if kwargds["hidden_states"].size()[1] == 1:
                         kwargds["hidden_states"][:, -1:, :] += delta
                     else:
                         kwargds["hidden_states"][:, elem.try_keep_nr :, :] += delta
                 elif isinstance(args[0], Tensor):
                     if args[0].size()[1] == 1:
                         args[0][:, -1:, :] += delta
                     else:
                         args[0][:, elem.try_keep_nr :, :] += delta
                 else:
                     raise Exception(
-                        "The model is not currently supported. Plase open an issue in the official github repository."
+                        "The model is not currently supported. Please open an issue in the official GitHub repository."
                     )
 
             return self.steers[layer_idx].orig_forward_fn(*args, **kwargds)
 
         return _steer_vector_forward_inner
 
     def get_all(self):
-        """
-        Get all the steering vectors data that are applied on the model.
-        Can be used for replicating in the future the state.
-        """
         return [{'layer_idx': val.layer_idx, 'text': x.text, 'coeff': x.coeff, 'try_keep_nr': x.try_keep_nr, 'exclude_bos_token': x.exclude_bos_token} for val in self.steers.values() for x in val.steer_vectors]
 
     def reset(self, layer_idx: int):
-        """
-        Remove the steering vectors on a particular layer.      
-
-        Args:
-            layer_idx (int): The layer index that will have the steering vectors removed.
-        """
         self._set_forward_fn(ActivationMode.ORIGINAL, layer_idx)
 
     def reset_all(self):
-        """
-        Remove all steering vectors that were applied on the model.
-        Gets the model to initial state, before wrapping it in the Steer class and using add(). 
-        """
         [self.reset(idx) for idx in range(len(self.model._modules["model"].layers))]
 
     def add(
         self,
         layer_idx: int,
         coeff: float,
         text: str,
         try_keep_nr: int = None,
         exclude_bos_token: bool = False,
+        steering_method: Callable = None,
     ):
-        """
-        Add a steering vector.
-        Args:
-            layer_idx (int): The layer index to apply the steering vector on. Usually is toward the end.
-            coeff: The steerging vectors coefficient. Usually is below 1. Can also be negative.
-            text: The steering vector text.
-            try_keep_nr: This is used in advanced usage and determines the number of rows of the initial
-                matrix to be kept. The param is used for expetimenting. Leave to default value for best usage.
-            exclude_bos_token: This is used in advanced usage and determines if the beginning of a sentence
-                (bos) token should be removed. By default, the code ensures the tokens used for generating
-                start with the bos token. The param is used for expetimenting. Leave to default value for best usage.
-        """
-        
         assert layer_idx >= 0 and layer_idx < len(
             self.model._modules["model"].layers
         ), f"""Current model has {len(self.model._modules['model'].layers)} layers, 
         but the provided layer_idx is not within 
         [0, {len(self.model._modules['model'].layers) - 1}] interval."""
         
         text_tokens = self.tokenizer.encode(text)
 
-        #inject bos_token
-        #This can be reverted with exclude_bos_token=True
         if self.tokenizer.bos_token is not None and text_tokens[0] != self.tokenizer.encode(self.tokenizer.bos_token)[-1]:
             text_tokens.insert(0, self.tokenizer.encode(self.tokenizer.bos_token)[-1])
         
         if (
             exclude_bos_token
             and self.tokenizer.bos_token is not None
         ):
@@ -197,15 +172,20 @@
 
         if try_keep_nr is None:
             try_keep_nr = 0 if self.tokenizer.bos_token is None else 1
 
         self._add_steer_vector(
             layer_idx,
             SteerElement(
-                text=text, tensor=layer_tensor, coeff=coeff, try_keep_nr=try_keep_nr, exclude_bos_token=exclude_bos_token
+                text=text,
+                tensor=layer_tensor,
+                coeff=coeff,
+                try_keep_nr=try_keep_nr,
+                exclude_bos_token=exclude_bos_token,
+                steering_method=steering_method,
             ),
         )
 
     def _add_steer_vector(self, layer_idx: int, steerElem: SteerElement):
         steer = self.steers.setdefault(
             layer_idx,
             SteerData(
@@ -218,8 +198,8 @@
         self._set_forward_fn(ActivationMode.STEER, layer_idx)
 
     def _capture_tensor(self, layer_idx: int, tokens: Tensor):
         self._set_forward_fn(ActivationMode.CAPTURE, layer_idx)
         self.model(tokens)
         result = self.captured_tensor
         print(f"captured tensor: {result}")
-        return result
+        return result
```

### Comparing `llm_steer-1.0.2/setup.py` & `llm_steer-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='llm_steer',
-    version='1.0.2',
+    version='1.1.0',
     description='Steer LLM outputs towards a certain topic/subject and enhance response capabilities using activation engineering by adding steer vectors',
     author='Mihai Chirculescu',
     author_email='apropodemine@gmail.com',
     py_modules=['llm_steer'],
     url="https://github.com/Mihaiii/llm_steer",
     install_requires=[
         'transformers'
```

