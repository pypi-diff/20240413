# Comparing `tmp/hfer-0.0.3.tar.gz` & `tmp/hfer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfer-0.0.3.tar", last modified: Sat Mar 23 05:17:07 2024, max compression
+gzip compressed data, was "hfer-0.0.4.tar", last modified: Sat Apr 13 10:17:25 2024, max compression
```

## Comparing `hfer-0.0.3.tar` & `hfer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-03-23 05:17:07.770416 hfer-0.0.3/
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)    11357 2024-03-19 07:26:01.000000 hfer-0.0.3/LICENSE
--rw-r--r--   0 shenxuyang (10233) shenxuyang (10233)      277 2024-03-23 05:17:07.769766 hfer-0.0.3/PKG-INFO
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)       41 2024-03-19 06:58:48.000000 hfer-0.0.3/README.md
-drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-03-23 05:17:07.768016 hfer-0.0.3/hfer/
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      189 2024-03-19 06:59:13.000000 hfer-0.0.3/hfer/__init__.py
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      947 2024-03-19 06:59:33.000000 hfer-0.0.3/hfer/_builder.py
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)     2392 2024-03-19 06:59:13.000000 hfer-0.0.3/hfer/_registry.py
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)     9269 2024-03-23 04:38:06.000000 hfer-0.0.3/hfer/hf_backend.py
-drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-03-23 05:17:07.768986 hfer-0.0.3/hfer.egg-info/
--rw-r--r--   0 shenxuyang (10233) shenxuyang (10233)      277 2024-03-23 05:17:07.768366 hfer-0.0.3/hfer.egg-info/PKG-INFO
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      209 2024-03-23 05:17:07.768607 hfer-0.0.3/hfer.egg-info/SOURCES.txt
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)        1 2024-03-23 05:17:07.768817 hfer-0.0.3/hfer.egg-info/dependency_links.txt
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)        5 2024-03-23 05:17:07.769029 hfer-0.0.3/hfer.egg-info/top_level.txt
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)       38 2024-03-23 05:17:07.770469 hfer-0.0.3/setup.cfg
--rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      382 2024-03-23 05:16:55.000000 hfer-0.0.3/setup.py
+drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-04-13 10:17:25.211608 hfer-0.0.4/
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)    11357 2024-03-19 07:26:01.000000 hfer-0.0.4/LICENSE
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      321 2024-04-13 10:17:25.211252 hfer-0.0.4/PKG-INFO
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)       85 2024-04-13 10:17:12.000000 hfer-0.0.4/README.md
+drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-04-13 10:17:25.209881 hfer-0.0.4/hfer/
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      189 2024-03-19 06:59:13.000000 hfer-0.0.4/hfer/__init__.py
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      947 2024-03-19 06:59:33.000000 hfer-0.0.4/hfer/_builder.py
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)     2392 2024-03-19 06:59:13.000000 hfer-0.0.4/hfer/_registry.py
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)    11128 2024-04-10 11:07:17.000000 hfer-0.0.4/hfer/hf_backend.py
+drwxrwxr-x   0 shenxuyang (10233) shenxuyang (10233)        0 2024-04-13 10:17:25.210943 hfer-0.0.4/hfer.egg-info/
+-rw-r--r--   0 shenxuyang (10233) shenxuyang (10233)      321 2024-04-13 10:17:25.210286 hfer-0.0.4/hfer.egg-info/PKG-INFO
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      209 2024-04-13 10:17:25.210542 hfer-0.0.4/hfer.egg-info/SOURCES.txt
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)        1 2024-04-13 10:17:25.210769 hfer-0.0.4/hfer.egg-info/dependency_links.txt
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)        5 2024-04-13 10:17:25.211006 hfer-0.0.4/hfer.egg-info/top_level.txt
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)       38 2024-04-13 10:17:25.211684 hfer-0.0.4/setup.cfg
+-rw-rw-r--   0 shenxuyang (10233) shenxuyang (10233)      382 2024-04-13 10:11:44.000000 hfer-0.0.4/setup.py
```

### Comparing `hfer-0.0.3/LICENSE` & `hfer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hfer-0.0.3/hfer/_builder.py` & `hfer-0.0.4/hfer/_builder.py`

 * *Files identical despite different names*

### Comparing `hfer-0.0.3/hfer/_registry.py` & `hfer-0.0.4/hfer/_registry.py`

 * *Files identical despite different names*

### Comparing `hfer-0.0.3/hfer/hf_backend.py` & `hfer-0.0.4/hfer/hf_backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 import logging
 
 import torch
+
 import transformers
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForCausalLM,
     AutoTokenizer,
     BloomForCausalLM,
@@ -15,15 +16,15 @@
 )
 from transformers.generation.utils import GenerationConfig
 
 from ._registry import register_model
 
 __all__ = [
     'tnl3', 'tnl', 'llama', 'baichuan', 'baichuan2', 'qwen', 'qwen1_5', 'bloom', 'pythia', 'mistral', 'mistral_moe',
-    'mamba', 'LLModel', 'HuggingFaceModel'
+    'mamba', 'mpt', 'jamba', 'recurrentgemma', 'LLModel', 'HuggingFaceModel'
 ]
 
 # detect transformers version
 logging.info(f'transformers version: {transformers.__version__}')
 
 
 class LLModel(ABC):
@@ -40,29 +41,27 @@
     def chat(self):
         pass
 
 
 class HuggingFaceModel(LLModel):
 
     def __init__(self, tokenizer, model):
-        self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         model.eval()
-        model.to(self.device)
 
         self.tok = tokenizer
         self.model = model
 
     def get_tokenizer(self) -> AutoTokenizer:
         return self.tok
 
     def get_model(self) -> AutoModelForCausalLM:
         return self.model
 
     def chat(self, messages, config):
-        inputs = self.tok(messages, return_tensors='pt').to(self.device)
+        inputs = self.tok(messages, return_tensors='pt').to("cuda")
         outputs = self.model.generate(inputs.input_ids, do_sample=True, **config)
         try:
             response = self.tok.batch_decode(outputs[:, inputs.input_ids.shape[1]:], skip_special_tokens=True)[0]
         except Exception as e:
             logging.error(e)
             response = ''
 
@@ -75,14 +74,15 @@
         tok: AutoTokenizer = AutoTokenizer.from_pretrained(repo_or_path,
                                                            trust_remote_code=True,
                                                            add_bos_token=False,
                                                            padding_side='left',
                                                            **tok_configs)
         model: AutoModelForCausalLM = AutoModelForCausalLM.from_pretrained(repo_or_path,
                                                                            trust_remote_code=True,
+                                                                           device_map='auto',
                                                                            **model_configs)
 
         model_vocab_size = model.get_input_embeddings().weight.size(0)
         tokenzier_vocab_size = len(tok)
         logging.info(f'Vocab of the base model: {model_vocab_size}')
         logging.info(f'Vocab of the tokenizer: {tokenzier_vocab_size}')
 
@@ -141,15 +141,18 @@
                                          use_fast=True,
                                          legacy=False)
     if 'llama2' or 'LLaMA2' or 'llama-2' or 'LLaMA-2' in repo_or_path:
         config = AutoConfig.from_pretrained(repo_or_path, pretraining_tp=0)
     else:
         config = AutoConfig.from_pretrained(repo_or_path)
 
-    model = LlamaForCausalLM.from_pretrained(repo_or_path, config=config, torch_dtype=torch.bfloat16)
+    model = LlamaForCausalLM.from_pretrained(repo_or_path,
+                                             config=config,
+                                             torch_dtype=torch.bfloat16,
+                                             device_map='auto')
 
     model_vocab_size = model.get_input_embeddings().weight.size(0)
     tokenzier_vocab_size = len(tok)
     logging.info(f'Vocab of the base model: {model_vocab_size}')
     logging.info(f'Vocab of the tokenizer: {tokenzier_vocab_size}')
 
     tok.pad_token = tok.eos_token
@@ -214,29 +217,29 @@
     return HuggingFaceModelWrap(repo_or_path, tok_configs, model_configs)
 
 
 @register_model
 def bloom(repo_or_path) -> HuggingFaceModel:
     tok = AutoTokenizer.from_pretrained(repo_or_path, trust_remote_code=True, add_bos_token=False, padding_side='left')
 
-    model = BloomForCausalLM.from_pretrained(repo_or_path)
+    model = BloomForCausalLM.from_pretrained(repo_or_path, device_map='auto')
 
     model_vocab_size = model.get_input_embeddings().weight.size(0)
     tokenzier_vocab_size = len(tok)
     logging.info(f'Vocab of the base model: {model_vocab_size}')
     logging.info(f'Vocab of the tokenizer: {tokenzier_vocab_size}')
 
     return HuggingFaceModel(tok, model)
 
 
 @register_model
 def pythia(repo_or_path) -> HuggingFaceModel:
     tok = AutoTokenizer.from_pretrained(repo_or_path, trust_remote_code=True, add_bos_token=False, padding_side='left')
 
-    model = GPTNeoXForCausalLM.from_pretrained(repo_or_path)
+    model = GPTNeoXForCausalLM.from_pretrained(repo_or_path, device_map='auto')
 
     tok.eos_token_id = 0
     model.config.eos_token_id = 0
     tok.pad_token_id = 1
     model.config.pad_token_id = 1
 
     model_vocab_size = model.get_input_embeddings().weight.size(0)
@@ -252,15 +255,14 @@
     def __init__(self, repo_or_path):
         try:
             from mamba_ssm.models.mixer_seq_simple import MambaLMHeadModel
         except Exception as e:
             print('Please try to install mamba!')
             raise e
 
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.device = device
 
         tokenizer = AutoTokenizer.from_pretrained("EleutherAI/gpt-neox-20b")
         model = MambaLMHeadModel.from_pretrained(repo_or_path, device=device, dtype=torch.float16)
         model.eval()
 
         self.tok = tokenizer
@@ -269,15 +271,15 @@
     def get_tokenizer(self) -> AutoTokenizer:
         return self.tok
 
     def get_model(self) -> AutoModelForCausalLM:
         return self.model
 
     def chat(self, messages, config={}):
-        input_ids = self.tok(messages, return_tensors='pt').to(self.device).input_ids
+        input_ids = self.tok(messages, return_tensors='pt').input_ids
         max_length = input_ids.shape[1] + config['max_new_tokens']
         del config['max_new_tokens']
 
         outputs = self.model.generate(input_ids, max_length=max_length, cg=True, enable_timing=False, **config)
         try:
             response = self.tok.batch_decode(outputs[:, input_ids.shape[1]:], skip_special_tokens=True)[0]
         except Exception as e:
@@ -286,7 +288,54 @@
 
         return response
 
 
 @register_model
 def mamba(repo_or_path) -> LLModel:
     return MambaModel(repo_or_path)
+
+
+@register_model
+def jamba(repo_or_path) -> HuggingFaceModel:
+    try:
+        from mamba_ssm import Mamba
+    except Exception as e:
+        logging.error('Try to pip install mamba_ssm!')
+        raise e
+
+    tok_configs = {'use_fast': True}
+    model_configs = {'torch_dtype': torch.bfloat16}
+
+    return HuggingFaceModelWrap(repo_or_path, tok_configs, model_configs)
+
+
+@register_model
+def recurrentgemma(repo_or_path) -> HuggingFaceModel:
+
+    tok_configs = {}
+    model_configs = {'torch_dtype': torch.bfloat16}
+
+    return HuggingFaceModelWrap(repo_or_path, tok_configs, model_configs)
+
+
+@register_model
+def mpt(repo_or_path) -> HuggingFaceModel:
+    # tok = AutoTokenizer.from_pretrained('EleutherAI/gpt-neox-20b', add_bos_token=False, padding_side='left')
+    tok = AutoTokenizer.from_pretrained("/cpfs01/user/shenxuyang/LLM/models-hf/gpt-neox-20b",
+                                        trust_remote_code=True,
+                                        add_bos_token=False,
+                                        padding_side='left')
+
+    config = AutoConfig.from_pretrained(repo_or_path, trust_remote_code=True)
+    config.max_seq_len = 12000  # (input + output) tokens can now be up to 4096
+
+    model = AutoModelForCausalLM.from_pretrained(repo_or_path,
+                                                 config=config,
+                                                 trust_remote_code=True,
+                                                 device_map='auto')
+
+    model_vocab_size = model.get_input_embeddings().weight.size(0)
+    tokenzier_vocab_size = len(tok)
+    logging.info(f'Vocab of the base model: {model_vocab_size}')
+    logging.info(f'Vocab of the tokenizer: {tokenzier_vocab_size}')
+
+    return HuggingFaceModel(tok, model)
```

