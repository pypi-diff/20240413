# Comparing `tmp/autogluon-1.1.0b20240411.tar.gz` & `tmp/autogluon-1.1.0b20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.0b20240411.tar", last modified: Thu Apr 11 09:05:11 2024, max compression
+gzip compressed data, was "autogluon-1.1.0b20240412.tar", last modified: Fri Apr 12 09:05:48 2024, max compression
```

## Comparing `autogluon-1.1.0b20240411.tar` & `autogluon-1.1.0b20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-11 09:03:38.000000 autogluon-1.1.0b20240411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:03:38.000000 autogluon-1.1.0b20240411/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:11.906863 autogluon-1.1.0b20240411/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:11.000000 autogluon-1.1.0b20240411/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-12 09:04:11.000000 autogluon-1.1.0b20240412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:04:11.000000 autogluon-1.1.0b20240412/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:48.938234 autogluon-1.1.0b20240412/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:05:48.000000 autogluon-1.1.0b20240412/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.0b20240411/PKG-INFO` & `autogluon-1.1.0b20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240411
+Version: 1.1.0b20240412
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.0b20240411/setup.py` & `autogluon-1.1.0b20240412/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.0b20240411/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.0b20240412/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.0b20240411
+Version: 1.1.0b20240412
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```
