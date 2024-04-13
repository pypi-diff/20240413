# Comparing `tmp/pynovnc-1.0.4.tar.gz` & `tmp/pynovnc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.0.4.tar", last modified: Sat Apr 13 08:02:53 2024, max compression
+gzip compressed data, was "pynovnc-1.0.5.tar", last modified: Sat Apr 13 08:12:12 2024, max compression
```

## Comparing `pynovnc-1.0.4.tar` & `pynovnc-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:02:53.041330 pynovnc-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 08:02:53.041330 pynovnc-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-04-13 08:02:43.000000 pynovnc-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:02:53.039330 pynovnc-1.0.4/pynovnc/
--rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-13 08:02:43.000000 pynovnc-1.0.4/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:02:53.040330 pynovnc-1.0.4/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-13 08:02:52.000000 pynovnc-1.0.4/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-13 08:02:53.000000 pynovnc-1.0.4/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:02:52.000000 pynovnc-1.0.4/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:02:52.000000 pynovnc-1.0.4/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:02:52.000000 pynovnc-1.0.4/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:02:53.041330 pynovnc-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2882 2024-04-13 08:02:43.000000 pynovnc-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.334454 pynovnc-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:12:12.334454 pynovnc-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.332453 pynovnc-1.0.5/pynovnc/
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.5/pynovnc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.333454 pynovnc-1.0.5/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:12:12.334454 pynovnc-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2882 2024-04-13 08:09:24.000000 pynovnc-1.0.5/setup.py
```

### Comparing `pynovnc-1.0.4/PKG-INFO` & `pynovnc-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Package made by Mhadhbi Issam . 
-Home-page: https://gitlab.com/isampypi/pynovnc
-Author: Mhadhbi Issam
+Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
+Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bashi
 
 # pynovnc
 
 <a href="https://colab.research.google.com/drive/1SMHc4PmG9AjnotQD6R5KQQfL7dNvvyE0" style="background-color: #007bff; color: white; padding: 10px 20px; border-radius: 5px; text-decoration: none; display: inline-block;width:100%;text-align:center;font-weight:900;font-size:30">Colab</a>
 
 ## Install Requiements  : 
 ```bash
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.4 Summary: Python Package made
-by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
-Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
-apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
-apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
-: ```bash pip install pynovnc ``` ## Quick start : ```python with
-VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(["gedit"]) port =
-x.vncport app.wait() ```
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.5 Summary: Python Package made
+by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
+zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
+email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
+Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
+x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
+utils gnumeric ``` ## Installation : ```bash pip install pynovnc ``` ## Quick
+start : ```python with VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(
+["gedit"]) port = x.vncport app.wait() ```
```

### Comparing `pynovnc-1.0.4/README.md` & `pynovnc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.4/pynovnc/__init__.py` & `pynovnc-1.0.5/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.4/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.0.5/pynovnc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python Package made by Mhadhbi Issam . 
-Home-page: https://gitlab.com/isampypi/pynovnc
-Author: Mhadhbi Issam
+Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
+Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bashi
 
 # pynovnc
 
 <a href="https://colab.research.google.com/drive/1SMHc4PmG9AjnotQD6R5KQQfL7dNvvyE0" style="background-color: #007bff; color: white; padding: 10px 20px; border-radius: 5px; text-decoration: none; display: inline-block;width:100%;text-align:center;font-weight:900;font-size:30">Colab</a>
 
 ## Install Requiements  : 
 ```bash
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.4 Summary: Python Package made
-by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
-Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
-apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
-apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
-: ```bash pip install pynovnc ``` ## Quick start : ```python with
-VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(["gedit"]) port =
-x.vncport app.wait() ```
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.5 Summary: Python Package made
+by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
+zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
+email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
+Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
+x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
+utils gnumeric ``` ## Installation : ```bash pip install pynovnc ``` ## Quick
+start : ```python with VirtualDisplay(h = 1040 , w = 1920 ) as x : app = x.run(
+["gedit"]) port = x.vncport app.wait() ```
```

### Comparing `pynovnc-1.0.4/setup.py` & `pynovnc-1.0.5/setup.py`

 * *Files identical despite different names*

