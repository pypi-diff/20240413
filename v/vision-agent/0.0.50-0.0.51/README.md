# Comparing `tmp/vision_agent-0.0.50.tar.gz` & `tmp/vision_agent-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.50.tar", max compression
+gzip compressed data, was "vision_agent-0.0.51.tar", max compression
```

## Comparing `vision_agent-0.0.50.tar` & `vision_agent-0.0.51.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-04-11 17:26:24.250919 vision_agent-0.0.50/LICENSE
--rw-r--r--   0        0        0     4993 2024-04-11 17:26:24.250919 vision_agent-0.0.50/README.md
--rw-r--r--   0        0        0     2166 2024-04-11 17:26:24.818924 vision_agent-0.0.50/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4519 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    19104 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6192 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4436 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     9535 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    25644 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-04-11 17:26:24.262919 vision_agent-0.0.50/vision_agent/tools/video.py
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 vision_agent-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 23:26:59.794842 vision_agent-0.0.51/LICENSE
+-rw-r--r--   0        0        0     4993 2024-04-11 23:26:59.794842 vision_agent-0.0.51/README.md
+-rw-r--r--   0        0        0     2166 2024-04-11 23:27:00.370843 vision_agent-0.0.51/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4519 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    19103 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6192 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-11 23:26:59.806842 vision_agent-0.0.51/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4436 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     9535 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    25644 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-11 23:26:59.810842 vision_agent-0.0.51/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 vision_agent-0.0.51/PKG-INFO
```

### Comparing `vision_agent-0.0.50/LICENSE` & `vision_agent-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/README.md` & `vision_agent-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/pyproject.toml` & `vision_agent-0.0.51/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.50"
+version = "0.0.51"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.50/vision_agent/agent/agent.py` & `vision_agent-0.0.51/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/agent/easytool.py` & `vision_agent-0.0.51/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.51/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/agent/reflexion.py` & `vision_agent-0.0.51/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.51/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.51/vision_agent/agent/vision_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
             self.log_progress(f"Reflection: {reflection}")
             if parse_reflect(reflection):
                 break
             else:
                 reflections += reflection
         # '<ANSWER>' is a symbol to indicate the end of the chat, which is useful for streaming logs.
         self.log_progress(
-            f"The Vision Agent has concluded this chat. <ANSWER>{final_answer}</<ANSWER>"
+            f"The Vision Agent has concluded this chat. <ANSWER>{final_answer}</ANSWER>"
         )
         return final_answer, all_tool_results
 
     def chat(
         self, chat: List[Dict[str, str]], image: Optional[Union[str, Path]] = None
     ) -> str:
         answer, _ = self.chat_with_workflow(chat, image=image)
```

### Comparing `vision_agent-0.0.50/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.51/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/data/data.py` & `vision_agent-0.0.51/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/emb/emb.py` & `vision_agent-0.0.51/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/image_utils.py` & `vision_agent-0.0.51/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/llm/llm.py` & `vision_agent-0.0.51/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/lmm/lmm.py` & `vision_agent-0.0.51/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/tools/prompts.py` & `vision_agent-0.0.51/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/tools/tools.py` & `vision_agent-0.0.51/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/vision_agent/tools/video.py` & `vision_agent-0.0.51/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.50/PKG-INFO` & `vision_agent-0.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.50
+Version: 0.0.51
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

