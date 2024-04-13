# Comparing `tmp/flapi-1.0.0.tar.gz` & `tmp/flapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flapi-1.0.0.tar", max compression
+gzip compressed data, was "flapi-1.0.1.tar", max compression
```

## Comparing `flapi-1.0.0.tar` & `flapi-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1088 2024-04-07 14:03:21.651530 flapi-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     2664 2024-04-07 14:03:21.655530 flapi-1.0.0/README.md
--rw-r--r--   0        0        0     8369 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__comms.py
--rw-r--r--   0        0        0     1551 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__context.py
--rw-r--r--   0        0        0     2220 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__decorate.py
--rw-r--r--   0        0        0     6259 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__enable.py
--rw-r--r--   0        0        0      684 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__init__.py
--rw-r--r--   0        0        0      500 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__main__.py
--rw-r--r--   0        0        0      765 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/__util.py
--rw-r--r--   0        0        0     3780 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/_consts.py
--rw-r--r--   0        0        0      199 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/__init__.py
--rw-r--r--   0        0        0      333 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/consts.py
--rw-r--r--   0        0        0     1670 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/install.py
--rw-r--r--   0        0        0     6885 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/repl.py
--rw-r--r--   0        0        0      841 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/uninstall.py
--rw-r--r--   0        0        0     1066 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/cli/util.py
--rw-r--r--   0        0        0     3474 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/errors.py
--rw-r--r--   0        0        0        0 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/py.typed
--rw-r--r--   0        0        0     3803 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/capout.py
--rw-r--r--   0        0        0     3780 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/consts.py
--rw-r--r--   0        0        0     4556 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/device_flapi_receive.py
--rw-r--r--   0        0        0     1694 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/device_flapi_respond.py
--rw-r--r--   0        0        0     5550 2024-04-07 14:03:21.655530 flapi-1.0.0/flapi/server/flapi_response.py
--rw-r--r--   0        0        0     1545 2024-04-07 14:03:21.655530 flapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 flapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-13 09:59:04.906697 flapi-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2664 2024-04-13 09:59:04.906697 flapi-1.0.1/README.md
+-rw-r--r--   0        0        0     8369 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__comms.py
+-rw-r--r--   0        0        0     1551 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__context.py
+-rw-r--r--   0        0        0     2220 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__decorate.py
+-rw-r--r--   0        0        0     6259 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__enable.py
+-rw-r--r--   0        0        0      684 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__init__.py
+-rw-r--r--   0        0        0      500 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__main__.py
+-rw-r--r--   0        0        0      765 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/__util.py
+-rw-r--r--   0        0        0     3780 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/_consts.py
+-rw-r--r--   0        0        0      199 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/consts.py
+-rw-r--r--   0        0        0     1670 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/install.py
+-rw-r--r--   0        0        0     6885 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/repl.py
+-rw-r--r--   0        0        0      841 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/uninstall.py
+-rw-r--r--   0        0        0     1066 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/cli/util.py
+-rw-r--r--   0        0        0     3474 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/errors.py
+-rw-r--r--   0        0        0        0 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/py.typed
+-rw-r--r--   0        0        0     3803 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/server/capout.py
+-rw-r--r--   0        0        0     3780 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/server/consts.py
+-rw-r--r--   0        0        0     4783 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/server/device_flapi_receive.py
+-rw-r--r--   0        0        0     2006 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/server/device_flapi_respond.py
+-rw-r--r--   0        0        0     5550 2024-04-13 09:59:04.906697 flapi-1.0.1/flapi/server/flapi_response.py
+-rw-r--r--   0        0        0     1545 2024-04-13 09:59:04.906697 flapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 flapi-1.0.1/PKG-INFO
```

### Comparing `flapi-1.0.0/LICENSE.md` & `flapi-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/README.md` & `flapi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__comms.py` & `flapi-1.0.1/flapi/__comms.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__context.py` & `flapi-1.0.1/flapi/__context.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__decorate.py` & `flapi-1.0.1/flapi/__decorate.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__enable.py` & `flapi-1.0.1/flapi/__enable.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__init__.py` & `flapi-1.0.1/flapi/__init__.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/__util.py` & `flapi-1.0.1/flapi/__util.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/_consts.py` & `flapi-1.0.1/flapi/_consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 # Flapi > Consts
 
 Constants used by Flapi
 """
 from enum import IntEnum
 
-VERSION = (1, 0, 0)
+VERSION = (1, 0, 1)
 """
 The version of Flapi in the format (major, minor, revision)
 """
 
 TIMEOUT_DURATION = 0.1
 """
 The amount of time to wait for a response before giving an error
```

### Comparing `flapi-1.0.0/flapi/cli/install.py` & `flapi-1.0.1/flapi/cli/install.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/cli/repl.py` & `flapi-1.0.1/flapi/cli/repl.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/cli/uninstall.py` & `flapi-1.0.1/flapi/cli/uninstall.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/cli/util.py` & `flapi-1.0.1/flapi/cli/util.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/errors.py` & `flapi-1.0.1/flapi/errors.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/server/capout.py` & `flapi-1.0.1/flapi/server/capout.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/flapi/server/consts.py` & `flapi-1.0.1/flapi/server/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 # Flapi > Consts
 
 Constants used by Flapi
 """
 from enum import IntEnum
 
-VERSION = (1, 0, 0)
+VERSION = (1, 0, 1)
 """
 The version of Flapi in the format (major, minor, revision)
 """
 
 TIMEOUT_DURATION = 0.1
 """
 The amount of time to wait for a response before giving an error
```

### Comparing `flapi-1.0.0/flapi/server/device_flapi_receive.py` & `flapi-1.0.1/flapi/server/device_flapi_receive.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 capout = Capout(send_stdout)
 
 
 def OnInit():
     print("\n".join([
-        "Flapi server",
+        "Flapi request server",
         f"Server version: {'.'.join(str(n) for n in consts.VERSION)}",
         f"Device name: {device.getName()}",
         f"Device assigned: {bool(device.isAssigned())}",
         f"FL Studio port number: {device.getPortNumber()}",
     ]))
 
 
@@ -93,29 +93,27 @@
     res.version_query(consts.VERSION)
 
 
 def fl_exec(res: FlapiResponse, data: bytes):
     statement = b64decode(data)
     try:
         # Exec in global scope so that the imports are remembered
-        # TODO: Give each client separate global and local scopes
         exec(statement, connected_clients[res.client_id])
     except Exception as e:
         # Something went wrong, give the error
         return res.exec(MessageStatus.ERR, e)
 
     # Operation was a success, give response
     return res.exec(MessageStatus.OK)
 
 
 def fl_eval(res: FlapiResponse, data: bytes):
     expression = b64decode(data)
     try:
         # Exec in global scope so that the imports are remembered
-        # TODO: Give each client separate global and local scopes
         result = eval(expression, connected_clients[res.client_id])
     except Exception as e:
         # Something went wrong, give the error
         return res.eval(MessageStatus.ERR, e)
 
     # Operation was a success, give response
     return res.eval(MessageStatus.OK, result)
@@ -157,14 +155,24 @@
     # Ignore messages from us, to prevent feedback
     if message_origin != MessageOrigin.CLIENT:
         return
 
     handler = message_handlers.get(message_type)
 
     if handler is None:
-        return res.fail(message_type, f"Unknown message type {message_type}")
+        log.error(f"Unknown handler for message type {message_type}")
+        return res \
+            .fail(message_type, f"Unknown message type {message_type}") \
+            .send()
 
     # Capture stdout for the duration of the operation
-    with capout(client_id):
-        handler(res, data)
+    try:
+        with capout(client_id):
+            handler(res, data)
+    except Exception as e:
+        log.error(f"Unhandled error for handler {handler}", exc_info=e)
+        res.fail(
+            message_type,
+            f"Unhandled exception in {handler}: {type(e).__name__}: {e}",
+        )
 
     res.send()
```

### Comparing `flapi-1.0.0/flapi/server/device_flapi_respond.py` & `flapi-1.0.1/flapi/server/device_flapi_respond.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 Responsible for sending response messages from the Flapi Server within FL
 Studio.
 
 It attaches to the "Flapi Response" device and sends MIDI messages back to the
 Flapi client.
 """
 import device
-from consts import MessageOrigin, MessageType, SYSEX_HEADER
+from consts import MessageOrigin, MessageType, SYSEX_HEADER, VERSION
 
 try:
     from fl_classes import FlMidiMsg
 except ImportError:
     pass
 
 
+def OnInit():
+    print("\n".join([
+        "Flapi response server",
+        f"Server version: {'.'.join(str(n) for n in VERSION)}",
+        f"Device name: {device.getName()}",
+        f"Device assigned: {bool(device.isAssigned())}",
+        f"FL Studio port number: {device.getPortNumber()}",
+    ]))
+
+
 # def print_msg(name: str, msg: bytes):
 #     print(f"{name}: {[hex(b) for b in msg]}")
 
 
 def OnSysEx(event: 'FlMidiMsg'):
-
     header = event.sysex[1:len(SYSEX_HEADER)+1]  # Sysex header
     # print_msg("Header", header)
     # Remaining sysex data
     sysex_data = event.sysex[len(SYSEX_HEADER)+1:]
     # print_msg("Data", sysex_data)
 
     # Ignore events that don't target the respond script
```

### Comparing `flapi-1.0.0/flapi/server/flapi_response.py` & `flapi-1.0.1/flapi/server/flapi_response.py`

 * *Files identical despite different names*

### Comparing `flapi-1.0.0/pyproject.toml` & `flapi-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flapi"
-version = "1.0.0"
+version = "1.0.1"
 description = "Remotely control FL Studio using the MIDI Controller Scripting API"
 authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MiguelGuthridge/Flapi"
 
 keywords = [
```

### Comparing `flapi-1.0.0/PKG-INFO` & `flapi-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Remotely control FL Studio using the MIDI Controller Scripting API
 Home-page: https://github.com/MiguelGuthridge/Flapi
 License: MIT
 Keywords: fl,studio,fl studio,midi,script,midi controller scripting,remote,remote control
 Author: Miguel Guthridge
 Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.9,<4.0
```

