# Comparing `tmp/micropython_senml-0.1.0-py2.py3-none-any.whl.zip` & `tmp/micropython_senml-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10755 bytes, number of entries: 8
+Zip file size: 10743 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     1290 b- defN 20-Feb-02 00:00 senml/__init__.py
 -rw-r--r--  2.0 unx     1232 b- defN 20-Feb-02 00:00 senml/senml_base.py
--rw-r--r--  2.0 unx    11675 b- defN 20-Feb-02 00:00 senml/senml_pack.py
+-rw-r--r--  2.0 unx    11630 b- defN 20-Feb-02 00:00 senml/senml_pack.py
 -rw-r--r--  2.0 unx     9203 b- defN 20-Feb-02 00:00 senml/senml_record.py
 -rw-r--r--  2.0 unx     3062 b- defN 20-Feb-02 00:00 senml/senml_unit.py
-?rw-r--r--  2.0 unx      804 b- defN 20-Feb-02 00:00 micropython_senml-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 micropython_senml-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      617 b- defN 20-Feb-02 00:00 micropython_senml-0.1.0.dist-info/RECORD
-8 files, 27988 bytes uncompressed, 9693 bytes compressed:  65.4%
+?rw-r--r--  2.0 unx      802 b- defN 20-Feb-02 00:00 micropython_senml-0.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 micropython_senml-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      617 b- defN 20-Feb-02 00:00 micropython_senml-0.1.1.dist-info/RECORD
+8 files, 27941 bytes uncompressed, 9681 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -9,17 +9,17 @@
 
 Filename: senml/senml_record.py
 Comment: 
 
 Filename: senml/senml_unit.py
 Comment: 
 
-Filename: micropython_senml-0.1.0.dist-info/METADATA
+Filename: micropython_senml-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: micropython_senml-0.1.0.dist-info/WHEEL
+Filename: micropython_senml-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: micropython_senml-0.1.0.dist-info/RECORD
+Filename: micropython_senml-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## senml/__init__.py

```diff
@@ -26,8 +26,8 @@
 
 from .senml_base import SenmlBase
 from .senml_pack import SenmlPack
 from .senml_record import SenmlRecord
 from .senml_unit import SenmlUnits
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## senml/senml_base.py

```diff
@@ -26,8 +26,8 @@
 
 class SenmlBase(object):
     """
     the base class for all senml objects.
     """
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## senml/senml_pack.py

```diff
@@ -23,16 +23,15 @@
 THE SOFTWARE.
 """
 
 
 from senml.senml_record import SenmlRecord
 from senml.senml_base import SenmlBase
 import json
-from cbor2 import encoder
-from cbor2 import decoder
+import cbor2
 
 
 class SenmlPackIterator:
     """an iterator to walk over all records in a pack"""
 
     def __init__(self, list):
         self._list = list
@@ -43,15 +42,15 @@
 
     def __next__(self):
         if self._index < len(self._list):
             res = self._list[self._index]
             self._index += 1
             return res
         else:
-            raise StopIteration()
+            raise StopIteration
 
 
 class SenmlPack(SenmlBase):
     """
     represents a sneml pack object. This can contain multiple records but also other (child) pack objects.
     When the pack object only contains records, it represents the data of a device.
     If the pack object has child pack objects, then it represents a gateway
@@ -152,15 +151,15 @@
         self._base_time = value
 
     def _check_value_type(self, value, field_name):
         """
         checks if the type of value is allowed for senml
         :return: None, raisee exception if not ok.
         """
-        if not value == None:
+        if value is not None:
             if not (isinstance(value, int) or isinstance(value, float)):
                 raise Exception("invalid type for " + field_name + ", only numbers allowed")
 
     def from_json(self, data):
         """
         parse a json string and convert it to a senml pack structure
         :param data: a string containing json data.
@@ -274,15 +273,15 @@
 
     def from_cbor(self, data):
         """
         parse a cbor data byte array to a senml pack structure.
         :param data: a byte array.
         :return: None
         """
-        records = decoder.loads(data)  # load the raw senml data
+        records = cbor2.loads(data)  # load the raw senml data
         naming_map = {
             "bn": -2,
             "bt": -3,
             "bu": -4,
             "bv": -5,
             "bs": -16,
             "n": 0,
@@ -316,25 +315,25 @@
             "vd": 8,
             "s": 5,
             "t": 6,
             "ut": 7,
         }
         converted = []
         self._build_rec_dict(naming_map, converted)
-        return encoder.dumps(converted)
+        return cbor2.dumps(converted)
 
     def add(self, item):
         """
         adds the item to the list of records
         :param item: {SenmlRecord} the item that needs to be added to the pack
         :return: None
         """
         if not (isinstance(item, SenmlBase)):
             raise Exception("invalid type of param, SenmlRecord or SenmlPack expected")
-        if not item._parent == None:
+        if item._parent is not None:
             raise Exception("item is already part of a pack")
 
         self._data.append(item)
         item._parent = self
 
     def remove(self, item):
         """
@@ -356,8 +355,8 @@
         :return: None
         """
         for item in self._data:
             item._parent = None
         self._data = []
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## senml/senml_record.py

```diff
@@ -75,15 +75,15 @@
             self._parent.remove(self)
 
     def _check_value_type(self, value):
         """
         checks if the type of value is allowed for senml
         :return: None, raisee exception if not ok.
         """
-        if not value == None:
+        if value is not None:
             if not (
                 isinstance(value, bool)
                 or isinstance(value, int)
                 or isinstance(value, float)
                 or isinstance(value, bytearray)
                 or isinstance(value, str)
             ):
@@ -92,15 +92,15 @@
                 )
 
     def _check_number_type(self, value, field_name):
         """
         checks if the type of value is allowed for senml
         :return: None, raisee exception if not ok.
         """
-        if not value == None:
+        if value is not None:
             if not (isinstance(value, int) or isinstance(value, float)):
                 raise Exception("invalid type for " + field_name + ", only numbers allowed")
 
     @property
     def value(self):
         """get the value currently assigned to the object"""
         return self._value
@@ -243,8 +243,8 @@
         :return: None
         """
         self._from_raw(raw, naming_map)
         if self.actuate:
             self.actuate(self)
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## senml/senml_unit.py

```diff
@@ -85,8 +85,8 @@
     SENML_UNIT_EVENT_RATE_PER_MINUTE="1/min",
     SENML_UNIT_BPM="beat/min",
     SENML_UNIT_BEATS="beats",
     SENML_UNIT_SIEMENS_PER_METER="S/m",
 )
 
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

## Comparing `micropython_senml-0.1.0.dist-info/METADATA` & `micropython_senml-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: micropython-senml
-Version: 0.1.0
+Version: 0.1.1
 Summary: SenML serialisation for MicroPython.
 Project-URL: Homepage, https://github.com/micropython/micropython-lib
 Author-email: micropython-lib <contact@micropython.org>
-License: 0.1.0
+License: MIT
 Requires-Dist: cbor2
 Description-Content-Type: text/markdown
 
 # Introduction
 
 The SenML library helps you create and parse [senml documents](https://tools.ietf.org/html/draft-ietf-core-senml-13)
 in both json and cbor format.
```

## Comparing `micropython_senml-0.1.0.dist-info/RECORD` & `micropython_senml-0.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-senml/__init__.py,sha256=Rp92vCztcJUMa-S1YbWf48_ZMpOAnzPWOQvEZV7phk8,1290
-senml/senml_base.py,sha256=nc2TDBjBmV1v_t-cuWD2LqJvgXgmEmg75081mQlhyIg,1232
-senml/senml_pack.py,sha256=X60rb-IspoQFaqx7jXkmLHJeASXwGjBSSTKyA9NrDg0,11675
-senml/senml_record.py,sha256=Woxr1OhS0cnzIbPO_JYn6lY_NWh4NYw7kUL9HrTeqdY,9203
-senml/senml_unit.py,sha256=0bJevySlZ1EyLmvud-TArmqXjySB0yyOhnP8wBhDrNY,3062
-micropython_senml-0.1.0.dist-info/METADATA,sha256=py-AE9bYBCHDKlwxSumW01G42URspi5dEdII0RmxzBc,804
-micropython_senml-0.1.0.dist-info/WHEEL,sha256=3jNpu59JHbFdu1Yeq_fYJQsnHZ21dBRf7JjglSW4K9A,105
-micropython_senml-0.1.0.dist-info/RECORD,,
+senml/__init__.py,sha256=2LfPOLNKe3G4kAyWZfxq9vqbRCzifxmqSibm3KgeTMA,1290
+senml/senml_base.py,sha256=QnMq3p4Civq4S3l8j9CRuX1tg8XJF4EWyTcpp7FG5Ws,1232
+senml/senml_pack.py,sha256=cbvq946HxWYXilWhqmYtGQ4oRdLb8QnnQLxtm8_kx8s,11630
+senml/senml_record.py,sha256=ODzZC7cgsK_caQ7ccFYRI6XcCwCPp9i1Cd1BKOPQn0A,9203
+senml/senml_unit.py,sha256=FezOMX9u88me458sg0CFBt3NjiW7w80_F4cElJrqzrc,3062
+micropython_senml-0.1.1.dist-info/METADATA,sha256=5VuHCnlAHTeU7MwYOM3XDCskgt_UKJixMdfW-iJtbxs,802
+micropython_senml-0.1.1.dist-info/WHEEL,sha256=wpsUbWzR9la66_V7_eWTdyvs6WD26tazKT2BBEAC-EM,105
+micropython_senml-0.1.1.dist-info/RECORD,,
```

