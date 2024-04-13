# Comparing `tmp/furtheredge-0.0.3.tar.gz` & `tmp/furtheredge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furtheredge-0.0.3.tar", last modified: Sat Apr 13 14:39:03 2024, max compression
+gzip compressed data, was "furtheredge-0.0.4.tar", last modified: Sat Apr 13 14:47:13 2024, max compression
```

## Comparing `furtheredge-0.0.3.tar` & `furtheredge-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.742156 furtheredge-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:39:03.742156 furtheredge-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:38:51.000000 furtheredge-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/inputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/proba.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/prospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/reserve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/modules/universal_life/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-13 14:38:51.000000 furtheredge-0.0.3/furtheredge/universal_life_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.742156 furtheredge-0.0.3/furtheredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:39:03.000000 furtheredge-0.0.3/furtheredge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:38:51.000000 furtheredge-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:39:03.742156 furtheredge-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-13 14:38:51.000000 furtheredge-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:39:03.738156 furtheredge-0.0.3/tests/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/sub_modules/duration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 14:38:51.000000 furtheredge-0.0.3/tests/universal_life/universal_life_module_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:47:13.029734 furtheredge-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:47:00.000000 furtheredge-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/inputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.025734 furtheredge-0.0.4/furtheredge/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge/modules/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/prospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/reserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/modules/universal_life/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-13 14:47:00.000000 furtheredge-0.0.4/furtheredge/universal_life_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/furtheredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 14:47:13.000000 furtheredge-0.0.4/furtheredge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 14:47:00.000000 furtheredge-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:47:13.029734 furtheredge-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 14:47:00.000000 furtheredge-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:13.029734 furtheredge-0.0.4/tests/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/sub_modules/duration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 14:47:00.000000 furtheredge-0.0.4/tests/universal_life/universal_life_module_test.py
```

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/run.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/run.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/duration.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/duration.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/proba.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/proba.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/prospective.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/prospective.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/sub_modules/reserve.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/sub_modules/reserve.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/modules/universal_life/tools.py` & `furtheredge-0.0.4/furtheredge/modules/universal_life/tools.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge/universal_life_module.py` & `furtheredge-0.0.4/furtheredge/universal_life_module.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/furtheredge.egg-info/SOURCES.txt` & `furtheredge-0.0.4/furtheredge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/setup.py` & `furtheredge-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,20 +5,21 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="furtheredge",
-    version="0.0.3",
+    version="0.0.4",
     description="""furtheredge-modules""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Novacture",
     author_email="amine.zemni@novacture.com",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     install_requires=required,
+    include_package_data=True,
     # url="https://github.com/Novacture/furtheredge-modules",
 )
```

### Comparing `furtheredge-0.0.3/tests/universal_life/sub_modules/duration_test.py` & `furtheredge-0.0.4/tests/universal_life/sub_modules/duration_test.py`

 * *Files identical despite different names*

### Comparing `furtheredge-0.0.3/tests/universal_life/universal_life_module_test.py` & `furtheredge-0.0.4/tests/universal_life/universal_life_module_test.py`

 * *Files identical despite different names*

