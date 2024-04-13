# Comparing `tmp/diaspora-event-sdk-0.2.2.tar.gz` & `tmp/diaspora-event-sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.2.tar", last modified: Wed Apr 10 18:50:28 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.3.tar", last modified: Sat Apr 13 12:43:22 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.2.tar` & `diaspora-event-sdk-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499890 diaspora-event-sdk-0.2.2/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-10 18:50:28.499773 diaspora-event-sdk-0.2.2/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.496796 diaspora-event-sdk-0.2.2/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.498102 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     7503 2024-04-10 18:49:14.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499063 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499252 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     3679 2024-04-10 18:01:19.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-10 18:49:26.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.497355 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-10 18:50:28.000000 diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-10 18:50:28.499939 diaspora-event-sdk-0.2.2/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499371 diaspora-event-sdk-0.2.2/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.2/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-10 18:50:28.499452 diaspora-event-sdk-0.2.2/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.2/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.2/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.217507 diaspora-event-sdk-0.2.3/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-13 12:43:22.217389 diaspora-event-sdk-0.2.3/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1722 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.214683 diaspora-event-sdk-0.2.3/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.215896 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     8016 2024-04-13 12:31:39.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4361 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.216819 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.217024 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4222 2024-04-13 12:42:58.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-04-13 12:31:44.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.215210 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2092 2024-04-13 12:43:22.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1068 2024-04-13 12:43:22.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-04-13 12:43:22.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      141 2024-04-13 12:43:22.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-04-13 12:43:22.000000 diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-04-13 12:43:22.217703 diaspora-event-sdk-0.2.3/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1389 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.217125 diaspora-event-sdk-0.2.3/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.3/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-04-13 12:43:22.217207 diaspora-event-sdk-0.2.3/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.3/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.3/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.2/LICENSE` & `diaspora-event-sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/PKG-INFO` & `diaspora-event-sdk-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.2/README.md` & `diaspora-event-sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -192,7 +192,23 @@
 
     @requires_login
     def update_trigger(self, trigger_uuid, trigger_configs):
         """
         Updates invocation configurations of an existing trigger, identified by its unique trigger UUID.
         """
         return self.web_client.update_trigger(self.subject_openid, trigger_uuid, trigger_configs)
+
+    @requires_login
+    def list_log_streams(self, trigger):
+        """
+        List log streams of a trigger under the user's account
+        """
+        return self.web_client.list_log_streams(
+            self.subject_openid, trigger)
+
+    @requires_login
+    def get_log_events(self, trigger, stream):
+        """
+        Get events in a particular log stream of a trigger under the user's account
+        """
+        return self.web_client.get_log_events(
+            self.subject_openid, trigger, stream)
```

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk/sdk/web_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Optional
 import json
+from typing import Optional
+
 import globus_sdk
+
 from diaspora_event_sdk.sdk.utils.uuid_like import UUID_LIKE_T
 
 from ._environments import TOKEN_EXCHANGE
 
 
 class WebClient(globus_sdk.BaseClient):
     def __init__(
@@ -94,7 +96,24 @@
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.post(
             f"/api/v2/triggers/{trigger_uuid}",
             headers={"Subject": str(subject), "Trigger_id": str(trigger_uuid),
                      "Content-Type": "text/plain"},
             data=json.dumps(trigger_configs).encode("utf-8")
         )
+
+    def list_log_streams(
+        self, subject: UUID_LIKE_T, trigger: str
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.get(
+            f"/api/v2/logs",
+            headers={"Subject": str(subject), "Trigger": trigger}
+        )
+
+    def get_log_events(
+        self, subject: UUID_LIKE_T, trigger: str, stream: str
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.get(
+            f"/api/v2/log",
+            headers={"Subject": str(subject), "Trigger": trigger,
+                     "Stream": stream}
+        )
```

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: LICENSE
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.2/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.3/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/setup.py` & `diaspora-event-sdk-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.2/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.3/tests/unit/test_client.py`

 * *Files identical despite different names*

