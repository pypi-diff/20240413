# Comparing `tmp/maitai-sdk-python-0.420.tar.gz` & `tmp/maitai-sdk-python-0.422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai-sdk-python-0.420.tar", last modified: Fri Apr 12 15:28:18 2024, max compression
+gzip compressed data, was "maitai-sdk-python-0.422.tar", last modified: Sat Apr 13 20:55:36 2024, max compression
```

## Comparing `maitai-sdk-python-0.420.tar` & `maitai-sdk-python-0.422.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.936898 maitai-sdk-python-0.420/
--rw-rw-rw-   0        0        0      356 2024-04-12 15:28:18.934899 maitai-sdk-python-0.420/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai-sdk-python-0.420/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.899668 maitai-sdk-python-0.420/maitai/
--rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai-sdk-python-0.420/maitai/__init__.py
--rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai-sdk-python-0.420/maitai/_config.py
--rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.420/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     7137 2024-04-09 05:44:47.000000 maitai-sdk-python-0.420/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.420/maitai/_loadable.py
--rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai-sdk-python-0.420/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.932899 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      356 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 15:28:18.937898 maitai-sdk-python-0.420/setup.cfg
--rw-rw-rw-   0        0        0      554 2024-04-12 15:27:37.000000 maitai-sdk-python-0.420/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.837799 maitai-sdk-python-0.422/
+-rw-rw-rw-   0        0        0      380 2024-04-13 20:55:36.835799 maitai-sdk-python-0.422/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai-sdk-python-0.422/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.820799 maitai-sdk-python-0.422/maitai/
+-rw-rw-rw-   0        0        0      327 2024-04-13 18:48:05.000000 maitai-sdk-python-0.422/maitai/__init__.py
+-rw-rw-rw-   0        0        0      413 2024-04-13 18:48:23.000000 maitai-sdk-python-0.422/maitai/_config.py
+-rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.422/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0     9656 2024-04-13 20:55:17.000000 maitai-sdk-python-0.422/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.422/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      206 2024-04-13 18:48:42.000000 maitai-sdk-python-0.422/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.834799 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 20:55:36.837799 maitai-sdk-python-0.422/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-04-13 20:02:42.000000 maitai-sdk-python-0.422/setup.py
```

### Comparing `maitai-sdk-python-0.420/README.md` & `maitai-sdk-python-0.422/README.md`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.420/maitai/_eval_request.py` & `maitai-sdk-python-0.422/maitai/_eval_request.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.420/maitai/_evaluator.py` & `maitai-sdk-python-0.422/maitai/_evaluator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,210 @@
 import json
+import asyncio
 import threading
-
-import requests
-
+import aiohttp
+import ssl
 from maitai._eval_request import EvalRequestEncoder
 from maitai._config import config
 from maitai import MaiTaiObject, EvalRequest
 
 
 class Evaluator(MaiTaiObject):
 
-    # MAITAI_HOST = 'https://maitai.ai.yewpay.com'
     MAITAI_HOST = 'https://api.dev.yewpay.com'
 
     def __init__(self):
         super().__init__()
 
     @classmethod
-    def evaluate(cls, session_id, reference_id, action_type, content):
-        eval_request: EvalRequest = cls.create_eval_request(session_id, reference_id, action_type, content)
-        cls.send_evaluation_request(eval_request)
+    def evaluate(cls, application_id, session_id, reference_id, action_type, content):
+        eval_request: EvalRequest = cls.create_eval_request(application_id, session_id, reference_id, action_type, content)
+        cls.run_async(cls.send_evaluation_request(eval_request))
 
     @classmethod
-    def create_eval_request(cls, session_id, reference_id, action_type, content):
+    def create_eval_request(cls, application_id, session_id, reference_id, action_type, content):
         if type(content) != str:
             raise Exception('Content must be a string')
         eval_request: EvalRequest = EvalRequest()
-        eval_request.application_id = config.application_id
+        eval_request.application_id = application_id
         eval_request.session_id = session_id
         eval_request.reference_id = reference_id
         eval_request.action_type = action_type
         eval_request.evaluation_content = content
         eval_request.evaluation_content_type = 'text'
         return eval_request
 
     @classmethod
-    def update_session_context(cls, session_id, context):
+    def update_session_context(cls, application_id, session_id, context):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
         session_context = {
-            'application_id': config.application_id,
+            'application_id': application_id,
             'session_id': session_id,
             'context': context
         }
-        cls.send_session_context_update(session_context)
+        cls.run_async(cls.send_session_context_update(session_context))
 
     @classmethod
-    def append_session_context(cls, session_id, context):
+    def append_session_context(cls, application_id, session_id, context):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
         session_context = {
-            'application_id': config.application_id,
+            'application_id': application_id,
             'session_id': session_id,
             'context': context
         }
-        cls.send_session_context_append(session_context)
+        cls.run_async(cls.send_session_context_append(session_context))
 
     @classmethod
-    def update_application_context(cls, context):
+    def update_application_context(cls, application_id, context):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
-        session_context = {
-            'application_id': config.application_id,
+        application_context = {
+            'application_id': application_id,
             'context': context
         }
-        cls.send_application_context_update(session_context)
+        cls.run_async(cls.send_application_context_update(application_context))
 
     @classmethod
-    def append_application_context(cls, context):
+    def append_application_context(cls, application_id, context):
         if type(context) != dict:
             raise Exception('Context must be a dictionary')
-        session_context = {
-            'application_id': config.application_id,
+        application_context = {
+            'application_id': application_id,
             'context': context
         }
-        cls.send_application_context_append(session_context)
+        cls.run_async(cls.send_application_context_append(application_context))
 
     @classmethod
-    def send_evaluation_request(cls, eval_request):
-        def send_request():
-            host = cls.MAITAI_HOST
-            url = f'{host}/evaluation/request'
-            headers = {
-                'Content-Type': 'application/json',
-                'x-api-key': config.api_key
-            }
-            response = requests.post(url, headers=headers, data=json.dumps(eval_request, cls=EvalRequestEncoder))
-            if response.status_code != 200:
-                error_text = response.text
-                print(f"Failed to send evaluation request. Status code: {response.status_code}. Error: {error_text}")
-            else:
-                print(f"Successfully sent evaluation request. Status code: {response.status_code}")
-
-        # Start a new thread to send the request without waiting for the response
-        threading.Thread(target=send_request).start()
-
-    @classmethod
-    def send_session_context_update(cls, session_context):
-        def send_context():
-            host = cls.MAITAI_HOST
-            url = f'{host}/context/session'
-            headers = {
-                'Content-Type': 'application/json',
-                'x-api-key': config.api_key
-            }
-            response = requests.put(url, headers=headers, data=json.dumps(session_context))
-            if response.status_code != 200:
-                error_text = response.text
-                print(f"Failed to send session context update. Status code: {response.status_code}. Error: {error_text}")
-            else:
-                print(f"Successfully sent session context update. Status code: {response.status_code}")
-
-        # Start a new thread to send the request without waiting for the response
-        threading.Thread(target=send_context()).start()
-
-    @classmethod
-    def send_session_context_append(cls, session_context):
-        def send_context():
-            host = cls.MAITAI_HOST
-            url = f'{host}/context/session/append'
-            headers = {
-                'Content-Type': 'application/json',
-                'x-api-key': config.api_key
-            }
-            response = requests.put(url, headers=headers, data=json.dumps(session_context))
-            if response.status_code != 200:
-                error_text = response.text
-                print(f"Failed to send session context for append. Status code: {response.status_code}. Error: {error_text}")
-            else:
-                print(f"Successfully sent session context for append. Status code: {response.status_code}")
-
-        threading.Thread(target=send_context()).start()
-
-    @classmethod
-    def send_application_context_update(cls, application_context):
-        def send_context():
-            host = cls.MAITAI_HOST
-            url = f'{host}/context/application'
-            headers = {
-                'Content-Type': 'application/json',
-                'x-api-key': config.api_key
-            }
-            response = requests.put(url, headers=headers, data=json.dumps(application_context))
-            if response.status_code != 200:
-                error_text = response.text
-                print(f"Failed to send application context update. Status code: {response.status_code}. Error: {error_text}")
-            else:
-                print(f"Successfully sent application context update. Status code: {response.status_code}")
-
-        # Start a new thread to send the request without waiting for the response
-        threading.Thread(target=send_context()).start()
-
-    @classmethod
-    def send_application_context_append(cls, application_context):
-        def send_context():
-            host = cls.MAITAI_HOST
-            url = f'{host}/context/application/append'
-            headers = {
-                'Content-Type': 'application/json',
-                'x-api-key': config.api_key
-            }
-            response = requests.put(url, headers=headers, data=json.dumps(application_context))
-            if response.status_code != 200:
-                error_text = response.text
-                print(f"Failed to send application context for append. Status code: {response.status_code}. Error: {error_text}")
-            else:
-                print(f"Successfully sent application context for append. Status code: {response.status_code}")
+    async def send_evaluation_request(cls, eval_request):
+        async def send_request():
+            try:
+                host = cls.MAITAI_HOST
+                url = f'{host}/evaluation/request'
+                headers = {
+                    'Content-Type': 'application/json',
+                    'x-api-key': config.api_key
+                }
+                async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
+                    async with session.post(url, headers=headers, data=json.dumps(eval_request, cls=EvalRequestEncoder)) as response:
+                        if response.status != 200:
+                            error_text = await response.text()
+                            print(f"Failed to send evaluation request. Status code: {response.status}. Error: {error_text}")
+                        else:
+                            print(f"Successfully sent evaluation request. Status code: {response.status}")
+            except Exception as e:
+                print(f"An error occurred while sending evaluation request: {e}")
+
+        await send_request()
+
+    @classmethod
+    async def send_session_context_update(cls, session_context):
+        async def send_context():
+            try:
+                host = cls.MAITAI_HOST
+                url = f'{host}/context/session'
+                headers = {
+                    'Content-Type': 'application/json',
+                    'x-api-key': config.api_key
+                }
+                async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
+                    async with session.put(url, headers=headers, data=json.dumps(session_context)) as response:
+                        if response.status != 200:
+                            error_text = await response.text()
+                            print(f"Failed to send session context update. Status code: {response.status}. Error: {error_text}")
+                        else:
+                            print(f"Successfully sent session context update. Status code: {response.status}")
+            except Exception as e:
+                print(f"An error occurred while sending session context update: {e}")
+
+        await send_context()
+
+    @classmethod
+    async def send_session_context_append(cls, session_context):
+        async def send_context():
+            try:
+                host = cls.MAITAI_HOST
+                url = f'{host}/context/session/append'
+                headers = {
+                    'Content-Type': 'application/json',
+                    'x-api-key': config.api_key
+                }
+                async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
+                    async with session.put(url, headers=headers, data=json.dumps(session_context)) as response:
+                        if response.status != 200:
+                            error_text = await response.text()
+                            print(f"Failed to send session context for append. Status code: {response.status}. Error: {error_text}")
+                        else:
+                            print(f"Successfully sent session context for append. Status code: {response.status}")
+            except Exception as e:
+                print(f"An error occurred while sending session context for append: {e}")
+
+        await send_context()
+
+    @classmethod
+    async def send_application_context_update(cls, application_context):
+        async def send_context():
+            try:
+                host = cls.MAITAI_HOST
+                url = f'{host}/context/application'
+                headers = {
+                    'Content-Type': 'application/json',
+                    'x-api-key': config.api_key
+                }
+                async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
+                    async with session.put(url, headers=headers, data=json.dumps(application_context)) as response:
+                        if response.status != 200:
+                            error_text = await response.text()
+                            print(f"Failed to send application context update. Status code: {response.status}. Error: {error_text}")
+                        else:
+                            print(f"Successfully sent application context update. Status code: {response.status}")
+            except Exception as e:
+                print(f"An error occurred while sending application context update: {e}")
+
+        await send_context()
+
+    @classmethod
+    async def send_application_context_append(cls, application_context):
+        async def send_context():
+            try:
+                host = cls.MAITAI_HOST
+                url = f'{host}/context/application/append'
+                headers = {
+                    'Content-Type': 'application/json',
+                    'x-api-key': config.api_key
+                }
+                async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
+                    async with session.put(url, headers=headers, data=json.dumps(application_context)) as response:
+                        if response.status != 200:
+                            error_text = await response.text()
+                            print(f"Failed to send application context for append. Status code: {response.status}. Error: {error_text}")
+                        else:
+                            print(f"Successfully sent application context for append. Status code: {response.status}")
+            except Exception as e:
+                print(f"An error occurred while sending application context for append: {e}")
+
+        await send_context()
+        
+    @classmethod
+    def run_async(cls, coro):
+        """
+        Modified helper method to run coroutine in a background thread if not already in an asyncio loop,
+        otherwise just run it. This allows for both asyncio and non-asyncio applications to use this method.
+        """
+        try:
+            loop = asyncio.get_running_loop()
+        except RuntimeError:  # No running event loop
+            loop = None
+
+        if loop and loop.is_running():
+            # We are in an asyncio loop, schedule coroutine execution
+            asyncio.create_task(coro, name='maitai')
+        else:
+            # Not in an asyncio loop, run in a new event loop in a background thread
+            def run():
+                new_loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(new_loop)
+                new_loop.run_until_complete(coro)
+                new_loop.close()
+            threading.Thread(target=run).start()
 
-        threading.Thread(target=send_context()).start()
```

### Comparing `maitai-sdk-python-0.420/maitai/_loadable.py` & `maitai-sdk-python-0.422/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.420/setup.py` & `maitai-sdk-python-0.422/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai-sdk-python',
-    version='0.420',
+    version='0.422',
     packages=find_packages(),
     install_requires=[
         'requests',
+        'aiohttp'
     ],
     # Optional metadata
     author='Christian DalSanto',
     author_email='christian@yewpay.com',
     description='MaiTai SDK for Python',
     url='https://github.com/yewpay/maitai-sdk-python',
     license='MIT',
```

