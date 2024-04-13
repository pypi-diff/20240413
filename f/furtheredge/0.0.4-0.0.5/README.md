# Comparing `tmp/furtheredge-0.0.4.tar.gz` & `tmp/furtheredge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furtheredge-0.0.4.tar", last modified: Sat Apr 13 14:47:13 2024, max compression
+gzip compressed data, was "furtheredge-0.0.5.tar", last modified: Sat Apr 13 14:55:27 2024, max compression
```

## Comparing `furtheredge-0.0.4.tar` & `furtheredge-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:47:13.029734 furtheredge-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:47:00.000000 furtheredge-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/inputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge/modules/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/proba.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/prospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/reserve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/universal_life_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:47:00.000000 furtheredge-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:47:13.029734 furtheredge-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 14:47:00.000000 furtheredge-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/sub_modules/duration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/universal_life_module_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.050337 furtheredge-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:55:27.046337 furtheredge-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:55:12.000000 furtheredge-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/inputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge/modules/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/prospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/reserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 14:55:12.000000 furtheredge-0.0.5/furtheredge/modules/universal_life/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 14:55:13.000000 furtheredge-0.0.5/furtheredge/universal_life_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/furtheredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:55:27.000000 furtheredge-0.0.5/furtheredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-13 14:55:27.000000 furtheredge-0.0.5/furtheredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:55:27.000000 furtheredge-0.0.5/furtheredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 14:55:27.000000 furtheredge-0.0.5/furtheredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:55:27.000000 furtheredge-0.0.5/furtheredge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:55:13.000000 furtheredge-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:55:27.050337 furtheredge-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 14:55:13.000000 furtheredge-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:13.000000 furtheredge-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/tests/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:13.000000 furtheredge-0.0.5/tests/universal_life/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:27.046337 furtheredge-0.0.5/tests/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:55:13.000000 furtheredge-0.0.5/tests/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 14:55:13.000000 furtheredge-0.0.5/tests/universal_life/sub_modules/duration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 14:55:13.000000 furtheredge-0.0.5/tests/universal_life/universal_life_module_test.py
```

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/run.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/run.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/duration.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/duration.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/proba.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/proba.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/prospective.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/prospective.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/reserve.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/sub_modules/reserve.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/modules/universal_life/tools.py` & `furtheredge-0.0.5/furtheredge/modules/universal_life/tools.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/furtheredge/universal_life_module.py` & `furtheredge-0.0.5/furtheredge/universal_life_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from furtheredge.modules.universal_life.run import universal_life_module
 import pkg_resources
 
 
 def universal_life():
-    package_dir = pkg_resources.resource_filename(__name__, "")
+    package_dir = pkg_resources.resource_filename("furtheredge", "")
 
     model_points_path = package_dir + "/inputs/model_points2.csv"
     ri_rates_path = package_dir + "/inputs/ri_rates.csv"
     wop_rates_path = package_dir + "/inputs/wop_rates.csv"
     tech_assumptions_path = package_dir + "/inputs/tech_assumptions.csv"
     product_path = package_dir + "/inputs/product.csv"
```

### Comparing `furtheredge-0.0.4/furtheredge.egg-info/SOURCES.txt` & `furtheredge-0.0.5/furtheredge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/setup.py` & `furtheredge-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="furtheredge",
-    version="0.0.4",
+    version="0.0.5",
     description="""furtheredge-modules""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Novacture",
     author_email="amine.zemni@novacture.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `furtheredge-0.0.4/tests/universal_life/sub_modules/duration_test.py` & `furtheredge-0.0.5/tests/universal_life/sub_modules/duration_test.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.4/tests/universal_life/universal_life_module_test.py` & `furtheredge-0.0.5/tests/universal_life/universal_life_module_test.py`

 * *Files identical despite different names*

