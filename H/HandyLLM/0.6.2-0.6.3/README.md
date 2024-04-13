# Comparing `tmp/HandyLLM-0.6.2.tar.gz` & `tmp/HandyLLM-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.6.2.tar", last modified: Wed Apr  3 15:46:14 2024, max compression
+gzip compressed data, was "HandyLLM-0.6.3.tar", last modified: Sat Apr 13 11:22:26 2024, max compression
```

## Comparing `HandyLLM-0.6.2.tar` & `HandyLLM-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.497467 HandyLLM-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.552732 HandyLLM-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_prompt.py
```

### Comparing `HandyLLM-0.6.2/PKG-INFO` & `HandyLLM-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.6.2
+Version: 0.6.3
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.6.2/README.md` & `HandyLLM-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/pyproject.toml` & `HandyLLM-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HandyLLM-0.6.2/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.6.3/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.6.2
+Version: 0.6.3
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.6.2/src/HandyLLM.egg-info/SOURCES.txt` & `HandyLLM-0.6.3/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/_utils.py` & `HandyLLM-0.6.3/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/deprecated/api_request.py` & `HandyLLM-0.6.3/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/deprecated/openai_api.py` & `HandyLLM-0.6.3/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/endpoint_manager.py` & `HandyLLM-0.6.3/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/openai_api.py` & `HandyLLM-0.6.3/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/openai_client.py` & `HandyLLM-0.6.3/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/prompt_converter.py` & `HandyLLM-0.6.3/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/src/handyllm/requestor.py` & `HandyLLM-0.6.3/src/handyllm/requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
             return response
         except Exception as e:
             if self._exception_callback:
                 self._exception_callback(e, prepare_ret)
             raise e
 
     def _call_raw(self) -> requests.Response:
+        import requests
         response = self._sync_client.request(
             self.method,
             self.url,
             headers=self.headers,
             data=self.data,
             json=self.json_data,
             files=self.files,
@@ -228,14 +229,15 @@
             return response
         except Exception as e:
             if self._exception_callback:
                 self._exception_callback(e, prepare_ret)
             raise e
 
     async def _acall_raw(self):
+        import httpx
         request = self._async_client.build_request(
             self.method,
             self.url,
             headers=self.headers,
             data=self.data,
             json=self.json_data,
             files=self.files,
```

### Comparing `HandyLLM-0.6.2/src/handyllm/utils.py` & `HandyLLM-0.6.3/src/handyllm/utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/tests/test_azure.py` & `HandyLLM-0.6.3/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/tests/test_client_async_sync.py` & `HandyLLM-0.6.3/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/tests/test_endpoint.py` & `HandyLLM-0.6.3/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.2/tests/test_prompt.py` & `HandyLLM-0.6.3/tests/test_prompt.py`

 * *Files identical despite different names*

