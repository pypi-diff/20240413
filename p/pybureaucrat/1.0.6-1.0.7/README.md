# Comparing `tmp/pybureaucrat-1.0.6.tar.gz` & `tmp/pybureaucrat-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybureaucrat-1.0.6.tar", last modified: Wed Apr 10 15:29:35 2024, max compression
+gzip compressed data, was "pybureaucrat-1.0.7.tar", last modified: Sat Apr 13 04:38:59 2024, max compression
```

## Comparing `pybureaucrat-1.0.6.tar` & `pybureaucrat-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:29:35.173965 pybureaucrat-1.0.6/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.6/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.6/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-10 15:29:35.173965 pybureaucrat-1.0.6/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.6/README.MD
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:29:35.161965 pybureaucrat-1.0.6/client/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:29:35.169965 pybureaucrat-1.0.6/client/pybureaucrat/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/base.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/blobs.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      351 2024-04-10 15:28:20.000000 pybureaucrat-1.0.6/client/pybureaucrat/bureaucrat_connection.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/deserializers.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/queues.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/client/pybureaucrat/tables.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:29:35.173965 pybureaucrat-1.0.6/client/pybureaucrat.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-10 15:29:35.000000 pybureaucrat-1.0.6/client/pybureaucrat.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      468 2024-04-10 15:29:35.000000 pybureaucrat-1.0.6/client/pybureaucrat.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-10 15:29:35.000000 pybureaucrat-1.0.6/client/pybureaucrat.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2024-04-10 15:29:35.000000 pybureaucrat-1.0.6/client/pybureaucrat.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.6/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-10 15:29:35.173965 pybureaucrat-1.0.6/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1163 2024-04-10 15:11:05.000000 pybureaucrat-1.0.6/setup.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-10 15:28:20.000000 pybureaucrat-1.0.6/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 04:38:59.757109 pybureaucrat-1.0.7/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2024-04-06 03:57:44.000000 pybureaucrat-1.0.7/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2024-04-06 03:57:44.000000 pybureaucrat-1.0.7/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-13 04:38:59.757109 pybureaucrat-1.0.7/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-06 03:57:44.000000 pybureaucrat-1.0.7/README.MD
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 04:38:59.745109 pybureaucrat-1.0.7/client/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 04:38:59.753109 pybureaucrat-1.0.7/client/pybureaucrat/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2634 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/base.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1244 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/blobs.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      351 2024-04-10 15:28:20.000000 pybureaucrat-1.0.7/client/pybureaucrat/bureaucrat_connection.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      186 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/deserializers.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      813 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/queues.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1795 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/client/pybureaucrat/tables.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2024-04-13 04:38:14.000000 pybureaucrat-1.0.7/client/pybureaucrat/trees.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2024-04-13 04:38:59.757109 pybureaucrat-1.0.7/client/pybureaucrat.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      787 2024-04-13 04:38:59.000000 pybureaucrat-1.0.7/client/pybureaucrat.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      497 2024-04-13 04:38:59.000000 pybureaucrat-1.0.7/client/pybureaucrat.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2024-04-13 04:38:59.000000 pybureaucrat-1.0.7/client/pybureaucrat.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       13 2024-04-13 04:38:59.000000 pybureaucrat-1.0.7/client/pybureaucrat.egg-info/top_level.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2024-04-06 03:57:44.000000 pybureaucrat-1.0.7/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2024-04-13 04:38:59.757109 pybureaucrat-1.0.7/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1163 2024-04-10 15:11:05.000000 pybureaucrat-1.0.7/setup.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2024-04-13 04:38:14.000000 pybureaucrat-1.0.7/version.txt
```

### Comparing `pybureaucrat-1.0.6/LICENSE` & `pybureaucrat-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.6/PKG-INFO` & `pybureaucrat-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.6/client/pybureaucrat/base.py` & `pybureaucrat-1.0.7/client/pybureaucrat/base.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.6/client/pybureaucrat/blobs.py` & `pybureaucrat-1.0.7/client/pybureaucrat/blobs.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.6/client/pybureaucrat/queues.py` & `pybureaucrat-1.0.7/client/pybureaucrat/queues.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.6/client/pybureaucrat/tables.py` & `pybureaucrat-1.0.7/client/pybureaucrat/tables.py`

 * *Files identical despite different names*

### Comparing `pybureaucrat-1.0.6/client/pybureaucrat.egg-info/PKG-INFO` & `pybureaucrat-1.0.7/client/pybureaucrat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybureaucrat
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python client for bureaucrat server
 Home-page: https://github.com/LostSavannah/bureaucrat/tree/main/lib
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/pybureaucrat/issues
 Project-URL: Documentation, https://dev.moradev.dev/pybureaucrat/documentation
 Project-URL: Examples, https://dev.moradev.dev/pybureaucrat/examples
```

### Comparing `pybureaucrat-1.0.6/setup.py` & `pybureaucrat-1.0.7/setup.py`

 * *Files identical despite different names*

