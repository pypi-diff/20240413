# Comparing `tmp/invest-guard-0.1.7.tar.gz` & `tmp/invest-guard-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest-guard-0.1.7.tar", last modified: Sat Apr 13 20:44:39 2024, max compression
+gzip compressed data, was "invest-guard-0.1.8.tar", last modified: Sat Apr 13 21:01:31 2024, max compression
```

## Comparing `invest-guard-0.1.7.tar` & `invest-guard-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 20:44:39.807002 invest-guard-0.1.7/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 20:44:39.806658 invest-guard-0.1.7/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.7/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 20:44:39.806308 invest-guard-0.1.7/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       40 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 20:44:39.000000 invest-guard-0.1.7/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 20:44:39.807068 invest-guard-0.1.7/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1189 2024-04-13 20:43:52.000000 invest-guard-0.1.7/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:01:31.329910 invest-guard-0.1.8/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 21:01:31.329517 invest-guard-0.1.8/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 12:44:48.000000 invest-guard-0.1.8/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-13 21:01:31.329033 invest-guard-0.1.8/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2581 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       40 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-13 21:01:31.000000 invest-guard-0.1.8/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-13 21:01:31.329980 invest-guard-0.1.8/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1189 2024-04-13 21:01:23.000000 invest-guard-0.1.8/setup.py
```

### Comparing `invest-guard-0.1.7/PKG-INFO` & `invest-guard-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.7
+Version: 0.1.8
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest-guard-0.1.7/README.md` & `invest-guard-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `invest-guard-0.1.7/invest_guard.egg-info/PKG-INFO` & `invest-guard-0.1.8/invest_guard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest-guard
-Version: 0.1.7
+Version: 0.1.8
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://phoenixui.cloud/invest-guard-docs
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest-guard-0.1.7/setup.py` & `invest-guard-0.1.8/setup.py`

 * *Files identical despite different names*

