# Comparing `tmp/indipyclient-0.0.4.tar.gz` & `tmp/indipyclient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.4.tar` & `indipyclient-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.4/LICENSE
--rw-r--r--   0        0        0     2686 2024-04-03 21:19:09.000000 indipyclient-0.0.4/README.md
--rw-r--r--   0        0        0      291 2024-04-08 21:07:14.000000 indipyclient-0.0.4/indipyclient/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.4/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.4/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.4/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.4/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   143996 2024-04-08 20:45:37.000000 indipyclient-0.0.4/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.4/indipyclient/error.py
--rw-r--r--   0        0        0    24609 2024-04-03 21:17:26.000000 indipyclient-0.0.4/indipyclient/events.py
--rw-r--r--   0        0        0    34586 2024-04-04 22:04:06.000000 indipyclient-0.0.4/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    15364 2024-04-07 22:08:45.000000 indipyclient-0.0.4/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    25114 2024-04-03 21:17:26.000000 indipyclient-0.0.4/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-04-08 21:06:58.000000 indipyclient-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 indipyclient-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.5/README.md
+-rw-r--r--   0        0        0      291 2024-04-13 20:37:30.000000 indipyclient-0.0.5/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.5/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.5/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.5/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.5/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   143996 2024-04-08 20:45:37.000000 indipyclient-0.0.5/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.5/indipyclient/error.py
+-rw-r--r--   0        0        0    25044 2024-04-13 18:46:37.000000 indipyclient-0.0.5/indipyclient/events.py
+-rw-r--r--   0        0        0    34740 2024-04-12 08:47:00.000000 indipyclient-0.0.5/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    15584 2024-04-11 11:19:29.000000 indipyclient-0.0.5/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27590 2024-04-13 18:00:12.000000 indipyclient-0.0.5/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-04-13 20:37:50.000000 indipyclient-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.5/PKG-INFO
```

### Comparing `indipyclient-0.0.4/LICENSE` & `indipyclient-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.4/README.md` & `indipyclient-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # indipyclient
 Terminal client to communicate to an INDI service.
 
-NOTE: CURRENTLY STILL UNDER DEVELOPMENT
-
-This is a pure python package, with no dependencies, providing an INDI client terminal
+This is a pure python package, with no dependencies, providing an INDI terminal client.
 
 It also provides a set of classes which can be used to create an INDI client. Either a script, or a GUI implementation could use this to generate the INDI protocol XML, and to create the connection to a port serving INDI drivers.
 
 The client can be run with
 
 indipyclient [options]
```

### Comparing `indipyclient-0.0.4/indipyclient/__main__.py` & `indipyclient-0.0.5/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.4/indipyclient/console/consoleclient.py` & `indipyclient-0.0.5/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.4/indipyclient/console/widgets.py` & `indipyclient-0.0.5/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.4/indipyclient/console/windows.py` & `indipyclient-0.0.5/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.4/indipyclient/events.py` & `indipyclient-0.0.5/indipyclient/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,23 @@
             timestamp = None
     else:
         timestamp = datetime.now(tz=timezone.utc)
     return timestamp
 
 
 class VectorTimeOut:
-    "This event is generated by a timeout - not by received data"
+    """This event is generated by a timeout, not by received data."""
 
     def __init__(self, device, vector):
         self.device = device
         self.devicename = self.device.devicename
         self.vector = vector
         self.vectorname = self.vector.name
         self.timestamp = datetime.now(tz=timezone.utc)
+        self.eventtype = "TimeOut"
 
 
 class Event:
     "Parent class for events received from drivers"
     def __init__(self, root, device, client):
         self.device = device
         self._client = client
@@ -74,29 +75,33 @@
 
 class Message(Event):
     """This contains attribute 'message' with the message string sent by the remote driver.
        Attribute devicename could be None if the driver is sending a system wide message."""
 
     def __init__(self, root, device, client):
         super().__init__(root, device, client)
+        self.eventtype = "Message"
         self.message = root.get("message", "")
         if device is None:
             # state wide message
             client.messages.appendleft( (self.timestamp, self.message) )
         else:
             device.messages.appendleft( (self.timestamp, self.message) )
 
 
 class delProperty(Event):
     """The remote driver is instructing the client to delete either a device or a vector property.
        This contains attribute vectorname, if it is None, then the whole device is to be deleted.
-       A 'message' attribute contains any message sent by the client with this instruction."""
+       A 'message' attribute contains any message sent by the client with this instruction.
+       This event will automatically set the appropriate enable flag to False in the effected
+       device and vectors."""
 
     def __init__(self, root, device, client):
         super().__init__(root, device, client)
+        self.eventtype = "Delete"
         if self.devicename is None:
             raise ParseException("delProperty has no devicename")
         if not self.device.enable:
             # already deleted
             raise ParseException("device already deleted")
         self.vectorname = root.get("name")
         self.message = root.get("message", "")
@@ -115,14 +120,15 @@
 
 
 class defVector(Event, UserDict):
     "Parent to def vectors, adds a mapping of membername:value"
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
         UserDict.__init__(self)
+        self.eventtype = "Define"
         self.vectorname = root.get("name")
         if self.vectorname is None:
             raise ParseException("defVector has no vector name")
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "DEFAULT GROUP")
         state = root.get("state")
         if not state:
@@ -135,17 +141,16 @@
 
     def __setitem__(self, membername):
         raise KeyError
 
 
 class defSwitchVector(defVector):
 
-    """The remote driver has sent this to define a switch vector property, it has further
-       attributes perm, rule, timeout, and memberlabels which is a dictionary of
-       membername:label."""
+    """The remote driver has sent this to define a switch vector property, this
+       is a mapping of membername:value"""
 
     def __init__(self, root, device, client):
         defVector.__init__(self, root, device, client)
         self.perm = root.get("perm")
         if self.perm is None:
             raise ParseException("defSwitchVector has no perm given")
         if self.perm not in ('ro', 'wo', 'rw'):
@@ -202,17 +207,16 @@
             self.vector = propertyvectors.SwitchVector(self)
             # add it to properties
             properties[self.vectorname] = self.vector
 
 
 class defTextVector(defVector):
 
-    """The remote driver has sent this to define a text vector property, it has further
-       attributes perm, timeout, and memberlabels which is a dictionary of
-       membername:label."""
+    """The remote driver has sent this to define a text vector property, this
+       is a mapping of membername:value."""
 
     def __init__(self, root, device, client):
         defVector.__init__(self, root, device, client)
         self.perm = root.get("perm")
         if self.perm is None:
             raise ParseException
         if self.perm not in ('ro', 'wo', 'rw'):
@@ -258,20 +262,19 @@
         else:
             # create a new TextVector
             self.vector = propertyvectors.TextVector(self)
             # add it to properties
             properties[self.vectorname] = self.vector
 
 
-
-
 class defNumberVector(defVector):
 
-    """The remote driver has sent this to define a number vector property, it has further
-       attributes perm, timeout, and memberlabels which is a dictionary of
+    """The remote driver has sent this to define a number vector property, this
+       is a mapping of membername:value. Its attributes memberlabels gives further
+       description of members, being a dictionary of
        membername:(label, format, min, max, step)."""
 
     def __init__(self, root, device, client):
         defVector.__init__(self, root, device, client)
         self.perm = root.get("perm")
         if self.perm is None:
             raise ParseException
@@ -333,16 +336,16 @@
             # add it to properties
             properties[self.vectorname] = self.vector
 
 
 
 class defLightVector(defVector):
 
-    """The remote driver has sent this to define a light vector property, it has further
-       attribute memberlabels which is a dictionary of membername:label."""
+    """The remote driver has sent this to define a light vector property.
+       This is a mapping of membername:value."""
 
     def __init__(self, root, device, client):
         defVector.__init__(self, root, device, client)
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
@@ -380,23 +383,22 @@
             # add it to properties
             properties[self.vectorname] = self.vector
 
 
 
 class defBLOBVector(Event):
 
-    """The remote driver has sent this to define a BLOB vector property, it has further
-       attributes perm, timeout, and memberlabels which is a dictionary of
-       membername:label.
+    """The remote driver has sent this to define a BLOB vector property.
 
        However this class does not have an object mapping of member name to value, since
        values are not given in defBLOBVectors"""
 
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
+        self.eventtype = "DefineBLOB"
         if self.devicename is None:
             raise ParseException
         self.vectorname = root.get("name")
         if self.vectorname is None:
             raise ParseException
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "DEFAULT GROUP")
@@ -452,20 +454,22 @@
 
 
 class setVector(Event, UserDict):
     "Parent to set vectors, adds dictionary"
     def __init__(self, root, device, client):
         Event.__init__(self, root, device, client)
         UserDict.__init__(self)
+        self.eventtype = "Set"
         if self.devicename is None:
             raise ParseException
         self.vectorname = root.get("name")
         if self.vectorname is None:
             raise ParseException
         # This vector must already exist, and be enabled
+        self.timeout = None
         if self.vectorname in self.device:
             vector = self.device[self.vectorname]
             if not vector.enable:
                 raise ParseException
         else:
             raise ParseException
         state = root.get("state")
@@ -477,16 +481,16 @@
 
     def __setitem__(self, membername):
         raise KeyError
 
 
 
 class setSwitchVector(setVector):
-    """The remote driver is setting a Switch vector property, this
-       has further attribute timeout."""
+    """The remote driver is setting a Switch vector property.
+       This is a mapping of membername:value."""
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
@@ -514,16 +518,16 @@
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setTextVector(setVector):
 
-    """The remote driver is setting a Text vector property, this
-       has further attribute timeout."""
+    """The remote driver is setting a Text vector property.
+       This is a mapping of membername:value."""
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
@@ -547,17 +551,17 @@
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setNumberVector(setVector):
 
-    """The remote driver is setting a Number vector property, this
-       has further attribute timeout. The number values of the
-       membername:membervalue are string values."""
+    """The remote driver is setting a Number vector property.
+       This is a mapping of membername:value.
+       These number values are string values."""
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
@@ -579,15 +583,17 @@
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setLightVector(setVector):
 
-    """The remote driver is setting a Light vector property."""
+    """The remote driver is setting a Light vector property.
+       This is a mapping of membername:value.
+       Note, the timeout attribute will always be None"""
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneLight":
                 membername = member.get("name")
@@ -605,20 +611,25 @@
         self.vector = properties[self.vectorname]
         # set changed values into self.vector
         self.vector._setvector(self)
 
 
 class setBLOBVector(setVector):
 
-    """The remote driver is setting a BLOB vector property, this
-       has further attributes timeout and sizeformat which is a dictionary
-       of membername:(size, format)."""
+    """The remote driver is setting a BLOB vector property.
+       This is a mapping of membername:value, where value is a
+       bytes object, taken from the received xml and b64 decoded
+       This event has further attribute sizeformat being a dictionary
+       of membername:(size, format) and which are then set into the target
+       members as blobsize and blobformat attributes."""
+
 
     def __init__(self, root, device, client):
         setVector.__init__(self, root, device, client)
+        self.eventtype = "SetBLOB"
         try:
             timeout = root.get("timeout")
             if not timeout is None:
                 self.timeout = float(timeout)
         except:
             # dont update
             pass
```

### Comparing `indipyclient-0.0.4/indipyclient/ipyclient.py` & `indipyclient-0.0.5/indipyclient/ipyclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         # create queue where client will put xml data to be transmitted
         self.writerque = collections.deque()
 
         # and create readerque where received xmldata will be put
         self.readerque = asyncio.Queue(4)
         # self.data is a dictionary of devicename to device object
         self.data = {}
-        # self.messages is a deque of "Timestamp space message"
+        # self.messages is a deque of (Timestamp, message) tuples
         self.messages = collections.deque(maxlen=8)
 
         # note, messages are added with 'appendleft'
         # so newest message is messages[0]
         # oldest message is messages[-1] or can be obtained with .pop()
 
         # self.connected is True if connection has been made
@@ -166,16 +166,16 @@
     def logfp(self):
         "Can be read, but only set via setlogging method"
         return self._logfp
 
     def setlogging(self, level, logfile):
         """Sets the logging level and logfile, returns the level, which will be None on failure.
            As default, the level is None, indicating no logging. Apart from None, level should
-           be an integer, one of 1, 2, 3 or 4
-           Be warned, there is no logfile ration, files can become large.
+           be an integer, one of 1, 2, 3 or 4.
+           Be warned, there is no logfile rotation, files can become large.
            Note: it may be useful in another terminal to try tail -f logfile"""
         try:
             if self._logfp:
                 self._logfp.close()
                 self._logfp = None
 
             if level in (1, 2, 3, 4):
@@ -621,19 +621,18 @@
                 self._logfp.write(bytex)
         finally:
             self.shutdown()
 
 
     def snapshot(self):
         """Take a snapshot of the devices and returns a dictionary of device
-           names to objects which are copies of the current state of devices and
-           vectors.
-           These copies will not be updated. This is provided so that you can
-           handle the device data in another thread, without fear of their
-           values changing."""
+           names to objects which are restricted copies of the current state of devices and
+           vectors. Vector methods for sending data will not be available.
+           These copies will not be updated by events. This is provided so that you can
+           handle the device data, without fear of their values changing."""
         with threading.Lock():
             # other threads cannot change the client.data dictionary
             # while the snapshot is being taken
             snap = {}
             if self.data:
                 for devicename, device in self.data.items():
                     snap[devicename] = device._snapshot()
@@ -664,19 +663,20 @@
         except KeyboardInterrupt:
             self.shutdown()
 
     def set_vector_timeouts(self, timeout_enable=None, timeout_min=None, timeout_max=None):
         """Whenever you send updated values, a timer is started and if a timeout occurs
            before the server responds, a VectorTimeOut event will be created, which you
            could choose to ignore, or take action such as setting an Alert flag.
-           The protocol allows the server to suggest a timeout for each vector. This method
-           allows you to set minimum and maximum timeouts, which should be given as integer
-           values. If any parameter is not provided (left at None) then that value will not be
-           changed. If timeout_enable is set to False, no VectorTimeOut events will occur.
-           As default, timeouts are enabled, minimum is set to 2 seconds, maximum 10 seconds."""
+           The INDI protocol allows the server to suggest a timeout for each vector. This
+           method allows you to set minimum and maximum timeouts which restricts the
+           suggested values. These should be given as integer seconds. If any parameter
+           is not provided (left at None) then that value will not be changed. If
+           timeout_enable is set to False, no VectorTimeOut events will occur. As default,
+           timeouts are enabled, minimum is set to 2 seconds, maximum 10 seconds."""
         if not timeout_enable is None:
             self.vector_timeout_enable = timeout_enable
         if not timeout_min is None:
             self.vector_timeout_min = timeout_min
         if not timeout_max is None:
             self.vector_timeout_max = timeout_max
 
@@ -779,15 +779,15 @@
 
     def __init__(self, devicename):
         super().__init__()
 
         # This device name
         self.devicename = devicename
 
-        # this is a dictionary of property name to propertyvector this device owns
+        # this is a dictionary of vector name to vector this device owns
         self.data = {}
 
     @property
     def enable(self):
         "Returns True if any vector of this device has enable True, otherwise False"
         for vector in self.data.values():
             if vector.enable:
@@ -842,12 +842,13 @@
             return events.defBLOBVector(root, self, self._client)
         elif root.tag == "setBLOBVector":
             return events.setBLOBVector(root, self, self._client)
         else:
             raise ParseException("Unrecognised tag received")
 
     def _snapshot(self):
+        "Creates snapshot of this device and its vectors"
         snapdevice = Device(self.devicename)
         for vectorname, vector in self.data:
             snapdevice[vectorname] = vector._snapshot()
         snapdevice.messages = list(self.messages)
         return snapdevice
```

### Comparing `indipyclient-0.0.4/indipyclient/propertymembers.py` & `indipyclient-0.0.5/indipyclient/propertymembers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 
 import xml.etree.ElementTree as ET
 
-import sys, math, pathlib
+import sys, pathlib
 
 from .error import ParseException
 
 
 class Member():
 
+    """This class is the parent of further member classes.
+       Should you use the ipyclient.snapshot method to create a snapshot,
+       the snapshot vectors for Switch, Light and Text will contain objects
+       of this Member class."""
+
     def __init__(self, name, label=None, membervalue=None):
         self.name = name
         if label:
             self.label = label
         else:
             self.label = name
         self._membervalue = membervalue
@@ -21,30 +26,15 @@
         return self._membervalue
 
     @membervalue.setter
     def membervalue(self, value):
         self._membervalue = value
 
 
-
-class PropertyMember(Member):
-    "Parent class of SwitchMember etc"
-
-    def checkvalue(self, value, allowed):
-        "allowed is a list of values, checks if value is in it"
-        if value not in allowed:
-            raise ParseException(f"Error: Invalid value:{value}")
-        return value
-
-    def _snapshot(self):
-        snapmember = Member(self.name, self.label, self._membervalue)
-        return snapmember
-
-
-class SwitchMember(PropertyMember):
+class SwitchMember(Member):
     """A SwitchMember can only have one of 'On' or 'Off' values"""
 
     def __init__(self, name, label=None, membervalue="Off"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('On', 'Off'):
             raise ParseException(f"Error: Invalid value {membervalue}, should be On or Off")
 
@@ -56,23 +46,33 @@
     def membervalue(self, value):
         if not value:
             raise ParseException("Error: No value given, should be On or Off")
         newvalue = self.checkvalue(value, ['On', 'Off'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
+    def checkvalue(self, value, allowed):
+        "allowed is a list of values, checks if value is in it"
+        if value not in allowed:
+            raise ParseException(f"Error: Invalid value:{value}")
+        return value
+
+    def _snapshot(self):
+        snapmember = Member(self.name, self.label, self._membervalue)
+        return snapmember
+
     def oneswitch(self, newvalue):
         """Returns xml of a oneSwitch with the new value to send"""
         xmldata = ET.Element('oneSwitch')
         xmldata.set("name", self.name)
         xmldata.text = newvalue
         return xmldata
 
 
-class LightMember(PropertyMember):
+class LightMember(Member):
     """A LightMember can only have one of 'Idle', 'Ok', 'Busy' or 'Alert' values"""
 
     def __init__(self, name, label=None, membervalue="Idle"):
         super().__init__(name, label, membervalue)
         if membervalue not in ('Idle','Ok','Busy','Alert'):
             raise ParseException(f"Error: Invalid light value {membervalue}")
 
@@ -84,16 +84,26 @@
     def membervalue(self, value):
         if not value:
             raise ParseException("Error: No light value given")
         newvalue = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         if self._membervalue != newvalue:
             self._membervalue = newvalue
 
+    def checkvalue(self, value, allowed):
+        "allowed is a list of values, checks if value is in it"
+        if value not in allowed:
+            raise ParseException(f"Error: Invalid value:{value}")
+        return value
+
+    def _snapshot(self):
+        snapmember = Member(self.name, self.label, self._membervalue)
+        return snapmember
+
 
-class TextMember(PropertyMember):
+class TextMember(Member):
     """Contains a text string"""
 
     def __init__(self, name, label=None, membervalue=""):
         super().__init__(name, label, membervalue)
         if not isinstance(membervalue, str):
             raise ParseException("Error: The text value should be a string")
 
@@ -104,24 +114,33 @@
     @membervalue.setter
     def membervalue(self, value):
         if not isinstance(value, str):
             raise ParseException("Error: The text value should be a string")
         if self._membervalue != value:
             self._membervalue = value
 
+    def _snapshot(self):
+        snapmember = Member(self.name, self.label, self._membervalue)
+        return snapmember
+
     def onetext(self, newvalue):
         """Returns xml of a oneText"""
         xmldata = ET.Element('oneText')
         xmldata.set("name", self.name)
         xmldata.text = newvalue
         return xmldata
 
 
 class ParentNumberMember(Member):
 
+    """This class inherits from Member and is the parent of the NumberMember class.
+       Should you use the ipyclient.snapshot method to create a snapshot,
+       the snapshot vectors for Numbers will contain objects of this class."""
+
+
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, membervalue)
         self.format = format
         self.min = min
         self.max = max
         self.step = step
 
@@ -176,15 +195,15 @@
                 floatvalue = -1 * floatvalue
         except:
             raise TypeError("Error: Unable to parse number value")
         return floatvalue
 
 
     def getformattedvalue(self):
-        """This method returns this members value as a string float."""
+        """This method returns this members value as a formatted string."""
         return self.getformattedstring(self._membervalue)
 
 
     def getformattedstring(self, value):
         """Given a number this returns a formatted string"""
         try:
             value = self.getfloat(value)
@@ -199,15 +218,15 @@
             if value<0:
                 negative = True
             else:
                 negative = False
             absvalue = abs(value)
 
             # get integer part and fraction part
-            degrees = math.floor(absvalue)
+            degrees = int(absvalue)
             minutes = (absvalue - degrees) * 60.0
 
             if f == "3":   # three fractional values including the colon ":mm"
                 # create nearest integer minutes
                 minutes = round(minutes)
                 if minutes == 60:
                     minutes = 0
@@ -225,15 +244,15 @@
                     minutes = 0.0
                     degrees = degrees + 1
                 valstring = f"{'-' if negative else ''}{degrees}:{minutes:04.1f}"
                 if w:
                     return valstring.rjust(int(w), ' ')
                 return valstring
 
-            integerminutes = math.floor(minutes)
+            integerminutes = int(minutes)
             seconds = (minutes - integerminutes) * 60.0
 
             if f == "6":    # six fractional values including two colons ":mm:ss"
                 seconds = round(seconds)
                 if seconds == 60:
                     seconds = 0
                     integerminutes = integerminutes + 1
@@ -279,28 +298,14 @@
         # no other options accepted
         raise TypeError("Error: Unable to process number format")
 
 
 class NumberMember(ParentNumberMember):
     """Contains a number, the attributes inform the client how the number should be
        displayed.
-
-       format is a C printf style format, for example %7.2f means the client should
-       display the number string with seven characters (including the decimal point
-       as a character and leading spaces should be inserted if necessary), and with
-       two decimal digits after the decimal point.
-
-       min is the minimum value
-
-       max is the maximum, if min is equal to max, the client should ignore these.
-
-       step is incremental step values, set to string of zero if not used.
-
-       The above numbers, and the member value must be set as a string, this explicitly
-       controls how numbers are placed in the xml protocol.
     """
 
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, format, min, max, step, membervalue)
         self.format = format
         if not isinstance(min, str):
             raise ParseException("Error: minimum value must be given as a string")
@@ -338,28 +343,27 @@
     def _snapshot(self):
         snapmember = ParentNumberMember(self.name, self.label, self.format, self.min, self.max, self.step, self._membervalue)
         return snapmember
 
 
 class ParentBLOBMember(Member):
 
+    """This class inherits from Member and is the parent of the BLOBMember class.
+       Should you use the ipyclient.snapshot method to create a snapshot,
+       the snapshot vectors for BLOBs will contain objects of this class."""
+
+
     def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=None):
         super().__init__(name, label, membervalue)
         self.blobsize = blobsize
         self.blobformat = blobformat
 
 
 class BLOBMember(ParentBLOBMember):
-    """Contains a 'binary large object' such as an image.
-
-       blobsize is the size of the BLOB before any compression, if left at
-       zero, the length of the BLOB will be used.
-
-       The BLOB format should be a string describing the BLOB, such as .jpeg
-    """
+    """Contains a 'binary large object' such as an image."""
 
     def __init__(self, name, label=None, blobsize=0, blobformat='', membervalue=None):
         super().__init__(name, label, membervalue)
         if not isinstance(blobsize, int):
             raise ParseException("Error: blobsize must be given as an integer")
         # membervalue can be a byte string, path, string path or file like object
         self.blobsize = blobsize
```

### Comparing `indipyclient-0.0.4/indipyclient/propertyvectors.py` & `indipyclient-0.0.5/indipyclient/propertyvectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 from .propertymembers import SwitchMember, LightMember, TextMember, NumberMember, BLOBMember
 
 from .error import ParseException
 
 
 class Vector(collections.UserDict):
 
+    """This class is the parent of the PropertyVector class, which in turn
+       is the parent of SwitchVector, LightVector, TextVector, NumberVector
+       and BLOBVector classes.
+       It is a mapping of membername to member value.
+       Should you use the ipyclient.snapshot method to create a snapshot,
+       the snapshot device will contain objects of this vector class. Which
+       does not have the methods of SwitchVector, etc..
+       This allows the snapshot to be read without risk of creating any
+       side effects.
+       """
+
+
+
     def __init__(self, name, label, group, state, timestamp, message):
         super().__init__()
 
         self.name = name
         self.label = label
         self.group = group
         self._state = state
@@ -71,15 +84,15 @@
     def memberlabel(self, membername):
         "Returns the member label, given a member name"
         return self.data[membername].label
 
 
 
 class PropertyVector(Vector):
-    "Parent class of SwitchVector etc.."
+    "Inherits from Vector, and is the parent class of SwitchVector etc.."
 
     def __init__(self, name, label, group, state, timestamp, message, device, client):
         super().__init__(name, label, group, state, timestamp, message)
         self._client = client
         self.device = device
         self.devicename = device.devicename
 
@@ -139,15 +152,16 @@
         if event.state:
             self.state = event.state
         if event.timestamp:
             self.timestamp = event.timestamp
         if event.message:
             self.message = event.message
         if hasattr(event, 'timeout'):
-            self.timeout = event.timeout
+            if not self.timeout is None:
+                self.timeout = event.timeout
         for membername, membervalue in event.items():
             if membername in self.data:
                 member = self.data[membername]
                 member.membervalue = membervalue
 
 
     def _snapshot(self):
@@ -280,15 +294,16 @@
             xmldata.append(switch.oneswitch(value))
         return xmldata
 
 
     def send_newSwitchVector(self, timestamp=None, members={}):
         """Transmits the vector (newSwitchVector) and the members given in the members
            dictionary which consists of member names:values to be sent.
-           This method will transmit the xml, and change the vector state to busy."""
+           This method will encode and transmit the xml, and change the vector state to busy.
+           If no timestamp is given, a current UTC time will be created."""
         xmldata = self._newSwitchVector(timestamp, members)
         if xmldata is None:
             return
         self._timer = True
         self._newtimer = time.time()
         self._client.send(xmldata)
 
@@ -432,26 +447,37 @@
                 xmldata.append(textmember.onetext(members[membername]))
             else:
                 xmldata.append(textmember.onetext(textmember.membervalue))
         return xmldata
 
 
     def send_newTextVector(self, timestamp=None, members={}):
-        """Transmits the vector (newTextVector) together with all text members.
-           (The spec requires text vectors to be sent with all members)
-           This method will transmit the vector and change the vector state to busy."""
+        """Transmits the vector (newTextVector) with members and values.
+           The spec requires text vectors to be sent with all members, so if the given
+           members dictionary only includes changed values, the remaining members with
+           unchanged values will still be sent.
+           This method will transmit the vector and change the vector state to busy.
+           If no timestamp is given, a current UTC time will be created."""
         xmldata = self._newTextVector(timestamp, members)
         if xmldata is None:
             return
         self._timer = True
         self._newtimer = time.time()
         self._client.send(xmldata)
 
 
 class NumberVector(PropertyVector):
+    """A NumberVector is used to send and receive numbers between instrument and client.
+       As data is received, this vector is a mapping of membername:membervalue where membervalue
+       is the string of the number taken from the received xml.
+       The INDI spec defines a number of formats, including degrees:minutes:seconds so
+       this class includes methods to obtain the number as a float, and to create a string
+       formatted as the particular member requires.
+       The member objects contain further information label, format spec, minimum, maximum and step size.
+       To obtain the member object, as opposed to the member value, use the members() method."""
 
     def __init__(self, event):
         super().__init__(event.vectorname, event.label, event.group, event.state,
                          event.timestamp, event.message, event.device, event._client)
         self._perm = event.perm
         self.timeout = event.timeout
         # self.data is a dictionary of number name : numbermember
@@ -541,45 +567,50 @@
             if membername in members:
                 xmldata.append(numbermember.onenumber(members[membername]))
             else:
                 xmldata.append(numbermember.onenumber(numbermember.membervalue))
         return xmldata
 
     def send_newNumberVector(self, timestamp=None, members={}):
-        """Transmits the vector (newNumberVector) with new number members
-           together with any unchanged numbers.
-           (The spec requires number vectors to be sent with all members)
-           This method will transmit the vector and change the vector state to busy."""
+        """Transmits the vector (newNumberVector) with members and values.
+           The spec requires number vectors to be sent with all members, so if the given
+           members dictionary only includes changed values, the remaining members with
+           unchanged values will still be sent.
+           This method will transmit the vector and change the vector state to busy.
+           If no timestamp is given, a current UTC time will be created."""
         xmldata = self._newNumberVector(timestamp, members)
         if xmldata is None:
             return
         self._timer = True
         self._newtimer = time.time()
         self._client.send(xmldata)
 
 
 
 class BLOBVector(PropertyVector):
 
+    """A BLOBVector is used to send and receive Binary Large Objects between instrument and client.
+       As data is received this vector will be a mapping of membername to membervalue where membervalue
+       will be a binary string of the received BLOB.  This binary string has been decoded from the
+       received XML and from the b64 encoding used.
+       The member object contains further information, label, blobsize and blobformat.
+       To obtain the member object, as opposed to the member value, use the members() method."""
+
     def __init__(self, event):
         super().__init__(event.vectorname, event.label, event.group, event.state,
                          event.timestamp, event.message, event.device, event._client)
         self._perm = event.perm
         self.timeout = event.timeout
         # self.data is a dictionary of blob name : blobmember
         # create  members
         for membername, label in event.memberlabels.items():
             self.data[membername] = BLOBMember(membername, label)
 
     def set_blobsize(self, membername, blobsize):
-        """Sets the blobsize attribute in the blob member. If the default of zero is used,
-           the size will be set to the number of bytes in the BLOB. The INDI standard
-           specifies the size should be that of the BLOB before any compression,
-           therefore if you are sending a compressed file, you should set the blobsize
-           prior to compression with this method."""
+        "Used when an event is received to set the member blobsize"
         if not isinstance(blobsize, int):
             return
         if membername in self.data:
             member = self.data[membername]
         else:
             return
         member.blobsize = blobsize
@@ -669,14 +700,20 @@
                 # expand (value, blobsize, blobformat) to required arguments
                 xmldata.append(blobmember.oneblob(*members[membername]))
         return xmldata
 
     def send_newBLOBVector(self, timestamp=None, members={}):
         """Transmits the vector (newBLOBVector) with new BLOB members
            This method will transmit the vector and change the vector state to busy.
-           members dictionary should be {membername:(value, blobsize, blobformat)}"""
+           The members dictionary should be {membername:(value, blobsize, blobformat)}
+           The value could be a bytes object, a pathlib.Path or a file-like object.
+           If blobsize of zero is used, the size value sent will be set to the number of bytes
+           in the BLOB. The INDI standard specifies the size should be that of the BLOB
+           before any compression, therefore if you are sending a compressed file, you
+           should set the blobsize prior to compression.
+           blobformat should be a file extension, such as '.png'"""
         xmldata = self._newBLOBVector(timestamp, members)
         if xmldata is None:
             return
         self._timer = True
         self._newtimer = time.time()
         self._client.send(xmldata)
```

### Comparing `indipyclient-0.0.4/pyproject.toml` & `indipyclient-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.4"
+version = "0.0.5"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.4/PKG-INFO` & `indipyclient-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -12,17 +12,15 @@
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Project-URL: Documentation, https://indipyclient.readthedocs.io
 Project-URL: Source, https://github.com/bernie-skipole/indipyclient
 
 # indipyclient
 Terminal client to communicate to an INDI service.
 
-NOTE: CURRENTLY STILL UNDER DEVELOPMENT
-
-This is a pure python package, with no dependencies, providing an INDI client terminal
+This is a pure python package, with no dependencies, providing an INDI terminal client.
 
 It also provides a set of classes which can be used to create an INDI client. Either a script, or a GUI implementation could use this to generate the INDI protocol XML, and to create the connection to a port serving INDI drivers.
 
 The client can be run with
 
 indipyclient [options]
```

