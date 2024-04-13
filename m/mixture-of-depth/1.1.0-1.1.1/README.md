# Comparing `tmp/mixture-of-depth-1.1.0.tar.gz` & `tmp/mixture-of-depth-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-depth-1.1.0.tar", last modified: Sat Apr 13 10:54:41 2024, max compression
+gzip compressed data, was "mixture-of-depth-1.1.1.tar", last modified: Sat Apr 13 10:55:37 2024, max compression
```

## Comparing `mixture-of-depth-1.1.0.tar` & `mixture-of-depth-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:54:41.040164 mixture-of-depth-1.1.0/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:54:41.036164 mixture-of-depth-1.1.0/MoD/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4517 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.0/MoD/MoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.0/MoD/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:54:41.036164 mixture-of-depth-1.1.0/MoD/modeling/
--rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.0/MoD/modeling/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.0/MoD/modeling/automodeling.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:54:41.040164 mixture-of-depth-1.1.0/MoD/modeling/models/
--rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/BloomMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    75772 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/FalconMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/GemmaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/LlamaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/MistralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.0/MoD/modeling/models/MixtralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    68583 2024-04-13 10:27:42.000000 mixture-of-depth-1.1.0/MoD/modeling/models/PhiMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.0/MoD/modeling/models/QwenMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73609 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.0/MoD/modeling/models/QwenMoEMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.0/MoD/modeling/models/StarCoderMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.0/MoD/modeling/models/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-13 10:54:41.040164 mixture-of-depth-1.1.0/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2120 2024-04-12 12:30:41.000000 mixture-of-depth-1.1.0/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:54:41.040164 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-13 10:54:41.000000 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-13 10:54:41.000000 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-13 10:54:41.000000 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-13 10:54:41.000000 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-13 10:54:41.000000 mixture-of-depth-1.1.0/mixture_of_depth.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-13 10:54:41.040164 mixture-of-depth-1.1.0/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-13 10:54:15.000000 mixture-of-depth-1.1.0/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:55:37.943929 mixture-of-depth-1.1.1/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:55:37.939928 mixture-of-depth-1.1.1/MoD/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4517 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.1/MoD/MoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.1/MoD/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:55:37.939928 mixture-of-depth-1.1.1/MoD/modeling/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.1/MoD/modeling/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.1/MoD/modeling/automodeling.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:55:37.943929 mixture-of-depth-1.1.1/MoD/modeling/models/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/BloomMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    75772 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/FalconMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/GemmaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/LlamaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/MistralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.1/MoD/modeling/models/MixtralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    68583 2024-04-13 10:27:42.000000 mixture-of-depth-1.1.1/MoD/modeling/models/PhiMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.1/MoD/modeling/models/QwenMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73609 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.1/MoD/modeling/models/QwenMoEMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.1/MoD/modeling/models/StarCoderMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.1/MoD/modeling/models/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-13 10:55:37.943929 mixture-of-depth-1.1.1/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2415 2024-04-13 10:55:20.000000 mixture-of-depth-1.1.1/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-13 10:55:37.943929 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-13 10:55:37.000000 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-13 10:55:37.000000 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-13 10:55:37.000000 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-13 10:55:37.000000 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-13 10:55:37.000000 mixture-of-depth-1.1.1/mixture_of_depth.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-13 10:55:37.943929 mixture-of-depth-1.1.1/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-13 10:55:28.000000 mixture-of-depth-1.1.1/setup.py
```

### Comparing `mixture-of-depth-1.1.0/MoD/MoD.py` & `mixture-of-depth-1.1.1/MoD/MoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/automodeling.py` & `mixture-of-depth-1.1.1/MoD/modeling/automodeling.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/BloomMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/BloomMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/FalconMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/FalconMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/GemmaMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/GemmaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/LlamaMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/LlamaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/MistralMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/MistralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/MixtralMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/MixtralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/PhiMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/PhiMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/QwenMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/QwenMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/QwenMoEMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/QwenMoEMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/MoD/modeling/models/StarCoderMoD.py` & `mixture-of-depth-1.1.1/MoD/modeling/models/StarCoderMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/PKG-INFO` & `mixture-of-depth-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,19 +18,34 @@
 ## Introduction
 This is an unofficial implementation for the paper [Mixture-of-Depths: Dynamically allocating compute in transformer-based language models](https://arxiv.org/abs/2404.02258)
 
 ## Currently supported models
 
 | Model  | Supported? |
 | ------------- | ------------- |
-| Mistral  | ✅  |
-| Mixtral  | ❌  |
-| LLama2  | ✅  |
-| Gemma  | ✅  |
-| Solar  | ❌  |
+| Mistral  |  ✅ |
+| Mixtral  |  ✅ |
+| LLama  |  ✅ |
+| LLama2  |  ✅ |
+| Gemma  |  ✅ |
+| BLOOMZ  |  ✅ |
+| BLOOM  |  ✅ |
+| DeepSeek  |  ✅ |
+| Phi (1.5 & 2)  |  ✅ |
+| Qwen2  |  ✅ |
+| StarCoder2  |  ✅ |
+| Qwen2-MoE  |  ❓ |
+| Solar  |  ❓ |
+| Baichuan  |  ❌ |
+| ChatGLM3  |  ❌ |
+| InternLM  |  ❌ |
+| Olmo  |  ❌ |
+| XVERSE  |  ❌ |
+| Yi  |  ❌ |
+| Yuan  |  ❌ |
 
 ## 💾 Installation
 ```bash
 pip install mixture-of-depth
 ```
 Both **Linux**, **Windows** and **MacOS** are supported.
 ## 🏁 Quick Start
```

### Comparing `mixture-of-depth-1.1.0/README.md` & `mixture-of-depth-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,34 @@
 ## Introduction
 This is an unofficial implementation for the paper [Mixture-of-Depths: Dynamically allocating compute in transformer-based language models](https://arxiv.org/abs/2404.02258)
 
 ## Currently supported models
 
 | Model  | Supported? |
 | ------------- | ------------- |
-| Mistral  | ✅  |
-| Mixtral  | ❌  |
-| LLama2  | ✅  |
-| Gemma  | ✅  |
-| Solar  | ❌  |
+| Mistral  |  ✅ |
+| Mixtral  |  ✅ |
+| LLama  |  ✅ |
+| LLama2  |  ✅ |
+| Gemma  |  ✅ |
+| BLOOMZ  |  ✅ |
+| BLOOM  |  ✅ |
+| DeepSeek  |  ✅ |
+| Phi (1.5 & 2)  |  ✅ |
+| Qwen2  |  ✅ |
+| StarCoder2  |  ✅ |
+| Qwen2-MoE  |  ❓ |
+| Solar  |  ❓ |
+| Baichuan  |  ❌ |
+| ChatGLM3  |  ❌ |
+| InternLM  |  ❌ |
+| Olmo  |  ❌ |
+| XVERSE  |  ❌ |
+| Yi  |  ❌ |
+| Yuan  |  ❌ |
 
 ## 💾 Installation
 ```bash
 pip install mixture-of-depth
 ```
 Both **Linux**, **Windows** and **MacOS** are supported.
 ## 🏁 Quick Start
@@ -57,8 +72,8 @@
   title={Unofficial implementation for the paper "Mixture-of-Depths"},
   author={AstraMind AI},
   journal={https://github.com/astramind-ai/Mixture-of-depths},
   year={2024}
 }
 ```
 ## Support
-For questions, issues, or support, please open an issue on our GitHub repository.
+For questions, issues, or support, please open an issue on our GitHub repository.
```

### Comparing `mixture-of-depth-1.1.0/mixture_of_depth.egg-info/PKG-INFO` & `mixture-of-depth-1.1.1/mixture_of_depth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,19 +18,34 @@
 ## Introduction
 This is an unofficial implementation for the paper [Mixture-of-Depths: Dynamically allocating compute in transformer-based language models](https://arxiv.org/abs/2404.02258)
 
 ## Currently supported models
 
 | Model  | Supported? |
 | ------------- | ------------- |
-| Mistral  | ✅  |
-| Mixtral  | ❌  |
-| LLama2  | ✅  |
-| Gemma  | ✅  |
-| Solar  | ❌  |
+| Mistral  |  ✅ |
+| Mixtral  |  ✅ |
+| LLama  |  ✅ |
+| LLama2  |  ✅ |
+| Gemma  |  ✅ |
+| BLOOMZ  |  ✅ |
+| BLOOM  |  ✅ |
+| DeepSeek  |  ✅ |
+| Phi (1.5 & 2)  |  ✅ |
+| Qwen2  |  ✅ |
+| StarCoder2  |  ✅ |
+| Qwen2-MoE  |  ❓ |
+| Solar  |  ❓ |
+| Baichuan  |  ❌ |
+| ChatGLM3  |  ❌ |
+| InternLM  |  ❌ |
+| Olmo  |  ❌ |
+| XVERSE  |  ❌ |
+| Yi  |  ❌ |
+| Yuan  |  ❌ |
 
 ## 💾 Installation
 ```bash
 pip install mixture-of-depth
 ```
 Both **Linux**, **Windows** and **MacOS** are supported.
 ## 🏁 Quick Start
```

### Comparing `mixture-of-depth-1.1.0/mixture_of_depth.egg-info/SOURCES.txt` & `mixture-of-depth-1.1.1/mixture_of_depth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.0/setup.py` & `mixture-of-depth-1.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mixture-of-depth',
-    version='1.1.0',
+    version='1.1.1',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/Mixture-of-depths',
     packages=find_packages(),
```

