# Comparing `tmp/efriser-0.1.4.tar.gz` & `tmp/efriser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.4.tar", last modified: Sat Apr 13 18:59:10 2024, max compression
+gzip compressed data, was "efriser-0.1.5.tar", last modified: Sat Apr 13 19:04:37 2024, max compression
```

## Comparing `efriser-0.1.4.tar` & `efriser-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 18:59:10.671320 efriser-0.1.4/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 18:59:10.671320 efriser-0.1.4/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      197 2024-04-13 18:03:20.000000 efriser-0.1.4/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 18:59:10.667319 efriser-0.1.4/efris/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      132 2024-04-13 18:57:00.000000 efriser-0.1.4/efris/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6253 2024-04-13 18:57:19.000000 efriser-0.1.4/efris/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.4/efris/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.4/efris/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.4/efris/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.4/efris/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 18:59:10.667319 efriser-0.1.4/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 18:59:10.000000 efriser-0.1.4/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-13 18:59:10.000000 efriser-0.1.4/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 18:59:10.000000 efriser-0.1.4/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 18:59:10.000000 efriser-0.1.4/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-13 18:59:10.000000 efriser-0.1.4/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 18:59:10.671320 efriser-0.1.4/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 18:58:56.000000 efriser-0.1.4/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:04:37.668964 efriser-0.1.5/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 19:04:37.668964 efriser-0.1.5/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      197 2024-04-13 18:03:20.000000 efriser-0.1.5/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:04:37.668964 efriser-0.1.5/efris/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      132 2024-04-13 18:57:00.000000 efriser-0.1.5/efris/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6253 2024-04-13 19:04:09.000000 efriser-0.1.5/efris/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-13 16:14:23.000000 efriser-0.1.5/efris/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.5/efris/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.5/efris/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     6816 2024-04-13 16:01:02.000000 efriser-0.1.5/efris/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-13 19:04:37.668964 efriser-0.1.5/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      453 2024-04-13 19:04:37.000000 efriser-0.1.5/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      283 2024-04-13 19:04:37.000000 efriser-0.1.5/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-13 19:04:37.000000 efriser-0.1.5/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-13 19:04:37.000000 efriser-0.1.5/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-13 19:04:37.000000 efriser-0.1.5/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-13 19:04:37.668964 efriser-0.1.5/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      564 2024-04-13 19:04:23.000000 efriser-0.1.5/setup.py
```

### Comparing `efriser-0.1.4/efris/invoicing.py` & `efriser-0.1.5/efris/invoicing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-from efris.utils import *
 from efris.services import process_response, encode
+from efris.utils import *
 from efris.output_cleaner import *
 
 class EFRISInvoicing:
     def __init__(self, ip, device_number, tin, seller_name):
         self.ip = f'http://{ip}/efristcs/ws/tcsapp/getInformation'
         self.device_number = device_number
         self.tin = tin
```

### Comparing `efriser-0.1.4/efris/output_cleaner.py` & `efriser-0.1.5/efris/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.4/efris/services.py` & `efriser-0.1.5/efris/services.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.4/efris/utils.py` & `efriser-0.1.5/efris/utils.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.4/setup.py` & `efriser-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='efriser',
-    version='0.1.4',
+    version='0.1.5',
     author='Douglas Ssekuwanda',
     author_email='cytixdoug@gmail.com',
     description='This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.',
     packages=find_packages(),
     install_requires=[
         'requests>=2.24.0',
     ],
```

