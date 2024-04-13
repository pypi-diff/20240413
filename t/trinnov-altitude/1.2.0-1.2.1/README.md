# Comparing `tmp/trinnov_altitude-1.2.0.tar.gz` & `tmp/trinnov_altitude-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov_altitude-1.2.0.tar", last modified: Sat Apr 13 19:07:10 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.2.1.tar", last modified: Sat Apr 13 19:14:31 2024, max compression
```

## Comparing `trinnov_altitude-1.2.0.tar` & `trinnov_altitude-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.118885 trinnov_altitude-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.118885 trinnov_altitude-1.2.0/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26147 2024-04-13 19:07:05.000000 trinnov_altitude-1.2.0/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:07:10.122885 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:07:10.000000 trinnov_altitude-1.2.0/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.568385 trinnov_altitude-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.568385 trinnov_altitude-1.2.1/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26143 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov_altitude-1.2.0/LICENSE` & `trinnov_altitude-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/PKG-INFO` & `trinnov_altitude-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.0
+Version: 1.2.1
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov_altitude-1.2.0/README.md` & `trinnov_altitude-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/setup.cfg` & `trinnov_altitude-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/tests/test_trinnov_altitude.py` & `trinnov_altitude-1.2.1/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude/const.py` & `trinnov_altitude-1.2.1/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude/exceptions.py` & `trinnov_altitude-1.2.1/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude/messages.py` & `trinnov_altitude-1.2.1/trinnov_altitude/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 class Message:
     pass
 
 
 class AudiosyncMessage(Message):
-    def __init__(self, mode: bool) -> None:
+    def __init__(self, mode: str) -> None:
         self.mode = mode
 
 
 class BypassMessage(Message):
     def __init__(self, state: bool) -> None:
         self.state = state
```

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude/mocks.py` & `trinnov_altitude-1.2.1/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude/trinnov_altitude.py` & `trinnov_altitude-1.2.1/trinnov_altitude/trinnov_altitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Implements the Trinnov Altitude processor automation protocol over TCP/IP
 """
 
 import asyncio
-from collections.abc import Callable, Set
+from collections.abc import Callable
 import logging
 import re
-from typing import Dict, TypeAlias
+from typing import TypeAlias
 from wakeonlan import send_magic_packet
 
 from trinnov_altitude import const, exceptions, messages
 
 Callback: TypeAlias = Callable[[str, messages.Message | None], None]
 
 
@@ -74,30 +74,30 @@
         self.port = port
         self.mac = mac
         self.client_id = client_id
         self.timeout = timeout
         self.logger = logger
 
         # State
-        self.audiosync: bool | None = None
+        self.audiosync: str | None = None
         self.bypass: bool | None = None
         self.decoder: str | None = None
         self.dim: bool | None = None
         self.id: str | None = None
         self.mute: bool | None = None
         self.preset: str | None = None
-        self.presets: Dict[int, str] = {}
+        self.presets: dict[int, str] = {}
         self.source: str | None = None
-        self.sources: Dict[int, str] = {}
+        self.sources: dict[int, str] = {}
         self.upmixer: str | None = None
         self.version: str | None = None
         self.volume: float | None = None
 
         # Utility
-        self._callbacks: Set[Callback] = set()
+        self._callbacks: set[Callback] = set()
         self._initial_sync = asyncio.Event()
         self._reader: asyncio.StreamReader | None = None
         self._response_handler_task: asyncio.Task | None = None
         self._writer: asyncio.StreamWriter | None = None
 
     # --------------------------
     # Connection
@@ -530,15 +530,15 @@
 
     async def source_set_by_name(
         self, name: str, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
         """
         Set the source identified by `name` from `sources`.
         """
-        for source_id, source_name in self.sources:
+        for source_id, source_name in self.sources.items():
             if source_name == name:
                 await self.source_set(source_id)
                 return
 
     async def time_alignment_off(
         self, timeout: int | float | None = USE_DEFAULT_TIMEOUT
     ):
```

### Comparing `trinnov_altitude-1.2.0/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1.2.1/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.0
+Version: 1.2.1
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

