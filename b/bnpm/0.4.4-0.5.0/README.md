# Comparing `tmp/bnpm-0.4.4.tar.gz` & `tmp/bnpm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnpm-0.4.4.tar", last modified: Wed Mar 27 23:30:11 2024, max compression
+gzip compressed data, was "bnpm-0.5.0.tar", last modified: Sat Apr 13 02:17:33 2024, max compression
```

## Comparing `bnpm-0.4.4.tar` & `bnpm-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:30:11.953613 bnpm-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 23:30:04.000000 bnpm-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 23:30:04.000000 bnpm-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-03-27 23:30:11.953613 bnpm-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-27 23:30:04.000000 bnpm-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:30:11.941613 bnpm-0.4.4/bnpm/
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57948 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/automatic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    37853 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/ca2p_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    49222 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/container_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/cupy_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/email_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/featurization.py
--rw-r--r--   0 runner    (1001) docker     (127)    24549 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/h5_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/image_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    64030 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25013 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/neural_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14176 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/other_peoples_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/parallel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/path_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    44685 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/plotting_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/resource_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43153 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    31408 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/sql_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    43442 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/timeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30820 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/torch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53601 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/welford_moving.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-03-27 23:30:04.000000 bnpm-0.4.4/bnpm/welford_moving_2D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:30:11.941613 bnpm-0.4.4/bnpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-03-27 23:30:11.000000 bnpm-0.4.4/bnpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-27 23:30:11.000000 bnpm-0.4.4/bnpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:30:11.000000 bnpm-0.4.4/bnpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-27 23:30:11.000000 bnpm-0.4.4/bnpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 23:30:11.000000 bnpm-0.4.4/bnpm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-27 23:30:04.000000 bnpm-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-27 23:30:11.953613 bnpm-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-27 23:30:04.000000 bnpm-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:17:33.474675 bnpm-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 02:17:27.000000 bnpm-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 02:17:27.000000 bnpm-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-13 02:17:33.474675 bnpm-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-13 02:17:27.000000 bnpm-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:17:33.462675 bnpm-0.5.0/bnpm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57948 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/automatic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37853 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/ca2p_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49222 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18244 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/container_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/cupy_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29002 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/email_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/featurization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24549 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/h5_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/image_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64030 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25013 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/neural_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/other_peoples_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/parallel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/path_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44685 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/plotting_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/resource_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33621 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17139 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/sql_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47053 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/timeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32955 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/torch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53601 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/welford_moving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-13 02:17:27.000000 bnpm-0.5.0/bnpm/welford_moving_2D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:17:33.462675 bnpm-0.5.0/bnpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-13 02:17:33.000000 bnpm-0.5.0/bnpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-13 02:17:33.000000 bnpm-0.5.0/bnpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 02:17:33.000000 bnpm-0.5.0/bnpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-13 02:17:33.000000 bnpm-0.5.0/bnpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 02:17:33.000000 bnpm-0.5.0/bnpm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 02:17:27.000000 bnpm-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 02:17:33.474675 bnpm-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-13 02:17:27.000000 bnpm-0.5.0/setup.py
```

### Comparing `bnpm-0.4.4/LICENSE` & `bnpm-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/PKG-INFO` & `bnpm-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.4.4
+Version: 0.5.0
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bnpm-0.4.4/README.md` & `bnpm-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/__init__.py` & `bnpm-0.5.0/bnpm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,8 @@
         cv2.destroyWindow('startup')
     prepare_cv2_imshow()
 
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.4.4'
+__version__ = '0.5.0'
```

### Comparing `bnpm-0.4.4/bnpm/automatic_regression.py` & `bnpm-0.5.0/bnpm/automatic_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/ca2p_preprocessing.py` & `bnpm-0.5.0/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/circular.py` & `bnpm-0.5.0/bnpm/circular.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/classification.py` & `bnpm-0.5.0/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/clustering.py` & `bnpm-0.5.0/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/container_helpers.py` & `bnpm-0.5.0/bnpm/container_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/cross_validation.py` & `bnpm-0.5.0/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/cupy_helpers.py` & `bnpm-0.5.0/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/email_helpers.py` & `bnpm-0.5.0/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/featurization.py` & `bnpm-0.5.0/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/file_helpers.py` & `bnpm-0.5.0/bnpm/file_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/h5_handling.py` & `bnpm-0.5.0/bnpm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/image_augmentation.py` & `bnpm-0.5.0/bnpm/image_augmentation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/image_processing.py` & `bnpm-0.5.0/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/indexing.py` & `bnpm-0.5.0/bnpm/indexing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/linear_regression.py` & `bnpm-0.5.0/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/math_functions.py` & `bnpm-0.5.0/bnpm/math_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -300,8 +300,60 @@
 
     Returns:
         output (np.ndarray):
             Random numbers from the log-uniform distribution
     """
     if isinstance(size, int):
         size = (size,)
-    return low*10**(np.random.rand(*size)*(np.log(high/low) / np.log(10)))
+    return low*10**(np.random.rand(*size)*(np.log(high/low) / np.log(10)))
+
+
+def make_odd(n, mode='up'):
+    """
+    Make a number odd.
+    RH 2023
+
+    Args:
+        n (int):
+            Number to make odd
+        mode (str):
+            'up' or 'down'
+            Whether to round up or down to the nearest odd number
+
+    Returns:
+        output (int):
+            Odd number
+    """
+    if n % 2 == 0:
+        if mode == 'up':
+            return n + 1
+        elif mode == 'down':
+            return n - 1
+        else:
+            raise ValueError("mode must be 'up' or 'down'")
+    else:
+        return n
+def make_even(n, mode='up'):
+    """
+    Make a number even.
+    RH 2023
+
+    Args:
+        n (int):
+            Number to make even
+        mode (str):
+            'up' or 'down'
+            Whether to round up or down to the nearest even number
+
+    Returns:
+        output (int):
+            Even number
+    """
+    if n % 2 != 0:
+        if mode == 'up':
+            return n + 1
+        elif mode == 'down':
+            return n - 1
+        else:
+            raise ValueError("mode must be 'up' or 'down'")
+    else:
+        return n
```

### Comparing `bnpm-0.4.4/bnpm/misc.py` & `bnpm-0.5.0/bnpm/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import sys
 import re
 import hashlib
 from pathlib import Path
 import warnings
 from typing import Callable, List, Any, Dict
-from contextlib import contextmanager
+from contextlib import contextmanager, ExitStack
 
 
 def estimate_array_size(
     array=None, 
     numel=None, 
     input_shape=None, 
     bitsize=64, 
@@ -387,14 +387,35 @@
     Returns a function that hashes an array.
     """
     from functools import partial
     import xxhash
     return partial(xxhash.xxh64_hexdigest, seed=0)
 
 
+def reset_warnings():
+    """
+    Resets warnings to default settings.
+    """
+    import warnings
+    warnings.simplefilter('default')
+
+def reset_numpy_warnings():
+    """
+    Resets numpy warnings to default settings.
+    """
+    import numpy as np
+    np.seterr(all='warn')
+    
+
+
+#####################################################################
+################# CONTEXT MANAGERS AND DECORATORS ###################
+#####################################################################
+
+
 @contextmanager
 def temp_set_attr(obj, attr_name, new_value):
     """
     Temporarily set an attribute of an object to a new value within a context
     manager / closure.
     RH 2024
 
@@ -459,14 +480,64 @@
                 k_toRename = ix_nk_k.pop()
                 kwargs[k_toUse] = kwargs.pop(k_toRename)
             return func(*args, **kwargs)
         return wrapped
     return wrapper
 
 
+class MultiContextManager:
+    """
+    A context manager that allows multiple context managers to be used at once.
+    RH 2024
+
+    Args:
+        *managers (context managers):
+            Multiple context managers to be used at once.
+
+    Demo:
+        .. code-block:: python
+
+            with MultiContextManager(
+                torch.no_grad(), 
+                temp_set_attr(obj, attr, new_val), 
+                open('file.txt', 'w') as f,
+            ):
+                # do something
+    """
+    def __init__(self, *managers):
+        self.managers = managers
+        self.stack = ExitStack()
+
+    def __enter__(self):
+        for manager in self.managers:
+            self.stack.enter_context(manager)
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.stack.__exit__(exc_type, exc_value, traceback)
+        
+        
+class TimeoutException(Exception):
+    pass
+@contextmanager
+def time_limit(seconds):
+    """
+    Wrapper to set a time limit for a block of code, after which a
+    TimeoutException is raised.
+    """
+    import signal
+    def signal_handler(signum, frame):
+        raise TimeoutException("Timed out")
+    signal.signal(signal.SIGALRM, signal_handler)
+    signal.alarm(seconds)
+    try:
+        yield
+    finally:
+        signal.alarm(0)
+
+
 #########################################################
 ############ INTRA-MODULE HELPER FUNCTIONS ##############
 #########################################################
 
 
 def convert_size(size, return_size='GB'):
     """
```

### Comparing `bnpm-0.4.4/bnpm/neural_networks.py` & `bnpm-0.5.0/bnpm/neural_networks.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/optimization.py` & `bnpm-0.5.0/bnpm/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         self.bests.append(self.best)
             
         bests_recent = np.unique(self.bests[-self.n_patience:])
         if self.num_trial > self.n_patience and ((np.abs(bests_recent.max() - bests_recent.min())/np.abs(self.best)) < self.tol_frac):
             self.converged, self.reason_converged = True, 'tol_frac'
             print(f'Stopping. Convergence reached. Best value ({self.best*10000}) over last ({self.n_patience}) trials fractionally changed less than ({self.tol_frac})') if self.verbose else None
             study.stop()
-        elif self.num_trial >= self.max_trials:
+        elif self.num_trial >= self.max_trials - 1:
             self.converged, self.reason_converged = True, 'max_trials'
             print(f'Stopping. Trial number limit reached. num_trial={self.num_trial}, max_trials={self.max_trials}.') if self.verbose else None
             study.stop()
         elif duration > self.max_duration:
             self.converged, self.reason_converged = True, 'max_duration'
             print(f'Stopping. Duration limit reached. study.duration={duration}, max_duration={self.max_duration}.') if self.verbose else None
             study.stop()
```

### Comparing `bnpm-0.4.4/bnpm/other_peoples_code.py` & `bnpm-0.5.0/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/parallel_helpers.py` & `bnpm-0.5.0/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/path_helpers.py` & `bnpm-0.5.0/bnpm/path_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 """
 from typing import Union, Optional, List
 
 import os
 import numpy as np
 from pathlib import Path
 import re
+import warnings
+import datetime
+
+from . import misc
 
 def mkdir(directory, parents=True, exist_ok=True):
     '''
     Create a directory if it doesn't exist.
     RH 2021
 
     Args:
@@ -141,16 +145,19 @@
             Whether to sort the output using natural sorting with the natsort
             package. (Default is ``True``)
         alg_ns (str): 
             Algorithm to use for natural sorting. See ``natsort.ns`` or
             https://natsort.readthedocs.io/en/4.0.4/ns_class.html/ for options.
             Default is PATH. Other commons are INT, FLOAT, VERSION. (Default is
             ``None``)
-        verbose (bool):
-            Whether to print the paths found. (Default is ``False``)
+        verbose (Union[bool, int]):
+            Whether to print the paths found. (Default is ``False``) \n
+                * If False/0, then no printout.
+                * If True/1, then printout.
+                * If 2, then printout with additional details.
 
     Returns:
         (List[str]): 
             paths (List[str]): 
                 Paths to matched files and/or folders in the directory.
     """
     import natsort
@@ -167,26 +174,32 @@
                 return False
         return True
 
     def get_paths_recursive_inner(dir_inner, depth_end, depth=0):
         paths = []
         for path in os.listdir(dir_inner):
             path = os.path.join(dir_inner, path)
+            print(f'Checking path: {path}') if verbose > 1 else None
             if os.path.isdir(path):
                 if find_folders:
                     if fn_match(path, reMatch, reMatch_in_path):
-                        print(f'Found folder: {path}') if verbose else None
+                        print(f'Found folder: {path}') if verbose > 0 else None
                         paths.append(path)
+                    else:
+                        print(f'Not matched: {path}') if verbose > 1 else None
                 if depth < depth_end:
+                    print(f'Entering folder: {path}') if verbose > 1 else None
                     paths += get_paths_recursive_inner(path, depth_end, depth=depth+1)
             else:
                 if find_files:
                     if fn_match(path, reMatch, reMatch_in_path):
-                        print(f'Found file: {path}') if verbose else None
+                        print(f'Found file: {path}') if verbose > 0 else None
                         paths.append(path)
+                    else:
+                        print(f'Not matched: {path}') if verbose > 1 else None
         return paths
 
     def fn_check_pathLike(obj):
         if isinstance(obj, (
             str,
             Path,
             os.PathLike,
@@ -331,7 +344,166 @@
         )
         if date is not None:
             ## Remove the modifiers from the date string.
             date = date[num[0]:-num[1] if num[1]>0 else None]
             break
 
     return date
+
+
+def check_files_openable(dir_outer, time_limit_per_file=1, verbose=False):
+    """
+    Check if files within an outer directory are able to be opened. \n
+    RH 2024
+
+    Args:
+        dir_outer (str):
+            Path to the outer directory
+        depth (int):
+            Maximum depth of subdirectories to search. \n
+            Depth=0 means only the outer directory. \n
+            Default is 2.
+        time_limit_per_file (int):
+            Time limit in seconds for checking if a file can be opened.
+        verbose (bool):
+            Whether to print the files that can't be opened. \n
+            Default is False.
+
+    Returns:
+        (dict):
+            Dictionary with keys as the file paths and values as booleans
+            indicating whether the file can be opened.
+    """
+    import os
+    from concurrent.futures import ThreadPoolExecutor, TimeoutError
+    from contextlib import contextmanager
+
+    def check_file_openable(file_path):
+        """
+        Check if a file can be opened.
+        """
+        try:
+            with open(file_path, 'rb') as f:
+                ## Read a maximum of 1024 bytes. If file is smaller, read the whole file.
+                f.read(1024)
+            print(f"File {file_path} can be opened.") if verbose > 1 else None
+            return True
+        except Exception as e:
+            print(f"FAILURE: File {file_path} could not be opened: {e}") if verbose > 0 else None
+            return False
+        
+    def check_with_timeout(file_path, time_limit):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(check_file_openable, file_path)
+            try:
+                return future.result(timeout=time_limit)
+            except TimeoutError:
+                print(f"FAILURE: File {file_path} took too long to open.") if verbose > 0 else None
+                return False
+        
+    def walk_files(dir_outer):
+        """
+        Walk through files in a directory.
+        """
+        files = []
+        for root, dirs, filenames in os.walk(dir_outer):
+            for filename in filenames:
+                files.append(os.path.join(root, filename))
+        return files
+    
+    files = walk_files(dir_outer)
+    file_openable = {file: check_with_timeout(file, time_limit=time_limit_per_file) for file in files}
+    return file_openable
+
+
+def touch_path(
+    path: Union[str, Path],
+    recursive: bool = False,
+    dt: Optional[datetime] = None,
+    files: bool = True,
+    directories: bool = True,
+    verbose: Union[bool, int] = False,
+) -> None:
+    """
+    Update the last modified datetime of specified files and/or directories
+    without creating new ones. Symbolic links are skipped. \n
+    RH 2024
+
+    Args:
+        path (Union[str, Path]): 
+            The directory or file path to modify.
+        recursive (bool): 
+            Whether to recursively apply changes to all subfiles and subfolders.
+        dt (Optional[datetime]): 
+            The datetime to set as the last modified time. If not specified, the
+            current datetime is used.
+        files (bool): 
+            If True, update modification times of files.
+        directories (bool): 
+            If True, update modification times of directories.
+        verbose (Union[bool, int]):
+            Whether to print the paths that are modified / Level of verbosity.
+            \n
+                * If False/0, then no printout.
+                * If True/1, then print changed paths.
+                * If 2, also print skipped paths.
+
+    Returns:
+        None
+
+    Raises:
+        FileNotFoundError: If the path does not exist or would be created by the touch command.
+
+    Demo:
+        .. code-block:: python
+            touch_path('/tmp/example.txt', dt=datetime(2024, 4, 8, 23, 30), files=True, directories=False)
+    """
+    ## Get the timestamp.
+    if dt:
+        timestamp = dt.timestamp()
+    else:
+        timestamp = datetime.datetime.now().timestamp()
+
+    def update_mod_time(target_path: Path) -> None:
+        """Updates the modification time of a file or directory."""
+        ## Pre-modification time.
+        try:
+            t_pre = datetime.datetime.fromtimestamp(target_path.stat().st_mtime)
+        except Exception as e:
+            t_pre = None
+            warnings.warn(f"Could not get the modification time of {target_path}: {e}")
+
+        ## Update the modification time.
+        ### utime inputs are (path, (atime, mtime)). atime: access time, mtime: modification time.
+        os.utime(target_path, (timestamp, timestamp))
+        print(f"Modified: {target_path}       from {t_pre} to {datetime.datetime.fromtimestamp(timestamp)}") if verbose > 0 else None
+
+    ## Convert the path to a Path object.
+    path = Path(path)
+
+    ## Check if the path exists.
+    if not path.exists():
+        raise FileNotFoundError(f"The path {path} does not exist.")
+
+    ## Update the modification time of the path.
+    if path.is_file():
+        if files:
+            update_mod_time(path)
+        else:
+            print(f"Skipping: {path}") if verbose > 1 else None
+    elif path.is_dir():
+        if directories:
+            update_mod_time(path)
+        else:
+            print(f"Skipping: {path}") if verbose > 1 else None
+        if recursive:
+            for sub_path in path.rglob('*'):  ## rglob('*') fetches all files and directories recursively.
+                if sub_path.is_file() and files:
+                    update_mod_time(sub_path)
+                elif sub_path.is_dir() and directories:
+                    update_mod_time(sub_path)
+                else:
+                    print(f"Skipping: {sub_path}") if verbose > 1 else None
+    elif path.is_symlink():  ## Skip symbolic links.
+        print(f"Skipping: {path} (symlink)") if verbose > 1 else None
+    else:
+        raise FileNotFoundError(f"The path {path} returned neither .is_file() nor .is_dir(). It may be a symlink, missing, or otherwise inaccessible.")
```

### Comparing `bnpm-0.4.4/bnpm/plotting_helpers.py` & `bnpm-0.5.0/bnpm/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/resource_tracking.py` & `bnpm-0.5.0/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/server.py` & `bnpm-0.5.0/bnpm/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -616,21 +616,22 @@
             port (int):
                 Port of the remote server.
         """
         if ssh_client is None:
             self.transport = paramiko.Transport((hostname, port))  ## open a transport object
         else:
             if isinstance(ssh_client, ssh_interface):
-                client = ssh_client.client
-                self.sftp = client.open_sftp()
+                self.client = ssh_client
+                self.sftp = self.client.open_sftp()
             elif isinstance(ssh_client, paramiko.SSHClient):
-                client = ssh_client
-                self.sftp = client.open_sftp()
+                self.client = ssh_client
+                self.sftp = self.client.open_sftp()
             elif isinstance(ssh_client, paramiko.Channel):
-                self.sftp = paramiko.SFTPClient.from_transport(ssh_client.get_transport())
+                self.transport = ssh_client.get_transport()
+                self.sftp = paramiko.SFTPClient.from_transport(self.transport)
         
     def connect(
         self,
         username='rh183',
         password=''
     ):
         """
@@ -638,16 +639,21 @@
         Args:
             username (str):
                 Username to log in with.
             password (str):
                 Password to log in with.
                 Is not stored.
         """
-        self.transport.connect(None, username, password)  ## authorization
-        self.sftp = paramiko.SFTPClient.from_transport(self.transport)  ## open sftp
+        if hasattr(self, 'transport'):
+            self.transport.connect(None, username, password)  ## authorization
+            self.sftp = paramiko.SFTPClient.from_transport(self.transport)  ## open sftp
+        elif hasattr(self, 'client'):
+            self.sftp = self.client.open_sftp()
+        else:
+            raise ValueError('No valid connection method found')
     
     def put_dir(self, source, target, mkdir=True, verbose=True):
         '''
         Uploads the contents of the source directory to the target path.
         All subdirectories in source are created under target recusively.
         Args:
             source (str):
@@ -999,17 +1005,23 @@
                     f_in=f_in,
                     f_out=f_out,
                     prefetch=prefetch,
                     callback=conj_func if prog_bar else callback,
                 ).download()
 
     def close(self):
-        self.sftp.close()
-        self.transport.close()
+        if hasattr(self, 'transport'):
+            self.transport.close()
+        elif hasattr(self, 'client'):
+            self.client.close()
+        elif hasattr(self, 'sftp'):
+            self.sftp.close()
 
+    def refresh_connection(self):
+        self.connect()
 
 def make_rsync_command(
     source, 
     destination, 
     recursive=True, 
     preserve_attributes=True, 
     verbose=True,
```

### Comparing `bnpm-0.4.4/bnpm/similarity.py` & `bnpm-0.5.0/bnpm/similarity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,20 @@
-'''
-Table of Contents
+from typing import Union, List, Tuple
+import copy
+import time
+from functools import partial
 
-Functions and Interdependencies:
-    proj
-    orthogonalize
-        - proj
-    OLS
-    EV
-    pairwise_similarity
-    best_permutation
-        - pairwise_similarity
-    self_similarity_pairwise
-        - best_permutation
-'''
 import numpy as np
 import scipy.optimize
-# import sklearn.decomposition
 from numba import njit, prange, jit
 import torch
 from tqdm import tqdm
 
-from . import indexing
+from . import indexing, torch_helpers
 
-import copy
-import time
-from functools import partial
 
 def proj(v1, v2):
     '''
     Projects one or more vectors (columns of v1) onto one or more vectors (v2)
     RH 2021
 
     Args:
@@ -245,14 +231,48 @@
             for key in pca_dict.keys():
                 if isinstance(pca_dict[key], torch.Tensor):
                     pca_dict[key] = pca_dict[key].cpu().numpy()
 
     return v1_orth, EVR, EVR_total, pca_dict
 
 
+def orthogonalize_matrix_nearest(X: Union[np.ndarray, torch.Tensor], center=True):
+    """
+    Orthogonalizes a matrix by finding the nearest orthogonal matrix. Nearest is
+    defined as solving the Procrustes problem via minimizing the Frobenius norm
+    of the difference between the original input matrix and the orthogonal
+    matrix. \n
+    X_orth = argmin ||X - X_orth||_F
+
+    Note: The solution to this problem is generally equivalent to the ZCA
+    whitening of PCA(X).
+
+    Args:
+        X (ndarray):
+            Matrix to orthogonalize. shape: (n_samples, n_features)
+        center (bool):
+            Whether to center the matrix. Default is True.
+
+    Returns:
+        (ndarray):
+            X_orth: orthogonalized matrix. shape: (n_samples, n_features)
+    """
+    if isinstance(X, np.ndarray):
+        op, qr = scipy.linalg.orthogonal_procrustes, np.linalg.qr
+    elif isinstance(X, torch.Tensor):
+        op, qr = torch_helpers.orthogonal_procrustes, torch.linalg.qr
+
+    if center:
+        X = X - X.mean(axis=0, keepdims=True)
+
+    Q = qr(X)[0]
+    w, scale = op(Q, X)
+    return w @ scale
+
+
 @njit
 def pair_orth_helper(v1, v2):
     """
     Helper function for main pairwise_orthogonalization
      function. Performs the pairwise orthogonalization
      by subtracting off v2 from v1. Uses numba to speed
      up the computation.
@@ -472,41 +492,46 @@
             unbiased calculation, 0 for biased calculation.
     Returns:
         ouput (ndarray):
             similarity matrix dependent on method
     '''
 
     methods = ['cov', 'pearson', 'R', 'cosine_similarity']
-    assert np.isin(method, methods), f'RH Error: method must be one of: {methods}'
+    assert method in methods, f'RH Error: method must be one of: {methods}'
+
+    if isinstance(v1, np.ndarray):
+        mean, sum, sqrt, norm = np.mean, np.sum, np.sqrt, np.linalg.norm
+    elif isinstance(v1, torch.Tensor):
+        mean, sum, sqrt, norm = torch.mean, torch.sum, torch.sqrt, torch.linalg.norm
 
     if v2 is None:
         v2 = v1
     
     if v1.ndim == 1:
         v1 = v1[:,None]
     if v2.ndim == 1:
         v2 = v2[:,None]
 
     if method=='cov':
-        v1_ms = v1 - np.mean(v1, axis=0) # 'mean subtracted'
-        v2_ms = v2 - np.mean(v2, axis=0)
+        v1_ms = v1 - mean(v1, axis=0) # 'mean subtracted'
+        v2_ms = v2 - mean(v2, axis=0)
         output = (v1_ms.T @ v2_ms) / (v1.shape[0] - ddof)
     if method in ['pearson', 'R']: 
         # Below method should be as fast as numpy.corrcoef . 
         # Output should be same within precision, but 
         # numpy.corrcoef makes a doublewide matrix and can be annoying
         
         # Note: Pearson's R-value can be different than sqrt(EV) 
         # calculated below if the residuals are not orthogonal to the 
         # prediction. Best to use EV for R^2 if unsure
-        v1_ms = v1 - np.mean(v1, axis=0) # 'mean subtracted'
-        v2_ms = v2 - np.mean(v2, axis=0)
-        output = (v1_ms.T @ v2_ms) / np.sqrt(np.sum(v1_ms**2, axis=0, keepdims=True).T * np.sum(v2_ms**2, axis=0, keepdims=True))
+        v1_ms = v1 - mean(v1, axis=0) # 'mean subtracted'
+        v2_ms = v2 - mean(v2, axis=0)
+        output = (v1_ms.T @ v2_ms) / sqrt(sum(v1_ms**2, axis=0, keepdims=True).T * sum(v2_ms**2, axis=0, keepdims=True))
     if method=='cosine_similarity':    
-        output = (v1 / (np.linalg.norm(v1 , axis=0, keepdims=True))).T  @ (v2  / np.linalg.norm(v2 , axis=0, keepdims=True))
+        output = (v1 / (norm(v1 , axis=0, keepdims=True))).T  @ (v2  / norm(v2 , axis=0, keepdims=True))
     return output
 
 
 def batched_covariance(X, batch_size=1000, device='cpu'):
     """
     Batched covariance matrix calculation.
     Allows for large datasets to be processed in batches on GPU.
@@ -631,15 +656,15 @@
         d = np.sqrt(1-(x+b))**a # fn 5: sqrt(1-x)
     if fn_toUse == 6:
         d = -np.log((x*a)+b) # fn 6: -log(x)
     
     return d + eps
     
 
-def cp_reconstruction_EV(tensor_dense, tensor_CP):
+def cp_reconstruction_EVR(tensor_dense, tensor_CP):
     """
     Explained variance of a reconstructed tensor using
     by a CP tensor (similar to kruskal tensor).
     RH 2023
 
     Args:
         tensor_dense (np.ndarray or torch.Tensor):
@@ -665,15 +690,51 @@
 
     if isinstance(tensor_dense, torch.Tensor):
         var = torch.var
     elif isinstance(tensor_dense, np.ndarray):
         var = np.var
     ev = 1 - (var(tensor_dense - tensor_rec) / var(tensor_dense))
     return ev
+
+
+def order_cp_factors_by_EVR(
+    tensor_dense,
+    tensor_CP,
+):
+    """
+    Get the sorting order of the CP factors by their
+    explained variance ratio.
+    RH 2024
+
+    Args:
+        tensor_dense (np.ndarray or torch.Tensor):
+            Dense tensor to be reconstructed. shape (n_samples, n_features)
+        tensor_CP (tensorly CPTensor or list of np.ndarray/torch.Tensor):
+            CP tensor.
+            If a list of factors, then each factor should be a 2D array of shape
+            (n_samples, rank).
+            Can also be a tensorly CPTensor object.
+    """
+    if isinstance(tensor_CP, list):
+        factors = tensor_CP
+    elif isinstance(tensor_CP, tl.cp_tensor.CPTensor):
+        import tensorly as tl
+        factors = tensor_CP.factors
+    else:
+        raise ValueError('tensor_CP must be a list of factors or a tensorly CPTensor object')
     
+    rank = factors[0].shape[1]
+    evrs = []
+    for ii in range(rank):
+        f = [f[:, ii][:, None] for f in factors]
+        evr = cp_reconstruction_EVR(tensor_dense, f)
+        evrs.append(evr)
+    order = np.argsort(evrs)[::-1]
+    return order, np.array(evrs)[order]
+
 
 ##########################################    
 ########### Linear Assignment ############
 ##########################################
 
 def best_permutation(mat1 , mat2 , method='pearson'):
     '''
```

### Comparing `bnpm-0.4.4/bnpm/spectral.py` & `bnpm-0.5.0/bnpm/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,66 +452,65 @@
     n = xf.shape[axis]
     k = arange(n)
     w = exp(-2j * pi * k / n)
     ## Apply the inverse shift operator
     return resolution(conj(xf * w))
 
 
-@misc.wrapper_flexible_args(['dim', 'axis'])
 def filtfilt_simple_fft(
     x: Union[torch.Tensor, np.ndarray],
     kernel: Union[torch.Tensor, np.ndarray],
     fast_len: bool = True,
-    axis: int = -1,
 ):
     """
-    Applies a zero-phase filter to the input signal using the FFT method.\n
-    Calculated as ifft(fft(x) * fft(kernel) * fft(kernel_flipped)).\n
-    This implementation is very fast and is suitable for large signals.\n
+    Applies a zero-phase filter to the input signal using the FFT method along
+    the last dimension.\n
+    Calculated as ``ifft(fft(x) * fft(kernel) * fft(kernel_flipped))``.\n
+    This implementation is very fast and is suitable when using long kernels.\n
     NOTE: This is a simple implementation and does not handle edge effects.
-    scipy.signal.filtfilt is recommended if speed is not a concern.\n
+    scipy.signal.filtfilt is recommended if speed is not a concern and/or if
+    kernel length is similar in length to x.\n
     RH 2024
 
     Args:
         x (torch.Tensor or np.ndarray):
-            Signal data.
+            Signal data. Convolution is done along the last dimension.
         kernel (torch.Tensor or np.ndarray):
-            Filter kernel.
+            Filter kernel. Convolution is done along the last dimension. \n
+            If not 1D, then shape should be broadcastable with x.
         fast_len (bool):
             Whether to use the fast length method.
-        axis (int):
-            Dimension along which to do the transformation.
 
     Returns:
         (nd tensor):
             Filtered signal
     """
     assert isinstance(x, torch.Tensor) or isinstance(x, np.ndarray), "x must be a torch tensor or numpy array"
 
     if isinstance(x, torch.Tensor) and isinstance(kernel, torch.Tensor):
         use_real = (torch.is_complex(x) == False) and (torch.is_complex(kernel) == False)
-        fft, ifft = (functools.partial(fn, dim=axis) for fn in ((torch.fft.rfft, torch.fft.irfft) if use_real else (torch.fft.fft, torch.fft.ifft)))
-        flip = functools.partial(torch.flip, dims=(axis,))
+        fft, ifft = (functools.partial(fn, dim=-1) for fn in ((torch.fft.rfft, torch.fft.irfft) if use_real else (torch.fft.fft, torch.fft.ifft)))
+        flip = functools.partial(torch.flip, dims=(-1,))
     elif isinstance(x, np.ndarray) and isinstance(kernel, np.ndarray):
         use_real = (np.iscomplexobj(x) == False) and (np.iscomplexobj(kernel) == False)
-        fft, ifft = (functools.partial(fn, axis=axis) for fn in ((np.fft.rfft, np.fft.irfft) if use_real else (np.fft.fft, np.fft.ifft)))
-        flip = functools.partial(np.flip, axis=axis)
+        fft, ifft = (functools.partial(fn, axis=-1) for fn in ((np.fft.rfft, np.fft.irfft) if use_real else (np.fft.fft, np.fft.ifft)))
+        flip = functools.partial(np.flip, axis=-1)
     else:
         raise ValueError("x and kernel must be torch tensors or numpy arrays")
     
-    f_flip = functools.partial(time_domain_reversal_in_fourier_domain, axis=axis)
+    f_flip = functools.partial(time_domain_reversal_in_fourier_domain, axis=-1)
 
-    n = x.shape[axis] + kernel.shape[axis] - 1
+    n = x.shape[-1] + kernel.shape[-1] - 1
     n = timeSeries.next_fast_len(n) if fast_len else n
 
     out = fft(x, n=n)  ## x_fft
     kernel_fft = fft(flip(kernel), n=n)
     out = out * kernel_fft  ## xk_fft_1
     out = out * f_flip(kernel_fft)  ## xk_fft_2
     out = ifft(out, n=n)  ## xk
     out = torch_helpers.slice_along_dim(
         X=out,
-        dim=axis,
-        idx=slice(0, x.shape[axis]),
+        dim=-1,
+        idx=slice(0, x.shape[-1]),
     )
     out = out.real if use_real else out
     return out
```

### Comparing `bnpm-0.4.4/bnpm/stats.py` & `bnpm-0.5.0/bnpm/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import scipy.stats
+import torch
 
 def ttest_paired_ratio(a, b):
     """
     Computes the ratio paired t-test between two arrays of data.
     This is useful for comparing ratios of data, and can be
      thought of as a geometric mean paired t-test.
     The ratio t-test takes the logarithm of the ratio of
@@ -32,26 +33,42 @@
     p_val = scipy.stats.t.sf(np.abs(t_stat), len(a)-1)*2
 
     ## above is equivalent to:
     # t_stat, p_val = scipy.stats.ttest_rel(np.log(a/b), np.zeros_like(a))
     return p_val
 
 
-def geometric_mean(a):
+def geometric_mean(a, axis=0, nan_policy="omit"):
     """
     Computes the geometric mean of an array of data.
     This is useful for computing the geometric mean of ratios.
     
     RH 2023
 
     Args:
         a (np.ndarray or torch.Tensor):
             Array of data.
     """
-    return np.exp(np.mean(np.log(a)))
+    if isinstance(a, (np.ndarray, list)):
+        mean, nanmean, isnan, exp, log = np.mean, np.nanmean, np.isnan, np.exp, np.log
+    elif isinstance(a, torch.Tensor):
+        mean, nanmean, isnan, exp, log = torch.mean, torch.nanmean, torch.isnan, torch.exp, torch.log
+    else:
+        raise ValueError("Data must be a numpy array or a torch tensor.")
+
+    if nan_policy == "omit":
+        mean = nanmean
+    elif nan_policy == "propagate":
+        mean = mean
+    elif nan_policy == "raise":
+        mean = mean
+        if isnan(a).any():
+            raise ValueError("Data contains nan values.")
+        
+    return exp(mean(log(a), axis=axis))
 
 
 def sparsity(a, axis=0):
     """
     A normalized dispersion index. Varies from 0 (dense) to 1 (sparse).
     Computes the lifetime sparseness of an array of data.
     From Vinje & Gallant 2000; and Willmore, Mazer, & Gallant 2011.
```

### Comparing `bnpm-0.4.4/bnpm/testing.py` & `bnpm-0.5.0/bnpm/testing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/timeSeries.py` & `bnpm-0.5.0/bnpm/timeSeries.py`

 * *Files 4% similar despite different names*

```diff
@@ -697,14 +697,106 @@
         return out
     
     def __call__(self, arr):
         return self.convolve(arr)
     def __repr__(self) -> str:
         return f"Convolver_1d(kernel shape={self.kernel.shape}, pad_mode={self.pad_mode})"
     
+
+@njit(parallel=False, fastmath=True, nogil=True)
+def _helper_dampening_filter_numba(X: np.ndarray, X_diff: np.ndarray, dampening_factor: float):
+    """
+    Numba helper function for dampening_filter_numba.
+    """
+    Y = np.zeros_like(X)
+    for i in range(1, len(X)):
+        Y[i] = Y[i-1]*dampening_factor + X_diff[i-1]
+    return Y
+def dampening_filter(X: np.ndarray, dampening_factor: float = 0.9):
+    """
+    Dampening filter. Applies a recursive dampening filter that pulls values
+    back towards zero.
+    function: y[t] = y[t-1]*d + (x[t] - x[t-1])
+    numba implementation appears to be faster than torch
+
+    RH 2024
+
+    Args:
+        X (np.ndarray):
+            Input array. Dampening will be performed
+            along the first dimension (columns).
+        dampening_factor (float):
+            Dampening factor. Should typically be between 0 and 1.
+
+    Returns:
+        Y (np.ndarray):
+            Dampened array.
+    """
+    X_diff = np.diff(X, axis=0)
+    Y = _helper_dampening_filter_numba(X, X_diff, dampening_factor)
+    return Y
+
+
+## Import jax if available
+try:
+    import jax
+    import jax.numpy as jnp
+
+    def dampening_step(carry, x_curr):
+        """
+        Perform a single step of the dampening process.
+        
+        Args:
+            carry: A tuple containing the previous output y (y_prev), the previous input x (x_prev),
+                and the dampening factor.
+            x_curr: Current value of x.
+        
+        Returns:
+            Updated carry and the current y value.
+        """
+        y_prev, x_prev, dampening_factor = carry
+        
+        # # Handle division by zero safely. Ensure x_prev is not zero before dividing.
+        # # This avoids the ambiguous truth value error by not using arrays in conditions.
+        # division_result = 0 if x_prev == 0 else y_prev / x_prev
+        
+        # Calculate the current y value using the given formula.
+        y_curr = y_prev * dampening_factor + (x_curr - x_prev) * 1
+        
+        # Update the carry for the next iteration.
+        carry = (y_curr, x_curr, dampening_factor)
+        return carry, y_curr
+
+    @jax.jit
+    def dampening_filter_jax(X, dampening_factor=0.9):
+        """
+        Applies a recursive dampening filter on a series of data points using JAX.
+        Utilizes `lax.scan` for efficiently applying the dampening step function across the input series.
+        
+        Args:
+            X (jnp.ndarray): Input series on which the dampening filter is applied.
+            dampening_factor (float): Factor used in the dampening calculation.
+        
+        Returns:
+            jnp.ndarray: The series after applying the dampening filter.
+        """
+        # Initial conditions: y is zero and x is the first element of the series.
+        # The carry contains the initial y, initial x, and the dampening factor.
+        initial_carry = (jnp.zeros_like(X[0]), X[0], dampening_factor)
+        
+        # Apply the dampening step across the series. Skip the first element since it's part of the initial conditions.
+        _, Y = jax.lax.scan(dampening_step, initial_carry, X[1:])
+        
+        # Include the initial y value at the start of the series.
+        Y = jnp.concatenate([jnp.zeros_like(X[:1]), Y])
+        
+        return Y
+
+except ImportError:
+    pass
         
 ####################################
 ######## PYTORCH algorithms ########
 ####################################
 
 def convolve_torch(X, kernels, **conv1d_kwargs):
     """
@@ -1145,23 +1237,25 @@
 class FFTConvolve(torch.nn.Module):
     def __init__(
         self, 
         x: Optional[torch.Tensor]=None, 
         n: Optional[int]=None, 
         next_fast_length: bool=False,
         use_x_fft: bool=True,
+        return_real: bool=True,
     ):
         super(FFTConvolve, self).__init__()
         if x is not None:
             self.set_x_fft(x=x, n=n, next_fast_length=next_fast_length)
         else:
             self.n = None
             self.x_fft = None
 
         self.use_x_fft = use_x_fft
+        self.return_real = return_real
 
     def set_x_fft(self, x: torch.Tensor, n: Optional[int]=None, next_fast_length: bool=False):
         if next_fast_length:
             self.n = next_fast_len(size=n)
         self.x_fft = torch.fft.fft(x, n=self.n, dim=-1).contiguous()
 
         ## Check for any NaNs or inf or weird values in x_fft
@@ -1176,11 +1270,21 @@
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         mode: str='same',
         n: Optional[int]=None,
         fast_length: Union[int, bool]=False,
         x_fft: Optional[torch.Tensor]=None,
+        return_real: bool=None,
     ) -> torch.Tensor:
         x_fft = self.x_fft if x_fft is None else x_fft
+        return_real = self.return_real if return_real is None else return_real
         n = self.n if n is None else n
-        return fftconvolve(x=x, y=y, mode=mode, n=n, fast_length=fast_length, x_fft=x_fft if self.use_x_fft else None)
+        return fftconvolve(
+            x=x, 
+            y=y, 
+            mode=mode, 
+            n=n, 
+            fast_length=fast_length, 
+            x_fft=x_fft if self.use_x_fft else None,
+            return_real=return_real,
+        )
```

### Comparing `bnpm-0.4.4/bnpm/torch_helpers.py` & `bnpm-0.5.0/bnpm/torch_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,47 +12,29 @@
 from . import misc
 
 
 ############################################
 ############ VARIABLE HELPERS ##############
 ############################################
 
-def show_all_tensors(
-    globals: dict,
-    sort_by_size_pref: bool = False,
-    data_unit: str = 'GB',
-) -> None:
+def show_all_tensors() -> None:
     """
     Displays all tensors present in the provided dictionary.
-    RH 2021
-
-    Args:
-        globals (dict):
-            Dictionary of global variables. Use the built-in function
-            ``globals()`` to obtain this dictionary.
-        sort_by_size_pref (bool):
-            If ``True``, the displayed tensors will be sorted according to their
-            size.
-        data_unit (str):
-            The unit in which to display the size of tensors. Options are Bytes
-            ('B'), Kilobytes ('KB'), Megabytes ('MB'), and Gigabytes ('GB').
-    """
-    size = []
-    strings = []
-    for var in globals:
-        if (type(globals[var]) is torch.Tensor):
-            size.append(_convert_size(globals[var].element_size() * globals[var].nelement(), return_size=data_unit))
-            strings.append(f'var: {var},   device:{globals[var].device},   shape: {globals[var].shape},   size: {size[-1]} {data_unit},   requires_grad: {globals[var].requires_grad}')
-
-    if sort_by_size_pref:
-        i_sort = np.argsort(size)[::-1]
-        strings = [strings[ii] for ii in i_sort]
-
-    for string in strings:
-        print(string)
+    From: https://discuss.pytorch.org/t/how-to-debug-causes-of-gpu-memory-leaks/6741
+    RH 2024
+    """
+    # prints currently alive Tensors and Variables
+    import torch
+    import gc
+    for obj in gc.get_objects():
+        try:
+            if torch.is_tensor(obj) or (hasattr(obj, 'data') and torch.is_tensor(obj.data)):
+                print(type(obj), obj.size())
+        except:
+            pass
 
 
 
 @contextmanager
 def temp_eval(module):
     """
     Temporarily sets the network to evaluation mode within a context manager.
@@ -216,29 +198,26 @@
         device = "cpu"
         print(f"device: '{device}'") if verbose else None
 
     return device
     
 
 def initialize_torch_settings(
-    device: Union[str, torch.device] = 'cuda:0',
     benchmark: Optional[bool] = None,
     enable_cudnn: Optional[bool] = None,
     deterministic_cudnn: Optional[bool] = None,
     deterministic_torch: Optional[bool] = None,
-    set_global_device: bool = True,
-    init_linalg: bool = True,
+    set_global_device: Optional[Union[str, torch.device]] = None,
+    init_linalg_device: Optional[Union[str, torch.device]] = None,
 ) -> None:
     """
     Initalizes some CUDA libraries and sets some environment variables. \n
     RH 2024
 
     Args:
-        device (Union[str, torch.device]):
-            The device to use.
         benchmark (Optional[bool]):
             If ``True``, sets torch.backends.cudnn.benchmark to ``True``.\n 
             This results in the built-in cudnn auto-tuner to find the best
             algorithm for the hardware. Good for when input sizes are the same
             for each batch.
         enable_cudnn (Optional[bool]):
             If ``True``, sets torch.backends.cudnn.enabled to ``True``.\n
@@ -246,41 +225,68 @@
         deterministic_cudnn (Optional[bool]):
             If ``True``, sets torch.backends.cudnn.deterministic to ``True``.\n
             This makes cudnn deterministic. It may slow down operations.
         deterministic_torch (Optional[bool]):
             If ``True``, sets torch.set_deterministic to ``True``.\n
             This makes torch deterministic. It may slow down operations.
         set_global_device (bool):
-            If ``True``, sets the global device to the provided device.\n
-            This is discouraged in favor of explicit device setting, but useful
-            for when you want to set the device globally.
-        init_linalg (bool):
-            If ``True``, initializes the linalg library. This is necessary to
-            avoid a bug. Often solves the error: "RuntimeError: lazy wrapper
-            should be called at most once".
+            If ``False``, does not set the global device. If a string or torch.device,
+            sets the global device to the specified device.
+        init_linalg_device (str):
+            The device to use for initializing the linalg library. Either a
+            string or a torch.device. This is necessary to avoid a bug. Often
+            solves the error: "RuntimeError: lazy wrapper should be called at
+            most once". (Default is ``None``)
     """
-    if type(device) is str:
-        device = torch.device(device)
-    
     if benchmark is not None:
         torch.backends.cudnn.benchmark = benchmark
     if enable_cudnn:
         torch.backends.cudnn.enabled = enable_cudnn
     if deterministic_cudnn:
         torch.backends.cudnn.deterministic = False
     if deterministic_torch:
         torch.set_deterministic(False)
-    if set_global_device:
-        torch.cuda.set_device(device)
+    if set_global_device is not None:
+        torch.cuda.set_device(set_global_device)
     
     ## Initialize linalg libarary
     ## https://github.com/pytorch/pytorch/issues/90613
-    if init_linalg:
-        torch.inverse(torch.ones((1, 1), device=device))
-        torch.linalg.qr(torch.as_tensor([[1.0, 2.0], [3.0, 4.0]], device=device))
+    if init_linalg_device is not None:
+        if type(init_linalg_device) is str:
+            init_linalg_device = torch.device(init_linalg_device)
+        torch.inverse(torch.ones((1, 1), device=init_linalg_device))
+        torch.linalg.qr(torch.as_tensor([[1.0, 2.0], [3.0, 4.0]], device=init_linalg_device))
+
+
+def profiler_simple(
+    path_save: str = 'trace.json',
+):
+    """
+    Simple profiler for PyTorch. \n
+    Makes a context manager that can be used to profile code. \n
+    Upon exit, will save the trace to the specified path. \n
+    """
+    from torch.profiler import profile, record_function, ProfilerActivity
+    from contextlib import contextmanager
+    
+    @contextmanager
+    def simple_profiler(path_save: str = 'trace.json'):
+        with profile(
+            activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], 
+            record_shapes=True,
+            profile_memory=True,
+            with_stack=True,
+            # with_flops=True,
+            # with_modules=True,
+        ) as p:
+            with record_function("model_inference"):
+                yield
+        p.export_chrome_trace(path_save)
+
+    return simple_profiler(path_save=path_save)
 
 
 
 ######################################
 ############ DATA HELPERS ############
 ######################################
 
@@ -865,35 +871,85 @@
 def slice_along_dim(
     X: torch.Tensor, 
     dim: int, 
     idx: int
 ) -> torch.Tensor:
     """
     Slices a tensor along a specified dimension.
+    RH 2022
 
     Args:
         X (torch.Tensor): 
             Tensor to slice.
         dim (int): 
             Dimension to slice along.
         idx (int): 
             Index to slice at.
 
     Returns:
         (torch.Tensor): 
             sliced_tensor (torch.Tensor):
                 Sliced tensor.
-
-    RH 2022
     """
     slices = [slice(None)] * X.ndim
     slices[dim] = idx
     return X[tuple(slices)]
 
 
+def orthogonal_procrustes(
+    A: torch.Tensor,
+    B: torch.Tensor,
+    check_finite: bool = True,
+) -> Tuple[torch.Tensor, torch.Tensor]:
+    """
+    Port of the scipy.linalg.orthogonal_procrustes function:
+    https://github.com/scipy/scipy/blob/v1.13.0/scipy/linalg/_procrustes.py
+
+    Computes the matrix solution of the orthogonal Procrustes problem.
+    Given two matrices, A and B, find the orthogonal matrix that most closely
+    maps A to B using the algorithm in [1].
+
+    Args:
+        A (torch.Tensor): 
+            The input matrix.
+        B (torch.Tensor): 
+            The target matrix.
+        check_finite (bool): 
+            Whether to check that the input matrices contain only finite
+            numbers. Disabling may give a performance gain, but may result in
+            problems (crashes, non-termination) if the inputs do contain infinities
+            or NaNs. (Default is ``True``)
+
+    Returns:
+        (Tuple[torch.Tensor, torch.Tensor]): 
+            (R, scale):
+                R (torch.Tensor):
+                    The matrix solution of the orthogonal Procrustes problem.
+                    Minimizes the Frobenius norm of ``(A @ R) - B``, subject to
+                    ``R.T @ R = I``.
+                scale (torch.Tensor):
+                    Sum of the singular values of ``A.T @ B``.
+
+    References:
+        [1] Peter H. Schonemann, "A generalized solution of the orthogonal
+        Procrustes problem", Psychometrica -- Vol. 31, No. 1, March, 1966.
+        :doi:`10.1007/BF02289451`
+    """
+    if check_finite:
+        if not torch.isfinite(A).all() or not torch.isfinite(B).all():
+            raise ValueError("Input contains non-finite values.")
+    assert A.shape == B.shape, 'Input matrices must have the same shape.'
+    assert A.ndim == 2, 'Input matrices must be 2D.'
+
+    U, S, V = torch.linalg.svd((B.T @ A).T, full_matrices=False)
+    R = U @ V
+    scale = S.sum()
+    return R, scale
+
+
 #########################################################
 ############ INTRA-MODULE HELPER FUNCTIONS ##############
 #########################################################
 
 def _convert_size(
     size: Union[int, float], 
     return_size: str = 'GB'
```

### Comparing `bnpm-0.4.4/bnpm/video.py` & `bnpm-0.5.0/bnpm/video.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/welford_moving.py` & `bnpm-0.5.0/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm/welford_moving_2D.py` & `bnpm-0.5.0/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm.egg-info/PKG-INFO` & `bnpm-0.5.0/bnpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.4.4
+Version: 0.5.0
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bnpm-0.4.4/bnpm.egg-info/SOURCES.txt` & `bnpm-0.5.0/bnpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/bnpm.egg-info/requires.txt` & `bnpm-0.5.0/bnpm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.4.4/setup.py` & `bnpm-0.5.0/setup.py`

 * *Files identical despite different names*

