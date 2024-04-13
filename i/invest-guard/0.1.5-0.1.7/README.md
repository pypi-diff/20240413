# Comparing `tmp/invest-guard-0.1.5.tar.gz` & `tmp/invest-guard-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest-guard-0.1.5.tar", last modified: Sat Apr 13 19:00:19 2024, max compression
+gzip compressed data, was "invest-guard-0.1.7.tar", last modified: Sat Apr 13 20:44:39 2024, max compression
```

## Comparing `invest-guard-0.1.5.tar` & `invest-guard-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 19:00:19.114960 invest-guard-0.1.5/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 19:00:19.114612 invest-guard-0.1.5/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.5/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 19:00:19.114251 invest-guard-0.1.5/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2589 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       40 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 19:00:19.000000 invest-guard-0.1.5/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 19:00:19.115028 invest-guard-0.1.5/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1125 2024-04-13 19:00:09.000000 invest-guard-0.1.5/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 20:44:39.807002 invest-guard-0.1.7/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 20:44:39.806658 invest-guard-0.1.7/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.7/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 20:44:39.806308 invest-guard-0.1.7/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       40 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 20:44:39.807068 invest-guard-0.1.7/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1189 2024-04-13 20:43:52.000000 invest-guard-0.1.7/setup.py
```

### Comparing `invest-guard-0.1.5/PKG-INFO` & `invest-guard-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.5
+Version: 0.1.7
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
-Home-page: https://github.com/Work-With-Phoenix/invest-guard
+Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `invest-guard-0.1.5/README.md` & `invest-guard-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `invest-guard-0.1.5/invest_guard.egg-info/PKG-INFO` & `invest-guard-0.1.7/invest_guard.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.5
+Version: 0.1.7
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
-Home-page: https://github.com/Work-With-Phoenix/invest-guard
+Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `invest-guard-0.1.5/setup.py` & `invest-guard-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
+from version import VERSION
+
 
 setup(
     name='invest-guard',
-    version='0.1.5',
+    version=VERSION,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'guard = main:run_main'
+            'guard = main:main_run'
         ]
     },
     install_requires=[
         'rich',
         'tabulate',
         'yfinance',
         'pandas',
@@ -18,17 +20,16 @@
         'tqdm',
     ],
     author='Phoenix Interface',
     author_email='info@phoenixui.cloud',
     description='Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/Work-With-Phoenix/invest-guard',
+    url='https://phoenixui.cloud/invest-guard-docs',  # Update URL to point to documentation or homepage
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        
     ],
 )
```

