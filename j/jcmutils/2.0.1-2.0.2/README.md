# Comparing `tmp/jcmutils-2.0.1.tar.gz` & `tmp/jcmutils-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-2.0.1.tar", last modified: Sat Jan 27 10:30:30 2024, max compression
+gzip compressed data, was "jcmutils-2.0.2.tar", last modified: Sat Apr 13 04:41:35 2024, max compression
```

## Comparing `jcmutils-2.0.1.tar` & `jcmutils-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2024-01-27 10:30:30.469380 jcmutils-2.0.1/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-2.0.1/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2024-01-27 10:30:30.469380 jcmutils-2.0.1/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     4356 2024-01-27 10:30:13.000000 jcmutils-2.0.1/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2024-01-27 10:30:30.465380 jcmutils-2.0.1/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      166 2024-01-27 10:30:13.000000 jcmutils-2.0.1/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    14758 2024-01-27 10:30:13.000000 jcmutils-2.0.1/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2754 2024-01-27 10:30:13.000000 jcmutils-2.0.1/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2479 2024-01-27 10:30:13.000000 jcmutils-2.0.1/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    11066 2024-01-27 10:30:13.000000 jcmutils-2.0.1/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2024-01-27 10:30:30.469380 jcmutils-2.0.1/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2024-01-27 10:30:30.000000 jcmutils-2.0.1/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2024-01-27 10:30:30.000000 jcmutils-2.0.1/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2024-01-27 10:30:30.000000 jcmutils-2.0.1/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2024-01-27 10:30:30.000000 jcmutils-2.0.1/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2024-01-27 10:30:30.000000 jcmutils-2.0.1/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2024-01-27 10:30:30.469380 jcmutils-2.0.1/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2024-01-27 10:30:13.000000 jcmutils-2.0.1/setup.py
+drwxrwxr-x   0 mengchao  (1009) mengchao  (1010)        0 2024-04-13 04:41:35.481156 jcmutils-2.0.2/
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)     1073 2024-02-01 05:23:07.000000 jcmutils-2.0.2/LICENSE
+-rw-r--r--   0 mengchao  (1009) mengchao  (1010)      430 2024-04-13 04:41:35.481156 jcmutils-2.0.2/PKG-INFO
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)     4356 2024-02-01 05:23:07.000000 jcmutils-2.0.2/README.md
+drwxrwxr-x   0 mengchao  (1009) mengchao  (1010)        0 2024-04-13 04:41:35.477156 jcmutils-2.0.2/jcmutils/
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)      166 2024-02-01 05:23:07.000000 jcmutils-2.0.2/jcmutils/__init__.py
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)    14758 2024-02-01 05:23:07.000000 jcmutils-2.0.2/jcmutils/dataset_utils.py
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)     2754 2024-02-01 05:23:07.000000 jcmutils-2.0.2/jcmutils/gen_sources.py
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)     2479 2024-02-01 05:23:07.000000 jcmutils-2.0.2/jcmutils/logger.py
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)    11086 2024-02-01 05:27:27.000000 jcmutils-2.0.2/jcmutils/solver.py
+drwxrwxr-x   0 mengchao  (1009) mengchao  (1010)        0 2024-04-13 04:41:35.477156 jcmutils-2.0.2/jcmutils.egg-info/
+-rw-r--r--   0 mengchao  (1009) mengchao  (1010)      430 2024-04-13 04:41:35.000000 jcmutils-2.0.2/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)      294 2024-04-13 04:41:35.000000 jcmutils-2.0.2/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)        1 2024-04-13 04:41:35.000000 jcmutils-2.0.2/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)       38 2024-04-13 04:41:35.000000 jcmutils-2.0.2/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)        9 2024-04-13 04:41:35.000000 jcmutils-2.0.2/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)       38 2024-04-13 04:41:35.481156 jcmutils-2.0.2/setup.cfg
+-rw-rw-r--   0 mengchao  (1009) mengchao  (1010)      539 2024-04-13 04:40:57.000000 jcmutils-2.0.2/setup.py
```

### Comparing `jcmutils-2.0.1/LICENSE` & `jcmutils-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-2.0.1/README.md` & `jcmutils-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-2.0.1/jcmutils/dataset_utils.py` & `jcmutils-2.0.2/jcmutils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `jcmutils-2.0.1/jcmutils/gen_sources.py` & `jcmutils-2.0.2/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-2.0.1/jcmutils/logger.py` & `jcmutils-2.0.2/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-2.0.1/jcmutils/solver.py` & `jcmutils-2.0.2/jcmutils/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             (
                 temp_result[num_of_result]["field"][0].conj()
                 * temp_result[num_of_result]["field"][0]
             )
             .sum(axis=2)
             .real
         )
-        total_results = np.zeros(field.shape)
+        total_results = np.zeros((field.shape[1],field.shape[0]))
         logger.debug(f"total_result shape defined as {total_results.shape}")
 
         # 开始逐个提取结果
         for key in self.keys:
             # 目录检查
             if not os.path.exists(target_directory):
                 logger.debug("target directory dosen't exist,creating...")
```

### Comparing `jcmutils-2.0.1/setup.py` & `jcmutils-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '2.0.1'
+VERSION = '2.0.2'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

