# Comparing `tmp/tiffx-0.1.0.tar.gz` & `tmp/tiffx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiffx-0.1.0.tar", last modified: Sat Apr 13 01:49:11 2024, max compression
+gzip compressed data, was "tiffx-0.1.1.tar", last modified: Sat Apr 13 03:34:43 2024, max compression
```

## Comparing `tiffx-0.1.0.tar` & `tiffx-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 01:49:11.827921 tiffx-0.1.0/
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      747 2024-04-13 01:49:11.827921 tiffx-0.1.0/PKG-INFO
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      618 2024-04-13 01:49:06.000000 tiffx-0.1.0/README.md
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       38 2024-04-13 01:49:11.827921 tiffx-0.1.0/setup.cfg
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      971 2024-04-13 01:36:39.000000 tiffx-0.1.0/setup.py
-drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 01:49:11.827921 tiffx-0.1.0/tiffx/
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       25 2024-04-13 01:44:26.000000 tiffx-0.1.0/tiffx/__init__.py
-drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 01:49:11.827921 tiffx-0.1.0/tiffx.egg-info/
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      747 2024-04-13 01:49:11.000000 tiffx-0.1.0/tiffx.egg-info/PKG-INFO
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      180 2024-04-13 01:49:11.000000 tiffx-0.1.0/tiffx.egg-info/SOURCES.txt
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)        1 2024-04-13 01:49:11.000000 tiffx-0.1.0/tiffx.egg-info/dependency_links.txt
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       32 2024-04-13 01:49:11.000000 tiffx-0.1.0/tiffx.egg-info/requires.txt
--rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)        6 2024-04-13 01:49:11.000000 tiffx-0.1.0/tiffx.egg-info/top_level.txt
+drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 03:34:43.711809 tiffx-0.1.1/
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      773 2024-04-13 03:34:43.711809 tiffx-0.1.1/PKG-INFO
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      618 2024-04-13 03:34:38.000000 tiffx-0.1.1/README.md
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       38 2024-04-13 03:34:43.711809 tiffx-0.1.1/setup.cfg
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)     1061 2024-04-13 03:34:34.000000 tiffx-0.1.1/setup.py
+drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 03:34:43.707809 tiffx-0.1.1/tiffx/
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       25 2024-04-13 01:44:26.000000 tiffx-0.1.1/tiffx/__init__.py
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)     9354 2024-04-13 03:32:55.000000 tiffx-0.1.1/tiffx/tiffx.py
+drwxrwxr-x   0 zhihuang  (1000) zhihuang  (1000)        0 2024-04-13 03:34:43.711809 tiffx-0.1.1/tiffx.egg-info/
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      773 2024-04-13 03:34:43.000000 tiffx-0.1.1/tiffx.egg-info/PKG-INFO
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)      195 2024-04-13 03:34:43.000000 tiffx-0.1.1/tiffx.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)        1 2024-04-13 03:34:43.000000 tiffx-0.1.1/tiffx.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)       48 2024-04-13 03:34:43.000000 tiffx-0.1.1/tiffx.egg-info/requires.txt
+-rw-rw-r--   0 zhihuang  (1000) zhihuang  (1000)        6 2024-04-13 03:34:43.000000 tiffx-0.1.1/tiffx.egg-info/top_level.txt
```

### Comparing `tiffx-0.1.0/PKG-INFO` & `tiffx-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: tiffx
-Version: 0.1.0
-Summary: A package for handling complex data types with HDF5
+Version: 0.1.1
+Summary: A package for managing tiff-like whole slide image with annotation using HDF5
 Home-page: UNKNOWN
 Author: Zhi Huang
 Author-email: zhihuang.ai@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tiffx-0.1.0/README.md` & `tiffx-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tiffx-0.1.0/setup.py` & `tiffx-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tiffx',
-    version='0.1.0',
-    description='A package for handling complex data types with HDF5',
+    version='0.1.1',
+    description='A package for managing tiff-like whole slide image with annotation using HDF5',
     author='Zhi Huang',
     author_email='zhihuang.ai@gmail.com',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'Pillow',  # PIL fork for image handling
         'h5py',
         'tables'  # PyTables for pandas HDF5 support
+        'openslide-python'  # This is the package for OpenSlide
     ],
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `tiffx-0.1.0/tiffx.egg-info/PKG-INFO` & `tiffx-0.1.1/tiffx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.2
 Name: tiffx
-Version: 0.1.0
-Summary: A package for handling complex data types with HDF5
+Version: 0.1.1
+Summary: A package for managing tiff-like whole slide image with annotation using HDF5
 Home-page: UNKNOWN
 Author: Zhi Huang
 Author-email: zhihuang.ai@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

