# Comparing `tmp/diskinfo-3.1.1.tar.gz` & `tmp/diskinfo-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diskinfo-3.1.1.tar", last modified: Sat Apr  6 18:59:08 2024, max compression
+gzip compressed data, was "diskinfo-3.1.2.tar", last modified: Sat Apr 13 08:43:29 2024, max compression
```

## Comparing `diskinfo-3.1.1.tar` & `diskinfo-3.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.973962 diskinfo-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 18:59:02.000000 diskinfo-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-06 18:59:08.973962 diskinfo-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-06 18:59:02.000000 diskinfo-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-06 18:59:02.000000 diskinfo-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:59:08.973962 diskinfo-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.965962 diskinfo-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.969962 diskinfo-3.1.1/src/diskinfo/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    32708 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/diskinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disksmart.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/disktype.py
--rw-r--r--   0 runner    (1001) docker     (127)    29623 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-06 18:59:02.000000 diskinfo-3.1.1/src/diskinfo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.973962 diskinfo-3.1.1/src/diskinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 18:59:08.000000 diskinfo-3.1.1/src/diskinfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:59:08.969962 diskinfo-3.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_data_smart.py
--rw-r--r--   0 runner    (1001) docker     (127)    37869 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_diskinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_disksmart.py
--rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-06 18:59:02.000000 diskinfo-3.1.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:29.506069 diskinfo-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-13 08:43:26.000000 diskinfo-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-13 08:43:29.506069 diskinfo-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-13 08:43:26.000000 diskinfo-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-13 08:43:26.000000 diskinfo-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 08:43:29.506069 diskinfo-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:29.502069 diskinfo-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:29.506069 diskinfo-3.1.2/src/diskinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32708 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/diskinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/disksmart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/disktype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29623 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9108 2024-04-13 08:43:26.000000 diskinfo-3.1.2/src/diskinfo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:29.506069 diskinfo-3.1.2/src/diskinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-13 08:43:29.000000 diskinfo-3.1.2/src/diskinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 08:43:29.000000 diskinfo-3.1.2/src/diskinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:43:29.000000 diskinfo-3.1.2/src/diskinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 08:43:29.000000 diskinfo-3.1.2/src/diskinfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 08:43:29.000000 diskinfo-3.1.2/src/diskinfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:29.506069 diskinfo-3.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_data_smart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37869 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23188 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_diskinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_disksmart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-13 08:43:26.000000 diskinfo-3.1.2/test/test_utils.py
```

### Comparing `diskinfo-3.1.1/LICENSE` & `diskinfo-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/PKG-INFO` & `diskinfo-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskinfo
-Version: 3.1.1
+Version: 3.1.2
 Summary: Disk information Python library for Linux
 Author-email: Peter Sulyok <peter@sulyok.net>
 License: MIT License
         
         Copyright (c) 2022 Peter Sulyok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `diskinfo-3.1.1/README.md` & `diskinfo-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/pyproject.toml` & `diskinfo-3.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diskinfo"
 description = "Disk information Python library for Linux"
 readme = "README.md"
-version = "3.1.1"
+version = "3.1.2"
 authors = [
     { name = "Peter Sulyok", email = "peter@sulyok.net" }
 ]
 requires-python = ">=3.8"
 keywords = ["disk", "linux"]
 license = {file = "LICENSE"}
 dependencies = [
```

### Comparing `diskinfo-3.1.1/src/diskinfo/__init__.py` & `diskinfo-3.1.2/src/diskinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/demo.py` & `diskinfo-3.1.2/src/diskinfo/demo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/disk.py` & `diskinfo-3.1.2/src/diskinfo/disk.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/diskinfo.py` & `diskinfo-3.1.2/src/diskinfo/diskinfo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/disksmart.py` & `diskinfo-3.1.2/src/diskinfo/disksmart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/disktype.py` & `diskinfo-3.1.2/src/diskinfo/disktype.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/partition.py` & `diskinfo-3.1.2/src/diskinfo/partition.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo/utils.py` & `diskinfo-3.1.2/src/diskinfo/utils.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/src/diskinfo.egg-info/PKG-INFO` & `diskinfo-3.1.2/src/diskinfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diskinfo
-Version: 3.1.1
+Version: 3.1.2
 Summary: Disk information Python library for Linux
 Author-email: Peter Sulyok <peter@sulyok.net>
 License: MIT License
         
         Copyright (c) 2022 Peter Sulyok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `diskinfo-3.1.1/src/diskinfo.egg-info/SOURCES.txt` & `diskinfo-3.1.2/src/diskinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_data.py` & `diskinfo-3.1.2/test/test_data.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_data_smart.py` & `diskinfo-3.1.2/test/test_data_smart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_disk.py` & `diskinfo-3.1.2/test/test_disk.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_diskinfo.py` & `diskinfo-3.1.2/test/test_diskinfo.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_disksmart.py` & `diskinfo-3.1.2/test/test_disksmart.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_partition.py` & `diskinfo-3.1.2/test/test_partition.py`

 * *Files identical despite different names*

### Comparing `diskinfo-3.1.1/test/test_utils.py` & `diskinfo-3.1.2/test/test_utils.py`

 * *Files identical despite different names*

