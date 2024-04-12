# Comparing `tmp/viirs-tools-0.0.1.tar.gz` & `tmp/viirs-tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viirs-tools-0.0.1.tar", last modified: Fri Apr 12 21:20:45 2024, max compression
+gzip compressed data, was "viirs-tools-0.1.0.tar", last modified: Fri Apr 12 22:49:47 2024, max compression
```

## Comparing `viirs-tools-0.0.1.tar` & `viirs-tools-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 21:20:45.970987 viirs-tools-0.0.1/
--rw-r--r--   0 andmin    (1000) users      (984)      246 2024-04-12 21:20:45.970987 viirs-tools-0.0.1/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:04.000000 viirs-tools-0.0.1/README.md
--rw-r--r--   0 andmin    (1000) users      (984)       38 2024-04-12 21:20:45.970987 viirs-tools-0.0.1/setup.cfg
--rw-r--r--   0 andmin    (1000) users      (984)      344 2024-04-12 19:32:26.000000 viirs-tools-0.0.1/setup.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 21:20:45.960987 viirs-tools-0.0.1/viirs_tools/
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 21:20:45.967654 viirs-tools-0.0.1/viirs_tools/Assimilator/
--rw-r--r--   0 andmin    (1000) users      (984)     4362 2024-04-12 18:39:53.000000 viirs-tools-0.0.1/viirs_tools/Assimilator/Assimilator.py
--rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-0.0.1/viirs_tools/Assimilator/Reading.py
--rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-0.0.1/viirs_tools/Assimilator/ReadingHelpers.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-0.0.1/viirs_tools/Assimilator/__init__.py
--rw-r--r--   0 andmin    (1000) users      (984)     7759 2024-04-12 21:12:54.000000 viirs-tools-0.0.1/viirs_tools/CloudMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     3683 2024-04-12 21:14:32.000000 viirs-tools-0.0.1/viirs_tools/NightMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     2672 2024-04-12 21:19:10.000000 viirs-tools-0.0.1/viirs_tools/Utils.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-0.0.1/viirs_tools/__init__.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 21:20:45.967654 viirs-tools-0.0.1/viirs_tools.egg-info/
--rw-r--r--   0 andmin    (1000) users      (984)      246 2024-04-12 21:20:45.000000 viirs-tools-0.0.1/viirs_tools.egg-info/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)      439 2024-04-12 21:20:45.000000 viirs-tools-0.0.1/viirs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 andmin    (1000) users      (984)        1 2024-04-12 21:20:45.000000 viirs-tools-0.0.1/viirs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 andmin    (1000) users      (984)       36 2024-04-12 21:20:45.000000 viirs-tools-0.0.1/viirs_tools.egg-info/requires.txt
--rw-r--r--   0 andmin    (1000) users      (984)       12 2024-04-12 21:20:45.000000 viirs-tools-0.0.1/viirs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/
+-rw-r--r--   0 andmin    (1000) users      (984)    11358 2024-04-12 22:48:16.000000 viirs-tools-0.1.0/LICENSE
+-rw-r--r--   0 andmin    (1000) users      (984)    17178 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)     3589 2024-04-12 22:29:57.000000 viirs-tools-0.1.0/README.md
+-rw-r--r--   0 andmin    (1000) users      (984)       38 2024-04-12 22:49:47.429878 viirs-tools-0.1.0/setup.cfg
+-rw-r--r--   0 andmin    (1000) users      (984)      927 2024-04-12 22:46:13.000000 viirs-tools-0.1.0/setup.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools/
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools/Assimilator/
+-rw-r--r--   0 andmin    (1000) users      (984)     4362 2024-04-12 18:39:53.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/Assimilator.py
+-rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/Reading.py
+-rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/ReadingHelpers.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-0.1.0/viirs_tools/Assimilator/__init__.py
+-rw-r--r--   0 andmin    (1000) users      (984)     7759 2024-04-12 22:02:41.000000 viirs-tools-0.1.0/viirs_tools/CloudMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     3683 2024-04-12 21:14:32.000000 viirs-tools-0.1.0/viirs_tools/NightMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     2672 2024-04-12 21:19:10.000000 viirs-tools-0.1.0/viirs_tools/Utils.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-0.1.0/viirs_tools/__init__.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-12 22:49:47.426544 viirs-tools-0.1.0/viirs_tools.egg-info/
+-rw-r--r--   0 andmin    (1000) users      (984)    17178 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)      447 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 andmin    (1000) users      (984)        1 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       30 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/requires.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       12 2024-04-12 22:49:47.000000 viirs-tools-0.1.0/viirs_tools.egg-info/top_level.txt
```

### Comparing `viirs-tools-0.0.1/viirs_tools/Assimilator/Assimilator.py` & `viirs-tools-0.1.0/viirs_tools/Assimilator/Assimilator.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.0.1/viirs_tools/Assimilator/Reading.py` & `viirs-tools-0.1.0/viirs_tools/Assimilator/Reading.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.0.1/viirs_tools/Assimilator/ReadingHelpers.py` & `viirs-tools-0.1.0/viirs_tools/Assimilator/ReadingHelpers.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.0.1/viirs_tools/CloudMask.py` & `viirs-tools-0.1.0/viirs_tools/CloudMask.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.0.1/viirs_tools/NightMask.py` & `viirs-tools-0.1.0/viirs_tools/NightMask.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.0.1/viirs_tools/Utils.py` & `viirs-tools-0.1.0/viirs_tools/Utils.py`

 * *Files identical despite different names*

