# Comparing `tmp/furtheredge-0.0.2.tar.gz` & `tmp/furtheredge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furtheredge-0.0.2.tar", last modified: Sat Apr 13 11:03:42 2024, max compression
+gzip compressed data, was "furtheredge-0.0.3.tar", last modified: Sat Apr 13 14:39:03 2024, max compression
```

## Comparing `furtheredge-0.0.2.tar` & `furtheredge-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 11:03:42.222175 furtheredge-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 11:03:32.000000 furtheredge-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/furtheredge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/universal_life.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/furtheredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 11:03:32.000000 furtheredge-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:03:42.222175 furtheredge-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 11:03:32.000000 furtheredge-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.742156 furtheredge-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:39:03.742156 furtheredge-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:38:51.000000 furtheredge-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/inputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/prospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/reserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/universal_life_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.742156 furtheredge-0.0.3/furtheredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:38:51.000000 furtheredge-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:39:03.742156 furtheredge-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-13 14:38:51.000000 furtheredge-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/sub_modules/duration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/universal_life_module_test.py
```

### Comparing `furtheredge-0.0.2/furtheredge/universal_life.py` & `furtheredge-0.0.3/tests/universal_life/universal_life_module_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import pandas as pd
-from modules.universal_life.run import universal_life_module
+from pandas.testing import assert_frame_equal
+from furtheredge.modules.universal_life.run import universal_life_module
 
 
-def universal_life():
+def should_return_universal_life_product():
+    # Given
     model_points = pd.read_csv("furtheredge/inputs/model_points2.csv")
     ri_rates = pd.read_csv(
         "furtheredge/inputs/ri_rates.csv", sep=";", decimal=","
     )
     wop_rates = pd.read_csv(
         "furtheredge/inputs/wop_rates.csv", sep=";", decimal=","
     )
     tech_assumptions = pd.read_csv(
         "furtheredge/inputs/tech_assumptions.csv", sep=";", decimal=","
     )
     product = pd.read_csv(
         "furtheredge/inputs/product.csv", sep=";", decimal=","
     )
 
-    # print(f"Model points length: {len(model_points)}")
+    # expected = pd.read_csv("furtheredge/outputs/universal_life_output.csv")
+    # expected["fin_mois"] = pd.to_datetime(expected["fin_mois"])
 
+    # When
     result_universal_life = universal_life_module(
         model_points,
-        {"time_horizon": 50, "projection_date": "2023-10-31"},
+        {"time_horizon": 50, "projection_date": "2023-10-01"},
         tech_assumptions,
         ri_rates,
         wop_rates,
         product,
     )
 
-    # print(result_universal_life[result_universal_life["MP_ID"] == 169])
-    return result_universal_life
+    # Then
+    # assert_frame_equal(result_universal_life, expected)
```

### Comparing `furtheredge-0.0.2/setup.py` & `furtheredge-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,20 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="furtheredge",
-    version="0.0.2",
+    version="0.0.3",
     description="""furtheredge-modules""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Novacture",
     author_email="amine.zemni@novacture.com",
-    packages=find_packages(include=["furtheredge"]),
+    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     install_requires=required,
-    entry_points={"console_scripts": ["furtheredge = furtheredge.main:main"]},
     # url="https://github.com/Novacture/furtheredge-modules",
 )
```
