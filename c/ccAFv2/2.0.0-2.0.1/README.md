# Comparing `tmp/ccAFv2-2.0.0.tar.gz` & `tmp/ccAFv2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccAFv2-2.0.0.tar", last modified: Fri Apr 12 23:59:01 2024, max compression
+gzip compressed data, was "ccAFv2-2.0.1.tar", last modified: Sat Apr 13 15:56:35 2024, max compression
```

## Comparing `ccAFv2-2.0.0.tar` & `ccAFv2-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:59:01.114447 ccAFv2-2.0.0/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-04-12 14:01:10.000000 ccAFv2-2.0.0/.gitattributes
--rw-rw-r--   0 root         (0) root         (0)     2774 2024-04-12 14:01:10.000000 ccAFv2-2.0.0/.gitignore
--rw-rw-r--   0 root         (0) root         (0)    35129 2024-04-12 14:12:19.000000 ccAFv2-2.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      115 2024-04-12 18:23:46.000000 ccAFv2-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5129 2024-04-12 23:59:01.114447 ccAFv2-2.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3941 2024-04-12 14:01:10.000000 ccAFv2-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:59:01.094447 ccAFv2-2.0.0/ccAFv2/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-04-12 14:12:05.000000 ccAFv2-2.0.0/ccAFv2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5965 2024-04-12 16:56:32.000000 ccAFv2-2.0.0/ccAFv2/ccAFv2.py
--rw-rw-r--   0 root         (0) root         (0)       43 2024-04-12 14:12:06.000000 ccAFv2-2.0.0/ccAFv2/ccAFv2_classes.txt
--rw-rw-r--   0 root         (0) root         (0)    56847 2024-04-12 14:12:07.000000 ccAFv2-2.0.0/ccAFv2/ccAFv2_genes.csv
--rw-rw-r--   0 root         (0) root         (0)  5548392 2024-04-12 14:12:07.000000 ccAFv2-2.0.0/ccAFv2/ccAFv2_model.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:59:01.114447 ccAFv2-2.0.0/ccAFv2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5129 2024-04-12 23:59:00.000000 ccAFv2-2.0.0/ccAFv2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2024-04-12 23:59:01.000000 ccAFv2-2.0.0/ccAFv2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 23:59:00.000000 ccAFv2-2.0.0/ccAFv2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-12 23:59:00.000000 ccAFv2-2.0.0/ccAFv2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-12 23:59:00.000000 ccAFv2-2.0.0/ccAFv2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 23:59:01.114447 ccAFv2-2.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2219 2024-04-12 18:23:36.000000 ccAFv2-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 23:59:01.114447 ccAFv2-2.0.0/tests/
--rw-rw-r--   0 root         (0) root         (0)     1598 2024-04-12 17:11:05.000000 ccAFv2-2.0.0/tests/predict_samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:56:35.772726 ccAFv2-2.0.1/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-04-12 14:01:10.000000 ccAFv2-2.0.1/.gitattributes
+-rw-rw-r--   0 root         (0) root         (0)     2774 2024-04-12 14:01:10.000000 ccAFv2-2.0.1/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)    35129 2024-04-12 14:12:19.000000 ccAFv2-2.0.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      115 2024-04-12 18:23:46.000000 ccAFv2-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12813 2024-04-13 15:56:35.772726 ccAFv2-2.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    10545 2024-04-13 15:53:05.000000 ccAFv2-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:56:35.760726 ccAFv2-2.0.1/ccAFv2/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-04-12 14:12:05.000000 ccAFv2-2.0.1/ccAFv2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5965 2024-04-13 00:00:17.000000 ccAFv2-2.0.1/ccAFv2/ccAFv2.py
+-rw-rw-r--   0 root         (0) root         (0)       43 2024-04-12 14:12:06.000000 ccAFv2-2.0.1/ccAFv2/ccAFv2_classes.txt
+-rw-rw-r--   0 root         (0) root         (0)    56847 2024-04-12 14:12:07.000000 ccAFv2-2.0.1/ccAFv2/ccAFv2_genes.csv
+-rw-rw-r--   0 root         (0) root         (0)  5548392 2024-04-12 14:12:07.000000 ccAFv2-2.0.1/ccAFv2/ccAFv2_model.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:56:35.772726 ccAFv2-2.0.1/ccAFv2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12813 2024-04-13 15:56:35.000000 ccAFv2-2.0.1/ccAFv2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-13 15:56:35.000000 ccAFv2-2.0.1/ccAFv2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 15:56:35.000000 ccAFv2-2.0.1/ccAFv2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-13 15:56:35.000000 ccAFv2-2.0.1/ccAFv2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-13 15:56:35.000000 ccAFv2-2.0.1/ccAFv2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 15:56:35.772726 ccAFv2-2.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2219 2024-04-13 15:56:01.000000 ccAFv2-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:56:35.772726 ccAFv2-2.0.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)     1598 2024-04-12 17:11:05.000000 ccAFv2-2.0.1/tests/predict_samples.py
```

### Comparing `ccAFv2-2.0.0/.gitignore` & `ccAFv2-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ccAFv2-2.0.0/LICENSE` & `ccAFv2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccAFv2-2.0.0/ccAFv2/ccAFv2.py` & `ccAFv2-2.0.1/ccAFv2/ccAFv2.py`

 * *Files identical despite different names*

### Comparing `ccAFv2-2.0.0/ccAFv2/ccAFv2_genes.csv` & `ccAFv2-2.0.1/ccAFv2/ccAFv2_genes.csv`

 * *Files identical despite different names*

### Comparing `ccAFv2-2.0.0/ccAFv2/ccAFv2_model.h5` & `ccAFv2-2.0.1/ccAFv2/ccAFv2_model.h5`

 * *Files identical despite different names*

### Comparing `ccAFv2-2.0.0/setup.py` & `ccAFv2-2.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # The text of the README file
 long_description = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="ccAFv2",
-    version="2.0.0",
+    version="2.0.1",
     description="Classify scRNA-seq profiling with highly resolved cell cycle phases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/plaisier-lab/ccAFv2_py",
     author="Christopher Plaisier",
     author_email="plaisier@asu.edu",
     license="GNU General Public License v3.0",
```

### Comparing `ccAFv2-2.0.0/tests/predict_samples.py` & `ccAFv2-2.0.1/tests/predict_samples.py`

 * *Files identical despite different names*

