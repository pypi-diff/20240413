# Comparing `tmp/botocore-a-la-carte-importexport-1.34.83.tar.gz` & `tmp/botocore-a-la-carte-importexport-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-importexport-1.34.83.tar", last modified: Fri Apr 12 01:01:08 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-importexport-1.34.9.tar", last modified: Thu Dec 28 01:06:46 2023, max compression
```

## Comparing `botocore-a-la-carte-importexport-1.34.83.tar` & `botocore-a-la-carte-importexport-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/
--rw-r--r--   0 runner    (1001) docker     (127)    27094 2024-04-12 01:00:49.000000 botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 01:00:49.000000 botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    33582 2024-04-12 01:00:49.000000 botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:01:08.004906 botocore-a-la-carte-importexport-1.34.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 01:01:07.000000 botocore-a-la-carte-importexport-1.34.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.570316 botocore-a-la-carte-importexport-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 01:06:46.570316 botocore-a-la-carte-importexport-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.566316 botocore-a-la-carte-importexport-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.566316 botocore-a-la-carte-importexport-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.566316 botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.566316 botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/
+-rw-r--r--   0 runner    (1001) docker     (127)    27094 2023-12-28 01:06:26.000000 botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-28 01:06:26.000000 botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33582 2023-12-28 01:06:26.000000 botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:46.570316 botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:46.570316 botocore-a-la-carte-importexport-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-28 01:06:46.000000 botocore-a-la-carte-importexport-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-importexport-1.34.83/LICENSE.txt` & `botocore-a-la-carte-importexport-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-importexport-1.34.83/PKG-INFO` & `botocore-a-la-carte-importexport-1.34.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-importexport
-Version: 1.34.83
+Version: 1.34.9
 Summary: importexport data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-importexport-1.34.83/botocore/data/importexport/2010-06-01/service-2.json` & `botocore-a-la-carte-importexport-1.34.9/botocore/data/importexport/2010-06-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-importexport-1.34.83/botocore_a_la_carte_importexport.egg-info/PKG-INFO` & `botocore-a-la-carte-importexport-1.34.9/botocore_a_la_carte_importexport.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-importexport
-Version: 1.34.83
+Version: 1.34.9
 Summary: importexport data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-importexport-1.34.83/setup.py` & `botocore-a-la-carte-importexport-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-importexport',
-    version="1.34.83",
+    version="1.34.9",
     description='importexport data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/importexport/*/*.json'],
```

