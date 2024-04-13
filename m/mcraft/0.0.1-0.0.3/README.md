# Comparing `tmp/mcraft-0.0.1.tar.gz` & `tmp/mcraft-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcraft-0.0.1.tar", last modified: Thu Apr 11 22:28:24 2024, max compression
+gzip compressed data, was "mcraft-0.0.3.tar", last modified: Sat Apr 13 17:03:56 2024, max compression
```

## Comparing `mcraft-0.0.1.tar` & `mcraft-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:24.608703 mcraft-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 22:28:19.000000 mcraft-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-11 22:28:24.608703 mcraft-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-11 22:28:19.000000 mcraft-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:24.608703 mcraft-0.0.1/mcraft/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:24.608703 mcraft-0.0.1/mcraft/basenet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/basenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/basenet/vgg16_bn.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/craft.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9099 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/craft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/networks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2509 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/refinenet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-11 22:28:19.000000 mcraft-0.0.1/mcraft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:28:24.608703 mcraft-0.0.1/mcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-11 22:28:24.000000 mcraft-0.0.1/mcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 22:28:24.000000 mcraft-0.0.1/mcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:28:24.000000 mcraft-0.0.1/mcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 22:28:24.000000 mcraft-0.0.1/mcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 22:28:24.000000 mcraft-0.0.1/mcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:28:24.608703 mcraft-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-11 22:28:19.000000 mcraft-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:56.704591 mcraft-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-13 17:03:52.000000 mcraft-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-13 17:03:56.704591 mcraft-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-13 17:03:52.000000 mcraft-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:56.704591 mcraft-0.0.3/mcraft/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:56.704591 mcraft-0.0.3/mcraft/basenet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/basenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/basenet/vgg16_bn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2796 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/craft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9099 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/craft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/networks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2509 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/refinenet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-13 17:03:52.000000 mcraft-0.0.3/mcraft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:03:56.704591 mcraft-0.0.3/mcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-13 17:03:56.000000 mcraft-0.0.3/mcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 17:03:56.000000 mcraft-0.0.3/mcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:03:56.000000 mcraft-0.0.3/mcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 17:03:56.000000 mcraft-0.0.3/mcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 17:03:56.000000 mcraft-0.0.3/mcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:03:56.704591 mcraft-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-13 17:03:52.000000 mcraft-0.0.3/setup.py
```

### Comparing `mcraft-0.0.1/LICENSE` & `mcraft-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/PKG-INFO` & `mcraft-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcraft
-Version: 0.0.1
+Version: 0.0.3
 Summary: A modern version of CRAFT-pytorch using the latest versions
 Home-page: https://github.com/manbehindthemadness/modern-craft
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 License-File: LICENSE
 Requires-Dist: scikit-image>=0.14.2
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: numpy
 Requires-Dist: opencv-python>=3.4.2.17
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 # Modern CRAFT Library
 
 ## Overview
 This Python library provides an interface for using the CRAFT (Character Region Awareness For Text Detection) algorithm for text detection in images. The library is based on the CRAFT implementation in Python.
 
 This is an adaptation of the CRAFT-python library allowing for use on modern packages (pytorch 2 > opencv-python > 3.4).
@@ -36,15 +37,15 @@
 - NumPy
 
 ## Installation
 You can install the library via pip:
 
 
 ```
-pip install modern-craft
+pip install mcraft
 ```
 
 ## Usage
 
 ```
     from mcraft import TNet
```

### Comparing `mcraft-0.0.1/README.md` & `mcraft-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - NumPy
 
 ## Installation
 You can install the library via pip:
 
 
 ```
-pip install modern-craft
+pip install mcraft
 ```
 
 ## Usage
 
 ```
     from mcraft import TNet
```

### Comparing `mcraft-0.0.1/mcraft/basenet/vgg16_bn.py` & `mcraft-0.0.3/mcraft/basenet/vgg16_bn.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/craft.py` & `mcraft-0.0.3/mcraft/craft.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/craft_utils.py` & `mcraft-0.0.3/mcraft/craft_utils.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/file_utils.py` & `mcraft-0.0.3/mcraft/file_utils.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/imgproc.py` & `mcraft-0.0.3/mcraft/imgproc.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/networks.py` & `mcraft-0.0.3/mcraft/networks.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/refinenet.py` & `mcraft-0.0.3/mcraft/refinenet.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft/utils.py` & `mcraft-0.0.3/mcraft/utils.py`

 * *Files identical despite different names*

### Comparing `mcraft-0.0.1/mcraft.egg-info/PKG-INFO` & `mcraft-0.0.3/mcraft.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcraft
-Version: 0.0.1
+Version: 0.0.3
 Summary: A modern version of CRAFT-pytorch using the latest versions
 Home-page: https://github.com/manbehindthemadness/modern-craft
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 License-File: LICENSE
 Requires-Dist: scikit-image>=0.14.2
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: numpy
 Requires-Dist: opencv-python>=3.4.2.17
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 # Modern CRAFT Library
 
 ## Overview
 This Python library provides an interface for using the CRAFT (Character Region Awareness For Text Detection) algorithm for text detection in images. The library is based on the CRAFT implementation in Python.
 
 This is an adaptation of the CRAFT-python library allowing for use on modern packages (pytorch 2 > opencv-python > 3.4).
@@ -36,15 +37,15 @@
 - NumPy
 
 ## Installation
 You can install the library via pip:
 
 
 ```
-pip install modern-craft
+pip install mcraft
 ```
 
 ## Usage
 
 ```
     from mcraft import TNet
```

### Comparing `mcraft-0.0.1/setup.py` & `mcraft-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 install_requires = [
     'scikit-image>=0.14.2',
     'scipy>=1.1.0',
     'numpy',
     'opencv-python>=3.4.2.17',
     'torch>=2.0.0',
-    'torchvision>=0.17.0'
+    'torchvision>=0.17.0',
+    'quickdl',
 ]
 
 excludes = [
     'opencv-python:cv2',
     'torch',
     'torchvision'
 ]
@@ -26,15 +27,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='mcraft',
-    version='0.0.1',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

