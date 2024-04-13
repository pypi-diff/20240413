# Comparing `tmp/comfy_script-0.4.5.tar.gz` & `tmp/comfy_script-0.4.6.tar.gz`

## Comparing `comfy_script-0.4.5.tar` & `comfy_script-0.4.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.5/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.5/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.5/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.5/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    42547 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.5/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.5/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.5/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.4.5/README.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 comfy_script-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 comfy_script-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.6/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.6/requirements.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.6/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.6/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    42595 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.6/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.6/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.6/LICENSE.txt
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.4.6/README.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 comfy_script-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 comfy_script-0.4.6/PKG-INFO
```

### Comparing `comfy_script-0.4.5/__init__.py` & `comfy_script-0.4.6/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/README.md` & `comfy_script-0.4.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/Runtime.md` & `comfy_script-0.4.6/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/Image/README.md` & `comfy_script-0.4.6/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/Latent/README.md` & `comfy_script-0.4.6/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/Nodes/README.md` & `comfy_script-0.4.6/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/auto-queue.png` & `comfy_script-0.4.6/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/diff.png` & `comfy_script-0.4.6/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/plot.png` & `comfy_script-0.4.6/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/select.png` & `comfy_script-0.4.6/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/type-stubs.png` & `comfy_script-0.4.6/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/type-stubs2.png` & `comfy_script-0.4.6/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/workflow.png` & `comfy_script-0.4.6/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/README/workflow2.png` & `comfy_script-0.4.6/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/docs/images/Runtime/load-api-format.png` & `comfy_script-0.4.6/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/astutil.py` & `comfy_script-0.4.6/src/comfy_script/astutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 def is_xid_start(s: str) -> bool:
     return s.isidentifier()
 
 def is_xid_continue(s: str) -> bool:
     return f'_{s}'.isidentifier()
 
 def str_to_raw_id(s: str) -> str:
+    if not isinstance(s, str):
+        raise TypeError(f'Expected str, got {type(s)}: {s}')
+
     s = s.lstrip()
     if s == '':
         return '_'
 
     if s.isascii():
         s = re.sub(r'[^A-Za-z_0-9]', '_', s)
         s = re.sub(r'^[0-9]', r'_\g<0>', s, count=1)
```

### Comparing `comfy_script-0.4.5/src/comfy_script/client/__init__.py` & `comfy_script-0.4.6/src/comfy_script/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 import asyncio
 import nest_asyncio
 import aiohttp
 from yarl import URL
 
 nest_asyncio.apply()
 
-client: Client | None = None
-'''The global client object.'''
-
 class Client:
     def __init__(
         self,
         base_url: str | URL = 'http://127.0.0.1:8188/',
         *,
         session_factory: Callable[[], aiohttp.ClientSession] = aiohttp.ClientSession
     ):
@@ -46,22 +43,29 @@
         # Do not pass base_url to ClientSession, as it only supports absolute URLs without path part
         self._session_factory = session_factory
     
     def session(self) -> aiohttp.ClientSession:
         '''Because `aiohttp.ClientSession` is not event-loop-safe (thread-safe), a new session should be created for each request to avoid potential issues. Also, `aiohttp.ClientSession` cannot be closed in a sync manner.'''
         return self._session_factory()
 
+client: Client = Client()
+'''The global client object.'''
+
 async def response_to_str(response: aiohttp.ClientResponse) -> str:
     try:
         msg = json.dumps(await response.json(), indent=2)
     except Exception as e:
         msg = str(e)
     return f'{response}{msg}'
 
 async def _get_nodes_info() -> dict:
+    '''
+    When used with standalone runtime:
+    - The result may contain tuples intead of lists.
+    '''
     # Don't use `import nodes` with `except ImportError`, `nodes` may be in `sys.path` but not loaded (#15)
     nodes = sys.modules.get('nodes')
     if nodes is not None and 'NODE_CLASS_MAPPINGS' in vars(nodes) and 'NODE_DISPLAY_NAME_MAPPINGS' in vars(nodes):
         # https://github.com/comfyanonymous/ComfyUI/blob/1b103e0cb2d7aeb05fc8b7e006d4438e7bceca20/server.py#L393-L422
         def node_info(node_class):
             obj_class = nodes.NODE_CLASS_MAPPINGS[node_class]
             info = {}
@@ -99,14 +103,18 @@
         async with session.get(f'{client.base_url}object_info') as response:
             if response.status == 200:
                 return await response.json()
             else:
                 raise Exception(f'ComfyScript: Failed to get nodes info: {await response_to_str(response)}')
 
 def get_nodes_info() -> dict:
+    '''
+    When used with standalone runtime:
+    - The result may contain tuples intead of lists.
+    '''
     return asyncio.run(_get_nodes_info())
 
 async def _get_embeddings() -> list[str]:
     folder_paths = sys.modules.get('folder_paths')
     if folder_paths is not None and 'get_filename_list' in vars(folder_paths):
         embeddings = folder_paths.get_filename_list("embeddings")
         return list(map(lambda a: os.path.splitext(a)[0], embeddings))
```

### Comparing `comfy_script-0.4.5/src/comfy_script/nodes/__init__.py` & `comfy_script-0.4.6/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/__init__.py` & `comfy_script-0.4.6/src/comfy_script/runtime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     if comfyui_started and (comfyui_base_url is not None or no_server):
         return
     comfyui_started = False
     comfyui_base_url = None
     
     if comfyui is None:
         default_comfyui = Path(__file__).resolve().parents[5]
-        if (default_comfyui / 'main.py').exists():
+        if (default_comfyui / 'comfy_extras').exists() and (default_comfyui / 'main.py').exists():
             comfyui = default_comfyui
         else:
             try:
                 import comfy
             except ImportError:
                 raise ImportError(f'ComfyUI is not found at {default_comfyui} and comfyui package')
```

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/factory.py` & `comfy_script-0.4.6/src/comfy_script/runtime/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,16 @@
 
         def type_and_hint(type_info: str | list[str | bool], name: str = None, optional: bool = False, default = None, output: bool = False) -> (type, str):
             nonlocal enum_type_stubs
 
             id = astutil.str_to_raw_id(name)
 
             c = None
-            if isinstance(type_info, list):
+            # Standalone runtime: Some nodes may use tuple for enum values, possibly for bypassing validation
+            if isinstance(type_info, list) or isinstance(type_info, tuple):
                 # Output types can also be lists (#9):
                 '''
                 {
                   "output": [
                     [
                       "cyberrealistic_v41BackToBasics.safetensors",
                       "dreamshaper_8.safetensors",
```

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/nodes.py` & `comfy_script-0.4.6/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.4.6/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.4.6/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.4.6/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.4.6/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/transpile/__init__.py` & `comfy_script-0.4.6/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/transpile/prompt.py` & `comfy_script-0.4.6/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.4.6/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.4.6/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/tests/test_astutil.py` & `comfy_script-0.4.6/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/tests/transpile/bypass.json` & `comfy_script-0.4.6/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/tests/transpile/default.json` & `comfy_script-0.4.6/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/tests/transpile/test_transpiler.py` & `comfy_script-0.4.6/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/.gitignore` & `comfy_script-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/LICENSE.txt` & `comfy_script-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/README.md` & `comfy_script-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.5/pyproject.toml` & `comfy_script-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.4.5"
+version = "0.4.6"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
```

### Comparing `comfy_script-0.4.5/PKG-INFO` & `comfy_script-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
```

