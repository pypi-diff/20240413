# Comparing `tmp/invest_guard-0.1.1.tar.gz` & `tmp/invest_guard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_guard-0.1.1.tar", last modified: Sat Apr 13 17:57:13 2024, max compression
+gzip compressed data, was "invest_guard-0.1.2.tar", last modified: Sat Apr 13 18:06:08 2024, max compression
```

## Comparing `invest_guard-0.1.1.tar` & `invest_guard-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 17:57:13.534930 invest_guard-0.1.1/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 17:57:13.534530 invest_guard-0.1.1/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest_guard-0.1.1/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 17:57:13.534094 invest_guard-0.1.1/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       39 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 17:57:13.000000 invest_guard-0.1.1/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 17:57:13.534993 invest_guard-0.1.1/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1124 2024-04-13 17:54:02.000000 invest_guard-0.1.1/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:06:08.345881 invest_guard-0.1.2/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:06:08.345544 invest_guard-0.1.2/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest_guard-0.1.2/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:06:08.345226 invest_guard-0.1.2/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       39 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:06:08.000000 invest_guard-0.1.2/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 18:06:08.345954 invest_guard-0.1.2/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1124 2024-04-13 18:04:46.000000 invest_guard-0.1.2/setup.py
```

### Comparing `invest_guard-0.1.1/PKG-INFO` & `invest_guard-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_guard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest_guard-0.1.1/README.md` & `invest_guard-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `invest_guard-0.1.1/invest_guard.egg-info/PKG-INFO` & `invest_guard-0.1.2/invest_guard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_guard
-Version: 0.1.1
+Version: 0.1.2
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest_guard-0.1.1/setup.py` & `invest_guard-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='invest_guard',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'guard = src.main:run'
         ]
     },
     install_requires=[
```

