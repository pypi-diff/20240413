# Comparing `tmp/robothub-2.5.6.tar.gz` & `tmp/robothub-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub-2.5.6.tar", last modified: Thu Apr  4 14:51:06 2024, max compression
+gzip compressed data, was "robothub-2.5.7.tar", last modified: Fri Apr 12 22:56:08 2024, max compression
```

## Comparing `robothub-2.5.6.tar` & `robothub-2.5.7.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-04 14:50:43.000000 robothub-2.5.6/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-04 14:50:43.000000 robothub-2.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 14:51:06.213237 robothub-2.5.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-04-04 14:50:43.000000 robothub-2.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:51:06.213237 robothub-2.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-04 14:50:43.000000 robothub-2.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.205237 robothub-2.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.209237 robothub-2.5.6/src/robothub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/application.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/frame_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/live_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/live_view_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/replay_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.209237 robothub-2.5.6/src/robothub/robothub_core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_event_typechecks.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_stop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9335 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/src/robothub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-12 22:55:46.000000 robothub-2.5.7/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-12 22:55:46.000000 robothub-2.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-12 22:56:08.306031 robothub-2.5.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-12 22:55:46.000000 robothub-2.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:56:08.306031 robothub-2.5.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-12 22:55:46.000000 robothub-2.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.298031 robothub-2.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.302031 robothub-2.5.7/src/robothub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/application.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/frame_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/live_view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.302031 robothub-2.5.7/src/robothub/replay/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/capture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/captures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/replay_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32613 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/replay_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/src/robothub/robothub_core_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_event_typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_stop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/src/robothub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_manager.py
```

### Comparing `robothub-2.5.6/LICENSE` & `robothub-2.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/PKG-INFO` & `robothub-2.5.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.6
+Version: 2.5.7
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
@@ -38,14 +38,26 @@
 
 To install this package, run the following command in your terminal window
 
 ```
 $ python3 -m pip install robothub
 ```
 
+### Building and installing locally
+
+    python setup.py sdist 
+
+it will create a __dist__ folder in the project root and in there, it will create __robothub-version.tar.gz
+
+to install it locally, use
+
+    pip install --upgrade /path/to/robothub/source/dist/robothub-2.5.4.tar.gz
+
+replace the 2.4.5 with correct version
+
 ## Examples
 
 You can find examples in the [robothub-examples](https://github.com/luxonis/robothub-examples) repository.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `robothub-2.5.6/setup.py` & `robothub-2.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub',
-    version='2.5.6',
+    version='2.5.7',
     description='RobotHub integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub camera robot hub connect agent depthai sdk',
     author='Luxonis',
```

### Comparing `robothub-2.5.6/src/robothub/__init__.py` & `robothub-2.5.7/src/robothub/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-
 from robothub.application import *
 from robothub.events import *
 from robothub.frame_buffer import *
 from robothub.live_view import *
-from robothub.replay_camera import ReplayCamera
+from robothub.replay import *
 from robothub.utils import setup_logger
 
 try:
     import blobconverter
 
     # Suppress blobconverter logs
     blobconverter.set_defaults(silent=True)
@@ -16,11 +15,11 @@
 
 # Import symbols from robothub_core and make them available under the robothub namespace
 try:
     import robothub_core as robothub
 except ImportError:
     import robothub.robothub_core_wrapper as robothub
 
-__version__ = '2.5.6'
+__version__ = "2.5.7"
 
 # Setup logging for the module
 # setup_logger(__name__)
```

### Comparing `robothub-2.5.6/src/robothub/application.py` & `robothub-2.5.7/src/robothub/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import depthai
 try:
     import robothub_core
 except ImportError:
     import robothub.robothub_core_wrapper as robothub_core
 from depthai_sdk import OakCamera
-from robothub.replay_camera import ReplayCamera
+from robothub.replay import ReplayCamera
 from robothub.utils import get_device_details, get_device_performance_metrics
 
 __all__ = ["AGENT", "app_is_running", "BaseDepthAIApplication", "BaseSDKApplication", "LOCAL_DEV", "TEAM_ID", "APP_INSTANCE_ID", "APP_VERSION",
            "ROBOT_ID", "STORAGE_DIR", "PUBLIC_FILES_DIR", "COMMUNICATOR", "CONFIGURATION", "DEVICES", "STREAMS", "StreamHandle", "EVENTS",
            "DEVICE_MXID", "wait"]
 
 logger = logging.getLogger(__name__)
@@ -35,14 +35,16 @@
 ROBOT_ID = robothub_core.ROBOT_ID
 STORAGE_DIR = robothub_core.STORAGE_DIR
 StreamHandle = robothub_core.StreamHandle
 STREAMS = robothub_core.STREAMS
 TEAM_ID = robothub_core.TEAM_ID
 
 app_is_running = robothub_core.app_is_running
+DeviceState = robothub_core.DeviceState
+RobotHubDevice = robothub_core.RobotHubDevice
 wait = robothub_core.wait
 DEVICE_MXID = "unknown"
 
 # this needs to be in sync with globals.py from robothub_core wrapper
 LOCAL_DEV = APP_INSTANCE_ID == "ROBOTHUB_ROBOT_APP_ID" and APP_VERSION == "ROBOTHUB_APP_VERSION"
```

### Comparing `robothub-2.5.6/src/robothub/events.py` & `robothub-2.5.7/src/robothub/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/frame_buffer.py` & `robothub-2.5.7/src/robothub/frame_buffer.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/live_view.py` & `robothub-2.5.7/src/robothub/live_view.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/live_view_utils.py` & `robothub-2.5.7/src/robothub/live_view_utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/__init__.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/_event_typechecks.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/_event_typechecks.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/app.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,14 +194,17 @@
         non_daemon_threads_count = count_threads(include_daemon=False)
         log.debug(f"Exit code: {self._exit_code}")
         if non_daemon_threads_count > 1:
             log.warning(f"App exited with {non_daemon_threads_count} non-daemon threads still running")
             os._exit(self._exit_code)
         sys.exit(self._exit_code)
 
+    def _run(self) -> None:
+        self.run()
+
     def _run_inner(self) -> None:
         # Try to call on_start, if it fails, exit with code 47
         try:
             self._start_timers()
             self.on_start()
             self._dispose_timers()
             AGENT._send_start_notification()
```

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/client.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/communicator.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/communicator.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/device.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/device.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/events.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/globals.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/globals.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/robothub_core_wrapper/streams.py` & `robothub-2.5.7/src/robothub/robothub_core_wrapper/streams.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub/utils.py` & `robothub-2.5.7/src/robothub/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.6/src/robothub.egg-info/PKG-INFO` & `robothub-2.5.7/src/robothub.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.6
+Version: 2.5.7
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
@@ -38,14 +38,26 @@
 
 To install this package, run the following command in your terminal window
 
 ```
 $ python3 -m pip install robothub
 ```
 
+### Building and installing locally
+
+    python setup.py sdist 
+
+it will create a __dist__ folder in the project root and in there, it will create __robothub-version.tar.gz
+
+to install it locally, use
+
+    pip install --upgrade /path/to/robothub/source/dist/robothub-2.5.4.tar.gz
+
+replace the 2.4.5 with correct version
+
 ## Examples
 
 You can find examples in the [robothub-examples](https://github.com/luxonis/robothub-examples) repository.
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `robothub-2.5.6/src/robothub.egg-info/SOURCES.txt` & `robothub-2.5.7/src/robothub.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 setup.py
 src/robothub/__init__.py
 src/robothub/application.py
 src/robothub/events.py
 src/robothub/frame_buffer.py
 src/robothub/live_view.py
 src/robothub/live_view_utils.py
-src/robothub/replay_camera.py
 src/robothub/types.py
 src/robothub/utils.py
 src/robothub.egg-info/PKG-INFO
 src/robothub.egg-info/SOURCES.txt
 src/robothub.egg-info/dependency_links.txt
 src/robothub.egg-info/top_level.txt
+src/robothub/replay/__init__.py
+src/robothub/replay/capture_manager.py
+src/robothub/replay/captures.py
+src/robothub/replay/replay_builder.py
+src/robothub/replay/replay_camera.py
+src/robothub/replay/utils.py
 src/robothub/robothub_core_wrapper/__init__.py
 src/robothub/robothub_core_wrapper/_event_typechecks.py
 src/robothub/robothub_core_wrapper/_exceptions.py
 src/robothub/robothub_core_wrapper/_metadata.py
 src/robothub/robothub_core_wrapper/_stop_event.py
 src/robothub/robothub_core_wrapper/_utils.py
 src/robothub/robothub_core_wrapper/app.py
```

