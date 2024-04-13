# Comparing `tmp/classifyspectraltype-0.1.0.tar.gz` & `tmp/classifyspectraltype-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classifyspectraltype-0.1.0.tar", max compression
+gzip compressed data, was "classifyspectraltype-0.2.0.tar", max compression
```

## Comparing `classifyspectraltype-0.1.0.tar` & `classifyspectraltype-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1074 2024-04-12 06:32:08.223261 classifyspectraltype-0.1.0/LICENSE
--rw-r--r--   0        0        0     2099 2024-04-13 17:53:57.834123 classifyspectraltype-0.1.0/README.md
--rw-r--r--   0        0        0      860 2024-04-13 06:19:43.523310 classifyspectraltype-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      571 2024-04-13 18:34:19.339704 classifyspectraltype-0.1.0/src/classifyspectraltype/__init__.py
--rw-r--r--   0        0        0     1431 2024-04-13 17:53:57.834123 classifyspectraltype-0.1.0/src/classifyspectraltype/boxplot_table_function.py
--rw-r--r--   0        0        0      902 2024-04-13 06:17:01.963309 classifyspectraltype-0.1.0/src/classifyspectraltype/clean_confidence_intervals.py
--rw-r--r--   0        0        0     2230 2024-04-13 17:53:57.834123 classifyspectraltype-0.1.0/src/classifyspectraltype/fetch_exoplanet_dataset.py
--rw-r--r--   0        0        0     2044 2024-04-13 17:53:57.834123 classifyspectraltype-0.1.0/src/classifyspectraltype/split_cross_val.py
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 classifyspectraltype-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-04-12 06:32:08.223261 classifyspectraltype-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2099 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/README.md
+-rw-r--r--   0        0        0      860 2024-04-13 19:17:04.407077 classifyspectraltype-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      555 2024-04-13 19:11:32.467067 classifyspectraltype-0.2.0/src/classifyspectraltype/__init__.py
+-rw-r--r--   0        0        0     1431 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/boxplot_table_function.py
+-rw-r--r--   0        0        0      902 2024-04-13 06:17:01.963309 classifyspectraltype-0.2.0/src/classifyspectraltype/clean_confidence_intervals.py
+-rw-r--r--   0        0        0     2230 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/fetch_exoplanet_dataset.py
+-rw-r--r--   0        0        0     2044 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/split_cross_val.py
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 classifyspectraltype-0.2.0/PKG-INFO
```

### Comparing `classifyspectraltype-0.1.0/LICENSE` & `classifyspectraltype-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/README.md` & `classifyspectraltype-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/pyproject.toml` & `classifyspectraltype-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classifyspectraltype"
-version = "0.1.0"
+version = "0.2.0"
 description = "makes the analysis easier!"
 authors = ["DSCI310 Group16"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `classifyspectraltype-0.1.0/src/classifyspectraltype/__init__.py` & `classifyspectraltype-0.2.0/src/classifyspectraltype/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # these lines below make sure the package user doesn't have to import the package as 
 # `from classifyspectraltype.fetch_exoplanet_data import fetch_data` but rather 
 # `from classifyspectraltype import fetch_data etc.`
 
-from src.classifyspectraltype.boxplot_table_function import make_boxplot_and_table # ignore
-from src.classifyspectraltype.clean_confidence_intervals import clean_confidence_intervals # ignore
-from src.classifyspectraltype.fetch_exoplanet_dataset import fetch_data # ignore
-from src.classifyspectraltype.split_cross_val import split_cross_val # ignore
+from classifyspectraltype.boxplot_table_function import make_boxplot_and_table # ignore
+from classifyspectraltype.clean_confidence_intervals import clean_confidence_intervals # ignore
+from classifyspectraltype.fetch_exoplanet_dataset import fetch_data # ignore
+from classifyspectraltype.split_cross_val import split_cross_val # ignore
```

### Comparing `classifyspectraltype-0.1.0/src/classifyspectraltype/boxplot_table_function.py` & `classifyspectraltype-0.2.0/src/classifyspectraltype/boxplot_table_function.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/src/classifyspectraltype/clean_confidence_intervals.py` & `classifyspectraltype-0.2.0/src/classifyspectraltype/clean_confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/src/classifyspectraltype/fetch_exoplanet_dataset.py` & `classifyspectraltype-0.2.0/src/classifyspectraltype/fetch_exoplanet_dataset.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/src/classifyspectraltype/split_cross_val.py` & `classifyspectraltype-0.2.0/src/classifyspectraltype/split_cross_val.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.1.0/PKG-INFO` & `classifyspectraltype-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifyspectraltype
-Version: 0.1.0
+Version: 0.2.0
 Summary: makes the analysis easier!
 License: MIT
 Author: DSCI310 Group16
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

