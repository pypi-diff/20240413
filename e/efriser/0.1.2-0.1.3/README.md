# Comparing `tmp/efriser-0.1.2.tar.gz` & `tmp/efriser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.2.tar", last modified: Sat Apr 13 17:44:23 2024, max compression
+gzip compressed data, was "efriser-0.1.3.tar", last modified: Sat Apr 13 17:54:24 2024, max compression
```

## Comparing `efriser-0.1.2.tar` & `efriser-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.292012 efriser-0.1.2/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:44:23.292012 efriser-0.1.2/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      158 2024-04-13 17:29:42.000000 efriser-0.1.2/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.288011 efriser-0.1.2/efriser/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       54 2024-04-13 17:43:29.000000 efriser-0.1.2/efriser/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6221 2024-04-13 17:33:36.000000 efriser-0.1.2/efriser/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.2/efriser/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.2/efriser/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.2/efriser/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.2/efriser/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:44:23.292012 efriser-0.1.2/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      295 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        8 2024-04-13 17:44:23.000000 efriser-0.1.2/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 17:44:23.292012 efriser-0.1.2/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 17:43:52.000000 efriser-0.1.2/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:54:24.111937 efriser-0.1.3/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:54:24.111937 efriser-0.1.3/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      179 2024-04-13 17:44:30.000000 efriser-0.1.3/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:54:24.107936 efriser-0.1.3/efris/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       98 2024-04-13 17:53:52.000000 efriser-0.1.3/efris/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6239 2024-04-13 17:51:45.000000 efriser-0.1.3/efris/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.3/efris/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.3/efris/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.3/efris/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.3/efris/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 17:54:24.111937 efriser-0.1.3/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 17:54:24.000000 efriser-0.1.3/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-13 17:54:24.000000 efriser-0.1.3/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 17:54:24.000000 efriser-0.1.3/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 17:54:24.000000 efriser-0.1.3/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-13 17:54:24.000000 efriser-0.1.3/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 17:54:24.111937 efriser-0.1.3/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 17:54:04.000000 efriser-0.1.3/setup.py
```

### Comparing `efriser-0.1.2/efriser/invoicing.py` & `efriser-0.1.3/efris/invoicing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
-from utils import *
-from services import process_response, encode
-from output_cleaner import *
+from efris.utils import *
+from efris.services import process_response, encode
+from efris.output_cleaner import *
 
 class Efriser:
     def __init__(self, ip, device_number, tin, seller_name):
         self.ip = f'http://{ip}/efristcs/ws/tcsapp/getInformation'
         self.device_number = device_number
         self.tin = tin
         self.seller_name = seller_name
```

### Comparing `efriser-0.1.2/efriser/output_cleaner.py` & `efriser-0.1.3/efris/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.2/efriser/services.py` & `efriser-0.1.3/efris/services.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.2/efriser/utils.py` & `efriser-0.1.3/efris/utils.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.2/setup.py` & `efriser-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='efriser',
-    version='0.1.2',
+    version='0.1.3',
     author='Douglas Ssekuwanda',
     author_email='cytixdoug@gmail.com',
     description='This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.',
     packages=find_packages(),
     install_requires=[
         'requests>=2.24.0',
     ],
```

