# Comparing `tmp/pynovnc-1.0.5.tar.gz` & `tmp/pynovnc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.0.5.tar", last modified: Sat Apr 13 08:12:12 2024, max compression
+gzip compressed data, was "pynovnc-1.0.6.tar", last modified: Sat Apr 13 08:16:43 2024, max compression
```

## Comparing `pynovnc-1.0.5.tar` & `pynovnc-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.334454 pynovnc-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:12:12.334454 pynovnc-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.332453 pynovnc-1.0.5/pynovnc/
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.5/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:12:12.333454 pynovnc-1.0.5/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:12:12.000000 pynovnc-1.0.5/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:12:12.334454 pynovnc-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2882 2024-04-13 08:09:24.000000 pynovnc-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.169286 pynovnc-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:16:43.168286 pynovnc-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.165286 pynovnc-1.0.6/pynovnc/
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.6/pynovnc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-13 08:15:46.000000 pynovnc-1.0.6/pynovnc/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.168286 pynovnc-1.0.6/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:16:43.169286 pynovnc-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-04-13 08:16:36.000000 pynovnc-1.0.6/setup.py
```

### Comparing `pynovnc-1.0.5/PKG-INFO` & `pynovnc-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
 Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.5 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.6 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
```

### Comparing `pynovnc-1.0.5/README.md` & `pynovnc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.5/pynovnc/__init__.py` & `pynovnc-1.0.6/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.5/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.0.6/pynovnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://mhadhbixissam:glpat-6Y95Caz-zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git
 Author: mhadhbixissam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.5 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.6 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
```

### Comparing `pynovnc-1.0.5/setup.py` & `pynovnc-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from setuptools import setup, find_packages
 import os , requests 
 import subprocess
-import subprocess
 
 
 
 
 
 class PypiPublisher : 
     def __init__(self, start_version = "1.0.0") : 
@@ -34,14 +33,19 @@
             url= url    ,
             install_requires=["bashi"]  ,
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
+            entry_points={
+                'console_scripts': [
+                    f'{self.name} = {self.name}:main'
+                ]
+            }
         )
     def get_versions(self) : 
         response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
         version = self.start_version
         if response.status_code == 200 : 
             version  = response.json()["info"]["version"]
```

