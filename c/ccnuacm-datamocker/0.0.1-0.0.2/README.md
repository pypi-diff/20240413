# Comparing `tmp/ccnuacm_datamocker-0.0.1.tar.gz` & `tmp/ccnuacm_datamocker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccnuacm_datamocker-0.0.1.tar", last modified: Sat Apr 13 07:12:46 2024, max compression
+gzip compressed data, was "ccnuacm_datamocker-0.0.2.tar", last modified: Sat Apr 13 07:18:30 2024, max compression
```

## Comparing `ccnuacm_datamocker-0.0.1.tar` & `ccnuacm_datamocker-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:12:46.780183 ccnuacm_datamocker-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 07:12:42.000000 ccnuacm_datamocker-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-13 07:12:46.780183 ccnuacm_datamocker-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-13 07:12:42.000000 ccnuacm_datamocker-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:12:46.780183 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-13 07:12:42.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:12:46.780183 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-13 07:12:46.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-13 07:12:46.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:12:46.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 07:12:46.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 07:12:46.000000 ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:12:46.780183 ccnuacm_datamocker-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-13 07:12:42.000000 ccnuacm_datamocker-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:18:30.359870 ccnuacm_datamocker-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 07:18:26.000000 ccnuacm_datamocker-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-13 07:18:30.359870 ccnuacm_datamocker-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-13 07:18:26.000000 ccnuacm_datamocker-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:18:30.355869 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-13 07:18:26.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:18:30.355869 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-13 07:18:30.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-13 07:18:30.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:18:30.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 07:18:30.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 07:18:30.000000 ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:18:30.359870 ccnuacm_datamocker-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-13 07:18:26.000000 ccnuacm_datamocker-0.0.2/setup.py
```

### Comparing `ccnuacm_datamocker-0.0.1/LICENSE` & `ccnuacm_datamocker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccnuacm_datamocker-0.0.1/PKG-INFO` & `ccnuacm_datamocker-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccnuacm_datamocker
-Version: 0.0.1
+Version: 0.0.2
 Summary: A data mocking library for CCNU ACM
 Home-page: https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git
 Author: JixiangXiong
 Author-email: xiongjx751@qq.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 This project is a data mocker for CCNUACM. It is written in Python.
 
 ## Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
-pip3 install -e../ -U
+pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
 Here is a basic example of how to use the data mocker:
 
 ```python
```

### Comparing `ccnuacm_datamocker-0.0.1/README.md` & `ccnuacm_datamocker-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This project is a data mocker for CCNUACM. It is written in Python.
 
 ## Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
-pip3 install -e../ -U
+pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
 Here is a basic example of how to use the data mocker:
 
 ```python
```

### Comparing `ccnuacm_datamocker-0.0.1/ccnuacm_datamocker.egg-info/PKG-INFO` & `ccnuacm_datamocker-0.0.2/ccnuacm_datamocker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccnuacm_datamocker
-Version: 0.0.1
+Version: 0.0.2
 Summary: A data mocking library for CCNU ACM
 Home-page: https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git
 Author: JixiangXiong
 Author-email: xiongjx751@qq.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 This project is a data mocker for CCNUACM. It is written in Python.
 
 ## Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
-pip3 install -e../ -U
+pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
 Here is a basic example of how to use the data mocker:
 
 ```python
```

### Comparing `ccnuacm_datamocker-0.0.1/setup.py` & `ccnuacm_datamocker-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="ccnuacm_datamocker",
-    version="0.0.1",
+    version="0.0.2",
     description="A data mocking library for CCNU ACM",
     author="JixiangXiong",
     author_email="xiongjx751@qq.com",
     url="https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git",
     packages=["ccnuacm_datamocker"],
     install_requires=[
         "numpy",
```

