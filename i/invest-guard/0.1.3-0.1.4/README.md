# Comparing `tmp/invest-guard-0.1.3.tar.gz` & `tmp/invest-guard-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest-guard-0.1.3.tar", last modified: Sat Apr 13 18:22:37 2024, max compression
+gzip compressed data, was "invest-guard-0.1.4.tar", last modified: Sat Apr 13 18:47:50 2024, max compression
```

## Comparing `invest-guard-0.1.3.tar` & `invest-guard-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:22:37.153228 invest-guard-0.1.3/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:22:37.152906 invest-guard-0.1.3/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.3/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:22:37.152570 invest-guard-0.1.3/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       39 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:22:37.000000 invest-guard-0.1.3/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 18:22:37.153293 invest-guard-0.1.3/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1124 2024-04-13 18:22:14.000000 invest-guard-0.1.3/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:47:50.992059 invest-guard-0.1.4/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:47:50.991742 invest-guard-0.1.4/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.4/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 18:47:50.991375 invest-guard-0.1.4/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       44 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 18:47:50.000000 invest-guard-0.1.4/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 18:47:50.992125 invest-guard-0.1.4/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1129 2024-04-13 18:47:41.000000 invest-guard-0.1.4/setup.py
```

### Comparing `invest-guard-0.1.3/PKG-INFO` & `invest-guard-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest-guard-0.1.3/README.md` & `invest-guard-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `invest-guard-0.1.3/invest_guard.egg-info/PKG-INFO` & `invest-guard-0.1.4/invest_guard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest-guard-0.1.3/setup.py` & `invest-guard-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='invest-guard',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'guard = src.main:run'
+            'guard = src.main:run_main'
         ]
     },
     install_requires=[
         'rich',
         'tabulate',
         'yfinance',
         'pandas',
```
