# Comparing `tmp/botocore-a-la-carte-apigatewaymanagementapi-1.34.83.tar.gz` & `tmp/botocore-a-la-carte-apigatewaymanagementapi-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-apigatewaymanagementapi-1.34.83.tar", last modified: Fri Apr 12 01:00:56 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-apigatewaymanagementapi-1.34.9.tar", last modified: Thu Dec 28 01:06:37 2023, max compression
```

## Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83.tar` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.356815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-12 01:00:56.356815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.352815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.352815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.352815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.356815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-12 01:00:49.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 01:00:49.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-12 01:00:49.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:00:56.356815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:00:56.356815 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 01:00:56.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.186244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2023-12-28 01:06:37.186244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.182244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.182244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.182244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.182244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2023-12-28 01:06:26.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.186244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2023-12-28 01:06:37.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-28 01:06:37.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:37.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:37.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:37.186244 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-28 01:06:36.000000 botocore-a-la-carte-apigatewaymanagementapi-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/LICENSE.txt` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/PKG-INFO` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-apigatewaymanagementapi
-Version: 1.34.83
+Version: 1.34.9
 Summary: apigatewaymanagementapi data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/endpoint-rule-set-1.json` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore/data/apigatewaymanagementapi/2018-11-29/service-2.json` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore/data/apigatewaymanagementapi/2018-11-29/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/botocore_a_la_carte_apigatewaymanagementapi.egg-info/PKG-INFO` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/botocore_a_la_carte_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-apigatewaymanagementapi
-Version: 1.34.83
+Version: 1.34.9
 Summary: apigatewaymanagementapi data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-apigatewaymanagementapi-1.34.83/setup.py` & `botocore-a-la-carte-apigatewaymanagementapi-1.34.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-apigatewaymanagementapi',
-    version="1.34.83",
+    version="1.34.9",
     description='apigatewaymanagementapi data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/apigatewaymanagementapi/*/*.json'],
```

