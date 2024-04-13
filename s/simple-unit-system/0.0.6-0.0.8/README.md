# Comparing `tmp/simple-unit-system-0.0.6.tar.gz` & `tmp/simple-unit-system-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-unit-system-0.0.6.tar", last modified: Wed Mar 20 18:01:43 2024, max compression
+gzip compressed data, was "simple-unit-system-0.0.8.tar", last modified: Sat Apr 13 02:52:35 2024, max compression
```

## Comparing `simple-unit-system-0.0.6.tar` & `simple-unit-system-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 18:01:43.203183 simple-unit-system-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-09-08 02:54:23.000000 simple-unit-system-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1442 2024-03-20 18:01:43.203183 simple-unit-system-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      881 2024-03-18 19:33:33.000000 simple-unit-system-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 18:01:43.203183 simple-unit-system-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-03-20 18:00:22.000000 simple-unit-system-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 18:01:43.179230 simple-unit-system-0.0.6/src/
--rw-rw-rw-   0        0        0        0 2024-03-18 19:33:13.000000 simple-unit-system-0.0.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 18:01:43.203183 simple-unit-system-0.0.6/src/simple_unit_system.egg-info/
--rw-rw-rw-   0        0        0     1442 2024-03-20 18:01:43.000000 simple-unit-system-0.0.6/src/simple_unit_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-03-20 18:01:43.000000 simple-unit-system-0.0.6/src/simple_unit_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 18:01:43.000000 simple-unit-system-0.0.6/src/simple_unit_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-20 18:01:43.000000 simple-unit-system-0.0.6/src/simple_unit_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6500 2024-03-20 17:55:04.000000 simple-unit-system-0.0.6/src/units.py
+drwxrwxrwx   0        0        0        0 2024-04-13 02:52:35.425697 simple-unit-system-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-09-08 02:54:23.000000 simple-unit-system-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1442 2024-04-13 02:52:35.425697 simple-unit-system-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2024-03-18 19:33:33.000000 simple-unit-system-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 02:52:35.425697 simple-unit-system-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-04-13 02:36:53.000000 simple-unit-system-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 02:52:35.410062 simple-unit-system-0.0.8/src/
+-rw-rw-rw-   0        0        0        0 2024-03-18 19:33:13.000000 simple-unit-system-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 02:52:35.425697 simple-unit-system-0.0.8/src/simple_unit_system.egg-info/
+-rw-rw-rw-   0        0        0     1442 2024-04-13 02:52:35.000000 simple-unit-system-0.0.8/src/simple_unit_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-04-13 02:52:35.000000 simple-unit-system-0.0.8/src/simple_unit_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 02:52:35.000000 simple-unit-system-0.0.8/src/simple_unit_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-13 02:52:35.000000 simple-unit-system-0.0.8/src/simple_unit_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6788 2024-04-13 02:49:41.000000 simple-unit-system-0.0.8/src/units.py
```

### Comparing `simple-unit-system-0.0.6/LICENSE` & `simple-unit-system-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-unit-system-0.0.6/PKG-INFO` & `simple-unit-system-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-unit-system
-Version: 0.0.6
+Version: 0.0.8
 Summary: A framework for applying physical units and performing unit conversions, for scientific and engineering analyses, based on NIST conversions and constants
 Project-URL: Bug Reports, https://github.com/jeffcodez/PhysicalUnits/issues
 Project-URL: Source, https://github.com/jeffcodez/PhysicalUnits
 Keywords: unit,units,physical,system,SI,NIST,engineering,scientific,measurements,weights,physics
 Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `simple-unit-system-0.0.6/README.md` & `simple-unit-system-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `simple-unit-system-0.0.6/setup.py` & `simple-unit-system-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='simple-unit-system',
-    version='0.0.6',
+    version='0.0.8',
     description="A framework for applying physical units and performing unit conversions, for scientific and engineering analyses, based on NIST conversions and constants",
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     install_requires=[
     ],
     keywords=["unit","units","physical","system","SI","NIST","engineering","scientific","measurements","weights","physics",],
     package_dir={"": "src"},
```

### Comparing `simple-unit-system-0.0.6/src/simple_unit_system.egg-info/PKG-INFO` & `simple-unit-system-0.0.8/src/simple_unit_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-unit-system
-Version: 0.0.6
+Version: 0.0.8
 Summary: A framework for applying physical units and performing unit conversions, for scientific and engineering analyses, based on NIST conversions and constants
 Project-URL: Bug Reports, https://github.com/jeffcodez/PhysicalUnits/issues
 Project-URL: Source, https://github.com/jeffcodez/PhysicalUnits
 Keywords: unit,units,physical,system,SI,NIST,engineering,scientific,measurements,weights,physics
 Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `simple-unit-system-0.0.6/src/units.py` & `simple-unit-system-0.0.8/src/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,42 +144,51 @@
         self.CM         = self.M*1.0E-02
         self.KM         = self.M*1.0E+03
         self.NM         = self.M*1852
 
         # mass
         self.SLINCH     = self.SLUG*12
         self.LBM        = self.LBF/self.G0
-        self.OZ         = self.LBM/16
-
+        self.OZM        = self.LBM/16
         self.GM         = self.KG*1.0E-03
                        
         # force - ref Newton
+        self.OZF        = self.LBF/16
         self.TON        = self.LBF*2000
         self.KN         = self.N*1000
 
         # pressure - ref Pascal
         self.PSI        = self.LBF/self.IN**2
         self.KSI        = self.PSI*1.0E3
         self.MSI        = self.PSI*1.0E6
 
         self.PA         = self.N/self.M**2
-        self.BAR        = self.PA
+        self.BAR        = self.PA*1.0E5
 
         # speed ref m/sec
         self.FPS        = self.FT/self.SEC
-        self.FPM        = self.FT/self.MIN
-        self.IPS        = self.IN/self.SEC
         self.MPH        = self.MILE/self.HOUR
 
         self.KPH        = self.KM/self.HOUR
         self.KNOT       = self.NM/self.HOUR
 
         # volume ref m3
         self.QT         = self.GAL/4
         self.CUP        = self.GAL/16
         self.FLOZ       = self.GAL/16/8
         self.TBSP       = self.GAL/16/16
         self.TSP        = self.GAL/16/48
 
         self.L          = self.M3*1.0E-03
         self.ML         = self.M3*1.0E-06
-        self.CC         = self.M3*1.0E-06
+        self.CC         = self.M3*1.0E-06
+        
+        # energy
+        self.J          = self.KG*self.M**2/self.SEC**2
+        self.BTU        = self.J*1.055056E03
+        self.CAL        = self.J*4.1868
+        
+        # power
+        self.W          = self.KG*self.M**2/self.SEC**2
+        self.HP         = self.FT*self.LBF/self.SEC*550
+        
+
```

