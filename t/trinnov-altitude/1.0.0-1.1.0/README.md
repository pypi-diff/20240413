# Comparing `tmp/trinnov_altitude-1.tar.gz` & `tmp/trinnov_altitude-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov_altitude-1.tar", last modified: Fri Apr 12 21:54:51 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.1.0.tar", last modified: Sat Apr 13 17:48:30 2024, max compression
```

## Comparing `trinnov_altitude-1.tar` & `trinnov_altitude-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.086360 trinnov_altitude-1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-12 21:54:45.000000 trinnov_altitude-1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-12 21:54:51.086360 trinnov_altitude-1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-12 21:54:45.000000 trinnov_altitude-1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 21:54:45.000000 trinnov_altitude-1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-12 21:54:51.086360 trinnov_altitude-1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:54:45.000000 trinnov_altitude-1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.082360 trinnov_altitude-1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 21:54:45.000000 trinnov_altitude-1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-12 21:54:45.000000 trinnov_altitude-1/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.082360 trinnov_altitude-1/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24785 2024-04-12 21:54:45.000000 trinnov_altitude-1/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:54:51.086360 trinnov_altitude-1/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 21:54:51.000000 trinnov_altitude-1/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 17:48:30.826270 trinnov_altitude-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-04-13 17:48:26.000000 trinnov_altitude-1.1.0/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:48:30.822270 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 17:48:30.000000 trinnov_altitude-1.1.0/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov_altitude-1/LICENSE` & `trinnov_altitude-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/PKG-INFO` & `trinnov_altitude-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -87,33 +87,35 @@
 
 # Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
 # Start listening for updates in an async.io Task
-altitude.start_listening(callback: callback)
+asyncio.create_task(altitude.start_listening(callback: callback))
 ```
 
 ## State
 
 State will be available shortly after connecting. When a client connects to the
 processor, it will send a list of messages reflecting the current state. The
 `start_listening` method will receive these updates in the background and sync
 your object with the processor's state.
 
 ```python
 altitude.audiosync: bool | None # Current state of audiosync
 altitude.bypass: bool | None = None # Current state of bypass
+altitude.decoder: bool | None = None # Current decoder being used
 altitude.dim: bool | None = None # Current state of dim
 altitude.id: str | None = None # Unique ID of the processor
 altitude.mute: bool | None = None # Current state of mute
 altitude.presets: dict = {} # Dictionary of all presets and their names
 altitude.source: str | None = None # Current source
 altitude.sources: dict = {} # Dictionary of all sources and their names
+altitude.upmixer: str | None = None # Current upmixer being used
 altitude.version: str | None = None # Software version of the processor
 altitude.volume: float | None = None # Current volume level in dB
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
@@ -188,15 +190,16 @@
 altitude.power_on()
 await altitude.power_off()
 ```
 
 ### Presets
 
 ```python
-await altitude.preset_load(id: int)
+await altitude.preset_get()
+await altitude.preset_set(id: int)
 ```
 
 ### Quick optimized
 
 ```python
 await altitude.quick_optimized_off()
 await altitude.quick_optimized_on()
```

### Comparing `trinnov_altitude-1/README.md` & `trinnov_altitude-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,35 @@
 
 # Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
 # Start listening for updates in an async.io Task
-altitude.start_listening(callback: callback)
+asyncio.create_task(altitude.start_listening(callback: callback))
 ```
 
 ## State
 
 State will be available shortly after connecting. When a client connects to the
 processor, it will send a list of messages reflecting the current state. The
 `start_listening` method will receive these updates in the background and sync
 your object with the processor's state.
 
 ```python
 altitude.audiosync: bool | None # Current state of audiosync
 altitude.bypass: bool | None = None # Current state of bypass
+altitude.decoder: bool | None = None # Current decoder being used
 altitude.dim: bool | None = None # Current state of dim
 altitude.id: str | None = None # Unique ID of the processor
 altitude.mute: bool | None = None # Current state of mute
 altitude.presets: dict = {} # Dictionary of all presets and their names
 altitude.source: str | None = None # Current source
 altitude.sources: dict = {} # Dictionary of all sources and their names
+altitude.upmixer: str | None = None # Current upmixer being used
 altitude.version: str | None = None # Software version of the processor
 altitude.volume: float | None = None # Current volume level in dB
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
@@ -171,15 +173,16 @@
 altitude.power_on()
 await altitude.power_off()
 ```
 
 ### Presets
 
 ```python
-await altitude.preset_load(id: int)
+await altitude.preset_get()
+await altitude.preset_set(id: int)
 ```
 
 ### Quick optimized
 
 ```python
 await altitude.quick_optimized_off()
 await altitude.quick_optimized_on()
```

### Comparing `trinnov_altitude-1/setup.cfg` & `trinnov_altitude-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/tests/test_trinnov_altitude.py` & `trinnov_altitude-1.1.0/tests/test_trinnov_altitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,11 +123,18 @@
 async def test_volume_adjust(mock_server, connected_client):
     await connected_client.volume_adjust(2)
     await asyncio.sleep(0.5)
     assert connected_client.volume == -38.0
 
 
 @pytest.mark.asyncio
+async def test_volume_percentage_set(mock_server, connected_client):
+    await connected_client.volume_percentage_set(52.86)
+    await asyncio.sleep(0.5)
+    assert connected_client.volume == -46.0
+
+
+@pytest.mark.asyncio
 async def test_volume_set(mock_server, connected_client):
     await connected_client.volume_set(-46)
     await asyncio.sleep(0.5)
     assert connected_client.volume == -46.0
```

### Comparing `trinnov_altitude-1/trinnov_altitude/const.py` & `trinnov_altitude-1.1.0/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/trinnov_altitude/exceptions.py` & `trinnov_altitude-1.1.0/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/trinnov_altitude/messages.py` & `trinnov_altitude-1.1.0/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/trinnov_altitude/mocks.py` & `trinnov_altitude-1.1.0/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1/trinnov_altitude/trinnov_altitude.py` & `trinnov_altitude-1.1.0/trinnov_altitude/trinnov_altitude.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     DEFAULT_PORT = 44100
     DEFAULT_TIMEOUT = 2.0
     ENCODING = "ascii"
     VALID_OUIS = [
         "c8:7f:54",  # ASUSTek OUI (components inside Altitudes)
         "64:98:9e",  # Trinnov's OUI
     ]
+    VOLUME_MIN = -120.0
+    VOLUME_MAX = 20.0
 
     # Use a sentinel value to signal that the DEFAULT_TIMEOUT should be used.
     # This allows users to pass None and disable the timeout to wait indefinitely.
     USE_DEFAULT_TIMEOUT = -1.0
 
     @classmethod
     def validate_mac(cls, mac_address):
@@ -229,14 +231,25 @@
         the best approach is to monitor for changes that suggest the initial
         synchronization has been completed.
         """
 
         await asyncio.wait_for(self._initial_sync.wait(), timeout)
 
     # --------------------------
+    # Properties
+    # --------------------------
+    def volume_percentage(self) -> float | None:
+        if self.volume is None:
+            return None
+
+        return (
+            (self.volume - self.VOLUME_MIN) / (self.VOLUME_MAX - self.VOLUME_MIN)
+        ) * 100
+
+    # --------------------------
     # Commands
     # --------------------------
 
     async def acoustic_correction_off(
         self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
@@ -565,14 +578,29 @@
 
     async def volume_down(self, timeout: int | float | None = USE_DEFAULT_TIMEOUT):
         """
         Lower the volume by 0.5 dB
         """
         await self.volume_adjust(-0.5, timeout)
 
+    async def volume_percentage_set(self, percentage: float):
+        """
+        Set the volume based on a percentage.
+        """
+        if not (0 <= percentage <= 100):
+            raise ValueError("Percentage must be between 0 and 100")
+
+        # Calculate the corresponding volume level from the percentage
+        volume = (
+            (percentage / 100) * (self.VOLUME_MAX - self.VOLUME_MIN)
+        ) + self.VOLUME_MIN
+        volume = round(volume, 1)
+
+        await self.volume_set(volume)
+
     async def volume_set(
         self, db: int | float, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the volume to an absolute dB value.
         """
         await self._write(f"volume {db}", timeout)
```

### Comparing `trinnov_altitude-1/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1.1.0/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -87,33 +87,35 @@
 
 # Optionally define a callback to be fired on each individual update
 def callback(message):
     # react to the change here
     pass
 
 # Start listening for updates in an async.io Task
-altitude.start_listening(callback: callback)
+asyncio.create_task(altitude.start_listening(callback: callback))
 ```
 
 ## State
 
 State will be available shortly after connecting. When a client connects to the
 processor, it will send a list of messages reflecting the current state. The
 `start_listening` method will receive these updates in the background and sync
 your object with the processor's state.
 
 ```python
 altitude.audiosync: bool | None # Current state of audiosync
 altitude.bypass: bool | None = None # Current state of bypass
+altitude.decoder: bool | None = None # Current decoder being used
 altitude.dim: bool | None = None # Current state of dim
 altitude.id: str | None = None # Unique ID of the processor
 altitude.mute: bool | None = None # Current state of mute
 altitude.presets: dict = {} # Dictionary of all presets and their names
 altitude.source: str | None = None # Current source
 altitude.sources: dict = {} # Dictionary of all sources and their names
+altitude.upmixer: str | None = None # Current upmixer being used
 altitude.version: str | None = None # Software version of the processor
 altitude.volume: float | None = None # Current volume level in dB
 ```
 
 ## Commands
 
 All commands assume you have [setup](#setup) your Trinnov Altitude client.
@@ -188,15 +190,16 @@
 altitude.power_on()
 await altitude.power_off()
 ```
 
 ### Presets
 
 ```python
-await altitude.preset_load(id: int)
+await altitude.preset_get()
+await altitude.preset_set(id: int)
 ```
 
 ### Quick optimized
 
 ```python
 await altitude.quick_optimized_off()
 await altitude.quick_optimized_on()
```

