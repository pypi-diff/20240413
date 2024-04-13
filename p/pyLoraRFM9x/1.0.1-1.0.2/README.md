# Comparing `tmp/pyLoraRFM9x-1.0.1.tar.gz` & `tmp/pylorarfm9x-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLoraRFM9x-1.0.1.tar", last modified: Tue Apr  9 08:40:12 2024, max compression
+gzip compressed data, was "pylorarfm9x-1.0.2.tar", last modified: Sat Apr 13 20:53:10 2024, max compression
```

## Comparing `pyLoraRFM9x-1.0.1.tar` & `pylorarfm9x-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-09 08:40:12.423049 pyLoraRFM9x-1.0.1/
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     1090 2020-08-05 02:42:17.000000 pyLoraRFM9x-1.0.1/LICENSE
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    10053 2024-04-09 08:40:12.423049 pyLoraRFM9x-1.0.1/PKG-INFO
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     7981 2024-04-09 08:26:04.000000 pyLoraRFM9x-1.0.1/README.md
-drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-09 08:40:12.423049 pyLoraRFM9x-1.0.1/pyLoraRFM9x/
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       36 2020-04-11 10:16:58.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x/__init__.py
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     1191 2020-08-05 02:40:20.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x/constants.py
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    14794 2024-04-09 08:25:21.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x/lora.py
-drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-09 08:40:12.423049 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    10053 2024-04-09 08:40:12.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/PKG-INFO
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)      275 2024-04-09 08:40:12.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/SOURCES.txt
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)        1 2024-04-09 08:40:12.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/dependency_links.txt
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       13 2024-04-09 08:40:12.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/requires.txt
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       12 2024-04-09 08:40:12.000000 pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/top_level.txt
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)      828 2024-04-09 08:40:06.000000 pyLoraRFM9x-1.0.1/pyproject.toml
--rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       38 2024-04-09 08:40:12.423049 pyLoraRFM9x-1.0.1/setup.cfg
+drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-13 20:53:10.443902 pylorarfm9x-1.0.2/
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     1090 2020-08-05 02:42:17.000000 pylorarfm9x-1.0.2/LICENSE
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    10097 2024-04-13 20:53:10.443902 pylorarfm9x-1.0.2/PKG-INFO
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     8025 2024-04-13 06:20:13.000000 pylorarfm9x-1.0.2/README.md
+drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-13 20:53:10.440569 pylorarfm9x-1.0.2/pyLoraRFM9x/
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       36 2020-04-11 10:16:58.000000 pylorarfm9x-1.0.2/pyLoraRFM9x/__init__.py
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)     1191 2020-08-05 02:40:20.000000 pylorarfm9x-1.0.2/pyLoraRFM9x/constants.py
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    14795 2024-04-13 06:16:13.000000 pylorarfm9x-1.0.2/pyLoraRFM9x/lora.py
+drwxr-xr-x   0 mugpahug  (1000) mugpahug  (1000)        0 2024-04-13 20:53:10.443902 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)    10097 2024-04-13 20:53:10.000000 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/PKG-INFO
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)      275 2024-04-13 20:53:10.000000 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/SOURCES.txt
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)        1 2024-04-13 20:53:10.000000 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/dependency_links.txt
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       13 2024-04-13 20:53:10.000000 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/requires.txt
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       12 2024-04-13 20:53:10.000000 pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/top_level.txt
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)      828 2024-04-13 06:19:33.000000 pylorarfm9x-1.0.2/pyproject.toml
+-rw-r--r--   0 mugpahug  (1000) mugpahug  (1000)       38 2024-04-13 20:53:10.443902 pylorarfm9x-1.0.2/setup.cfg
```

### Comparing `pyLoraRFM9x-1.0.1/LICENSE` & `pylorarfm9x-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLoraRFM9x-1.0.1/PKG-INFO` & `pylorarfm9x-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLoraRFM9x
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interrupt driven LoRa RFM9x library for Raspberry Pi inspired by RadioHead
 Author-email: Edwin Peters <edwin.g.w.peters@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Anne Wood, 2020 Edwin G.W. Peters
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -206,14 +206,17 @@
 
 [pySX127x](https://github.com/mayeranalytics/pySX127x) - Another Python LoRa library that allows for a bit more configuration. 
 
 [Adafruit CircuitPython module for the RFM95/6/7/8](https://github.com/adafruit/Adafruit_CircuitPython_RFM9x) - LoRa library for CircuitPython
 
 # Changelog
 
+## 1.0.2
+Typo fixed in error handling call
+
 ## 1.0.1
 Added option to select SPI module
 
 ## 1.0.0
 Removed RPi.GPIO dependency and ported to lgpio due to the removal of the sysfs GPIO interface in newer kernels
 
 ## 0.9.4
```

### Comparing `pyLoraRFM9x-1.0.1/README.md` & `pylorarfm9x-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,17 @@
 
 [pySX127x](https://github.com/mayeranalytics/pySX127x) - Another Python LoRa library that allows for a bit more configuration. 
 
 [Adafruit CircuitPython module for the RFM95/6/7/8](https://github.com/adafruit/Adafruit_CircuitPython_RFM9x) - LoRa library for CircuitPython
 
 # Changelog
 
+## 1.0.2
+Typo fixed in error handling call
+
 ## 1.0.1
 Added option to select SPI module
 
 ## 1.0.0
 Removed RPi.GPIO dependency and ported to lgpio due to the removal of the sysfs GPIO interface in newer kernels
 
 ## 0.9.4
```

### Comparing `pyLoraRFM9x-1.0.1/pyLoraRFM9x/constants.py` & `pylorarfm9x-1.0.2/pyLoraRFM9x/constants.py`

 * *Files identical despite different names*

### Comparing `pyLoraRFM9x-1.0.1/pyLoraRFM9x/lora.py` & `pylorarfm9x-1.0.2/pyLoraRFM9x/lora.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
 
                 if self._my_address != header_to and BROADCAST_ADDRESS != header_to and self._receive_all is False:
                     return
 
                 if self.crypto and len(message) % 16 == 0:
                     message = self._decrypt(message)
 
-                if  (header_to == self._my_address and header_flags & FLAGS_REQ_ACK and not header_flags & FLAGS_ACK) and not self._ack:
+                if  (header_to == self._my_address and header_flags & FLAGS_REQ_ACK and not header_flags & FLAGS_ACK) and not self._acks:
                     self.send_ack(header_from, header_id)
 
                 self.set_mode_rx()
 
                 self._last_payload = namedtuple(
                     "Payload",
                     ['message', 'header_to', 'header_from', 'header_id', 'header_flags', 'rssi', 'snr']
```

### Comparing `pyLoraRFM9x-1.0.1/pyLoraRFM9x.egg-info/PKG-INFO` & `pylorarfm9x-1.0.2/pyLoraRFM9x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLoraRFM9x
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interrupt driven LoRa RFM9x library for Raspberry Pi inspired by RadioHead
 Author-email: Edwin Peters <edwin.g.w.peters@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Anne Wood, 2020 Edwin G.W. Peters
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -206,14 +206,17 @@
 
 [pySX127x](https://github.com/mayeranalytics/pySX127x) - Another Python LoRa library that allows for a bit more configuration. 
 
 [Adafruit CircuitPython module for the RFM95/6/7/8](https://github.com/adafruit/Adafruit_CircuitPython_RFM9x) - LoRa library for CircuitPython
 
 # Changelog
 
+## 1.0.2
+Typo fixed in error handling call
+
 ## 1.0.1
 Added option to select SPI module
 
 ## 1.0.0
 Removed RPi.GPIO dependency and ported to lgpio due to the removal of the sysfs GPIO interface in newer kernels
 
 ## 0.9.4
```

### Comparing `pyLoraRFM9x-1.0.1/pyproject.toml` & `pylorarfm9x-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyLoraRFM9x"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Edwin Peters", email="edwin.g.w.peters@gmail.com" },
 ]
 description = "Interrupt driven LoRa RFM9x library for Raspberry Pi inspired by RadioHead"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.5"
```

