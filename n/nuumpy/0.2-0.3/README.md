# Comparing `tmp/nuumpy-0.2.tar.gz` & `tmp/nuumpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuumpy-0.2.tar", last modified: Sat Apr 13 20:23:22 2024, max compression
+gzip compressed data, was "nuumpy-0.3.tar", last modified: Sat Apr 13 20:27:09 2024, max compression
```

## Comparing `nuumpy-0.2.tar` & `nuumpy-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:23:22.655265 nuumpy-0.2/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-13 20:23:22.655265 nuumpy-0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 nuumpy-0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:23:22.655265 nuumpy-0.2/nuumpy/
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-13 20:22:37.000000 nuumpy-0.2/nuumpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1163 2024-04-13 20:12:17.000000 nuumpy-0.2/nuumpy/nuumpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:23:22.655265 nuumpy-0.2/nuumpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-13 20:23:22.000000 nuumpy-0.2/nuumpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-13 20:23:22.000000 nuumpy-0.2/nuumpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 20:23:22.000000 nuumpy-0.2/nuumpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-13 20:23:22.000000 nuumpy-0.2/nuumpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 20:23:22.655265 nuumpy-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      248 2024-04-13 20:21:04.000000 nuumpy-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:27:09.965085 nuumpy-0.3/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-13 20:27:09.965085 nuumpy-0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 nuumpy-0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:27:09.965085 nuumpy-0.3/nuumpy/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-13 20:22:37.000000 nuumpy-0.3/nuumpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-13 20:26:30.000000 nuumpy-0.3/nuumpy/nuumpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:27:09.965085 nuumpy-0.3/nuumpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-13 20:27:09.000000 nuumpy-0.3/nuumpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-13 20:27:09.000000 nuumpy-0.3/nuumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 20:27:09.000000 nuumpy-0.3/nuumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-13 20:27:09.000000 nuumpy-0.3/nuumpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 20:27:09.965085 nuumpy-0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-13 20:26:58.000000 nuumpy-0.3/setup.py
```

### Comparing `nuumpy-0.2/nuumpy/nuumpy.py` & `nuumpy-0.3/nuumpy/nuumpy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 def nimpy():
     code = """
-    !pip install -Uq keras-nlp
-    !pip install -Uq keras
+!pip install -Uq keras-nlp
+!pip install -Uq keras
 
-    import keras
-    import keras_nlp
-    import numpy as np
-
-    def login_to_kaggle():
-        print('"username": "trilokvishwam", "key": "5829ba02d16cbacbda14d0b3d0570e98"')
-        import kagglehub
-        kagglehub.login()
-
-    login_to_kaggle()
-
-    gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset("gemma_instruct_2b_en")
-
-    import keras
-    import keras_nlp
-    import numpy as np
-
-    def generate_response(question):
-        prompt = """
-        You are an AI assistant designed to answer simple questions.
-        Please restrict your answer to the exact question asked.
-        Think step by step, use careful reasoning. Your name is Semban Surga
-        Question: {question}
-        Answer:
-        """
-        response = gemma_lm.generate(prompt.format(question=question), max_length=500)
-        start_idx = response.find("Answer:") + len("Answer:")
-        return response[start_idx:].strip()
-
-    def ask(question):
-        response = generate_response(question)
-        print(response)
+import keras
+import keras_nlp
+import numpy as np
+
+def login_to_kaggle():
+    print('"username": "trilokvishwam", "key": "5829ba02d16cbacbda14d0b3d0570e98"')
+    import kagglehub
+    kagglehub.login()
+
+login_to_kaggle()
+
+gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset("gemma_instruct_2b_en")
+
+import keras
+import keras_nlp
+import numpy as np
+
+def generate_response(question):
+    prompt = ""
+    You are an AI assistant designed to answer simple questions.
+    Please restrict your answer to the exact question asked.
+    Think step by step, use careful reasoning. Your name is Semban Surga
+    Question: {question}
+    Answer:
+    ""
+    response = gemma_lm.generate(prompt.format(question=question), max_length=500)
+    start_idx = response.find("Answer:") + len("Answer:")
+    return response[start_idx:].strip()
+
+def ask(question):
+    response = generate_response(question)
+    print(response)
     """
 
     print(code)
```

