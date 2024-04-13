# Comparing `tmp/pynovnc-1.0.8.tar.gz` & `tmp/pynovnc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.0.8.tar", last modified: Sat Apr 13 08:20:29 2024, max compression
+gzip compressed data, was "pynovnc-1.0.9.tar", last modified: Sat Apr 13 08:24:33 2024, max compression
```

## Comparing `pynovnc-1.0.8.tar` & `pynovnc-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:20:29.482535 pynovnc-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:20:29.481535 pynovnc-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:20:29.477534 pynovnc-1.0.8/pynovnc/
--rw-r--r--   0 root         (0) root         (0)      109 2024-04-13 08:19:04.000000 pynovnc-1.0.8/pynovnc/Main.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.8/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:20:29.481535 pynovnc-1.0.8/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:20:29.000000 pynovnc-1.0.8/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:20:29.482535 pynovnc-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3019 2024-04-13 08:20:22.000000 pynovnc-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:24:33.015560 pynovnc-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-13 08:24:33.015560 pynovnc-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      733 2024-04-13 08:23:13.000000 pynovnc-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:24:33.013559 pynovnc-1.0.9/pynovnc/
+-rw-r--r--   0 root         (0) root         (0)      173 2024-04-13 08:24:25.000000 pynovnc-1.0.9/pynovnc/Main.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.9/pynovnc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:24:33.014559 pynovnc-1.0.9/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:24:32.000000 pynovnc-1.0.9/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:24:33.015560 pynovnc-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3019 2024-04-13 08:20:22.000000 pynovnc-1.0.9/setup.py
```

### Comparing `pynovnc-1.0.8/PKG-INFO` & `pynovnc-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
 Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,13 +22,14 @@
 ## Installation : 
 ```bash
 pip install pynovnc 
 ```
 
 ## Quick start : 
 ```python
+from pynovnc import VirtualDisplay
 with  VirtualDisplay(h = 1040 , w = 1920 ) as x :
     app = x.run(["gedit"])
     port = x.vncport
     app.wait()
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.8 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.9 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
 utils gnumeric ``` ## Installation : ```bash pip install pynovnc ``` ## Quick
-start : ```python with VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(
-["gedit"]) port = x.vncport app.wait() ```
+start : ```python from pynovnc import VirtualDisplay with VirtualDisplay(h =
+1040 , w = 1920 ) as x : app = x.run(["gedit"]) port = x.vncport app.wait() ```
```

### Comparing `pynovnc-1.0.8/README.md` & `pynovnc-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 ## Installation : 
 ```bash
 pip install pynovnc 
 ```
 
 ## Quick start : 
 ```python
+from pynovnc import VirtualDisplay
 with  VirtualDisplay(h = 1040 , w = 1920 ) as x :
     app = x.run(["gedit"])
     port = x.vncport
     app.wait()
 ```
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 # pynovnc _C_o_l_a_b ## Install Requiements : ```bash apt install -y --fix-missing
 xserver-xephyr x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit
 tightvncserver x11-utils gnumeric ``` ## Installation : ```bash pip install
-pynovnc ``` ## Quick start : ```python with VirtualDisplay(h = 1040 , w = 1920
-) as x : app = x.run(["gedit"]) port = x.vncport app.wait() ```
+pynovnc ``` ## Quick start : ```python from pynovnc import VirtualDisplay with
+VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(["gedit"]) port =
+x.vncport app.wait() ```
```

### Comparing `pynovnc-1.0.8/pynovnc/__init__.py` & `pynovnc-1.0.9/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.8/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.0.9/pynovnc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
 Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,13 +22,14 @@
 ## Installation : 
 ```bash
 pip install pynovnc 
 ```
 
 ## Quick start : 
 ```python
+from pynovnc import VirtualDisplay
 with  VirtualDisplay(h = 1040 , w = 1920 ) as x :
     app = x.run(["gedit"])
     port = x.vncport
     app.wait()
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.8 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.9 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
 utils gnumeric ``` ## Installation : ```bash pip install pynovnc ``` ## Quick
-start : ```python with VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(
-["gedit"]) port = x.vncport app.wait() ```
+start : ```python from pynovnc import VirtualDisplay with VirtualDisplay(h =
+1040 , w = 1920 ) as x : app = x.run(["gedit"]) port = x.vncport app.wait() ```
```

### Comparing `pynovnc-1.0.8/setup.py` & `pynovnc-1.0.9/setup.py`

 * *Files identical despite different names*

