# Comparing `tmp/emerald_hws-0.0.4.tar.gz` & `tmp/emerald_hws-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emerald_hws-0.0.4.tar", last modified: Tue Jan 30 10:10:15 2024, max compression
+gzip compressed data, was "emerald_hws-0.0.5.tar", last modified: Sat Apr 13 04:11:13 2024, max compression
```

## Comparing `emerald_hws-0.0.4.tar` & `emerald_hws-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-01-30 10:10:15.628365 emerald_hws-0.0.4/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.4/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-01-30 10:10:15.627800 emerald_hws-0.0.4/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.4/README.md
--rw-r--r--   0 ross       (501) staff       (20)      824 2024-01-30 10:09:16.000000 emerald_hws-0.0.4/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-01-30 10:10:15.628471 emerald_hws-0.0.4/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-01-30 10:10:15.621492 emerald_hws-0.0.4/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-01-30 10:10:15.624350 emerald_hws-0.0.4/src/emerald_hws/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-01-30 10:10:15.626678 emerald_hws-0.0.4/src/emerald_hws/__assets__/
--rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.4/src/emerald_hws/__assets__/SFSRootCAG2.pem
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.4/src/emerald_hws/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    10525 2024-01-30 10:09:06.000000 emerald_hws-0.0.4/src/emerald_hws/emeraldhws.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-01-30 10:10:15.627311 emerald_hws-0.0.4/src/emerald_hws.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-01-30 10:10:15.000000 emerald_hws-0.0.4/src/emerald_hws.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      327 2024-01-30 10:10:15.000000 emerald_hws-0.0.4/src/emerald_hws.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-30 10:10:15.000000 emerald_hws-0.0.4/src/emerald_hws.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       22 2024-01-30 10:10:15.000000 emerald_hws-0.0.4/src/emerald_hws.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       12 2024-01-30 10:10:15.000000 emerald_hws-0.0.4/src/emerald_hws.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.693664 emerald_hws-0.0.5/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.5/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-13 04:11:13.692824 emerald_hws-0.0.5/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.5/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      824 2024-04-13 04:03:34.000000 emerald_hws-0.0.5/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-13 04:11:13.693904 emerald_hws-0.0.5/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.686475 emerald_hws-0.0.5/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.688860 emerald_hws-0.0.5/src/emerald_hws/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.690785 emerald_hws-0.0.5/src/emerald_hws/__assets__/
+-rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.5/src/emerald_hws/__assets__/SFSRootCAG2.pem
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.5/src/emerald_hws/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    12069 2024-04-13 03:44:49.000000 emerald_hws-0.0.5/src/emerald_hws/emeraldhws.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.691599 emerald_hws-0.0.5/src/emerald_hws.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       22 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/top_level.txt
```

### Comparing `emerald_hws-0.0.4/LICENSE` & `emerald_hws-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.4/PKG-INFO` & `emerald_hws-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `emerald_hws-0.0.4/pyproject.toml` & `emerald_hws-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emerald_hws"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
   "boto3",
   "AWSIoTPythonSDK"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
 ]
```

### Comparing `emerald_hws-0.0.4/src/emerald_hws/__assets__/SFSRootCAG2.pem` & `emerald_hws-0.0.5/src/emerald_hws/__assets__/SFSRootCAG2.pem`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.4/src/emerald_hws/emeraldhws.py` & `emerald_hws-0.0.5/src/emerald_hws/emeraldhws.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import requests
 import os
-# import logging
+import logging
 import boto3
 import random
 from AWSIoTPythonSDK.MQTTLib import AWSIoTMQTTClient
 
 
 class EmeraldHWS():
     """ Implementation of the web API for Emerald Heat Pump Hot Water Systems
@@ -26,14 +26,16 @@
         :param password: The password for the supplied user account
         """
 
         self.email = email
         self.password = password
         self.token = ""
         self.properties = {}
+        self.logger = logging.getLogger()
+        self.logger.setLevel(logging.DEBUG)
 
     def getLoginToken(self):
         """ Performs an API request to get a token from the API
         """
         url = "https://api.emerald-ems.com.au/api/v1/customer/sign-in"
 
         payload = {
@@ -67,50 +69,62 @@
         headers = self.COMMON_HEADERS
         headers["authorization"] = "Bearer {}".format(self.token)
 
         post_response = requests.get(url, headers=headers)
         post_response_json = post_response.json()
 
         if post_response_json.get("code") == 200:
+            self.logger.debug("Successfully logged into Emerald API")
             self.properties = post_response_json.get("info").get("property")
         else:
             raise Exception("Unable to fetch properties from Emerald API")
 
-    def connectMQTT(self):
-        """ Establishes a connection to Amazon IOT core's MQTT service
+    def getTemporaryCreds(self):
+        """ Returns temporary credentials for IoT Core
         """
 
-        cert_path = os.path.join(os.path.dirname(__file__), '__assets__', 'SFSRootCAG2.pem')
-
-        # Cognito auth
         identityPoolID = self.COGNITO_IDENTITY_POOL_ID
         region = self.MQTT_HOST.split('.')[2]
         cognitoIdentityClient = boto3.client('cognito-identity', region_name=region)
 
         temporaryIdentityId = cognitoIdentityClient.get_id(IdentityPoolId=identityPoolID)
         identityID = temporaryIdentityId["IdentityId"]
+        self.logger.debug("AWS IoT IdentityID: {}".format(identityID))
 
         temporaryCredentials = cognitoIdentityClient.get_credentials_for_identity(IdentityId=identityID)
-        AccessKeyId = temporaryCredentials["Credentials"]["AccessKeyId"]
-        SecretKey = temporaryCredentials["Credentials"]["SecretKey"]
-        SessionToken = temporaryCredentials["Credentials"]["SessionToken"]
+        self.logger.debug("Got new temporary credentials for AWS")
+        self.identityID = identityID
+        self.temporaryCredentials = temporaryCredentials
+
+
+    def connectMQTT(self):
+        """ Establishes a connection to Amazon IOT core's MQTT service
+        """
+
+        cert_path = os.path.join(os.path.dirname(__file__), '__assets__', 'SFSRootCAG2.pem')
+        self.getTemporaryCreds()
+
+        AccessKeyId = self.temporaryCredentials["Credentials"]["AccessKeyId"]
+        SecretKey = self.temporaryCredentials["Credentials"]["SecretKey"]
+        SessionToken = self.temporaryCredentials["Credentials"]["SessionToken"]
 
         # Init AWSIoTMQTTClient
-        myAWSIoTMQTTClient = AWSIoTMQTTClient(identityID, useWebsocket=True)
+        myAWSIoTMQTTClient = AWSIoTMQTTClient(self.identityID, useWebsocket=True)
 
         # AWSIoTMQTTClient configuration
         myAWSIoTMQTTClient.configureEndpoint(self.MQTT_HOST, 443)
         myAWSIoTMQTTClient.configureCredentials(cert_path)
         myAWSIoTMQTTClient.configureIAMCredentials(AccessKeyId, SecretKey, SessionToken)
         myAWSIoTMQTTClient.configureAutoReconnectBackoffTime(1, 32, 20)
         myAWSIoTMQTTClient.configureOfflinePublishQueueing(-1)  # Infinite offline Publish queueing
         myAWSIoTMQTTClient.configureDrainingFrequency(2)  # Draining: 2 Hz
         myAWSIoTMQTTClient.configureConnectDisconnectTimeout(10)  # 10 sec
         myAWSIoTMQTTClient.configureMQTTOperationTimeout(10)  # 10 sec
-
+        myAWSIoTMQTTClient.onOffline = self.on_offline
+        myAWSIoTMQTTClient.onOnline = self.on_online
         # Connect and subscribe to AWS IoT
         myAWSIoTMQTTClient.connect()
 
         self.myAWSIoTMQTTClient = myAWSIoTMQTTClient
 
     def mqttDecodeUpdate(self, topic, payload):
         """ Attempt to decode a received MQTT message and direct appropriately
@@ -123,22 +137,36 @@
         command = json_payload[0].get("command")
         if command is not None:
             if command == "upload_status":
                 for key in json_payload[1]:
                     self.updateHWSState(hws_id, key, json_payload[1][key])
 
     def mqttCallback(self, client, userdata, message):
-        # print("Received a new message: ")
-        # print(message.payload.decode("utf-8"))
-        # print("from topic: ")
-        # print(message.topic)
-        # print("--------------\n\n")
+        """ Calls decode update for received message
+        """
 
+        self.logger.debug("Received message from MQTT topic {}: {}".format(message.topic,message.payload.decode("utf-8")))
         self.mqttDecodeUpdate(message.topic, message.payload)
 
+    def on_offline(self):
+        """ Reconfigures temporary credentials
+        """
+
+        self.logger.debug("AWS IoT offline")
+        self.getTemporaryCreds()
+        AccessKeyId = self.temporaryCredentials["Credentials"]["AccessKeyId"]
+        SecretKey = self.temporaryCredentials["Credentials"]["SecretKey"]
+        SessionToken = self.temporaryCredentials["Credentials"]["SessionToken"]
+        self.myAWSIoTMQTTClient.configureIAMCredentials(AccessKeyId, SecretKey, SessionToken)
+
+    def on_online(self):
+        """ Logs online state
+        """
+        self.logger.debug("AWS IoT online")
+
     def updateHWSState(self, id, key, value):
         """ Updates the specified value for the supplied key in the HWS id specified
         :param id: ID of the HWS
         :param key: key to update (eg temp_current)
         :param value: value to set
         """
 
@@ -197,38 +225,43 @@
 
         self.myAWSIoTMQTTClient.publish("ep/heat_pump/to_gw/{}".format(id), json.dumps(msg), 1)
 
     def turnOn(self, id):
         """ Turns the specified HWS on
         :param id: The UUID of the HWS to turn on
         """
+        self.logger.debug("Sending control message: turn on")
         self.sendControlMessage(id, {"switch":1})
 
     def turnOff(self, id):
         """ Turns the specified HWS off
         :param id: The UUID of the HWS to turn off
         """
+        self.logger.debug("Sending control message: turn off")
         self.sendControlMessage(id, {"switch":0})
 
     def setNormalMode(self, id):
         """ Sets the specified HWS to normal (not Boost or Quiet) mode
         :param id: The UUID of the HWS to set to normal mode
         """
+        self.logger.debug("Sending control message: normal mode")
         self.sendControlMessage(id, {"mode":1})
 
     def setBoostMode(self, id):
         """ Sets the specified HWS to boost (high power) mode
         :param id: The UUID of the HWS to set to boost mode
         """
+        self.logger.debug("Sending control message: boost mode")
         self.sendControlMessage(id, {"mode":0})
 
     def setQuietMode(self, id):
         """ Sets the specified HWS to quiet (low power) mode
         :param id: The UUID of the HWS to set to quiet mode
         """
+        self.logger.debug("Sending control message: quiet mode")
         self.sendControlMessage(id, {"mode":2})
 
     def isOn(self, id):
         """ Returns true if the specified HWS is currently on
         :param id: The UUID of the HWS to query
         """
         switch_status = self.getFullStatus(id).get("last_state").get("switch")
```

### Comparing `emerald_hws-0.0.4/src/emerald_hws.egg-info/PKG-INFO` & `emerald_hws-0.0.5/src/emerald_hws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

