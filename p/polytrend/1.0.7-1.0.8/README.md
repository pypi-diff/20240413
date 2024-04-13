# Comparing `tmp/polytrend-1.0.7.tar.gz` & `tmp/polytrend-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.7.tar", last modified: Sat Apr 13 10:55:03 2024, max compression
+gzip compressed data, was "polytrend-1.0.8.tar", last modified: Sat Apr 13 11:17:56 2024, max compression
```

## Comparing `polytrend-1.0.7.tar` & `polytrend-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.7/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 10:55:03.470687 polytrend-1.0.7/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.7/README.md
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      963 2024-04-13 10:54:26.000000 polytrend-1.0.7/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-13 10:55:03.470687 polytrend-1.0.7/setup.cfg
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:08:44.000000 polytrend-1.0.7/setup.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/polytrend/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      780 2024-04-13 10:52:00.000000 polytrend-1.0.7/src/polytrend/__init__.py
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.7/src/polytrend/polytrend.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 10:55:03.470687 polytrend-1.0.7/src/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      278 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      141 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/requires.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-13 10:55:03.000000 polytrend-1.0.7/src/polytrend.egg-info/top_level.txt
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 11:17:56.889867 polytrend-1.0.8/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.8/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 11:17:56.879867 polytrend-1.0.8/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.8/README.md
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      963 2024-04-13 11:17:48.000000 polytrend-1.0.8/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-13 11:17:56.889867 polytrend-1.0.8/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:08:44.000000 polytrend-1.0.8/setup.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 11:17:56.879867 polytrend-1.0.8/src/
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 11:17:56.879867 polytrend-1.0.8/src/polytrend/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3000 2024-04-13 11:16:58.000000 polytrend-1.0.8/src/polytrend/__init__.py
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.8/src/polytrend/polytrend.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-13 11:17:56.879867 polytrend-1.0.8/src/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-13 11:17:56.000000 polytrend-1.0.8/src/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      278 2024-04-13 11:17:56.000000 polytrend-1.0.8/src/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-13 11:17:56.000000 polytrend-1.0.8/src/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      141 2024-04-13 11:17:56.000000 polytrend-1.0.8/src/polytrend.egg-info/requires.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-13 11:17:56.000000 polytrend-1.0.8/src/polytrend.egg-info/top_level.txt
```

### Comparing `polytrend-1.0.7/LICENSE` & `polytrend-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.7/PKG-INFO` & `polytrend-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.7
+Version: 1.0.8
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `polytrend-1.0.7/README.md` & `polytrend-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.7/pyproject.toml` & `polytrend-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polytrend"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Emmanuel Asiimwe", email="asiimwemmanuel47@gmail.com" },
 ]
 description = "PolyTrend is a regression tool that fits polynomial curves to noisy data."
 readme = "README.md"
 requires-python = ">= 3.11.8"
 dependencies = [
```

### Comparing `polytrend-1.0.7/src/polytrend/polytrend.py` & `polytrend-1.0.8/src/polytrend/polytrend.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.7/src/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.8/src/polytrend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.7
+Version: 1.0.8
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

