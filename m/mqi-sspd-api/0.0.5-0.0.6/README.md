# Comparing `tmp/mqi_sspd_api-0.0.5.tar.gz` & `tmp/mqi_sspd_api-0.0.6.tar.gz`

## Comparing `mqi_sspd_api-0.0.5.tar` & `mqi_sspd_api-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/examples/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/examples/set_current.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/mqi/v1/__init__.py
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/mqi/v1/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/examples/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/examples/set_current.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/mqi/v1/__init__.py
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/mqi/v1/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.6/PKG-INFO
```

### Comparing `mqi_sspd_api-0.0.5/mqi/v1/api.py` & `mqi_sspd_api-0.0.6/mqi/v1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     get_bias will return the bias of the channel for the given arduino id
 
     @param arduino_id:int -- id of the arduino (0-7)
     @param channel:int -- value of the channel, can vary but will be in the range 0-8
     @returns JsonObject
 
     """
-    def get_bias(channel, arduino_id=0):
+    def get_bias(self, channel, arduino_id=0):
         data = {
                 "__MESSAGE__": "message",
                 "command": "getBias",
                 "id": channel,
                 "name": "",
                 "value": "0"
 
@@ -84,25 +84,25 @@
 
     """
     get_resolution will return the resolution of the arduino
 
     @param arduino_id
     @returns JsonObject
     """
-    def get_resolution(arduino_id):
+    def get_resolution(self, arduino_id):
         pass
 
 
     """
     get_all_bias will return the bias currents of all channels of the arduino
 
     @param arduino_id:int -- the id of the arduino to select
     @returns JsonObject -- the id of the arduino to select
     """
-    def get_all_bias(arduino_id):
+    def get_all_bias(self, arduino_id):
         data = {
           "__MESSAGE__": "message",
           "command": "allChannels",
           "id": "",
           "name": "",
           "value": "0"
         }
@@ -116,47 +116,47 @@
     @param fr:float -- short for from, this is the current to start from (mA)
     @param to:float -- the current to stop at (mA)
     @param channel:int -- channel to select
     @param step_size:float -- the value to increment by
     @returns bool
     
     """
-    def current_sweep(arduino_id, fr, to, channel, step_size):
+    def current_sweep(self, arduino_id, fr, to, channel, step_size):
         pass
 
 
     """
     current_sweep_full will initiate a current sweep for all channels on the arduino
 
     @param arduino_id:int -- id of the arduino to select
     @param fr:float -- short for from, this is the current to start from (mA)
     @param to:float -- the current to stop at (mA)
     @param channel:int -- channel to select
     @param step_size:float -- the value to increment by
     @returns bool
 
     """
-    def current_sweep_full(arduino_id, fr, to, channel, step_size):
+    def current_sweep_full(self, arduino_id, fr, to, channel, step_size):
         pass
 
     """
     get_arduino_info will return the hardware specs of the arduino
 
     @param arduino_id:int -- id of the arduino to select
     @returns JsonObject
     """
-    def get_arduino_info(arduino_id):
+    def get_arduino_info(self, arduino_id):
         pass
 
     """
     get_arduino_config will return the current config of the selected arduino
 
     @param arduino_id:int -- id of the arduino to select
     """
-    def get_arduino_config(arduino_id):
+    def get_arduino_config(self, arduino_id):
         data = {
                 "__MESSAGE__": "message",
                 "command": "initinfo",
                 "id": "",
                 "name": "",
                 "value": "" 
 
@@ -171,28 +171,28 @@
     """
     set_arduino_config will set the config for the selected arduino
 
     @param arduino_id: int -- id of the arduino to select
     @returns bool
 
     """
-    def set_arduino_config(arduino_id):
+    def set_arduino_config(self, arduino_id):
         pass
 
 
     """ 
 
     auth will authenticate a user
 
     @param username: string -- this is the username usually just an email
     @param password:string -- a secret password 
     @returns bool
 
     """
-    def auth(username, password):
+    def auth(self, username, password):
         data = {
                 "__MESSAGE__": "message",
                 "command": "login",
                 "id": username,
                 "name": "",
                 "value": password
 
@@ -206,25 +206,25 @@
     """
     get_logs will return the logs of the managing_module 
 
     @param filename:string
     @returns bool
 
     """
-    def get_logs(filename):
+    def get_logs(self, filename):
         pass
 
     """
     set_channels will update the number of channels for the given arduino
 
     @param arduino_id:int -- the arduino to update
     @param channel_num:int -- the new number of channels
     @returns bool
     """
-    def set_channels(channel_num, arduino_id=0):
+    def set_channels(self, channel_num, arduino_id=0):
 
         data = {
                 "__MESSAGE__": "message",
                 "command": "setChannels",
                 "id": channel,
                 "name": "",
                 "value": channel_num 
@@ -236,52 +236,52 @@
 
         return True
 
     """
 
     @returns JsonObject
     """
-    def get_current_ws():
-        return ws;
+    def get_current_ws(self):
+        return self.ws;
 
     """
     get_number_of_arduinos returns the number of arduinos currently connected
 
     @returns int
     """
-    def get_number_of_arduinos():
+    def get_number_of_arduinos(self):
         pass
 
 
     """
     get_max_currents returns the switching currents for all channels
 
     @returns int[]
     """
-    def get_max_currents():
+    def get_max_currents(self):
         pass
 
 
     """
     get_max_current returns the switching currents for the given arduino
     """
-    def get_max_current(arduino_id):
+    def get_max_current(self, arduino_id):
         pass
 
 
     """
     get_current_sweep returns timeseries of the current sweep
 
     @param arduino_id:int -- id of the arduino
     """
-    def get_current_sweep(arduino_id):
+    def get_current_sweep(self, arduino_id):
         pass
 
 
     """
     get_current_sweep_all 
 
     @returns int[]
     """
-    def get_current_sweep_all():
+    def get_current_sweep_all(self):
         pass
```

### Comparing `mqi_sspd_api-0.0.5/LICENSE` & `mqi_sspd_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mqi_sspd_api-0.0.5/pyproject.toml` & `mqi_sspd_api-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "websocket-client", "rel"]
 build-backend = "hatchling.build"
 [project]
 dependencies = ['websocket-client', 'rel']
 name = "mqi_sspd_api"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Filip Zlatoidsky", email="fillatino@gmail.com" },
 ]
 description = "This is the official API of the MQI biasing box"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `mqi_sspd_api-0.0.5/PKG-INFO` & `mqi_sspd_api-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mqi_sspd_api
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is the official API of the MQI biasing box
 Project-URL: Homepage, https://github.com/MQI-Software/mqi-api
 Project-URL: Issues, https://github.com/MQI-Software/mqi-api/issues
 Author-email: Filip Zlatoidsky <fillatino@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

