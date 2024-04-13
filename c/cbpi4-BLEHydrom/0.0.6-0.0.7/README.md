# Comparing `tmp/cbpi4-BLEHydrom-0.0.6.tar.gz` & `tmp/cbpi4-BLEHydrom-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-BLEHydrom-0.0.6.tar", last modified: Fri Jan 12 14:28:10 2024, max compression
+gzip compressed data, was "cbpi4-BLEHydrom-0.0.7.tar", last modified: Sat Apr 13 13:10:57 2024, max compression
```

## Comparing `cbpi4-BLEHydrom-0.0.6.tar` & `cbpi4-BLEHydrom-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 14:28:10.393426 cbpi4-BLEHydrom-0.0.6/
--rw-rw-rw-   0        0        0    35149 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       78 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5769 2024-01-12 14:28:10.392425 cbpi4-BLEHydrom-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5352 2024-01-12 14:27:15.000000 cbpi4-BLEHydrom-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-01-12 14:28:10.346425 cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/
--rw-rw-rw-   0        0        0     7532 2024-01-10 20:19:33.000000 cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/__init__.py
--rw-rw-rw-   0        0        0     7701 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/blescan.py
--rw-rw-rw-   0        0        0       32 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/config.yaml
-drwxrwxrwx   0        0        0        0 2024-01-12 14:28:10.390425 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/
--rw-rw-rw-   0        0        0     5769 2024-01-12 14:28:09.000000 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-01-12 14:28:09.000000 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 14:28:09.000000 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2024-01-12 14:28:09.000000 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-12 14:28:09.000000 cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-12 14:28:10.393426 cbpi4-BLEHydrom-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1398 2024-01-12 14:27:23.000000 cbpi4-BLEHydrom-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:10:57.883178 cbpi4-BLEHydrom-0.0.7/
+-rw-rw-rw-   0        0        0    35149 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       78 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5825 2024-04-13 13:10:57.881175 cbpi4-BLEHydrom-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5407 2024-04-13 11:10:17.000000 cbpi4-BLEHydrom-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 13:10:57.837421 cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/
+-rw-rw-rw-   0        0        0     7532 2024-01-10 20:19:33.000000 cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/__init__.py
+-rw-rw-rw-   0        0        0     7701 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/blescan.py
+-rw-rw-rw-   0        0        0       32 2022-02-25 17:25:07.000000 cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/config.yaml
+drwxrwxrwx   0        0        0        0 2024-04-13 13:10:57.879174 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/
+-rw-rw-rw-   0        0        0     5825 2024-04-13 13:10:57.000000 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-13 13:10:57.000000 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 13:10:57.000000 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-04-13 13:10:57.000000 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-13 13:10:57.000000 cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 13:10:57.883178 cbpi4-BLEHydrom-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-13 11:09:49.000000 cbpi4-BLEHydrom-0.0.7/setup.py
```

### Comparing `cbpi4-BLEHydrom-0.0.6/LICENSE` & `cbpi4-BLEHydrom-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-BLEHydrom-0.0.6/PKG-INFO` & `cbpi4-BLEHydrom-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-BLEHydrom
-Version: 0.0.6
+Version: 0.0.7
 Summary: CraftBeerPi4 Plugin for Hydrom and Tilt (BLE connection)
 Home-page: https://github.com/avollkopf/cbpi4-BLEHydrom
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -62,14 +62,15 @@
 - To fine tune the calibration even more, you can make a low and/or high gravity calibration point by taking readings of one or two solutions with a known gravity and enter those readings as ***tilt reading* = *solution's actual gravity***.
 - If you enter only a single calibration point, the difference will be applied to every reading equally. So you could enter **0 = 5** if you just want 5 added to every reading that the Tilt takes, or **5 = 0** if you want to subtract 5 from every reading.  If you enter two or more calibration points, a linear relationship between the points will be determined and used to adjust the readings accordingly (known as linear regression).
 - These calibration procedures work the same for both gravity readings and temperature readings, and are calculated after the conversion to the desired units (°C to °F, SG to Brix), so you should calibrate your Tilt with the units set to what they will be when you use it for actual brewing.
 
 
 ### Changelog:
 
+- 13.04.24: (0.0.7) Test with new gattlib-dbus package
 - 10.01.23: (0.0.6) Test with PyBluez Mod as interim solution
 - 01.12.23: (0.0.6.a1) updated requirements
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 25.02.22: (0.0.4) Updated README
 - 16.01.22: (0.0.3) Reduced mqtt traffic (->cbpi 4.0.1.2 required!!)
 - 08.01.22: (0.0.2) Added RSSI value from blescan as parameter
 - 07.01.22: (0.0.1) Initial Commit
```

### Comparing `cbpi4-BLEHydrom-0.0.6/README.md` & `cbpi4-BLEHydrom-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 - To fine tune the calibration even more, you can make a low and/or high gravity calibration point by taking readings of one or two solutions with a known gravity and enter those readings as ***tilt reading* = *solution's actual gravity***.
 - If you enter only a single calibration point, the difference will be applied to every reading equally. So you could enter **0 = 5** if you just want 5 added to every reading that the Tilt takes, or **5 = 0** if you want to subtract 5 from every reading.  If you enter two or more calibration points, a linear relationship between the points will be determined and used to adjust the readings accordingly (known as linear regression).
 - These calibration procedures work the same for both gravity readings and temperature readings, and are calculated after the conversion to the desired units (°C to °F, SG to Brix), so you should calibrate your Tilt with the units set to what they will be when you use it for actual brewing.
 
 
 ### Changelog:
 
+- 13.04.24: (0.0.7) Test with new gattlib-dbus package
 - 10.01.23: (0.0.6) Test with PyBluez Mod as interim solution
 - 01.12.23: (0.0.6.a1) updated requirements
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 25.02.22: (0.0.4) Updated README
 - 16.01.22: (0.0.3) Reduced mqtt traffic (->cbpi 4.0.1.2 required!!)
 - 08.01.22: (0.0.2) Added RSSI value from blescan as parameter
 - 07.01.22: (0.0.1) Initial Commit
```

### Comparing `cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/__init__.py` & `cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/__init__.py`

 * *Files identical despite different names*

### Comparing `cbpi4-BLEHydrom-0.0.6/cbpi4-BLEHydrom/blescan.py` & `cbpi4-BLEHydrom-0.0.7/cbpi4-BLEHydrom/blescan.py`

 * *Files identical despite different names*

### Comparing `cbpi4-BLEHydrom-0.0.6/cbpi4_BLEHydrom.egg-info/PKG-INFO` & `cbpi4-BLEHydrom-0.0.7/cbpi4_BLEHydrom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-BLEHydrom
-Version: 0.0.6
+Version: 0.0.7
 Summary: CraftBeerPi4 Plugin for Hydrom and Tilt (BLE connection)
 Home-page: https://github.com/avollkopf/cbpi4-BLEHydrom
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -62,14 +62,15 @@
 - To fine tune the calibration even more, you can make a low and/or high gravity calibration point by taking readings of one or two solutions with a known gravity and enter those readings as ***tilt reading* = *solution's actual gravity***.
 - If you enter only a single calibration point, the difference will be applied to every reading equally. So you could enter **0 = 5** if you just want 5 added to every reading that the Tilt takes, or **5 = 0** if you want to subtract 5 from every reading.  If you enter two or more calibration points, a linear relationship between the points will be determined and used to adjust the readings accordingly (known as linear regression).
 - These calibration procedures work the same for both gravity readings and temperature readings, and are calculated after the conversion to the desired units (°C to °F, SG to Brix), so you should calibrate your Tilt with the units set to what they will be when you use it for actual brewing.
 
 
 ### Changelog:
 
+- 13.04.24: (0.0.7) Test with new gattlib-dbus package
 - 10.01.23: (0.0.6) Test with PyBluez Mod as interim solution
 - 01.12.23: (0.0.6.a1) updated requirements
 - 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 25.02.22: (0.0.4) Updated README
 - 16.01.22: (0.0.3) Reduced mqtt traffic (->cbpi 4.0.1.2 required!!)
 - 08.01.22: (0.0.2) Added RSSI value from blescan as parameter
 - 07.01.22: (0.0.1) Initial Commit
```

### Comparing `cbpi4-BLEHydrom-0.0.6/setup.py` & `cbpi4-BLEHydrom-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(name='cbpi4-BLEHydrom',
-      version='0.0.6',
+      version='0.0.7',
       description='CraftBeerPi4 Plugin for Hydrom and Tilt (BLE connection)',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/avollkopf/cbpi4-BLEHydrom',
       include_package_data=True,
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-BLEHydrom': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-BLEHydrom'],
       install_requires=[
       'PyBluez @ https://github.com/AcrossTheCloud/pybluez/archive/master.zip#egg=PyBluez-0.30',
-      'gattlib==0.20210616',
+      'gattlib-dbus @ https://github.com/oscaracena/pygattlib/archive/dbus.zip#egg=gattlib-dbus-24.1.8',
       ],
       long_description=long_description,
       long_description_content_type='text/markdown'
      )
```

