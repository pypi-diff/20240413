# Comparing `tmp/trinnov_altitude-1.1.0.tar.gz` & `tmp/trinnov_altitude-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov_altitude-1.1.0.tar", last modified: Sat Apr 13 17:48:30 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.2.0.tar", last modified: Sat Apr 13 19:07:10 2024, max compression
```

## Comparing `trinnov_altitude-1.1.0.tar` & `trinnov_altitude-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 17:48:30.826270 trinnov_altitude-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.118885 trinnov_altitude-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.118885 trinnov_altitude-1.2.0/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov_altitude-1.1.0/LICENSE` & `trinnov_altitude-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/PKG-INFO` & `trinnov_altitude-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov_altitude-1.1.0/README.md` & `trinnov_altitude-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/setup.cfg` & `trinnov_altitude-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/tests/test_trinnov_altitude.py` & `trinnov_altitude-1.2.0/tests/test_trinnov_altitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     assert connected_client.bypass is False
     assert connected_client.decoder == "none"
     assert connected_client.dim is False
     assert connected_client.id == "10485761"
     assert connected_client.mute is False
     assert connected_client.preset == "Builtin"
     assert connected_client.source == "Apple TV"
+    assert connected_client.source_format == "Atmos narrow"
     assert connected_client.upmixer == "none"
     assert connected_client.version == "4.3.2rc1"
     assert connected_client.volume == -40
 
 
 @pytest.mark.asyncio
 async def test_start_listening_reconnects(mock_server, connected_client):
```

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude/const.py` & `trinnov_altitude-1.2.0/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude/exceptions.py` & `trinnov_altitude-1.2.0/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude/messages.py` & `trinnov_altitude-1.2.0/trinnov_altitude/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     elif match := re.match(r"^CURRENT_PRESET\s(-?\d+)", message):
         # A -1 will be sent, which means the built-in preset is being used
         state = max(0, int(match.group(1)))
         return CurrentPresetMessage(state)
     elif match := re.match(r"^CURRENT_PROFILE\s(-?\d+)", message):
         state = int(match.group(1))
         return CurrentSourceMessage(state)
+    elif match := re.match(r"^CURRENT_SOURCE_FORMAT_NAME\s(.*)", message):
+        format = match.group(1)
+        return CurrentSourceFormat(format)
     elif match := re.match(
-        r"DECODER NONAUDIO (\d+) PLAYABLE (\d+) DECODER (\w+) UPMIXER (\w+)", message
+        r"^DECODER NONAUDIO (\d+) PLAYABLE (\d+) DECODER (\w+) UPMIXER (\w+)", message
     ):
         nonaudio = bool(int(match.group(1)))
         playable = bool(int(match.group(2)))
         decoder = match.group(3)
         upmixer = match.group(4)
         return DecoderMessage(nonaudio, playable, decoder, upmixer)
     elif match := re.match(r"^DIM\s(-?\d+)", message):
@@ -80,14 +83,19 @@
 
 
 class CurrentPresetMessage(Message):
     def __init__(self, index: int) -> None:
         self.index = index
 
 
+class CurrentSourceFormat(Message):
+    def __init__(self, format: str) -> None:
+        self.format = format
+
+
 class CurrentSourceMessage(Message):
     def __init__(self, index: int) -> None:
         self.index = index
 
 
 class DecoderMessage(Message):
     def __init__(
```

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude/mocks.py` & `trinnov_altitude-1.2.0/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude/trinnov_altitude.py` & `trinnov_altitude-1.2.0/trinnov_altitude/trinnov_altitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         self.audiosync = None
         self.bypass = None
         self.decoder = None
         self.dim = None
         self.mute = None
         self.preset = None
         self.source = None
+        self.source_format = None
         self.upmixer = None
         self.volume = None
 
         # Fire the callback to signal a connection state change
         for callback in self._callbacks:
             callback("disconnected", None)
 
@@ -523,14 +524,25 @@
         self, id: int, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the source identified by `id`, where `0` is the first source.
         """
         await self._write(f"profile {id}", timeout)
 
+    async def source_set_by_name(
+        self, name: str, timeout: int | float | None = USE_DEFAULT_TIMEOUT
+    ):
+        """
+        Set the source identified by `name` from `sources`.
+        """
+        for source_id, source_name in self.sources:
+            if source_name == name:
+                await self.source_set(source_id)
+                return
+
     async def time_alignment_off(
         self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Turn time alignment off.
         """
         await self.time_alignment_set(False)
@@ -672,14 +684,16 @@
 
         if isinstance(message, messages.AudiosyncMessage):
             self.audiosync = message.mode
         elif isinstance(message, messages.BypassMessage):
             self.bypass = message.state
         elif isinstance(message, messages.CurrentPresetMessage):
             self.preset = self.presets.get(message.index)
+        elif isinstance(message, messages.CurrentSourceFormat):
+            self.source_format = message.format
         elif isinstance(message, messages.CurrentSourceMessage):
             self.source = self.sources.get(message.index)
         elif isinstance(message, messages.DecoderMessage):
             self.decoder = message.decoder
             self.upmixer = message.upmixer
         elif isinstance(message, messages.DimMessage):
             self.dim = message.state
```

### Comparing `trinnov_altitude-1.1.0/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1.2.0/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.1.0
+Version: 1.2.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

