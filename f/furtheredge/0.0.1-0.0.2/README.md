# Comparing `tmp/furtheredge-0.0.1.tar.gz` & `tmp/furtheredge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furtheredge-0.0.1.tar", last modified: Sat Apr 13 10:37:00 2024, max compression
+gzip compressed data, was "furtheredge-0.0.2.tar", last modified: Sat Apr 13 11:03:42 2024, max compression
```

## Comparing `furtheredge-0.0.1.tar` & `furtheredge-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:37:00.962067 furtheredge-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 10:37:00.962067 furtheredge-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 10:36:52.000000 furtheredge-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:37:00.958067 furtheredge-0.0.1/furtheredge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 10:36:52.000000 furtheredge-0.0.1/furtheredge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-13 10:36:52.000000 furtheredge-0.0.1/furtheredge/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:37:00.962067 furtheredge-0.0.1/furtheredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 10:37:00.000000 furtheredge-0.0.1/furtheredge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 10:36:52.000000 furtheredge-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:37:00.962067 furtheredge-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 10:36:52.000000 furtheredge-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 11:03:42.222175 furtheredge-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 11:03:32.000000 furtheredge-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/furtheredge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-13 11:03:32.000000 furtheredge-0.0.2/furtheredge/universal_life.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:03:42.222175 furtheredge-0.0.2/furtheredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 11:03:42.000000 furtheredge-0.0.2/furtheredge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 11:03:32.000000 furtheredge-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:03:42.222175 furtheredge-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 11:03:32.000000 furtheredge-0.0.2/setup.py
```

### Comparing `furtheredge-0.0.1/furtheredge/main.py` & `furtheredge-0.0.2/furtheredge/universal_life.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 from modules.universal_life.run import universal_life_module
 
 
-# Loading input data
 def universal_life():
     model_points = pd.read_csv("furtheredge/inputs/model_points2.csv")
     ri_rates = pd.read_csv(
         "furtheredge/inputs/ri_rates.csv", sep=";", decimal=","
     )
     wop_rates = pd.read_csv(
         "furtheredge/inputs/wop_rates.csv", sep=";", decimal=","
@@ -27,13 +26,7 @@
         ri_rates,
         wop_rates,
         product,
     )
 
     # print(result_universal_life[result_universal_life["MP_ID"] == 169])
     return result_universal_life
-
-
-# result_universal_life = universal_life()
-# result_universal_life.to_csv(
-#     "furtheredge/outputs/universal_life_output.csv", index=False
-# )
```

### Comparing `furtheredge-0.0.1/setup.py` & `furtheredge-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="furtheredge",
-    version="0.0.1",
+    version="0.0.2",
     description="""furtheredge-modules""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Novacture",
     author_email="amine.zemni@novacture.com",
     packages=find_packages(include=["furtheredge"]),
     classifiers=[
```

