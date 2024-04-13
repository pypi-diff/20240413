# Comparing `tmp/mixture-of-depth-0.0.1.tar.gz` & `tmp/mixture-of-depth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-depth-0.0.1.tar", last modified: Fri Apr 12 16:12:00 2024, max compression
+gzip compressed data, was "mixture-of-depth-1.0.0.tar", last modified: Fri Apr 12 16:12:40 2024, max compression
```

## Comparing `mixture-of-depth-0.0.1.tar` & `mixture-of-depth-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/MoD/
--rw-rw-r--   0 marco     (1000) marco     (1000)     4200 2024-04-12 14:12:27.000000 mixture-of-depth-0.0.1/MoD/MoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-0.0.1/MoD/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/MoD/modeling/
--rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-0.0.1/MoD/modeling/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1732 2024-04-12 13:53:03.000000 mixture-of-depth-0.0.1/MoD/modeling/automodeling.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/MoD/modeling/models/
--rw-rw-r--   0 marco     (1000) marco     (1000)    66684 2024-04-12 14:12:27.000000 mixture-of-depth-0.0.1/MoD/modeling/models/GemmaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    76063 2024-04-12 14:12:27.000000 mixture-of-depth-0.0.1/MoD/modeling/models/LlamaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    66827 2024-04-12 14:12:27.000000 mixture-of-depth-0.0.1/MoD/modeling/models/MistralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      130 2024-04-12 13:59:17.000000 mixture-of-depth-0.0.1/MoD/modeling/models/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2120 2024-04-12 12:30:41.000000 mixture-of-depth-0.0.1/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-12 16:12:00.000000 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      428 2024-04-12 16:12:00.000000 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-12 16:12:00.000000 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-12 16:12:00.000000 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-12 16:12:00.000000 mixture-of-depth-0.0.1/mixture_of_depth.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-12 16:12:00.437677 mixture-of-depth-0.0.1/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-12 11:11:25.000000 mixture-of-depth-0.0.1/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:40.629663 mixture-of-depth-1.0.0/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:40.625663 mixture-of-depth-1.0.0/MoD/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     4200 2024-04-12 14:12:27.000000 mixture-of-depth-1.0.0/MoD/MoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.0.0/MoD/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:40.625663 mixture-of-depth-1.0.0/MoD/modeling/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.0.0/MoD/modeling/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1732 2024-04-12 13:53:03.000000 mixture-of-depth-1.0.0/MoD/modeling/automodeling.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:40.625663 mixture-of-depth-1.0.0/MoD/modeling/models/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    66684 2024-04-12 14:12:27.000000 mixture-of-depth-1.0.0/MoD/modeling/models/GemmaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    76063 2024-04-12 14:12:27.000000 mixture-of-depth-1.0.0/MoD/modeling/models/LlamaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    66827 2024-04-12 14:12:27.000000 mixture-of-depth-1.0.0/MoD/modeling/models/MistralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      130 2024-04-12 13:59:17.000000 mixture-of-depth-1.0.0/MoD/modeling/models/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-12 16:12:40.629663 mixture-of-depth-1.0.0/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2120 2024-04-12 12:30:41.000000 mixture-of-depth-1.0.0/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-12 16:12:40.629663 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2682 2024-04-12 16:12:40.000000 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      428 2024-04-12 16:12:40.000000 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-12 16:12:40.000000 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-12 16:12:40.000000 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-12 16:12:40.000000 mixture-of-depth-1.0.0/mixture_of_depth.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-12 16:12:40.629663 mixture-of-depth-1.0.0/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-12 16:12:29.000000 mixture-of-depth-1.0.0/setup.py
```

### Comparing `mixture-of-depth-0.0.1/MoD/MoD.py` & `mixture-of-depth-1.0.0/MoD/MoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/MoD/modeling/automodeling.py` & `mixture-of-depth-1.0.0/MoD/modeling/automodeling.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/MoD/modeling/models/GemmaMoD.py` & `mixture-of-depth-1.0.0/MoD/modeling/models/GemmaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/MoD/modeling/models/LlamaMoD.py` & `mixture-of-depth-1.0.0/MoD/modeling/models/LlamaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/MoD/modeling/models/MistralMoD.py` & `mixture-of-depth-1.0.0/MoD/modeling/models/MistralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/PKG-INFO` & `mixture-of-depth-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 0.0.1
+Version: 1.0.0
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-0.0.1/README.md` & `mixture-of-depth-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-0.0.1/mixture_of_depth.egg-info/PKG-INFO` & `mixture-of-depth-1.0.0/mixture_of_depth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 0.0.1
+Version: 1.0.0
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-0.0.1/setup.py` & `mixture-of-depth-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mixture-of-depth',
-    version='0.0.1',
+    version='1.0.0',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/Mixture-of-depths',
     packages=find_packages(),
```

