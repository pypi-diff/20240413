# Comparing `tmp/langalf-0.0.1.tar.gz` & `tmp/langalf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langalf-0.0.1.tar", max compression
+gzip compressed data, was "langalf-0.0.2.tar", max compression
```

## Comparing `langalf-0.0.1.tar` & `langalf-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11367 2024-04-13 15:12:17.797836 langalf-0.0.1/LICENSE
--rw-r--r--   0        0        0     9036 2024-04-13 15:12:17.797836 langalf-0.0.1/Readme.md
--rw-r--r--   0        0        0        0 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/__init__.py
--rw-r--r--   0        0        0      429 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/__main__.py
--rw-r--r--   0        0        0     3473 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/app.py
--rw-r--r--   0        0        0     2234 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/http_spec.py
--rw-r--r--   0        0        0        0 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_actor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_actor/__main__.py
--rw-r--r--   0        0        0     3315 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_actor/fuzzer.py
--rw-r--r--   0        0        0     1180 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_actor/refusal.py
--rw-r--r--   0        0        0      449 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_actor/test_refusal.py
--rw-r--r--   0        0        0     3591 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_data/__init__.py
--rw-r--r--   0        0        0     8416 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_data/data.py
--rw-r--r--   0        0        0     2645 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/probe_data/stenography_fn.py
--rw-r--r--   0        0        0    26270 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/static/index.html
--rw-r--r--   0        0        0     1952 2024-04-13 15:12:17.797836 langalf-0.0.1/langalf/test_spec.py
--rw-r--r--   0        0        0     1094 2024-04-13 15:12:17.797836 langalf-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10252 1970-01-01 00:00:00.000000 langalf-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2024-04-13 15:20:26.376835 langalf-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9036 2024-04-13 15:20:26.376835 langalf-0.0.2/Readme.md
+-rw-r--r--   0        0        0        0 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/__main__.py
+-rw-r--r--   0        0        0     3522 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/app.py
+-rw-r--r--   0        0        0     2234 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/http_spec.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_actor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_actor/__main__.py
+-rw-r--r--   0        0        0     3315 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_actor/fuzzer.py
+-rw-r--r--   0        0        0     1180 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_actor/refusal.py
+-rw-r--r--   0        0        0      449 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_actor/test_refusal.py
+-rw-r--r--   0        0        0     3591 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_data/__init__.py
+-rw-r--r--   0        0        0     8416 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_data/data.py
+-rw-r--r--   0        0        0     2645 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/probe_data/stenography_fn.py
+-rw-r--r--   0        0        0    26270 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/static/index.html
+-rw-r--r--   0        0        0     1952 2024-04-13 15:20:26.376835 langalf-0.0.2/langalf/test_spec.py
+-rw-r--r--   0        0        0     1122 2024-04-13 15:20:26.376835 langalf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10273 1970-01-01 00:00:00.000000 langalf-0.0.2/PKG-INFO
```

### Comparing `langalf-0.0.1/LICENSE` & `langalf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/Readme.md` & `langalf-0.0.2/Readme.md`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/app.py` & `langalf-0.0.2/langalf/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     allow_methods=["*"],  # Allows all methods
     allow_headers=["*"],  # Allows all headers
 )
 
 
 @app.get("/")
 async def root():
-    return FileResponse("langalf/static/index.html")
+    langalf_path = Path(__file__).parent
+    return FileResponse(f"{langalf_path}/static/index.html")
 
 
 class LLMInfo(BaseModel):
     spec: str
 
 
 @app.post("/verify")
```

### Comparing `langalf-0.0.1/langalf/http_spec.py` & `langalf-0.0.2/langalf/http_spec.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/probe_actor/fuzzer.py` & `langalf-0.0.2/langalf/probe_actor/fuzzer.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/probe_actor/refusal.py` & `langalf-0.0.2/langalf/probe_actor/refusal.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/probe_data/__init__.py` & `langalf-0.0.2/langalf/probe_data/__init__.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/probe_data/data.py` & `langalf-0.0.2/langalf/probe_data/data.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/probe_data/stenography_fn.py` & `langalf-0.0.2/langalf/probe_data/stenography_fn.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/static/index.html` & `langalf-0.0.2/langalf/static/index.html`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/langalf/test_spec.py` & `langalf-0.0.2/langalf/test_spec.py`

 * *Files identical despite different names*

### Comparing `langalf-0.0.1/pyproject.toml` & `langalf-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "langalf"
-version = "0.0.1"
+version = "0.0.2"
 description = "Agentic LLM vulnerability scanner"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 repository = "https://github.com/msoedov/langalf"
 license = "MIT"
 readme = "Readme.md"
 keywords = [
     "LLM vulnerability scanner",
     "llm security",
-    "adversarial attacks",
+    "llm adversarial attacks",
     "prompt injection",
     "prompt leakage",
     "prompt injection attacks",
     "prompt leakage prevention",
     "llm vulnerabilities",
+    "owasp-llm-top-10",
 ]
 packages = [{ include = "langalf", from = "." }]
 
 
 [tool.poetry.scripts]
 langalf = "langalf.__main__:entrypoint"
```

### Comparing `langalf-0.0.1/PKG-INFO` & `langalf-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langalf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agentic LLM vulnerability scanner
 Home-page: https://github.com/msoedov/langalf
 License: MIT
-Keywords: LLM vulnerability scanner,llm security,adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities
+Keywords: LLM vulnerability scanner,llm security,llm adversarial attacks,prompt injection,prompt leakage,prompt injection attacks,prompt leakage prevention,llm vulnerabilities,owasp-llm-top-10
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
 Maintainer-email: msoedov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

