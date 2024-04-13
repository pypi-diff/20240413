# Comparing `tmp/realtime-1.0.3.tar.gz` & `tmp/realtime-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime-1.0.3.tar", max compression
+gzip compressed data, was "realtime-1.0.4.tar", max compression
```

## Comparing `realtime-1.0.3.tar` & `realtime-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-03-26 21:18:08.210027 realtime-1.0.3/LICENSE
--rw-r--r--   0        0        0     1744 2024-03-26 21:18:08.210027 realtime-1.0.3/README.md
--rw-r--r--   0        0        0     1205 2024-03-26 21:18:09.102039 realtime-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      235 2024-03-26 21:18:09.102039 realtime-1.0.3/realtime/__init__.py
--rw-r--r--   0        0        0     2559 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/channel.py
--rw-r--r--   0        0        0     5739 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/connection.py
--rw-r--r--   0        0        0      403 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/exceptions.py
--rw-r--r--   0        0        0      744 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/message.py
--rw-r--r--   0        0        0     5521 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/transformers.py
--rw-r--r--   0        0        0      209 2024-03-26 21:18:08.210027 realtime-1.0.3/realtime/types.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 realtime-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-13 00:31:43.750297 realtime-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1744 2024-04-13 00:31:43.750297 realtime-1.0.4/README.md
+-rw-r--r--   0        0        0     1206 2024-04-13 00:31:44.574297 realtime-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      235 2024-04-13 00:31:44.574297 realtime-1.0.4/realtime/__init__.py
+-rw-r--r--   0        0        0     2559 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/channel.py
+-rw-r--r--   0        0        0     5744 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/connection.py
+-rw-r--r--   0        0        0      403 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/exceptions.py
+-rw-r--r--   0        0        0      744 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/message.py
+-rw-r--r--   0        0        0     5521 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/transformers.py
+-rw-r--r--   0        0        0      209 2024-04-13 00:31:43.754297 realtime-1.0.4/realtime/types.py
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 realtime-1.0.4/PKG-INFO
```

### Comparing `realtime-1.0.3/LICENSE` & `realtime-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime-1.0.3/README.md` & `realtime-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `realtime-1.0.3/pyproject.toml` & `realtime-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "realtime"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = [
     "Joel Lee <joel@joellee.org>",
     "Andrew Smith <a.smith@silentworks.co.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/supabase-community/realtime-py"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 websockets = ">=11,<13"
 python-dateutil = "^2.8.1"
-typing-extensions = "^4.2.0"
+typing-extensions = "^4.11.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = ">=8.3,<10.0"
 black = ">=23.11,<25.0"
```

### Comparing `realtime-1.0.3/realtime/channel.py` & `realtime-1.0.4/realtime/channel.py`

 * *Files identical despite different names*

### Comparing `realtime-1.0.3/realtime/connection.py` & `realtime-1.0.4/realtime/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from typing_extensions import ParamSpec
 
 from realtime.channel import Channel
 from realtime.exceptions import NotConnectedError
 from realtime.message import HEARTBEAT_PAYLOAD, PHOENIX_CHANNEL, ChannelEvents, Message
 from realtime.types import Callback, T_ParamSpec, T_Retval
 
-logging.basicConfig(
-    format="%(asctime)s:%(levelname)s - %(message)s", level=logging.INFO
-)
-
+# logging.basicConfig(
+#     format="%(asctime)s:%(levelname)s - %(message)s", level=logging.INFO
+# )
 
 def ensure_connection(func: Callback):
     @wraps(func)
     def wrapper(*args: T_ParamSpec.args, **kwargs: T_ParamSpec.kwargs) -> T_Retval:
         if not args[0].connected:
             raise NotConnectedError(func.__name__)
```

### Comparing `realtime-1.0.3/realtime/message.py` & `realtime-1.0.4/realtime/message.py`

 * *Files identical despite different names*

### Comparing `realtime-1.0.3/realtime/transformers.py` & `realtime-1.0.4/realtime/transformers.py`

 * *Files identical despite different names*

### Comparing `realtime-1.0.3/PKG-INFO` & `realtime-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: realtime
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Home-page: https://github.com/supabase-community/realtime-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
-Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Requires-Dist: websockets (>=11,<13)
 Project-URL: Repository, https://github.com/supabase-community/realtime-py
 Description-Content-Type: text/markdown
 
 # realtime-py
 Python Client Library to interface with the Phoenix Realtime Server
```

