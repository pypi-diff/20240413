# Comparing `tmp/sling-1.2.3.post2.tar.gz` & `tmp/sling-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sling-1.2.3.post2.tar", last modified: Thu Apr 11 14:16:16 2024, max compression
+gzip compressed data, was "sling-1.2.4.tar", last modified: Sat Apr 13 14:16:53 2024, max compression
```

## Comparing `sling-1.2.3.post2.tar` & `sling-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:16:16.623723 sling-1.2.3.post2/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 14:11:53.000000 sling-1.2.3.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-11 14:16:16.623723 sling-1.2.3.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-11 14:16:13.000000 sling-1.2.3.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 14:16:13.000000 sling-1.2.3.post2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:16:16.623723 sling-1.2.3.post2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2235 2024-04-11 14:11:53.000000 sling-1.2.3.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:16:16.623723 sling-1.2.3.post2/sling/
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-11 14:11:53.000000 sling-1.2.3.post2/sling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:16:16.623723 sling-1.2.3.post2/sling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 14:16:16.000000 sling-1.2.3.post2/sling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:16:53.733955 sling-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-13 14:13:20.000000 sling-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-13 14:16:53.733955 sling-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-13 14:16:50.000000 sling-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 14:16:50.000000 sling-1.2.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:16:53.733955 sling-1.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2235 2024-04-13 14:13:20.000000 sling-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:16:53.729955 sling-1.2.4/sling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-13 14:13:20.000000 sling-1.2.4/sling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:16:53.733955 sling-1.2.4/sling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 14:16:53.000000 sling-1.2.4/sling.egg-info/top_level.txt
```

### Comparing `sling-1.2.3.post2/PKG-INFO` & `sling-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.3.post2
+Version: 1.2.4
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

### Comparing `sling-1.2.3.post2/README.md` & `sling-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sling-1.2.3.post2/setup.py` & `sling-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `sling-1.2.3.post2/sling/__init__.py` & `sling-1.2.4/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `sling-1.2.3.post2/sling.egg-info/PKG-INFO` & `sling-1.2.4/sling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.3.post2
+Version: 1.2.4
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

