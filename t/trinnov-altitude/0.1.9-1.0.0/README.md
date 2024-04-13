# Comparing `tmp/trinnov-altitude-0.1.9.tar.gz` & `tmp/trinnov_altitude-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov-altitude-0.1.9.tar", last modified: Thu Apr 11 00:41:18 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.tar", last modified: Fri Apr 12 21:54:51 2024, max compression
```

## Comparing `trinnov-altitude-0.1.9.tar` & `trinnov_altitude-1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.029314 trinnov-altitude-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19790 2024-04-11 00:41:04.000000 trinnov-altitude-0.1.9/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:41:18.033314 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 00:41:18.000000 trinnov-altitude-0.1.9/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.086360 trinnov_altitude-1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-12 21:54:45.000000 trinnov_altitude-1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-12 21:54:51.086360 trinnov_altitude-1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-12 21:54:45.000000 trinnov_altitude-1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 21:54:45.000000 trinnov_altitude-1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-12 21:54:51.086360 trinnov_altitude-1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:54:45.000000 trinnov_altitude-1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.082360 trinnov_altitude-1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 21:54:45.000000 trinnov_altitude-1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-12 21:54:45.000000 trinnov_altitude-1/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.082360 trinnov_altitude-1/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.086360 trinnov_altitude-1/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov-altitude-0.1.9/LICENSE` & `trinnov_altitude-1/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.9/PKG-INFO` & `trinnov_altitude-1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.9
+Version: 1.0.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov-altitude-0.1.9/README.md` & `trinnov_altitude-1/README.md`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.9/setup.cfg` & `trinnov_altitude-1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.9/tests/test_trinnov_altitude.py` & `trinnov_altitude-1/tests/test_trinnov_altitude.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,27 +4,37 @@
 
 from trinnov_altitude.exceptions import (
     ConnectionFailedError,
     ConnectionTimeoutError,
     InvalidMacAddressOUIError,
     MalformedMacAddressError,
 )
-from trinnov_altitude.messages import Message, OKMessage
+from trinnov_altitude.messages import Message
 from trinnov_altitude.mocks import MockTrinnovAltitudeServer
 from trinnov_altitude.trinnov_altitude import TrinnovAltitude
 
 
 @pytest_asyncio.fixture
 async def mock_server():
     server = MockTrinnovAltitudeServer()
     await server.start_server()
     yield server
     await server.stop_server()
 
 
+@pytest_asyncio.fixture
+async def connected_client():
+    client = TrinnovAltitude(host="localhost")
+    await client.connect()
+    client.start_listening()
+    yield client
+    await client.stop_listening()
+    await client.disconnect()
+
+
 @pytest.mark.asyncio
 async def test_validate_mac():
     with pytest.raises(MalformedMacAddressError):
         TrinnovAltitude.validate_mac("malformed")
 
     with pytest.raises(InvalidMacAddressOUIError):
         TrinnovAltitude.validate_mac("c9:7f:32:2b:ea:f4")
@@ -43,57 +53,81 @@
 async def test_connect_timeout(mock_server):
     client = TrinnovAltitude(host="1.1.1.1")
     with pytest.raises(ConnectionTimeoutError):
         await client.connect(1)
 
 
 @pytest.mark.asyncio
-async def test_connect(mock_server):
+async def test_connect_success(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
     await client.connect()
     assert client.connected() is True
     await client.disconnect()
 
 
 @pytest.mark.asyncio
-async def test_callback(mock_server):
+async def test_register_callback(mock_server):
     client = TrinnovAltitude(host="localhost", port=mock_server.port)
+    client._last_event = None  # type: ignore
 
-    def _update(message: Message):
-        client._last_message = message  # type: ignore
+    def _update(event: str, message: Message | None = None):
+        client._last_event = event  # type: ignore
 
     client.register_callback(_update)
-    client.start_listening()
 
-    # Wait for listen task to process all messages
-    await asyncio.sleep(2)
+    await client.connect()
+    client.start_listening()
+    await client.wait_for_initial_sync()
+    await client.stop_listening()
     await client.disconnect()
 
-    assert isinstance(client._last_message, OKMessage)  # type: ignore
+    assert client._last_event  # type: ignore
 
 
 @pytest.mark.asyncio
-async def test_volume_adjust(mock_server):
-    client = TrinnovAltitude(host="localhost", port=mock_server.port)
-    await client.connect()
-    await client.volume_adjust(2)
+async def test_start_listening_syncs(mock_server, connected_client):
+    await asyncio.sleep(0.5)
+    assert connected_client.audiosync == "Slave"
+    assert connected_client.bypass is False
+    assert connected_client.decoder == "none"
+    assert connected_client.dim is False
+    assert connected_client.id == "10485761"
+    assert connected_client.mute is False
+    assert connected_client.preset == "Builtin"
+    assert connected_client.source == "Apple TV"
+    assert connected_client.upmixer == "none"
+    assert connected_client.version == "4.3.2rc1"
+    assert connected_client.volume == -40
 
-    # Wait for sync task
-    client.start_listening()
+
+@pytest.mark.asyncio
+async def test_start_listening_reconnects(mock_server, connected_client):
+    await connected_client.disconnect()
+    assert not connected_client.connected()
     await asyncio.sleep(0.5)
+    assert connected_client.connected()
 
-    assert client.volume == -38.0
-    await client.disconnect()
+
+# --------------------------
+# Commands
+# --------------------------
 
 
 @pytest.mark.asyncio
-async def test_volume_set(mock_server):
-    client = TrinnovAltitude(host="localhost", port=mock_server.port)
-    await client.connect()
-    await client.volume_set(-46)
+async def test_power_off(mock_server, connected_client):
+    await connected_client.power_off()
+    await asyncio.sleep(1)
+    assert not connected_client.connected()
 
-    # Wait for sync task
-    client.start_listening()
+
+@pytest.mark.asyncio
+async def test_volume_adjust(mock_server, connected_client):
+    await connected_client.volume_adjust(2)
     await asyncio.sleep(0.5)
+    assert connected_client.volume == -38.0
 
-    assert client.volume == -46.0
-    await client.disconnect()
+
+@pytest.mark.asyncio
+async def test_volume_set(mock_server, connected_client):
+    await connected_client.volume_set(-46)
+    await asyncio.sleep(0.5)
+    assert connected_client.volume == -46.0
```

### Comparing `trinnov-altitude-0.1.9/trinnov_altitude/const.py` & `trinnov_altitude-1/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov-altitude-0.1.9/trinnov_altitude/exceptions.py` & `trinnov_altitude-1/trinnov_altitude/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,12 @@
         message="You must supply a mac address up instantiation to power on the Trinnov Altitude.?",
     ):
         self.message = message
         super().__init__(self.message)
 
 
 class NotConnectedError(Exception):
-    """Raised when an operation is performed that requires a connect and none is present."""
+    """Raised the client is not connected and an operation requires a connection."""
 
-    def __init__(
-        self, message="Not connected to Trinnov Altitude. Did you call `connect()`?"
-    ):
+    def __init__(self, message="Not connected to Trinnov Altitude."):
         self.message = message
         super().__init__(self.message)
```

### Comparing `trinnov-altitude-0.1.9/trinnov_altitude/messages.py` & `trinnov_altitude-1/trinnov_altitude/messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 from __future__ import annotations
 
 import re
 
 
-def message_factory(message) -> Message | None:  # noqa: C901
-    if match := re.match(r"^AUDIOSYNC\s(0|1)", message):
-        state = bool(int(match.group(1)))
-        return AudiosyncMessage(state)
+def message_factory(message) -> Message:  # noqa: C901
+    if match := re.match(r"^AUDIOSYNC\s(.*)", message):
+        mode = match.group(1)
+        return AudiosyncMessage(mode)
     elif match := re.match(r"^BYPASS\s(0|1)", message):
         state = bool(int(match.group(1)))
         return BypassMessage(state)
+    elif match := re.match(r"^CURRENT_PRESET\s(-?\d+)", message):
+        # A -1 will be sent, which means the built-in preset is being used
+        state = max(0, int(match.group(1)))
+        return CurrentPresetMessage(state)
+    elif match := re.match(r"^CURRENT_PROFILE\s(-?\d+)", message):
+        state = int(match.group(1))
+        return CurrentSourceMessage(state)
+    elif match := re.match(
+        r"DECODER NONAUDIO (\d+) PLAYABLE (\d+) DECODER (\w+) UPMIXER (\w+)", message
+    ):
+        nonaudio = bool(int(match.group(1)))
+        playable = bool(int(match.group(2)))
+        decoder = match.group(3)
+        upmixer = match.group(4)
+        return DecoderMessage(nonaudio, playable, decoder, upmixer)
     elif match := re.match(r"^DIM\s(-?\d+)", message):
         state = bool(int(match.group(1)))
         return DimMessage(state)
     elif match := re.match(r"^ERROR: (.*)", message):
         error = match.group(1)
         return ErrorMessage(error)
     elif match := re.match(r"^LABEL\s(-?\d+): (.*)", message):
@@ -43,31 +58,51 @@
         r"^Welcome on Trinnov Optimizer \(Version (\S+), ID (\d+)\)",
         message,
     ):
         version = match.group(1)
         id = match.group(2)
         return WelcomeMessage(version, id)
     else:
-        return None
+        return UnknownMessage(message)
 
 
 class Message:
     pass
 
 
 class AudiosyncMessage(Message):
-    def __init__(self, state: bool) -> None:
-        self.state = state
+    def __init__(self, mode: bool) -> None:
+        self.mode = mode
 
 
 class BypassMessage(Message):
     def __init__(self, state: bool) -> None:
         self.state = state
 
 
+class CurrentPresetMessage(Message):
+    def __init__(self, index: int) -> None:
+        self.index = index
+
+
+class CurrentSourceMessage(Message):
+    def __init__(self, index: int) -> None:
+        self.index = index
+
+
+class DecoderMessage(Message):
+    def __init__(
+        self, nonaudio: bool, playable: bool, decoder: str, upmixer: str
+    ) -> None:
+        self.nonaudio = nonaudio
+        self.playable = playable
+        self.decoder = decoder
+        self.upmixer = upmixer
+
+
 class DimMessage(Message):
     def __init__(self, state: bool) -> None:
         self.state = state
 
 
 class ErrorMessage(Message):
     def __init__(self, error: str) -> None:
@@ -104,14 +139,19 @@
         self.name = name
 
 
 class SourcesClearMessage(Message):
     pass
 
 
+class UnknownMessage(Message):
+    def __init__(self, raw_message: str) -> None:
+        self.raw_message = raw_message
+
+
 class VolumeMessage(Message):
     def __init__(self, volume: float) -> None:
         self.volume = volume
 
 
 class WelcomeMessage(Message):
     def __init__(self, version: str, id: str) -> None:
```

### Comparing `trinnov-altitude-0.1.9/trinnov_altitude/mocks.py` & `trinnov_altitude-1/trinnov_altitude/mocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         "CURRENT_SOURCE_FORMAT_NAME Atmos narrow",
         "CURRENT_SOURCE_CHANNELS_ORDER_IS_DCI 0",
         "CURRENT_SOURCE_CHANNELS_ORDER L-R-C-Ls-Rs-Lrs-Rrs-Ltm-Rtm-LFE",
         "START_RUNNING",
         "CALIBRATION_DONE",
         "STOP_COMPUTING",
         "REMAPPING_MODE none",
+        "MON_VOL -40.0",
+        "VOLUME -40.0",
+        "DISPLAY_VOLUME -40.0",
         "MON_REMOTE_SPKER_MAIN -1",
         "MON_REMOTE_SPKER_ALT1 -1",
         "MON_REMOTE_SPKER_ALT2 -1",
         "MON_REMOTE_MAINSRC1 -1",
         "MON_REMOTE_MAINSRC2 -1",
         "MON_REMOTE_MAINSRC3 -1",
         "MON_REMOTE_MAINSRC4 -1",
@@ -47,14 +50,17 @@
         "MON_REMOTE_CUEIN2 -1",
         "MON_REMOTE_CUEIN3 -1",
         "MON_REMOTE_CUEOUT1 -1",
         "MON_REMOTE_CUEOUT2 -1",
         "MON_REMOTE_CUEOUT3 -1",
         "MON_REMOTE_CUEOUT4 -1",
         "MON_REMOTE_CUEOUT5 -1",
+        "BYPASS 0",
+        "DIM 0",
+        "MUTE 0",
         "FAV_LIGHT 0",
         "RIAA_PHONO 0",
         'NETSTATUS ETH LINK "Connected" DHCP "1" IP "192.168.60.90" '
         'NETMASK "255.255.255.0" GATEWAY "192.168.60.1" DNS "192.168.60.1"',
         'NETSTATUS WLAN WLANMODE "ap" LINK "Disconnected" SSID "" AP_SSID '
         '"Altitude-2541" AP_PASSWORD "abc" AP_IP "192.168.12.101" AP_NETMASK '
         '"255.255.255.0" IP "0.0.0.0" NETMASK "0.0.0.0" WPA_STATE ""',
@@ -96,14 +102,16 @@
         "PROFILE 29: ANALOG SE4 IN",
         "PROFILE 30: ROON",
         "OK",
         "SRATE 48000",
         "AUDIOSYNC_STATUS 0",
         "DECODER NONAUDIO 1 PLAYABLE 0 DECODER none UPMIXER none",
         "AUDIOSYNC Slave",
+        "CURRENT_PROFILE 1",
+        "CURRENT_PRESET -1",
     ]
 
     def __init__(self, host=DEFAULT_HOST, port=TrinnovAltitude.DEFAULT_PORT):
         # Configuration
         self.host = host
         self.port = port
         self.server = None
@@ -145,14 +153,15 @@
         self.logger.info("Mock server stopped")
 
     async def handle_client(self, reader, writer):
         self.logger.debug("Client connected")
 
         task = asyncio.current_task()
         self.active_handlers.add(task)
+        power_off = False
 
         try:
             # When you connect to an Altitude it will send a welcome message with
             # the firmware vesion and ID of the unit.
             writer.write(
                 b"Welcome on Trinnov Optimizer (Version 4.3.2rc1, ID 10485761)\n"
             )
@@ -170,31 +179,41 @@
             # Listen for messages
             while True:
                 message_bytes = await reader.readline()
                 if not message_bytes:
                     break
 
                 message = message_bytes.decode(self.ENCODING).strip()
-                responses = self._handle_message(message)
+                if message == "power_off_SECURED_FHZMCH48FE":
+                    self.logger.info("Received shut down signal")
+                    power_off = True
+                    break
+                elif message == "bye":
+                    break
+                else:
+                    responses = self._handle_message(message)
 
-                for response in responses:
-                    writer.write(f"{response}\n".encode(self.ENCODING))
-                    await writer.drain()
-        except asyncio.CancelledError:
+                    for response in responses:
+                        writer.write(f"{response}\n".encode(self.ENCODING))
+                        await writer.drain()
+        except (asyncio.CancelledError, OSError):
             pass
         finally:
             self.active_handlers.discard(task)
             writer.close()
 
             try:
                 await writer.wait_closed()
-            except ConnectionResetError:
+            except OSError:
                 pass
 
-        self.logger.info("Client disconnected")
+            self.logger.info("Client disconnected")
+
+            if power_off:
+                await self.stop_server()
 
     def _handle_message(self, message):
         self.logger.debug("Received message from client: %s", message)
 
         if match := re.match(r"^dvolume\s(-?\d+(\.\d+)?)", message):
             delta = float(match.group(1))
             self.volume += delta
```

### Comparing `trinnov-altitude-0.1.9/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 0.1.9
+Version: 1.0.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

