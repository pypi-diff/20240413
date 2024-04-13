# Comparing `tmp/pynovnc-1.0.6.tar.gz` & `tmp/pynovnc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.0.6.tar", last modified: Sat Apr 13 08:16:43 2024, max compression
+gzip compressed data, was "pynovnc-1.0.7.tar", last modified: Sat Apr 13 08:18:17 2024, max compression
```

## Comparing `pynovnc-1.0.6.tar` & `pynovnc-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.169286 pynovnc-1.0.6/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:16:43.168286 pynovnc-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.165286 pynovnc-1.0.6/pynovnc/
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.6/pynovnc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-13 08:15:46.000000 pynovnc-1.0.6/pynovnc/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:16:43.168286 pynovnc-1.0.6/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:16:43.000000 pynovnc-1.0.6/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:16:43.169286 pynovnc-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3014 2024-04-13 08:16:36.000000 pynovnc-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:18:17.364966 pynovnc-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:18:17.364966 pynovnc-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-13 08:09:24.000000 pynovnc-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:18:17.362965 pynovnc-1.0.7/pynovnc/
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-13 08:09:24.000000 pynovnc-1.0.7/pynovnc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-13 08:15:46.000000 pynovnc-1.0.7/pynovnc/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:18:17.364966 pynovnc-1.0.7/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:18:17.000000 pynovnc-1.0.7/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:18:17.365966 pynovnc-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3026 2024-04-13 08:18:10.000000 pynovnc-1.0.7/setup.py
```

### Comparing `pynovnc-1.0.6/PKG-INFO` & `pynovnc-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.6
+Version: 1.0.7
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
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.6 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.7 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
```

### Comparing `pynovnc-1.0.6/README.md` & `pynovnc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.6/pynovnc/__init__.py` & `pynovnc-1.0.7/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.0.6/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.0.7/pynovnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.0.6
+Version: 1.0.7
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
-Metadata-Version: 2.1 Name: pynovnc Version: 1.0.6 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.0.7 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://mhadhbixissam:glpat-6Y95Caz-
 zjCHUJFBUwYg@gitlab.com/isampypi/pynovnc.git Author: mhadhbixissam Author-
 email: mhadhbixissam@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown # pynovnc _C_o_l_a_b ##
 Install Requiements : ```bash apt install -y --fix-missing xserver-xephyr
 x11vnc xvfb novnc net-tools x11-apps x11-xkb-utils gedit tightvncserver x11-
```

### Comparing `pynovnc-1.0.6/setup.py` & `pynovnc-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
             entry_points={
                 'console_scripts': [
-                    f'{self.name} = {self.name}:main'
+                    f'{self.name} = {self.name}.{self.name}:main'
                 ]
             }
         )
     def get_versions(self) : 
         response = requests.get(f"https://pypi.org/pypi/{self.name}/json")
         version = self.start_version
         if response.status_code == 200 :
```

