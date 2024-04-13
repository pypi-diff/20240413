# Comparing `tmp/cryptopian_infra-0.1.2.tar.gz` & `tmp/cryptopian_infra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptopian_infra-0.1.2.tar", last modified: Wed Apr  3 04:37:30 2024, max compression
+gzip compressed data, was "cryptopian_infra-0.1.3.tar", last modified: Sat Apr 13 08:10:43 2024, max compression
```

## Comparing `cryptopian_infra-0.1.2.tar` & `cryptopian_infra-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.183656 cryptopian_infra-0.1.2/
--rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.2/LICENSE
--rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-04-03 04:37:30.183373 cryptopian_infra-0.1.2/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.2/README.md
--rw-r--r--   0 wuhan      (501) staff       (20)      690 2024-04-03 04:37:04.000000 cryptopian_infra-0.1.2/pyproject.toml
--rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-04-03 04:37:30.183852 cryptopian_infra-0.1.2/setup.cfg
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.172361 cryptopian_infra-0.1.2/src/
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.173713 cryptopian_infra-0.1.2/src/cryptopian_infra/
--rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/__init__.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.176145 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/
--rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alert.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alertwrapper.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/alert/slackwebhook.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.178256 cryptopian_infra-0.1.2/src/cryptopian_infra/config/
--rw-r--r--   0 wuhan      (501) staff       (20)      278 2024-03-12 15:01:14.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-03-05 08:29:11.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/apimanager.py
--rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/configloader.py
--rw-r--r--   0 wuhan      (501) staff       (20)      902 2022-05-08 03:39:06.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/docencryptionfactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/influxfactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2341 2024-01-28 08:42:04.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/mongofactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2799 2024-03-31 15:39:56.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/secretmanagerbase.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1878 2024-03-31 08:39:28.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/config/slackwebhookfactory.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.179263 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/
--rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/duration.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/emailclient.py
--rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/gracefullystopdocker.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/infra/stopwatch.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.179773 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/
--rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/mongoparameters.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/sendalert.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.180658 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/
--rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/atomicaccstore.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/threading/messagepump.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.182297 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/
--rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/asyncutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/datetimeutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1017 2024-04-03 04:36:40.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/dictutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/listutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1496 2024-03-05 04:22:42.000000 cryptopian_infra-0.1.2/src/cryptopian_infra/utils/mathutils.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.183061 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/
--rw-r--r--   0 wuhan      (501) staff       (20)     1187 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)     1545 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/SOURCES.txt
--rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/dependency_links.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       75 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/requires.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-04-03 04:37:30.000000 cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/top_level.txt
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-03 04:37:30.182617 cryptopian_infra-0.1.2/tests/
--rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.2/tests/test_random.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.654268 cryptopian_infra-0.1.3/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.3/LICENSE
+-rw-r--r--   0 wuhan      (501) staff       (20)     1218 2024-04-13 08:10:43.654060 cryptopian_infra-0.1.3/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.3/README.md
+-rw-r--r--   0 wuhan      (501) staff       (20)      713 2024-04-13 07:28:44.000000 cryptopian_infra-0.1.3/pyproject.toml
+-rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-04-13 08:10:43.654310 cryptopian_infra-0.1.3/setup.cfg
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.643385 cryptopian_infra-0.1.3/src/
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.645042 cryptopian_infra-0.1.3/src/cryptopian_infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/__init__.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.647171 cryptopian_infra-0.1.3/src/cryptopian_infra/alert/
+-rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/alert/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/alert/alert.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/alert/alertwrapper.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/alert/slackwebhook.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.649403 cryptopian_infra-0.1.3/src/cryptopian_infra/config/
+-rw-r--r--   0 wuhan      (501) staff       (20)      364 2024-04-12 11:47:42.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-04-12 14:51:39.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/apimanager.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/configloader.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     4116 2024-04-13 08:08:20.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/influxdb2factory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/influxfactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2297 2024-04-13 04:28:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/mongofactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2725 2024-04-12 14:50:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/secretmanagerbase.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2133 2024-04-12 15:09:21.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/config/slackwebhookfactory.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.650647 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/duration.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/emailclient.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/gracefullystopdocker.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/infra/stopwatch.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.650934 cryptopian_infra-0.1.3/src/cryptopian_infra/mongo/
+-rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/mongo/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/mongo/mongoparameters.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/sendalert.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.651646 cryptopian_infra-0.1.3/src/cryptopian_infra/threading/
+-rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/threading/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/threading/atomicaccstore.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/threading/messagepump.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.653370 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/
+-rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/asyncutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/datetimeutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      124 2024-04-12 15:38:53.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/dictobj.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1017 2024-04-03 04:36:40.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/dictutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/listutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1496 2024-03-05 04:22:42.000000 cryptopian_infra-0.1.3/src/cryptopian_infra/utils/mathutils.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.653815 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1218 2024-04-13 08:10:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)     1579 2024-04-13 08:10:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/SOURCES.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-04-13 08:10:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/dependency_links.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       91 2024-04-13 08:10:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/requires.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-04-13 08:10:43.000000 cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/top_level.txt
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-13 08:10:43.653528 cryptopian_infra-0.1.3/tests/
+-rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.3/tests/test_random.py
```

### Comparing `cryptopian_infra-0.1.2/LICENSE` & `cryptopian_infra-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/PKG-INFO` & `cryptopian_infra-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb
+Requires-Dist: influxdb-client
 Requires-Dist: jsmin
 Requires-Dist: onepasswordconnectsdk
 Requires-Dist: pandas
 Requires-Dist: pymongo
 Requires-Dist: python-dotenv
 Requires-Dist: requests
```

### Comparing `cryptopian_infra-0.1.2/pyproject.toml` & `cryptopian_infra-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [project]
 name = "cryptopian_infra"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name = "Han Wu", email = "xjohnwu@gmail.com" },
 ]
 dependencies = [
     "influxdb",
+    "influxdb-client",
     "jsmin",
     "onepasswordconnectsdk",
     "pandas",
     "pymongo",
     "python-dotenv",
     "requests",
 ]
```

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alert.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/alert/alert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/alertwrapper.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/alert/alertwrapper.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/alert/slackwebhook.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/alert/slackwebhook.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/apimanager.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/apimanager.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/configloader.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/configloader.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/influxfactory.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/influxfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/mongofactory.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/mongofactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,14 @@
         self.privilege = MongoPrivilege[kwargs['database permission']]
 
     def metadata(self):
         md = dict(self.__dict__)
         del md['password']
         return md
 
-    def __repr__(self):
-        return repr(self.__dict__)
-
-    def __str__(self):
-        return repr(self)
-
 
 class MongoFactory(SecretManagerBase[MongoSecretItem]):
     def __init__(self):
         super().__init__()
 
     def tag_filter(self):
         return 'DB/Mongo'
@@ -56,16 +50,18 @@
         for item in items:
             if item.privilege.value >= privilege.value:
                 return item
 
     def create_mongo_db(self, database, privilege: MongoPrivilege = MongoPrivilege.read):
         item = self.find_item(database, privilege)
         if item:
-            client = MongoClient(host=item.server, port=item.port,
-                                 username=item.username, password=item.password)
+            client = MongoClient(host=item.server,
+                                 port=item.port,
+                                 username=item.username,
+                                 password=item.password)
             return client[item.database]
         else:
             raise KeyError(f'Unable to find database={database}')
 
     def create_mongo_parameters(self, database, collection_name, privilege: MongoPrivilege = MongoPrivilege.readWrite):
         mongo_db = self.create_mongo_db(database=database, privilege=privilege)
         return MongoParameters(mongo_db, collection_name)
```

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/secretmanagerbase.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/secretmanagerbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 
     def __repr__(self):
         return repr(self.metadata())
 
     def __str__(self):
         return repr(self)
 
+    def match_filter(self, **kwargs):
+        metadata = self.metadata()
+        for key, value in kwargs.items():
+            if key not in metadata or not value == metadata[key]:
+                return False
+        return True
+
 
 S = TypeVar('S', bound=SecretMetadata)
 
 
 class SecretItem(SecretMetadata):
     def __init__(self, metadata: dict):
         self._metadata = metadata
@@ -51,33 +58,26 @@
         vaults = self.client.get_vaults()
         for vault in vaults:
             vault_items = self.client.get_items(vault.id)
             for vault_item in vault_items:
                 item = self.client.get_item(vault_item.id, vault.id)
                 if item.tags is not None and self.tag_filter() in item.tags:
                     secret_item = self.process_item(item)
-                    if secret_item is not None and self.match_filter(secret_item.metadata(), **metadata_filter):
+                    if secret_item is not None and secret_item.match_filter(**metadata_filter):
                         results.append(secret_item)
                         if find_one:
                             return results
         return results
 
     def find_one(self, **metadata_filter):
         results = self.__find(True, **metadata_filter)
         if len(results) > 0:
             return results[0]
 
     @staticmethod
-    def match_filter(metadata: dict, **kwargs):
-        for key, value in kwargs.items():
-            if key not in metadata or not (value == metadata[key] or isinstance(metadata[key], list) and value in metadata[key]):
-                return False
-        return True
-
-    @staticmethod
     def get_section_lookup(item: Item) -> dict:
         section_lookup = {}
         if item.sections:
             for section in item.sections:
                 if section.label is not None:
                     section_lookup[section.id] = section.label
         return section_lookup
```

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/config/slackwebhookfactory.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/config/slackwebhookfactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,38 @@
     def __init__(self, metadata: dict, channel_url_lookup: dict):
         super().__init__(metadata)
         self.channel_url_lookup = channel_url_lookup
 
     def get_webhook_config(self, channel: str):
         return {'channel': channel, 'url': self.channel_url_lookup[channel]}
 
+    def match_filter(self, **kwargs):
+        metadata = self.metadata()
+        for key, value in kwargs.items():
+            if key == 'channel':
+                if value not in self.channel_url_lookup:
+                    return False
+            elif key not in metadata or not value == metadata[key]:
+                return False
+        return True
+
 
 class SlackWebhookFactory(SecretManagerBase[SlackWebhookItem]):
 
     def __init__(self):
         super().__init__()
 
     def tag_filter(self):
         return 'Slack/Webhook'
 
     def process_item(self, item: Item):
         section_lookup = SecretManagerBase.get_section_lookup(item)
 
         webhook_configs = {}
-        metadata = {
-            'channel': []
-        }
+        metadata = {}
         for field in item.fields:
             if field.id == 'username':
                 metadata['username'] = field.value
             elif field.section is not None:
                 section_id = field.section.id
                 if section_id in section_lookup:
                     section_label = section_lookup[section_id]
@@ -39,14 +47,13 @@
                         if section_id not in webhook_configs:
                             webhook_configs[section_id] = {}
                         webhook_configs[section_id][field.label] = field.value
 
         channel_url_lookup = {}
         for webhook_config in webhook_configs.values():
             channel_url_lookup[webhook_config['channel']] = webhook_config['url']
-            metadata['channel'].append(webhook_config['channel'])
 
         return SlackWebhookItem(metadata, channel_url_lookup)
 
     def create_webhook(self, channel: str):
         item = self.find_one(channel=channel)
         return SlackWebhook(**item.get_webhook_config(channel))
```

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/duration.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/infra/duration.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/emailclient.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/infra/emailclient.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/infra/stopwatch.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/infra/stopwatch.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/mongo/mongoparameters.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/mongo/mongoparameters.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/sendalert.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/sendalert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/threading/messagepump.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/threading/messagepump.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/datetimeutils.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/dictutils.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra/utils/mathutils.py` & `cryptopian_infra-0.1.3/src/cryptopian_infra/utils/mathutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/PKG-INFO` & `cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb
+Requires-Dist: influxdb-client
 Requires-Dist: jsmin
 Requires-Dist: onepasswordconnectsdk
 Requires-Dist: pandas
 Requires-Dist: pymongo
 Requires-Dist: python-dotenv
 Requires-Dist: requests
```

### Comparing `cryptopian_infra-0.1.2/src/cryptopian_infra.egg-info/SOURCES.txt` & `cryptopian_infra-0.1.3/src/cryptopian_infra.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 src/cryptopian_infra/alert/__init__.py
 src/cryptopian_infra/alert/alert.py
 src/cryptopian_infra/alert/alertwrapper.py
 src/cryptopian_infra/alert/slackwebhook.py
 src/cryptopian_infra/config/__init__.py
 src/cryptopian_infra/config/apimanager.py
 src/cryptopian_infra/config/configloader.py
-src/cryptopian_infra/config/docencryptionfactory.py
+src/cryptopian_infra/config/influxdb2factory.py
 src/cryptopian_infra/config/influxfactory.py
 src/cryptopian_infra/config/mongofactory.py
 src/cryptopian_infra/config/secretmanagerbase.py
 src/cryptopian_infra/config/slackwebhookfactory.py
 src/cryptopian_infra/infra/__init__.py
 src/cryptopian_infra/infra/duration.py
 src/cryptopian_infra/infra/emailclient.py
@@ -29,11 +29,12 @@
 src/cryptopian_infra/mongo/mongoparameters.py
 src/cryptopian_infra/threading/__init__.py
 src/cryptopian_infra/threading/atomicaccstore.py
 src/cryptopian_infra/threading/messagepump.py
 src/cryptopian_infra/utils/__init__.py
 src/cryptopian_infra/utils/asyncutils.py
 src/cryptopian_infra/utils/datetimeutils.py
+src/cryptopian_infra/utils/dictobj.py
 src/cryptopian_infra/utils/dictutils.py
 src/cryptopian_infra/utils/listutils.py
 src/cryptopian_infra/utils/mathutils.py
 tests/test_random.py
```

### Comparing `cryptopian_infra-0.1.2/tests/test_random.py` & `cryptopian_infra-0.1.3/tests/test_random.py`

 * *Files identical despite different names*

