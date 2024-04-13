# Comparing `tmp/petrovisor-0.1.2.tar.gz` & `tmp/petrovisor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrovisor-0.1.2.tar", last modified: Thu Feb 15 00:53:49 2024, max compression
+gzip compressed data, was "petrovisor-0.1.3.tar", last modified: Sat Apr 13 05:33:43 2024, max compression
```

## Comparing `petrovisor-0.1.2.tar` & `petrovisor-0.1.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.668668 petrovisor-0.1.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-02-15 00:53:36.000000 petrovisor-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-02-15 00:53:49.668668 petrovisor-0.1.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-02-15 00:53:36.000000 petrovisor-0.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-02-15 00:53:36.000000 petrovisor-0.1.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-02-15 00:53:49.668668 petrovisor-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-02-15 00:53:36.000000 petrovisor-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.660668 petrovisor-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.660668 petrovisor-0.1.2/src/petrovisor/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.664668 petrovisor-0.1.2/src/petrovisor/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17667 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.664668 petrovisor-0.1.2/src/petrovisor/api/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/increments.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/internal_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/items.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/dtypes/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.664668 petrovisor-0.1.2/src/petrovisor/api/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/data_grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    46016 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/pivot_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/psharp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15689 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/reference_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)    27560 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/methods/workspace_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.668668 petrovisor-0.1.2/src/petrovisor/api/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/protocols/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.668668 petrovisor-0.1.2/src/petrovisor/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/utils/datastructs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/utils/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    15517 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/api/utils/requests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2860 2024-02-15 00:53:36.000000 petrovisor-0.1.2/src/petrovisor/petrovisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.668668 petrovisor-0.1.2/src/petrovisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-02-15 00:53:49.000000 petrovisor-0.1.2/src/petrovisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-15 00:53:49.000000 petrovisor-0.1.2/src/petrovisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 00:53:49.000000 petrovisor-0.1.2/src/petrovisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 00:53:49.000000 petrovisor-0.1.2/src/petrovisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-15 00:53:49.000000 petrovisor-0.1.2/src/petrovisor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:53:49.668668 petrovisor-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-15 00:53:36.000000 petrovisor-0.1.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-15 00:53:36.000000 petrovisor-0.1.2/tests/test_entities_and_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-15 00:53:36.000000 petrovisor-0.1.2/tests/test_reference_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-13 05:33:38.000000 petrovisor-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-13 05:33:43.569536 petrovisor-0.1.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3311 2024-04-13 05:33:38.000000 petrovisor-0.1.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-13 05:33:38.000000 petrovisor-0.1.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-04-13 05:33:43.573536 petrovisor-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       91 2024-04-13 05:33:38.000000 petrovisor-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.561536 petrovisor-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18461 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.565536 petrovisor-0.1.3/src/petrovisor/api/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/increments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/internal_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/dtypes/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/data_grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48356 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/pivot_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/psharp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/reference_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63537 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/methods/workspace_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/protocols/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/datastructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/api/utils/requests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2637 2024-04-13 05:33:38.000000 petrovisor-0.1.3/src/petrovisor/petrovisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/src/petrovisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 05:33:43.000000 petrovisor-0.1.3/src/petrovisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:33:43.569536 petrovisor-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_entities_and_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-13 05:33:38.000000 petrovisor-0.1.3/tests/test_reference_tables.py
```

### Comparing `petrovisor-0.1.2/LICENSE` & `petrovisor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/PKG-INFO` & `petrovisor-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.2/README.md` & `petrovisor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/pyproject.toml` & `petrovisor-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/setup.cfg` & `petrovisor-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/src/petrovisor/__init__.py` & `petrovisor-0.1.3/src/petrovisor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # api
 from petrovisor.petrovisor import PetroVisor
 
 # data types
 from petrovisor.api.dtypes.items import ItemType
 from petrovisor.api.dtypes.internal_dtypes import SignalType, RefTableColumnType
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/base.py` & `petrovisor-0.1.3/src/petrovisor/api/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -100,24 +100,26 @@
     @property
     def InfoItemRoutes(self):
         """
         Routes to items with custom info
         """
         return self.__info_item_routes
 
-    def __init__(self,
-                 workspace: Optional[str] = '',
-                 api: Optional[str] = '',
-                 token: Optional[str] = '',
-                 discovery_url: Optional[str] = '',
-                 key: Optional[str] = '',
-                 username: Optional[str] = '',
-                 password: Optional[str] = '',
-                 errors: Optional[str] = 'coerce',
-                 **kwargs):
+    def __init__(
+        self,
+        workspace: Optional[str] = "",
+        api: Optional[str] = "",
+        token: Optional[str] = "",
+        discovery_url: Optional[str] = "",
+        key: Optional[str] = "",
+        username: Optional[str] = "",
+        password: Optional[str] = "",
+        errors: Optional[str] = "coerce",
+        **kwargs,
+    ):
         """
         Parameters
         ----------
         workspace : str, default None
             Workspace name
         api : str, default None
             Web api endpoint
@@ -136,81 +138,97 @@
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
         """
         # workspace
         self.__workspace = workspace
 
         # route
-        self.__route = 'PetroVisor/API/'
+        self.__route = "PetroVisor/API/"
 
         # api and token
         if api and token:
             # api endpoint
             self.__api = api
             # access token
             self.__access_token = token
-            self.__refresh_token = ''
-            self.__key = ''
-            self.__discovery_url = ''
-            self.__token_endpoint = ''
+            self.__refresh_token = ""
+            self.__key = ""
+            self.__discovery_url = ""
+            self.__token_endpoint = ""
         else:
             # discovery url (identity service)
             if not discovery_url:
                 default_discovery_url = ApiHelper.get_discovery_urls()
                 urls = [f"'{url}'" for url in default_discovery_url]
                 msg = f"Use one of the discovery urls: {urls}"
-                raise ValueError(f"PetroVisor::__init__(): "
-                                 f"'discovery_url' is undefined! {msg}")
+                raise ValueError(
+                    f"PetroVisor::__init__(): 'discovery_url' is undefined! {msg}"
+                )
             self.__discovery_url = discovery_url
 
             # api endpoint
-            self.__api = api if api else RequestsMixin.get_web_api_endpoint(discovery_url)
+            self.__api = (
+                api if api else RequestsMixin.get_web_api_endpoint(discovery_url)
+            )
 
             # access token
             if token:
                 self.__access_token = token
-                self.__refresh_token = ''
-                self.__key = ''
-                self.__token_endpoint = ''
+                self.__refresh_token = ""
+                self.__key = ""
+                self.__token_endpoint = ""
             else:
                 # get key
                 if not key:
-                    key = RequestsMixin.generate_credentials_key(username=username, password=password)
+                    key = RequestsMixin.generate_credentials_key(
+                        username=username, password=password
+                    )
                 # get access token
                 if not key:
-                    raise ValueError("PetroVisor::__init__(): "
-                                     "neither 'token', nor 'key', "
-                                     "nor 'username' and 'password' are defined!")
-                access_response = ApiLogin.get_access_token(key=key, discovery_url=discovery_url)
-                self.__access_token = access_response['access_token']
-                self.__refresh_token = access_response['refresh_token'] if ('refresh_token' in access_response) else ''
+                    raise ValueError(
+                        "PetroVisor::__init__(): "
+                        "neither 'token', nor 'key', "
+                        "nor 'username' and 'password' are defined!"
+                    )
+                access_response = ApiLogin.get_access_token(
+                    key=key, discovery_url=discovery_url
+                )
+                self.__access_token = access_response["access_token"]
+                self.__refresh_token = (
+                    access_response["refresh_token"]
+                    if ("refresh_token" in access_response)
+                    else ""
+                )
                 self.__key = key
                 self.__token_endpoint = RequestsMixin.get_token_endpoint(discovery_url)
 
         # 'NamedItem' routes
         self.__item_routes = ItemsMixinHelper.get_item_routes()
         # 'PetroVisorItem' routes
         self.__petrovisor_item_routes = ItemsMixinHelper.get_petrovisor_item_routes()
         # 'InfoItem' routes
         self.__info_item_routes = ItemsMixinHelper.get_info_item_routes()
 
         # errors handling
-        error_handling_types = ['raise', 'coerce', 'ignore']
-        self.__errors = errors if errors in error_handling_types else 'coerce'
+        error_handling_types = ["raise", "coerce", "ignore"]
+        self.__errors = errors if errors in error_handling_types else "coerce"
 
         super().__init__(**kwargs)
 
     # 'GET' request
-    def get(self,
-            rqst: str, data: Optional[Any] = None,
-            query: Optional[Any] = None,
-            files: Optional[Any] = None,
-            format: Optional[str] = 'json',
-            errors: Optional[str] = None,
-            **kwargs) -> Any:
+    def get(
+        self,
+        rqst: str,
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        format: Optional[str] = "json",
+        errors: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Get request
 
         Parameters
         ----------
         rqst : str
             Request
@@ -224,37 +242,64 @@
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         errors : str | None, default None
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
             If None, then the 'errors' parameter defined in api session constructor is used.
         """
-        response = ApiRequests.get(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                   files=files, format=format, route=self.Route, token=self.Token,
-                                   refresh_token=self.RefreshToken, key=self.Key,
-                                   discovery_url=self.DiscoveryUrl,
-                                   errors=errors or self.__errors, **kwargs)
-        if ApiHelper.has_field(response, 'status_code') and response.status_code == requests.codes.unauthorized:
+        response = ApiRequests.get(
+            self.Api,
+            rqst,
+            workspace=self.Workspace,
+            data=data,
+            query=query,
+            files=files,
+            format=format,
+            route=self.Route,
+            token=self.Token,
+            refresh_token=self.RefreshToken,
+            key=self.Key,
+            discovery_url=self.DiscoveryUrl,
+            errors=errors or self.__errors,
+            **kwargs,
+        )
+        if (
+            ApiHelper.has_field(response, "status_code")
+            and response.status_code == requests.codes.unauthorized
+        ):
             self.__reset_token(**kwargs)
-            response = ApiRequests.get(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                       files=files, format=format, route=self.Route, token=self.Token,
-                                       refresh_token=self.RefreshToken, key=self.Key,
-                                       discovery_url=self.DiscoveryUrl,
-                                       errors=errors or self.__errors, **kwargs)
+            response = ApiRequests.get(
+                self.Api,
+                rqst,
+                workspace=self.Workspace,
+                data=data,
+                query=query,
+                files=files,
+                format=format,
+                route=self.Route,
+                token=self.Token,
+                refresh_token=self.RefreshToken,
+                key=self.Key,
+                discovery_url=self.DiscoveryUrl,
+                errors=errors or self.__errors,
+                **kwargs,
+            )
         return response
 
     # 'POST' request
-    def post(self,
-             rqst: str,
-             data: Optional[Any] = None,
-             query: Optional[Any] = None,
-             files: Optional[Any] = None,
-             format: str = 'json',
-             errors: Optional[str] = None,
-             **kwargs) -> Any:
+    def post(
+        self,
+        rqst: str,
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        format: str = "json",
+        errors: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Post request
 
         Parameters
         ----------
         rqst : str
             Request
@@ -268,37 +313,64 @@
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         errors : str, default None
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
             If None, then the 'errors' parameter defined in api session constructor is used.
         """
-        response = ApiRequests.post(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                    files=files, format=format, route=self.Route, token=self.Token,
-                                    refresh_token=self.RefreshToken, key=self.Key,
-                                    discovery_url=self.DiscoveryUrl,
-                                    errors=errors or self.__errors, **kwargs)
-        if ApiHelper.has_field(response, 'status_code') and response.status_code == requests.codes.unauthorized:
+        response = ApiRequests.post(
+            self.Api,
+            rqst,
+            workspace=self.Workspace,
+            data=data,
+            query=query,
+            files=files,
+            format=format,
+            route=self.Route,
+            token=self.Token,
+            refresh_token=self.RefreshToken,
+            key=self.Key,
+            discovery_url=self.DiscoveryUrl,
+            errors=errors or self.__errors,
+            **kwargs,
+        )
+        if (
+            ApiHelper.has_field(response, "status_code")
+            and response.status_code == requests.codes.unauthorized
+        ):
             self.__reset_token(**kwargs)
-            response = ApiRequests.post(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                        files=files, format=format, route=self.Route, token=self.Token,
-                                        refresh_token=self.RefreshToken, key=self.Key,
-                                        discovery_url=self.DiscoveryUrl,
-                                        errors=errors or self.__errors, **kwargs)
+            response = ApiRequests.post(
+                self.Api,
+                rqst,
+                workspace=self.Workspace,
+                data=data,
+                query=query,
+                files=files,
+                format=format,
+                route=self.Route,
+                token=self.Token,
+                refresh_token=self.RefreshToken,
+                key=self.Key,
+                discovery_url=self.DiscoveryUrl,
+                errors=errors or self.__errors,
+                **kwargs,
+            )
         return response
 
     # 'PUT' request
-    def put(self,
-            rqst: str,
-            data: Optional[Any] = None,
-            query: Optional[Any] = None,
-            files: Optional[Any] = None,
-            format: str = 'json',
-            errors: Optional[str] = None,
-            **kwargs) -> Any:
+    def put(
+        self,
+        rqst: str,
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        format: str = "json",
+        errors: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Put request
 
         Parameters
         ----------
         rqst : str
             Request
@@ -312,37 +384,64 @@
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         errors : str, default None
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
             If None, then the 'errors' parameter defined in api session constructor is used.
         """
-        response = ApiRequests.put(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                   files=files, format=format, route=self.Route, token=self.Token,
-                                   refresh_token=self.RefreshToken, key=self.Key,
-                                   discovery_url=self.DiscoveryUrl,
-                                   errors=errors or self.__errors, **kwargs)
-        if ApiHelper.has_field(response, 'status_code') and response.status_code == requests.codes.unauthorized:
+        response = ApiRequests.put(
+            self.Api,
+            rqst,
+            workspace=self.Workspace,
+            data=data,
+            query=query,
+            files=files,
+            format=format,
+            route=self.Route,
+            token=self.Token,
+            refresh_token=self.RefreshToken,
+            key=self.Key,
+            discovery_url=self.DiscoveryUrl,
+            errors=errors or self.__errors,
+            **kwargs,
+        )
+        if (
+            ApiHelper.has_field(response, "status_code")
+            and response.status_code == requests.codes.unauthorized
+        ):
             self.__reset_token(**kwargs)
-            response = ApiRequests.put(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                       files=files, format=format, route=self.Route, token=self.Token,
-                                       refresh_token=self.RefreshToken, key=self.Key,
-                                       discovery_url=self.DiscoveryUrl,
-                                       errors=errors or self.__errors, **kwargs)
+            response = ApiRequests.put(
+                self.Api,
+                rqst,
+                workspace=self.Workspace,
+                data=data,
+                query=query,
+                files=files,
+                format=format,
+                route=self.Route,
+                token=self.Token,
+                refresh_token=self.RefreshToken,
+                key=self.Key,
+                discovery_url=self.DiscoveryUrl,
+                errors=errors or self.__errors,
+                **kwargs,
+            )
         return response
 
     # 'DELETE' request
-    def delete(self,
-               rqst: str,
-               data: Optional[Any] = None,
-               query: Optional[Any] = None,
-               files: Optional[Any] = None,
-               format: str = 'json',
-               errors: Optional[str] = None,
-               **kwargs) -> Any:
+    def delete(
+        self,
+        rqst: str,
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        format: str = "json",
+        errors: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Delete request
 
         Parameters
         ----------
         rqst : str
             Request
@@ -356,68 +455,102 @@
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         errors : str, default None
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
             If None, then the 'errors' parameter defined in api session constructor is used.
         """
-        response = ApiRequests.delete(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                      files=files, format=format, route=self.Route, token=self.Token,
-                                      refresh_token=self.RefreshToken, key=self.Key,
-                                      discovery_url=self.DiscoveryUrl,
-                                      errors=errors or self.__errors, **kwargs)
-        if ApiHelper.has_field(response, 'status_code') and response.status_code == requests.codes.unauthorized:
+        response = ApiRequests.delete(
+            self.Api,
+            rqst,
+            workspace=self.Workspace,
+            data=data,
+            query=query,
+            files=files,
+            format=format,
+            route=self.Route,
+            token=self.Token,
+            refresh_token=self.RefreshToken,
+            key=self.Key,
+            discovery_url=self.DiscoveryUrl,
+            errors=errors or self.__errors,
+            **kwargs,
+        )
+        if (
+            ApiHelper.has_field(response, "status_code")
+            and response.status_code == requests.codes.unauthorized
+        ):
             self.__reset_token(**kwargs)
-            response = ApiRequests.delete(self.Api, rqst, workspace=self.Workspace, data=data, query=query,
-                                          files=files, format=format, route=self.Route, token=self.Token,
-                                          refresh_token=self.RefreshToken, key=self.Key,
-                                          discovery_url=self.DiscoveryUrl,
-                                          errors=errors or self.__errors, **kwargs)
+            response = ApiRequests.delete(
+                self.Api,
+                rqst,
+                workspace=self.Workspace,
+                data=data,
+                query=query,
+                files=files,
+                format=format,
+                route=self.Route,
+                token=self.Token,
+                refresh_token=self.RefreshToken,
+                key=self.Key,
+                discovery_url=self.DiscoveryUrl,
+                errors=errors or self.__errors,
+                **kwargs,
+            )
         return response
 
     # encode url component
     @staticmethod
-    def encode(url_component: str, safe: Union[str, bytes] = '~', **kwargs: Any) -> str:
+    def encode(url_component: str, safe: Union[str, bytes] = "~", **kwargs: Any) -> str:
         """
         Encode url component
 
         Parameters
         ----------
         url_component : str
             URL component
         safe : str
             Safe symbols which do not need to be encoded
         """
         return ApiRequests.encode(url_component, safe=safe, **kwargs)
 
     # generate credentials key
     @staticmethod
-    def generate_credentials_key(username: Optional[str] = '', password: Optional[str] = '') -> str:
+    def generate_credentials_key(
+        username: Optional[str] = "", password: Optional[str] = ""
+    ) -> str:
         """
         Generate credentials key from username  and password.
         If either of username or password is not provided, the dialog is launched
 
         Parameters
         ----------
         username : str, default empty str
             Username
         password : str, default empty str
             Password
         """
         if username and password:
-            return ApiLogin.generate_credentials_key(username=username, password=password)
+            return ApiLogin.generate_credentials_key(
+                username=username, password=password
+            )
         else:
             from getpass import getpass
+
             if username:
-                return ApiLogin.generate_credentials_key(username=username,
-                                                         password=getpass(prompt='Password: '))
+                return ApiLogin.generate_credentials_key(
+                    username=username, password=getpass(prompt="Password: ")
+                )
             elif password:
-                return ApiLogin.generate_credentials_key(username=input('Username: '), password=password)
-            return ApiLogin.generate_credentials_key(username=input('Username: '),
-                                                     password=getpass(prompt='Password: '))
+                return ApiLogin.generate_credentials_key(
+                    username=input("Username: "), password=password
+                )
+            return ApiLogin.generate_credentials_key(
+                username=input("Username: "), password=getpass(prompt="Password: ")
+            )
 
     # get web api endpoint
     @staticmethod
     def get_web_api_endpoint(discovery_url: str) -> str:
         """
         Get web api endpoint
 
@@ -468,9 +601,15 @@
         return ApiHelper.remove_from_dict(d, keys, **kwargs)
 
     # reset token
     def __reset_token(self, **kwargs) -> Any:
         """
         Reset token
         """
-        access_response = ApiLogin.get_access_token(key=self.Key, discovery_url=self.DiscoveryUrl, **kwargs)
-        self.__access_token = access_response['access_token'] if ('access_token' in access_response) else ''
+        access_response = ApiLogin.get_access_token(
+            key=self.Key, discovery_url=self.DiscoveryUrl, **kwargs
+        )
+        self.__access_token = (
+            access_response["access_token"]
+            if ("access_token" in access_response)
+            else ""
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/dtypes/data_grids.py` & `petrovisor-0.1.3/src/petrovisor/api/dtypes/data_grids.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 # DataGrid types
 class DataGridType(IntEnum):
     """
     DataGrid types
     """
+
     # Unknown (custom)
     Unknown = 0
     # One Polygon (no data)
     Polygon = auto()
     # Several polygons (no data)
     Polygons = auto()
     # Geo data grid (ZMap like)
@@ -26,14 +27,15 @@
 
 
 # PointSet types
 class PointSetType(IntEnum):
     """
     PointSet types
     """
+
     # Unknown (custom)
     Unknown = 0
     # Single point
     Point = auto()
     # Multipoint(set of points)
     MultiPoint = auto()
     # Two connected points
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/dtypes/increments.py` & `petrovisor-0.1.3/src/petrovisor/api/dtypes/increments.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 # Time increment for aggregation
 class TimeIncrement(IntEnum):
     """
     PetroVisor time increments
     """
+
     # Every second
     EverySecond = auto()
     # Every minute
     EveryMinute = auto()
     # Every five minute
     EveryFiveMinutes = auto()
     # Every fifteen minute
@@ -30,14 +31,15 @@
 
 
 # Depth increment for aggregation
 class DepthIncrement(IntEnum):
     """
     PetroVisor depth increments
     """
+
     # 0.1 m (Every tenth of meter)
     TenthMeter = 0
     # 0.125 m (Every eighth of meter)
     EighthMeter = 1
     # 0.1524 m (Every half of foot)
     HalfFoot = 2
     # 0.3048 m (Every foot)
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/dtypes/internal_dtypes.py` & `petrovisor-0.1.3/src/petrovisor/api/dtypes/internal_dtypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 
 # Signal types
 class SignalType(IntEnum):
     """
     PetroVisor signal types
     """
+
     # Static signal type specifies signals which value is a numeric constant over a time or depth
     Static = 0
     # Time-dependent type specifies signals which are functions of time
     TimeDependent = 1
     # Depth-dependent type specifies signals which are functions of depth
     DepthDependent = 2
     # String signal type specifies signals which value is a string constant over a time or depth
     String = 3
     # PVT signal type specifies signals which are functions of pressure and temperature
     PVT = 4
     # String time-dependent signal type specifies signals which value is a string constant over a time or depth
     StringTimeDependent = 5
+    # Signals which have a series of depth-based string values
+    StringDepthDependent = 6
 
 
 # Reference table column type
 class RefTableColumnType(Enum):
-    Numeric = 0,
-    String = 1,
-    DateTime = 2,
-    Bool = 3,
+    Numeric = (0,)
+    String = (1,)
+    DateTime = (2,)
+    Bool = (3,)
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/dtypes/ml.py` & `petrovisor-0.1.3/src/petrovisor/api/dtypes/ml.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/data_grids.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/data_grids.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,70 +13,67 @@
 # DataGrid API calls
 class DataGridsMixin(SupportsItemRequests, SupportsRequests):
     """
     DataGrid API calls
     """
 
     # import data grids according to specified filter
-    def import_data_grids(self,
-                          file_filter: Optional[str] = '',
-                          file_extension: Optional[str] = '',
-                          default_crs: Optional[str] = 'EPSG:3857',
-                          **kwargs) -> List[str]:
+    def import_data_grids(
+        self,
+        file_filter: Optional[str] = "",
+        file_extension: Optional[str] = "",
+        default_crs: Optional[str] = "EPSG:3857",
+        **kwargs,
+    ) -> List[str]:
         """
         Import DataGrid according to specified filter
 
         Parameters
         ----------
         file_extension : str, default None
             File extension
         file_filter : str, default None
             File filter
         default_crs : str, default 'EPSG:3857'
             Coordinate Reference System (CRS)
         """
-        route = 'DataGrids'
+        route = "DataGrids"
         options = {
-            'Extension': file_extension,
-            'Filter': file_filter,
-            'DefaultCRS': default_crs
+            "Extension": file_extension,
+            "Filter": file_filter,
+            "DefaultCRS": default_crs,
         }
-        return self.get(f'{route}/Import', query=options)
+        return self.get(f"{route}/Import", query=options)
 
     # update DataGrid's CRS
     def update_data_grid_crs(self, name: str, crs: str, **kwargs) -> Any:
         """
         Set DataGrid's CRS
 
         Parameters
         ----------
         name : str
             DataGrid name
         crs : str
             Coordinate Reference System (CRS)
         """
-        route = 'DataGrids'
-        options = {
-            'CRS': crs
-        }
-        return self.post(f'{route}/{self.encode(name)}/CRS', query=options)
+        route = "DataGrids"
+        options = {"CRS": crs}
+        return self.post(f"{route}/{self.encode(name)}/CRS", query=options)
 
     # project DataGrid to specified CRS
-    def project_data_grid_to_crs(self,
-                                 name: str,
-                                 crs: str = '+proj=longlat +datum=WGS84 +no_defs',
-                                 **kwargs) -> Any:
+    def project_data_grid_to_crs(
+        self, name: str, crs: str = "+proj=longlat +datum=WGS84 +no_defs", **kwargs
+    ) -> Any:
         """
         Project DataGrid to specified CRS
 
         Parameters
         ----------
         name : str
             DataGrid name
         crs : str, default '+proj=longlat +datum=WGS84 +no_defs'
             Coordinate Reference System (CRS)
         """
-        route = 'DataGrids'
-        options = {
-            'CRS': crs
-        }
-        return self.get(f'{route}/{self.encode(name)}/Project', query=options)
+        route = "DataGrids"
+        options = {"CRS": crs}
+        return self.get(f"{route}/{self.encode(name)}/Project", query=options)
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/dataframes.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/dataframes.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,65 +20,74 @@
     SupportsSignalsRequests,
     SupportsEntitiesRequests,
     SupportsDataFrames,
 )
 
 
 # DataFrames utilities
-class DataFrameMixin(SupportsDataFrames, SupportsSignalsRequests, SupportsEntitiesRequests, SupportsRequests):
+class DataFrameMixin(
+    SupportsDataFrames,
+    SupportsSignalsRequests,
+    SupportsEntitiesRequests,
+    SupportsRequests,
+):
     """
     DataFrames Utilities
     """
 
     # convert dataframe to file-like object
-    def convert_dataframe_to_file_object(self,
-                                         df: pd.DataFrame,
-                                         file_name: str,
-                                         date_format: Optional[str] = None,
-                                         **kwargs) -> io.BytesIO:
+    def convert_dataframe_to_file_object(
+        self,
+        df: pd.DataFrame,
+        file_name: str,
+        date_format: Optional[str] = None,
+        **kwargs,
+    ) -> io.BytesIO:
         """
         Convert dataframe to file-like object
 
         Parameters
         ----------
         df : DataFrame
             DataFrame
         file_name : str
             File name
         date_format : str, default None
             Date format
         """
         with io.BytesIO() as file_obj:
             file_obj.name = file_name
-            if file_name.lower().endswith('.csv'):
+            if file_name.lower().endswith(".csv"):
                 if date_format:
-                    df.to_csv(file_obj,
-                              header=True,
-                              index=False,
-                              encoding='utf-8',
-                              mode='wb',
-                              date_format='%Y-%m-%dT%H:%M:%S.%fZ')
+                    df.to_csv(
+                        file_obj,
+                        header=True,
+                        index=False,
+                        encoding="utf-8",
+                        mode="wb",
+                        date_format="%Y-%m-%dT%H:%M:%S.%fZ",
+                    )
                 else:
-                    df.to_csv(file_obj,
-                              header=True,
-                              index=True,
-                              encoding='utf-8',
-                              mode='wb')
+                    df.to_csv(
+                        file_obj, header=True, index=True, encoding="utf-8", mode="wb"
+                    )
                 file_obj.seek(0)
-            elif file_name.lower().endswith('.xlsx'):
-                excel_writer = pd.ExcelWriter(file_obj, engine='openpyxl')
-                df.to_excel(excel_writer, header=True, index=True, encoding='utf-8')
+            elif file_name.lower().endswith(".xlsx"):
+                excel_writer = pd.ExcelWriter(file_obj, engine="openpyxl")
+                df.to_excel(excel_writer, header=True, index=True, encoding="utf-8")
                 excel_writer.save()
                 file_obj.seek(0)
             else:
                 file_obj.close()
             return file_obj
 
     # convert PivotTable to DataFrame
-    def convert_pivot_table_to_dataframe(self, data: List, groupby_entity: bool = False, **kwargs):
+    def convert_pivot_table_to_dataframe(
+        self, data: List, groupby_entity: bool = False, **kwargs
+    ):
         """
         Convert PivotTable to DataFrame
 
         Parameters
         ----------
         data : list
             PivotTable data
@@ -94,43 +103,47 @@
                 else:
                     df = pd.DataFrame(columns=cols)
             else:
                 df = pd.DataFrame()
 
             # assign column types
             columns = df.columns
-            columns_dtype = {col: 'Numeric' for col in columns}
+            columns_dtype = {col: "Numeric" for col in columns}
             entity_col = self.get_entity_column_name(**kwargs)
             entity_type_col = self.get_entity_type_column_name(**kwargs)
             alias_col = self.get_alias_column_name(**kwargs)
             is_opportunity_col = self.get_opportunity_column_name(**kwargs)
             date_col = self.get_date_column_name(**kwargs)
             time_col = self.get_time_column_name(**kwargs)
             for col in [date_col, time_col]:
-                columns_dtype[col] = 'Time'
+                columns_dtype[col] = "Time"
             for col in [entity_col, alias_col, entity_type_col]:
-                columns_dtype[col] = 'String'
-            columns_dtype[is_opportunity_col] = 'Bool'
+                columns_dtype[col] = "String"
+            columns_dtype[is_opportunity_col] = "Bool"
             df = self.assign_dataframe_column_types(df, columns_dtype, **kwargs)
 
             # group by entity
             if groupby_entity:
                 df = {e: df_group for e, df_group in df.groupby(entity_col)}
         except BaseException:
-            raise RuntimeError("PetroVisor::convert_pivot_table_to_dataframe(): "
-                               "couldn't convert PivotTable to DataFrame")
+            raise RuntimeError(
+                "PetroVisor::convert_pivot_table_to_dataframe(): "
+                "couldn't convert PivotTable to DataFrame"
+            )
         return df
 
     # convert P# table to DataFrame
-    def convert_psharp_table_to_dataframe(self,
-                                          psharp_table: Union[Dict, List],
-                                          dropna: bool = True,
-                                          with_entity_column: bool = True,
-                                          groupby_entity: bool = False,
-                                          **kwargs) -> Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]:
+    def convert_psharp_table_to_dataframe(
+        self,
+        psharp_table: Union[Dict, List],
+        dropna: bool = True,
+        with_entity_column: bool = True,
+        groupby_entity: bool = False,
+        **kwargs,
+    ) -> Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]:
         """
         Convert P# table to DataFrame
 
         Parameters
         ----------
         psharp_table : dict, list
             P# table data
@@ -147,26 +160,26 @@
         # standard columns
         entity_col = self.get_entity_column_name()
         alias_col = self.get_alias_column_name()
         date_col = self.get_date_column_name()
         depth_col = self.get_depth_column_name()
         # known column types
         columns_dtype = {
-            entity_col: 'String',
-            alias_col: 'String',
-            date_col: 'Time',
-            depth_col: 'Numeric',
+            entity_col: "String",
+            alias_col: "String",
+            date_col: "Time",
+            depth_col: "Numeric",
         }
 
         # read P# table from list
         if isinstance(psharp_table, list):
             if len(psharp_table) < 2:
                 return None
 
-            columns = psharp_table[0].split('\t') if len(psharp_table) > 0 else []
+            columns = psharp_table[0].split("\t") if len(psharp_table) > 0 else []
 
             # define type of table
             has_entity_col = entity_col in columns
 
             # create DataFrame
             if has_entity_col or not groupby_entity:
                 # create DataFrame
@@ -191,74 +204,107 @@
                 # extract entity name from column names
                 col_entities = DataFrameMixinHelper.get_entities_from_columns(columns)
                 # list of all entities
                 entities = DataFrameMixinHelper.get_unique_non_empty_names(col_entities)
                 # create DataFrame
                 df = {}
                 for e in entities:
-                    e_columns = [cname for ce, cname in zip(col_entities, col_names)
-                                 if not ce or ce == e]
-                    df[e] = pd.DataFrame([cv for row in psharp_table[1:]
-                                          for cv, ce in zip(row.split('\t'), col_entities)
-                                          if not ce or ce == e],
-                                         columns=e_columns)
+                    e_columns = [
+                        cname
+                        for ce, cname in zip(col_entities, col_names)
+                        if not ce or ce == e
+                    ]
+                    df[e] = pd.DataFrame(
+                        [
+                            cv
+                            for row in psharp_table[1:]
+                            for cv, ce in zip(row.split("\t"), col_entities)
+                            if not ce or ce == e
+                        ],
+                        columns=e_columns,
+                    )
 
                 # assign column types
                 for e in entities:
-                    df[e] = self.assign_dataframe_column_types(df[e], columns_dtype, **kwargs)
-
-        elif psharp_table is not None and 'TableName' in psharp_table and 'ResultsOrder' in psharp_table:
+                    df[e] = self.assign_dataframe_column_types(
+                        df[e], columns_dtype, **kwargs
+                    )
+
+        elif (
+            psharp_table is not None
+            and "TableName" in psharp_table
+            and "ResultsOrder" in psharp_table
+        ):
             # results order
-            columns_short = psharp_table['ResultsOrder']
+            columns_short = psharp_table["ResultsOrder"]
             # create column names map from short to full name with unit
             columns_short_to_long = {col: None for col in columns_short}
 
             # get column specs
-            def get_column_specs(col: Dict[str, Any], is_not_full_spec: bool) -> Tuple[str, str, str]:
+            def get_column_specs(
+                col: Dict[str, Any], is_not_full_spec: bool
+            ) -> Tuple[str, str, str]:
                 if is_not_full_spec:
-                    centity = col['EntityName']
-                    cname = col['ResultName']
-                    cunit = col['UnitName']
+                    centity = col["EntityName"]
+                    cname = col["ResultName"]
+                    cunit = col["UnitName"]
                 else:
-                    centity = col['Entity']
-                    result = col['Result']
-                    cname = result['Name']
-                    cunit = col['Unit']
+                    centity = col["Entity"]
+                    result = col["Result"]
+                    cname = result["Name"]
+                    cunit = col["Unit"]
                     # cunit = result['Unit']['Name']
                 return centity, cname, cunit
 
             # get full column name
             def get_full_column_name(col_name: str, unit_name: str):
-                return f'{col_name} [{unit_name}]'
+                return f"{col_name} [{unit_name}]"
+
             # create DataFrame
-            data_field = 'Data'
-            value_field = 'Value'
+            data_field = "Data"
+            value_field = "Value"
             # result_field = ''
             fields = []
-            for i, table_fields in enumerate([
-                ['Columns', 'ColumnsDepth', 'ColumnsString', 'ColumnsTime', 'ColumnsBool'],
-                ['Data', 'DataDepth', 'DataString', 'DataTime', 'DataBool'],
-            ]):
+            for i, table_fields in enumerate(
+                [
+                    [
+                        "Columns",
+                        "ColumnsDepth",
+                        "ColumnsString",
+                        "ColumnsTime",
+                        "ColumnsBool",
+                    ],
+                    ["Data", "DataDepth", "DataString", "DataTime", "DataBool"],
+                ]
+            ):
                 is_not_full_spec = i == 0
-                entity_field = 'EntityName' if is_not_full_spec else 'Entity'
+                entity_field = "EntityName" if is_not_full_spec else "Entity"
                 # non-empty fields
-                fields = [field for field in table_fields if field in psharp_table and psharp_table[field]]
+                fields = [
+                    field
+                    for field in table_fields
+                    if field in psharp_table and psharp_table[field]
+                ]
                 for col_type in fields:
                     # column type
-                    col_dtype = 'Numeric'
-                    for suffix in ['String', 'Time', 'Bool']:
+                    col_dtype = "Numeric"
+                    for suffix in ["String", "Time", "Bool"]:
                         if suffix in col_type:
                             col_dtype = suffix
                             break
                     for col in psharp_table[col_type]:
                         # get column info
-                        col_entity_name, col_name, col_unit_name = get_column_specs(col, is_not_full_spec)
+                        col_entity_name, col_name, col_unit_name = get_column_specs(
+                            col, is_not_full_spec
+                        )
                         # assign column data type
                         if columns_short_to_long[col_name] is None:
-                            full_column_name = get_full_column_name(col_name, col_unit_name)
+                            full_column_name = get_full_column_name(
+                                col_name, col_unit_name
+                            )
                             columns_short_to_long[col_name] = full_column_name
                             columns_dtype[columns_short_to_long[col_name]] = col_dtype
                         else:
                             full_column_name = columns_short_to_long[col_name]
                         # change entity field to 'Entity'
                         if entity_field != entity_col:
                             col[entity_col] = col.pop(entity_field)
@@ -267,20 +313,24 @@
                             d[full_column_name] = d.pop(value_field)
                 if fields:
                     break
             if not fields:
                 return None
 
             # create DataFrame
-            df = pd.json_normalize([values for field in fields for values in psharp_table[field]]
-                                   if len(fields) > 1
-                                   else psharp_table[fields[0]],
-                                   record_path=data_field,
-                                   meta=[entity_col],
-                                   errors='ignore')
+            df = pd.json_normalize(
+                (
+                    [values for field in fields for values in psharp_table[field]]
+                    if len(fields) > 1
+                    else psharp_table[fields[0]]
+                ),
+                record_path=data_field,
+                meta=[entity_col],
+                errors="ignore",
+            )
 
             # reorder columns
             offset = 0
             reordered_columns = list(df.columns)
             # first columns 'Date', 'Depth', 'Entity'
             for col in [entity_col, depth_col, date_col]:
                 if col in reordered_columns:
@@ -301,37 +351,41 @@
 
             # assign column types
             df = self.assign_dataframe_column_types(df, columns_dtype, **kwargs)
 
             # drop NaNs
             if dropna:
                 # df = df.dropna(axis=0, how='all', inplace=False)
-                df.dropna(axis=0, how='all', inplace=True)
+                df.dropna(axis=0, how="all", inplace=True)
 
             # group by entity
             if groupby_entity:
                 df = {e: df_group for e, df_group in df.groupby(entity_col)}
             # convert to wide format with columns format "{entity_name} : {column_name"
             elif not with_entity_column:
                 df = self.convert_dataframe_from_long_to_wide(df)
         else:
-            raise ValueError("PetroVisor::convert_psharp_table_to_dataframe(): "
-                             "unknown P# table type!")
+            raise ValueError(
+                "PetroVisor::convert_psharp_table_to_dataframe(): "
+                "unknown P# table type!"
+            )
 
         return df
 
     # Get signal data from DataFrame
 
-    def get_signal_data_from_dataframe(self,
-                                       df: pd.DataFrame,
-                                       signals: Optional[Dict] = None,
-                                       only_existing_entities: bool = True,
-                                       entity_type: str = '',
-                                       entities: Optional[Dict] = None,
-                                       **kwargs) -> Dict[str, Any]:
+    def get_signal_data_from_dataframe(
+        self,
+        df: pd.DataFrame,
+        signals: Optional[Dict] = None,
+        only_existing_entities: bool = True,
+        entity_type: str = "",
+        entities: Optional[Dict] = None,
+        **kwargs,
+    ) -> Dict[str, Any]:
         """
         Get signal data from DataFrame
 
         Parameters
         ----------
         df : DataFrame
             Table
@@ -354,18 +408,25 @@
         date_col = self.get_date_column_name()
         depth_col = self.get_depth_column_name()
 
         # entities map
         entities_map = copy.deepcopy(entities) if entities else {}
 
         # filter out undefined entities
-        select_entities = self.get_entity_names(entity_type=entity_type, **kwargs) if only_existing_entities else None
+        select_entities = (
+            self.get_entity_names(entity_type=entity_type, **kwargs)
+            if only_existing_entities
+            else None
+        )
         if select_entities and entities_map:
             entities_map_rev = {v: k for k, v in entities_map.items()}
-            select_entities = [entities_map_rev[e] if (e in entities_map_rev) else e for e in select_entities]
+            select_entities = [
+                entities_map_rev[e] if (e in entities_map_rev) else e
+                for e in select_entities
+            ]
 
         # data containers
         data_to_save = {s.name: [] for s in SignalType}
 
         # collect data info
         with_entity_col = entity_col in columns
         if not with_entity_col:
@@ -373,28 +434,44 @@
             col_names = DataFrameMixinHelper.remove_entities_from_columns(columns)
             # extract entity name from column names
             col_entities = DataFrameMixinHelper.get_entities_from_columns(columns)
             # list of all entities
             entities = DataFrameMixinHelper.get_unique_non_empty_names(col_entities)
             # get column data info
             col_data = {
-                e: [(cname, cidx) for cidx, (centity, cname) in enumerate(zip(col_entities, col_names)) if centity == e]
-                for e in entities if (select_entities is None) or (e in select_entities)}
+                e: [
+                    (cname, cidx)
+                    for cidx, (centity, cname) in enumerate(
+                        zip(col_entities, col_names)
+                    )
+                    if centity == e
+                ]
+                for e in entities
+                if (select_entities is None) or (e in select_entities)
+            }
         else:
             # get column names
             col_names = columns
             # get list of entities
-            entities = list(set(df[entity_col].tolist())) if (entity_col in columns) else []
+            entities = (
+                list(set(df[entity_col].tolist())) if (entity_col in columns) else []
+            )
             # get column data info
-            col_data = {e: [(cname, cidx) for cidx, cname in enumerate(columns)]
-                        for e in entities if (select_entities is None) or (e in select_entities)}
+            col_data = {
+                e: [(cname, cidx) for cidx, cname in enumerate(columns)]
+                for e in entities
+                if (select_entities is None) or (e in select_entities)
+            }
 
         # remap entities data
         if entities_map:
-            col_data = {entities_map[e] if (e in entities_map) else e: d for e, d in col_data.items()}
+            col_data = {
+                entities_map[e] if (e in entities_map) else e: d
+                for e, d in col_data.items()
+            }
 
         # 'Date' column
         date_index = None
         for i, column_name in enumerate(col_names):
             if column_name == date_col:
                 date_index = i
                 break
@@ -403,61 +480,79 @@
         depth_index = None
         for i, column_name in enumerate(col_names):
             if column_name == depth_col:
                 depth_index = i
                 break
 
         # get signal info
-        def _get_signal_info(column_name: str, signal_names: List[str], signals: Optional[Dict] = None):
+        def _get_signal_info(
+            column_name: str, signal_names: List[str], signals: Optional[Dict] = None
+        ):
             column_name_without_unit = self.get_column_name_without_unit(column_name)
             column_unit_name = self.get_column_unit(column_name)
             if signals:
-                signal = signals[column_name] if (column_name in signals) else signals[column_name_without_unit] if (
-                            column_name_without_unit in signals) else None
+                signal = (
+                    signals[column_name]
+                    if (column_name in signals)
+                    else (
+                        signals[column_name_without_unit]
+                        if (column_name_without_unit in signals)
+                        else None
+                    )
+                )
             else:
                 signal = None
             if not signal:
                 signal_name = column_name_without_unit
                 signal_unit = column_unit_name
             elif isinstance(signal, str):
                 signal_name_without_unit = self.get_column_name_without_unit(signal)
                 signal_unit_name = self.get_column_unit(signal)
                 signal_name = signal_name_without_unit
                 signal_unit = signal_unit_name if signal_unit_name else column_unit_name
-            elif isinstance(signal, tuple) or isinstance(signal, list) and len(signal) > 0:
+            elif (
+                isinstance(signal, tuple)
+                or isinstance(signal, list)
+                and len(signal) > 0
+            ):
                 signal_name = signal[0]
                 signal_unit = signal[1] if (len(signal) > 1) else column_unit_name
             else:
                 signal_name = self.get_column_name_without_unit(column_name)
                 signal_unit = self.get_column_unit(column_name)
-                for fname in ['Signal', 'Name', 'SignalName']:
+                for fname in ["Signal", "Name", "SignalName"]:
                     if fname in signal:
                         signal_name = signal[fname]
                         break
                     elif fname.lower() in signal:
                         signal_name = signal[fname.lower()]
                         break
-                for fname in ['Unit', 'UnitName', 'SignalUnit']:
+                for fname in ["Unit", "UnitName", "SignalUnit"]:
                     if fname in signal:
                         signal_unit = signal[fname]
                         break
                     elif fname.lower() in signal:
                         signal_unit = signal[fname.lower()]
                         break
             # get signal
             if signal_name in signal_names:
                 signal_obj = self.get_signal(signal_name, **kwargs)
                 if signal_obj:
-                    if not signal_unit and 'StorageUnitName' in signal_obj:
-                        signal_unit = signal_obj['StorageUnitName']
-                    signal_type = signal_obj['SignalType'] if ('SignalType' in signal_obj) else None
+                    if not signal_unit and "StorageUnitName" in signal_obj:
+                        signal_unit = signal_obj["StorageUnitName"]
+                    signal_type = (
+                        signal_obj["SignalType"]
+                        if ("SignalType" in signal_obj)
+                        else None
+                    )
                     return {
-                        'Signal': signal_name,
-                        'Unit': signal_unit,
-                        'SignalType': signal_type}
+                        "Signal": signal_name,
+                        "Unit": signal_unit,
+                        "SignalType": signal_type,
+                    }
             return None
 
         # check whether non index column
         def _is_index_column(column_name: str) -> bool:
             return column_name in {date_col, depth_col, entity_col, alias_col}
 
         # get column data
@@ -465,80 +560,126 @@
             if not with_entity_col:
                 return df.iloc[:, column_index].to_list()
             return df[df[entity_col] == entity_name].iloc[:, column_index].to_list()
 
         # get signals
         col_names = list(set(col_names))
         existing_signal_names = self.get_signal_names(**kwargs)
-        column_signals = {cname: _get_signal_info(cname, existing_signal_names, signals=signals)
-                          for cname in col_names if not _is_index_column(cname)}
+        column_signals = {
+            cname: _get_signal_info(cname, existing_signal_names, signals=signals)
+            for cname in col_names
+            if not _is_index_column(cname)
+        }
 
         # collect signals data
         for _entity_name, d in col_data.items():
             # make sure that entity column is string
             entity_name = str(_entity_name)
             # collect signals data
             for col in d:
                 # column name
                 column_name = col[0]
                 # column index
                 column_index = col[1]
                 if column_name in column_signals and column_signals[column_name]:
 
                     signal = column_signals[column_name]
-                    signal_name = signal['Signal']
-                    signal_unit_name = signal['Unit']
-                    signal_type = signal['SignalType']
+                    signal_name = signal["Signal"]
+                    signal_unit_name = signal["Unit"]
+                    signal_type = signal["SignalType"]
 
                     # static signal
                     if signal_type in {SignalType.Static.name, SignalType.String.name}:
-                        dtype = 'Numeric' if (signal_type == 'Static') else 'String'
+                        dtype = "Numeric" if (signal_type == "Static") else "String"
                         static_data = _get_column_data(column_index, entity_name)
                         if static_data and len(static_data) > 0:
-                            value = static_data[0] if (signal_type == 'Static') else static_data[0]
-                            data_to_save[signal_type].append({
-                                'Entity': entity_name,
-                                'Signal': signal_name,
-                                'Unit': signal_unit_name,
-                                'Data': self.get_json_valid_value(value, dtype=dtype, **kwargs)
-                            })
+                            value = (
+                                static_data[0]
+                                if (signal_type == "Static")
+                                else static_data[0]
+                            )
+                            data_to_save[signal_type].append(
+                                {
+                                    "Entity": entity_name,
+                                    "Signal": signal_name,
+                                    "Unit": signal_unit_name,
+                                    "Data": self.get_json_valid_value(
+                                        value, dtype=dtype, **kwargs
+                                    ),
+                                }
+                            )
                     # time signal
-                    elif signal_type in (SignalType.TimeDependent.name, SignalType.StringTimeDependent.name):
-                        dtype = 'Numeric' if (signal_type == 'TimeDependent') else 'String'
-                        data_to_save[signal_type].append({
-                            'Entity': entity_name,
-                            'Signal': signal_name,
-                            'Unit': signal_unit_name,
-                            'Data': [{'Date': self.get_json_valid_value(dvalue, dtype='Time', **kwargs),
-                                      'Value': self.get_json_valid_value(value, dtype=dtype, **kwargs)} for
-                                     dvalue, value in zip(_get_column_data(date_index, entity_name),
-                                                          _get_column_data(column_index, entity_name))]
-                        })
+                    elif signal_type in (
+                        SignalType.TimeDependent.name,
+                        SignalType.StringTimeDependent.name,
+                    ):
+                        dtype = (
+                            "Numeric" if (signal_type == "TimeDependent") else "String"
+                        )
+                        data_to_save[signal_type].append(
+                            {
+                                "Entity": entity_name,
+                                "Signal": signal_name,
+                                "Unit": signal_unit_name,
+                                "Data": [
+                                    {
+                                        "Date": self.get_json_valid_value(
+                                            dvalue, dtype="Time", **kwargs
+                                        ),
+                                        "Value": self.get_json_valid_value(
+                                            value, dtype=dtype, **kwargs
+                                        ),
+                                    }
+                                    for dvalue, value in zip(
+                                        _get_column_data(date_index, entity_name),
+                                        _get_column_data(column_index, entity_name),
+                                    )
+                                ],
+                            }
+                        )
                     # depth signal
-                    elif signal_type == SignalType.DepthDependent.name:
-                        dtype = 'Numeric'
-                        data_to_save[signal_type].append({
-                            'Entity': entity_name,
-                            'Signal': signal_name,
-                            'Unit': signal_unit_name,
-                            'Data': [{'Depth': self.get_json_valid_value(dvalue, dtype='Numeric', **kwargs),
-                                      'Value': self.get_json_valid_value(value, dtype=dtype, **kwargs)} for
-                                     dvalue, value in zip(_get_column_data(depth_index, entity_name),
-                                                          _get_column_data(column_index, entity_name))]
-                        })
+                    elif signal_type in (
+                        SignalType.DepthDependent.name,
+                        SignalType.StringDepthDependent.name,
+                    ):
+                        dtype = (
+                            "Numeric" if (signal_type == "DepthDependent") else "String"
+                        )
+                        data_to_save[signal_type].append(
+                            {
+                                "Entity": entity_name,
+                                "Signal": signal_name,
+                                "Unit": signal_unit_name,
+                                "Data": [
+                                    {
+                                        "Depth": self.get_json_valid_value(
+                                            dvalue, dtype="Numeric", **kwargs
+                                        ),
+                                        "Value": self.get_json_valid_value(
+                                            value, dtype=dtype, **kwargs
+                                        ),
+                                    }
+                                    for dvalue, value in zip(
+                                        _get_column_data(depth_index, entity_name),
+                                        _get_column_data(column_index, entity_name),
+                                    )
+                                ],
+                            }
+                        )
                     else:
-                        raise ValueError(f"PetroVisor::get_signal_data_from_dataframe(): "
-                                         f"signal type: '{signal_type}' is not supported yet.")
+                        raise ValueError(
+                            f"PetroVisor::get_signal_data_from_dataframe(): "
+                            f"signal type: '{signal_type}' is not supported yet."
+                        )
         return data_to_save
 
     # convert dataframe from wide to long format
-    def convert_dataframe_from_wide_to_long(self,
-                                            df: pd.DataFrame,
-                                            inplace: bool = False,
-                                            **kwargs):
+    def convert_dataframe_from_wide_to_long(
+        self, df: pd.DataFrame, inplace: bool = False, **kwargs
+    ):
         """
         Convert DataFrame from wide to long format.
         Wide format assumes column names as '{entity_name} : {column_name}'
         Long format assumes that DataFrame has 'Entity' column.
 
         Parameters
         ----------
@@ -551,40 +692,41 @@
         # standard columns
         entity_col = self.get_entity_column_name()
 
         # define column indices and entities
         column_indices = []
         entity_columns = []
         for col in df.columns:
-            c = col.split(' : ')
+            c = col.split(" : ")
             if len(c) > 1:
                 entity_columns.append((c[0], c[1]))
             else:
                 column_indices.append(col)
         if not entity_columns:
             return df
 
         # set indices
-        df_long, default_index_col = \
-            DataFrameMixinHelper.set_dataframe_index(df,
-                                                     column_indices,
-                                                     inplace=inplace,
-                                                     add_default_index=True,
-                                                     **kwargs)
+        df_long, default_index_col = DataFrameMixinHelper.set_dataframe_index(
+            df, column_indices, inplace=inplace, add_default_index=True, **kwargs
+        )
         # assign new column names
-        df_long.columns = pd.MultiIndex.from_tuples(entity_columns, names=[entity_col, None])
+        df_long.columns = pd.MultiIndex.from_tuples(
+            entity_columns, names=[entity_col, None]
+        )
         # stack entity column and reset index
         return df_long.stack(0).reset_index().drop(columns=default_index_col)
 
     # convert dataframe from long to wide format
-    def convert_dataframe_from_long_to_wide(self,
-                                            df: pd.DataFrame,
-                                            indices: Optional[Union[str, List[str]]] = None,
-                                            inplace: bool = False,
-                                            **kwargs):
+    def convert_dataframe_from_long_to_wide(
+        self,
+        df: pd.DataFrame,
+        indices: Optional[Union[str, List[str]]] = None,
+        inplace: bool = False,
+        **kwargs,
+    ):
         """
         Convert DataFrame from long to wide format.
         Wide format assumes column names as '{entity_name} : {column_name}'
         Long format assumes that DataFrame has 'Entity' column.
 
         Parameters
         ----------
@@ -601,70 +743,97 @@
         if entity_col not in df.columns:
             return df
 
         # define column indices
         date_col = self.get_date_column_name()
         depth_col = self.get_depth_column_name()
         alias_col = self.get_alias_column_name()
-        column_indices = copy.deepcopy(indices) if indices else [date_col, depth_col, alias_col, entity_col]
+        column_indices = (
+            copy.deepcopy(indices)
+            if indices
+            else [date_col, depth_col, alias_col, entity_col]
+        )
         if entity_col not in column_indices:
             column_indices.append(entity_col)
 
         # set indices
-        df_wide, default_index_col = \
-            DataFrameMixinHelper.set_dataframe_index(df,
-                                                     column_indices,
-                                                     inplace=inplace,
-                                                     add_default_index=True,
-                                                     **kwargs)
+        df_wide, default_index_col = DataFrameMixinHelper.set_dataframe_index(
+            df, column_indices, inplace=inplace, add_default_index=True, **kwargs
+        )
         # unstack 'Entity' column
-        df_wide = df_wide.unstack(entity_col).reset_index().sort_index(axis=1).drop(columns=default_index_col)
+        df_wide = (
+            df_wide.unstack(entity_col)
+            .reset_index()
+            .sort_index(axis=1)
+            .drop(columns=default_index_col)
+        )
         # rename column as '{entity_name} : {column_name}'
-        df_wide.columns = [f'{c[1]} : {c[0]}' if c[1] else c[0] for c in df_wide.columns]
+        df_wide.columns = [
+            f"{c[1]} : {c[0]}" if c[1] else c[0] for c in df_wide.columns
+        ]
         return df_wide
 
     # get valid json value
-    def get_json_valid_value(self, value: Any, dtype: Union[str, SignalType] = 'unknown', **kwargs) -> Any:
+    def get_json_valid_value(
+        self, value: Any, dtype: Union[str, SignalType] = "unknown", **kwargs
+    ) -> Any:
         """
         Convert value to json accepted format
 
         Parameters
         ----------
         value : Any
             Value
         dtype : str | SignalType, default 'unknown'
             data type: 'numeric' or 'float64', 'time', 'bool' or 'boolean', 'unknown' or 'object'
         """
         is_null = pd.isnull(value)
         if not isinstance(dtype, str):
             dtype = self.get_signal_data_type_name(dtype, **kwargs)
         dtype = dtype.lower()
-        if dtype in {'numeric', 'float64'}:
+        if dtype in {"numeric", "float64"}:
             # nan_value = pd.NA
             # nan_value = np.nan
             # nan_value = float('NaN')
-            nan_value = 'NaN'
-            return nan_value if is_null or (isinstance(value, str) and not value.strip()) else value
-        elif dtype in {'time', 'datetime64[ns]'}:
-            return None if is_null or (
-                    isinstance(value, str) and not value.strip()) else self.datetime_to_string(value, **kwargs)
-        elif dtype in {'string', 'str'}:
-            return '' if is_null else value
-        elif dtype in {'bool', 'boolean'}:
-            return None if is_null or (isinstance(value, str) and not value.strip()) else value
-        elif dtype in {'unknown', 'object'}:
-            return None if is_null or (isinstance(value, str) and not value.strip()) else value
+            nan_value = "NaN"
+            return (
+                nan_value
+                if is_null or (isinstance(value, str) and not value.strip())
+                else value
+            )
+        elif dtype in {"time", "datetime64[ns]"}:
+            return (
+                None
+                if is_null or (isinstance(value, str) and not value.strip())
+                else self.datetime_to_string(value, **kwargs)
+            )
+        elif dtype in {"string", "str"}:
+            return "" if is_null else value
+        elif dtype in {"bool", "boolean"}:
+            return (
+                None
+                if is_null or (isinstance(value, str) and not value.strip())
+                else value
+            )
+        elif dtype in {"unknown", "object"}:
+            return (
+                None
+                if is_null or (isinstance(value, str) and not value.strip())
+                else value
+            )
         return None if is_null else value
 
     # assign DataFrame column to corresponding types
-    def assign_dataframe_column_types(self,
-                                      df: pd.DataFrame,
-                                      columns_dtype: Dict,
-                                      default_dtype: Optional[str] = None,
-                                      **kwargs) -> pd.DataFrame:
+    def assign_dataframe_column_types(
+        self,
+        df: pd.DataFrame,
+        columns_dtype: Dict,
+        default_dtype: Optional[str] = None,
+        **kwargs,
+    ) -> pd.DataFrame:
         """
         Convert DataFrame columns to column types
 
         Parameters
         ----------
         df : DataFrame
             Table
@@ -688,50 +857,52 @@
 
         Parameters
         ----------
         dtype : str
             data type: 'numeric' or 'float64', 'time', 'bool' or 'boolean', 'unknown' or 'object'
         """
         dtype = dtype.lower()
-        if dtype in {'numeric', 'float64'}:
-            return 'float64'
-        elif dtype in {'time', 'datetime64[ns]'}:
-            return 'datetime64[ns]'
-        elif dtype in {'string'}:
-            return 'string'
-        elif dtype in {'boolean', 'bool'}:
-            return 'bool'
-        elif dtype in {'unknown', 'object'}:
-            return 'object'
-        return 'object'
+        if dtype in {"numeric", "float64"}:
+            return "float64"
+        elif dtype in {"time", "datetime64[ns]"}:
+            return "datetime64[ns]"
+        elif dtype in {"string"}:
+            return "string"
+        elif dtype in {"boolean", "bool"}:
+            return "bool"
+        elif dtype in {"unknown", "object"}:
+            return "object"
+        return "object"
 
     # convert DataFrame column to bool
-    def column_to_dtype(self, df: pd.DataFrame, column: str, dtype: str, **kwargs) -> pd.DataFrame:
+    def column_to_dtype(
+        self, df: pd.DataFrame, column: str, dtype: str, **kwargs
+    ) -> pd.DataFrame:
         """
         Convert DataFrame column to specified type
 
         Parameters
         ----------
         df : DataFrame
             Table
         column: str
             Column name
         dtype : str
             data type: 'numeric' or 'float64', 'time', 'bool' or 'boolean', 'unknown' or 'object'
         """
         dtype = dtype.lower()
-        if dtype in {'numeric', 'float64'}:
+        if dtype in {"numeric", "float64"}:
             df[column] = self.column_to_numeric(df, column, **kwargs)
-        elif dtype in {'time', 'datetime64[ns]'}:
+        elif dtype in {"time", "datetime64[ns]"}:
             df[column] = self.column_to_datetime(df, column, **kwargs)
-        elif dtype in {'string', 'str'}:
+        elif dtype in {"string", "str"}:
             df[column] = self.column_to_string(df, column, **kwargs)
-        elif dtype in {'bool', 'boolean'}:
+        elif dtype in {"bool", "boolean"}:
             df[column] = self.column_to_bool(df, column, **kwargs)
-        elif dtype in {'unknown', 'object'}:
+        elif dtype in {"unknown", "object"}:
             df[column] = self.column_to_object(df, column, **kwargs)
         return df[column]
 
     # convert DataFrame column to 'object'
     def column_to_object(self, df: pd.DataFrame, column: str, **kwargs) -> pd.Series:
         """
         Convert DataFrame column to 'object' type
@@ -739,43 +910,43 @@
         Parameters
         ----------
         df : DataFrame
             Table
         column : str
             Column name
         """
-        return df[column].astype('object')
+        return df[column].astype("object")
 
     # convert DataFrame column to 'bool'
     def column_to_bool(self, df: pd.DataFrame, column: str, **kwargs) -> pd.Series:
         """
         Convert DataFrame column to 'bool' type
 
         Parameters
         ----------
         df : DataFrame
             Table
         column : str
             Column name
         """
-        return df[column].astype('bool')
+        return df[column].astype("bool")
 
     # convert DataFrame column to 'string'
     def column_to_string(self, df: pd.DataFrame, column: str, **kwargs) -> pd.Series:
         """
         Convert DataFrame column to 'string' type
 
         Parameters
         ----------
         df : DataFrame
             Table
         column : str
             Column name
         """
-        return df[column].astype('string')
+        return df[column].astype("string")
 
     # convert DataFrame column to 'numeric'
     def column_to_numeric(self, df: pd.DataFrame, column: str, **kwargs) -> pd.Series:
         """
         Convert DataFrame column to 'numeric' type
 
         Parameters
@@ -801,57 +972,82 @@
             Column name
         """
         # return df[column].astype('datetime64[ns]')
         # return pd.to_datetime(df[column], infer_datetime_format=False)
         # return pd.to_datetime(df[column], infer_datetime_format=True)
         # return pd.to_datetime(df[column], format=format)
         # return pd.to_datetime(df[column])
-        datetime_args = {arg: kwargs[arg] for arg in
-                         ['errors', 'dayfirst', 'yearfirst', 'utc', 'format', 'exact', 'unit', 'infer_datetime_format',
-                          'origin', 'cache'] if (arg in kwargs)}
+        datetime_args = {
+            arg: kwargs[arg]
+            for arg in [
+                "errors",
+                "dayfirst",
+                "yearfirst",
+                "utc",
+                "format",
+                "exact",
+                "unit",
+                "infer_datetime_format",
+                "origin",
+                "cache",
+            ]
+            if (arg in kwargs)
+        }
         if datetime_args:
             return pd.to_datetime(df[column], **datetime_args)
         return pd.to_datetime(df[column])
 
     # convert datetime to string
-    def datetime_to_string(self,
-                           d: Union[datetime, str],
-                           format: Optional[str] = '%Y-%m-%dT%H:%M:%S.%f',
-                           **kwargs) -> str:
+    def datetime_to_string(
+        self,
+        d: Union[datetime, str],
+        format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%f",
+        **kwargs,
+    ) -> str:
         """
         Convert datetime object to string representation
 
         Parameters
         ----------
         d : datetime
             Date
         format : str, default '%Y-%m-%dT%H:%M:%S.%f'
             Time format
         """
+
         def parse_date(date_string: str, desired_format: str) -> str:
             formats_to_try = [
-                '%Y-%m-%d',
-                '%Y-%m-%dT%H:%M:%S',
-                '%Y-%m-%dT%H:%M:%S.%f',
+                "%Y-%m-%d",
+                "%Y-%m-%dT%H:%M:%S",
+                "%Y-%m-%dT%H:%M:%S.%f",
                 # other formats might be added
             ]
             for format_str in formats_to_try:
                 try:
                     date_object = datetime.strptime(date_string, format_str)
                     return date_object.strftime(desired_format)
                 except ValueError:
                     pass
             return str(date_string).strip()
-        return '' if pd.isnull(d) else d.strftime(format) if isinstance(d, datetime) else parse_date(d, format)
+
+        return (
+            ""
+            if pd.isnull(d)
+            else (
+                d.strftime(format) if isinstance(d, datetime) else parse_date(d, format)
+            )
+        )
 
     # convert string to datetime
-    def string_to_datetime(self,
-                           d: Union[datetime, str],
-                           format: Optional[str] = '%Y-%m-%d %H:%M:%S',
-                           **kwargs) -> datetime:
+    def string_to_datetime(
+        self,
+        d: Union[datetime, str],
+        format: Optional[str] = "%Y-%m-%d %H:%M:%S",
+        **kwargs,
+    ) -> datetime:
         """
         Convert date from string representation to datetime object
 
         Parameters
         ----------
         d : str
             Date
@@ -866,32 +1062,32 @@
         Get column name without unit from column name
 
         Parameters
         ----------
         column_name : str
             Column name
         """
-        cname = column_name.split('[')[0].strip()
+        cname = column_name.split("[")[0].strip()
         return cname
 
     # get column unit
     def get_column_unit(self, column_name: str, **kwargs) -> str:
         """
         Get column unit from column name
 
         Parameters
         ----------
         column_name : str
             Column name
         """
         column_name = column_name.strip()
-        cunit = re.findall(r'\[(.*?)\]', column_name)
+        cunit = re.findall(r"\[(.*?)\]", column_name)
         if cunit and len(cunit) > 0:
             return cunit[0]
-        return ''
+        return ""
 
     # get column name and unit
     def get_column_name_and_unit(self, column_name: str, **kwargs) -> Tuple[str, str]:
         """
         Get column name and unit from column name
 
         Parameters
@@ -905,147 +1101,168 @@
         return cname, cunit
 
     # get 'Entity' column name
     def get_entity_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Entity' column name used in return tables from api calls
         """
-        return 'Entity'
+        return "Entity"
 
     # get 'Alias' column name
     def get_alias_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Alias' column name used in return tables from api calls
         """
-        return 'Alias'
+        return "Alias"
 
     # get 'EntityType' column name
     def get_entity_type_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Type' column name used in return tables from api calls
         """
-        return 'Type'
+        return "Type"
 
     # get 'Opportunity' column name
     def get_opportunity_column_name(self, **kwargs) -> str:
         """
         Get predefined 'IsOpportunity' column name used in return tables from api calls
         """
-        return 'IsOpportunity'
+        return "IsOpportunity"
 
     # get 'Date' column name
     def get_date_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Date' column name used in return tables from api calls
         """
-        return 'Date'
+        return "Date"
 
     # get 'Time' column name
     def get_time_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Time' column name used in return tables from api calls
         """
-        return 'Time'
+        return "Time"
 
     # get 'Depth' column name
     def get_depth_column_name(self, **kwargs) -> str:
         """
         Get predefined 'Depth' column name used in return tables from api calls
         """
-        return 'Depth'
+        return "Depth"
 
     # get signal data type name
-    def get_signal_data_type_name(self, signal_type: Union[str, SignalType], **kwargs) -> str:
+    def get_signal_data_type_name(
+        self, signal_type: Union[str, SignalType], **kwargs
+    ) -> str:
         """
         Get data type name for corresponding signal type
 
         Parameters
         ----------
         signal_type : str, SignalType
             Signal type
         """
         if isinstance(signal_type, str):
             signal_type = self.get_signal_type_enum(signal_type, **kwargs)
         elif not isinstance(signal_type, SignalType):
-            raise ValueError(f"PetroVisor::get_signal_data_type_name(): "
-                             f"unknown 'signal_type'! "
-                             f"Should be one of {[t.name for t in SignalType]} or {SignalType.__name__} enum.")
-        if signal_type == SignalType.Static:
-            return 'numeric'
-        elif signal_type == SignalType.DepthDependent:
-            return 'numeric'
-        elif signal_type == SignalType.TimeDependent:
-            return 'numeric'
-        elif signal_type == SignalType.String:
-            return 'string'
-        elif signal_type == SignalType.StringTimeDependent:
-            return 'string'
-        elif signal_type == SignalType.PVT:
-            return 'numeric'
-        raise ValueError(f"PetroVisor::get_signal_data_type_name(): "
-                         f"'{signal_type}' is not supported yet.")
+            raise ValueError(
+                f"PetroVisor::get_signal_data_type_name(): "
+                f"unknown 'signal_type'! "
+                f"Should be one of {[t.name for t in SignalType]} or {SignalType.__name__} enum."
+            )
+        if signal_type in {
+            SignalType.Static,
+            SignalType.TimeDependent,
+            SignalType.DepthDependent,
+            SignalType.PVT,
+        }:
+            return "numeric"
+        elif signal_type in {
+            SignalType.String,
+            SignalType.StringTimeDependent,
+            SignalType.StringDepthDependent,
+        }:
+            return "string"
+        raise ValueError(
+            f"PetroVisor::get_signal_data_type_name(): "
+            f"'{signal_type}' is not supported yet."
+        )
 
     # get signal range name
-    def get_signal_range_type_name(self, signal_type: Union[str, SignalType], **kwargs) -> str:
+    def get_signal_range_type_name(
+        self, signal_type: Union[str, SignalType], **kwargs
+    ) -> str:
         """
         Get data range type name for corresponding signal type
 
         Parameters
         ----------
         signal_type : str, SignalType
             Signal type
         """
         if isinstance(signal_type, str):
             signal_type = self.get_signal_type_enum(signal_type, **kwargs)
         elif not isinstance(signal_type, SignalType):
-            raise ValueError(f"PetroVisor::get_signal_range_type_name(): "
-                             f"unknown 'signal_type'! "
-                             f"Should be one of {[t.name for t in SignalType]} or {SignalType.__name__} enum.")
-        if signal_type == SignalType.Static:
-            return ''
-        elif signal_type == SignalType.DepthDependent:
-            return 'numeric'
-        elif signal_type == SignalType.TimeDependent:
-            return 'time'
-        elif signal_type == SignalType.String:
-            return ''
-        elif signal_type == SignalType.StringTimeDependent:
-            return 'time'
-        elif signal_type == SignalType.PVT:
-            return ''
-        raise ValueError(f"PetroVisor::get_signal_range_type_name(): "
-                         f"'{signal_type}' is not supported yet.")
+            raise ValueError(
+                f"PetroVisor::get_signal_range_type_name(): "
+                f"unknown 'signal_type'! "
+                f"Should be one of {[t.name for t in SignalType]} or {SignalType.__name__} enum."
+            )
+        if signal_type in {SignalType.TimeDependent, SignalType.StringTimeDependent}:
+            return "time"
+        elif signal_type in {
+            SignalType.DepthDependent,
+            SignalType.StringDepthDependent,
+        }:
+            return "numeric"
+        elif signal_type in {SignalType.Static, SignalType.String, SignalType.PVT}:
+            return ""
+        raise ValueError(
+            f"PetroVisor::get_signal_range_type_name(): "
+            f"'{signal_type}' is not supported yet."
+        )
 
     # convert list to dictionary
     def list_to_dict(self, x, num_cols, **kwargs):
         if num_cols == 0:
             return {
-                self.get_json_valid_value(idx, 'numeric', **kwargs):
-                    self.get_json_valid_value(row, 'numeric', **kwargs) for idx, row in enumerate(x)}
+                self.get_json_valid_value(
+                    idx, "numeric", **kwargs
+                ): self.get_json_valid_value(row, "numeric", **kwargs)
+                for idx, row in enumerate(x)
+            }
         elif num_cols == 1:
             return {
-                self.get_json_valid_value(idx, 'numeric', **kwargs):
-                    self.get_json_valid_value(row[0], 'numeric', **kwargs) for idx, row in enumerate(x)}
+                self.get_json_valid_value(
+                    idx, "numeric", **kwargs
+                ): self.get_json_valid_value(row[0], "numeric", **kwargs)
+                for idx, row in enumerate(x)
+            }
         elif num_cols > 1:
             return {
-                self.get_json_valid_value(row[0], 'numeric', **kwargs):
-                    self.get_json_valid_value(row[1], 'numeric', **kwargs) for row in x}
+                self.get_json_valid_value(
+                    row[0], "numeric", **kwargs
+                ): self.get_json_valid_value(row[1], "numeric", **kwargs)
+                for row in x
+            }
 
 
 # DataFrame mixin helper
 class DataFrameMixinHelper:
 
     # set DataFrame indices
     @staticmethod
-    def set_dataframe_index(df: pd.DataFrame,
-                            indices: List[str],
-                            inplace: bool = False,
-                            add_default_index: bool = False,
-                            default_index_name: str = 'index',
-                            **kwargs):
+    def set_dataframe_index(
+        df: pd.DataFrame,
+        indices: List[str],
+        inplace: bool = False,
+        add_default_index: bool = False,
+        default_index_name: str = "index",
+        **kwargs,
+    ):
         """
         Set DataFrame index
 
         Parameters
         ----------
         df : DataFrame
             DataFrame
@@ -1063,24 +1280,25 @@
         Tuple (DataFrame, default_index_column)
         """
         # define working DataFrame
         df_with_index = df if inplace else df.copy()
         # get column indices
         idx = [item for item in indices if item in df.columns]
         # add default index
-        index_col = ''
+        index_col = ""
         if add_default_index:
             # get index name which does not match any column name
             def get_default_index_name(df: pd.DataFrame):
                 index_name = default_index_name
                 i = 0
                 while index_name in df.columns:
-                    index_name = f'{default_index_name}_{i}'
+                    index_name = f"{default_index_name}_{i}"
                     i += 1
                 return index_name
+
             index_col = get_default_index_name(df)
             df_with_index[index_col] = df_with_index.index
             idx.insert(0, index_col)
         # set indices
         df_with_index = df_with_index.set_index(idx)
         return df_with_index, index_col
 
@@ -1093,41 +1311,45 @@
         Parameters
         ----------
         data : list
             List of tabulated strings
         """
         if len(data) < 1:
             return None
-        return pd.read_csv(io.StringIO('\n'.join(data)), delimiter='\t')
+        return pd.read_csv(io.StringIO("\n".join(data)), delimiter="\t")
 
     # remove entity name from column names
     @staticmethod
     def remove_entities_from_columns(columns: Iterable[str]) -> List[str]:
         """
         Remove entity name from column names
 
         Parameters
         ----------
         columns : list
             Column names
         """
-        return [c[1] if len(c) > 1 else c[0] for c in (col.split(' : ') for col in columns)]
+        return [
+            c[1] if len(c) > 1 else c[0] for c in (col.split(" : ") for col in columns)
+        ]
 
     # extract entity name from column names
     @staticmethod
     def get_entities_from_columns(columns: Iterable[str]) -> List[str]:
         """
         Extract entity name from column names
 
         Parameters
         ----------
         columns : list
             Column names
         """
-        return [c[0] if len(c) > 1 else '' for c in (col.split(' : ') for col in columns)]
+        return [
+            c[0] if len(c) > 1 else "" for c in (col.split(" : ") for col in columns)
+        ]
 
     # get list of unique non-empty names
     @staticmethod
     def get_unique_non_empty_names(x: List[str]) -> List[str]:
         """
         get list of unique non-empty names
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/entities.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,136 +15,154 @@
 # Entities API calls
 class EntitiesMixin(SupportsItemRequests, SupportsRequests):
     """
     Entities API calls
     """
 
     # get entity
-    def get_entity(self, name: str, alias: Optional[str] = '', **kwargs) -> Dict:
+    def get_entity(self, name: str, alias: Optional[str] = "", **kwargs) -> Dict:
         """
         Get entity
 
         Parameters
         ----------
         name : str
             Entity name
         alias : str
             Entity alias
         """
-        route = 'Entities'
+        route = "Entities"
         if alias:
-            return self.get(f'{route}/{self.encode(alias)}/Entity', **kwargs)
-        return self.get(f'{route}/{self.encode(name)}', **kwargs)
+            return self.get(f"{route}/{self.encode(alias)}/Entity", **kwargs)
+        return self.get(f"{route}/{self.encode(name)}", **kwargs)
 
     # get entities
-    def get_entities(self, entity_type: Optional[str] = '', signal: Optional[str] = '', **kwargs) -> List[Dict]:
+    def get_entities(
+        self, entity_type: Optional[str] = "", signal: Optional[str] = "", **kwargs
+    ) -> List[Dict]:
         """
         Get entities. Filter optionally by entity type and signal
 
         Parameters
         ----------
         entity_type : str, default ''
             Entity type
         signal : str, default ''
             Signal object or Signal name
         """
-        route = 'Entities'
+        route = "Entities"
         # get entities by 'Entity' type
         if entity_type:
-            entities = self.get(f'{route}/{entity_type}/Entities', **kwargs)
+            entities = self.get(f"{route}/{entity_type}/Entities", **kwargs)
         # get all entities
         else:
-            entities = self.get(f'{route}/All', **kwargs)
+            entities = self.get(f"{route}/All", **kwargs)
         # get entities by 'Signal' name
         if signal:
-            entity_names = self.get_entity_names(signal_type=None, signal=signal, **kwargs)
+            entity_names = self.get_entity_names(
+                signal_type=None, signal=signal, **kwargs
+            )
             if entity_names:
-                return [e for e in entities if e['Name'] in entity_names]
+                return [e for e in entities if e["Name"] in entity_names]
         return entities if entities is not None else []
 
     # get entity names
-    def get_entity_names(self, entity_type: Optional[str] = '', signal: Optional[str] = '', **kwargs) -> List[str]:
+    def get_entity_names(
+        self, entity_type: Optional[str] = "", signal: Optional[str] = "", **kwargs
+    ) -> List[str]:
         """
         Get entity names. Filter optionally by entity type and signal
 
         Parameters
         ----------
         entity_type : str, default ''
             Entity type
         signal : str, default ''
             Signal object or Signal name
         """
 
-        route = 'Entities'
+        route = "Entities"
         # get entities by 'Signal' name
         if signal:
-            signals_route = 'Signals'
+            signals_route = "Signals"
             signal_name = ApiHelper.get_object_name(signal)
-            entity_names = self.get(f'{signals_route}/{self.encode(signal_name)}/Entities', **kwargs)
+            entity_names = self.get(
+                f"{signals_route}/{self.encode(signal_name)}/Entities", **kwargs
+            )
             if entity_type and entity_names is not None:
-                entity_type_names = self.get_entity_names(entity_type=entity_type, signal=None, **kwargs)
+                entity_type_names = self.get_entity_names(
+                    entity_type=entity_type, signal=None, **kwargs
+                )
                 if entity_type_names:
                     return [e for e in entity_names if e in entity_type_names]
         # get entities by 'Entity' type
         elif entity_type:
             entities = self.get_entities(entity_type=entity_type, signal=None, **kwargs)
-            return [e['Name'] for e in entities]
+            return [e["Name"] for e in entities]
         # get all entities
         else:
-            entity_names = self.get(f'{route}', **kwargs)
+            entity_names = self.get(f"{route}", **kwargs)
         return entity_names if entity_names is not None else []
 
     # add entities
     def add_entities(self, entities: List, **kwargs) -> Any:
         """
         Add multiple entities
 
         Parameters
         ----------
         entities : list
             List of entities
         """
-        route = 'Entities'
-        return self.post(f'{route}/AddOrEdit', data=entities, **kwargs)
+        route = "Entities"
+        return self.post(f"{route}/AddOrEdit", data=entities, **kwargs)
 
     # delete entities
     def delete_entities(self, entities: List, **kwargs) -> Any:
         """
         Delete multiple entities
 
         Parameters
         ----------
         entities : list
             List of entities
         """
-        route = 'Entities'
-        return self.post(f'{route}/Delete', data=entities, **kwargs)
+        route = "Entities"
+        return self.post(f"{route}/Delete", data=entities, **kwargs)
 
     # rename entity type
     def rename_entity_type(self, old_name: str, new_name: str, **kwargs) -> Any:
         """
         Rename entity type
 
         Parameters
         ----------
         old_name : str
             Old name
         new_name : str
             New name
         """
-        route = 'EntityTypes'
-        return self.post(f'{route}/Rename', query={'OldName': old_name, 'NewName': new_name}, **kwargs)
+        route = "EntityTypes"
+        return self.post(
+            f"{route}/Rename",
+            query={"OldName": old_name, "NewName": new_name},
+            **kwargs,
+        )
 
     # rename entity
     def rename_entity(self, old_name: str, new_name: str, **kwargs) -> Any:
         """
         Rename entity
 
         Parameters
         ----------
         old_name : str
             Old name
         new_name : str
             New name
         """
-        route = 'Entities'
-        return self.post(f'{route}/Rename', query={'OldName': old_name, 'NewName': new_name}, **kwargs)
+        route = "Entities"
+        return self.post(
+            f"{route}/Rename",
+            query={"OldName": old_name, "NewName": new_name},
+            **kwargs,
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/files.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,67 +21,75 @@
     """
 
     # get file names
     def get_file_names(self, **kwargs) -> List[str]:
         """
         Get file names
         """
-        return self.get('Files', **kwargs)
+        return self.get("Files", **kwargs)
 
     # get file by name
-    def get_file(self, filename: str, format: str = 'bytes', **kwargs) -> Any:
+    def get_file(self, filename: str, format: str = "bytes", **kwargs) -> Any:
         """
         Get file
 
         Parameters
         ----------
         filename : str
             File name
         format : str, default 'bytes'
             File format
         """
         filename = ApiHelper.get_windows_like_path(filename)
-        return self.get(f'Files/{self.encode(filename)}', format=format, **kwargs)
+        return self.get(f"Files/{self.encode(filename)}", format=format, **kwargs)
 
     # delete file by given name
     def delete_file(self, filename: str, **kwargs) -> Any:
         """
         Delete file
 
         Parameters
         ----------
         filename : str
             File name
         """
         filename = ApiHelper.get_windows_like_path(filename)
-        return self.delete(f'Files/{self.encode(filename)}', **kwargs)
+        return self.delete(f"Files/{self.encode(filename)}", **kwargs)
 
     # upload file
-    def upload_file(self, file: Any, name: str = '', **kwargs) -> Any:
+    def upload_file(self, file: Any, name: str = "", **kwargs) -> Any:
         """
         Upload file
 
         Parameters
         ----------
         file : str | stream
             File path or file-like object
         name : str
             File name
         """
         # upload file with specified name
         if name:
             name = ApiHelper.get_unix_like_path(name)
-            return self.post('Files/Upload',
-                             files={'file': (name, open(file, 'rb') if isinstance(file, str) else file)}, **kwargs)
+            return self.post(
+                "Files/Upload",
+                files={
+                    "file": (name, open(file, "rb") if isinstance(file, str) else file)
+                },
+                **kwargs,
+            )
         # upload file with the same name as file's name or name specified in the file-like object
-        return self.post('Files/Upload',
-                         files={'file': open(file, 'rb') if isinstance(file, str) else file}, **kwargs)
+        return self.post(
+            "Files/Upload",
+            files={"file": open(file, "rb") if isinstance(file, str) else file},
+            **kwargs,
+        )
 
     # upload folder
-    def upload_folder(self, folder: str, name: str = '', **kwargs) -> Any:
+    def upload_folder(self, folder: str, name: str = "", **kwargs) -> Any:
         """
         Upload folder
 
         Parameters
         ----------
         folder : str
             Folder path
@@ -129,45 +137,45 @@
         if folder:
             folder = ApiHelper.get_unix_like_path(folder)
         for filename in files:
             if filename.startswith(folder):
                 self.delete_file(filename, **kwargs)
 
     # get object by name
-    def get_object(self,
-                   name: str,
-                   func: Optional[Callable] = None,
-                   binary: bool = True,
-                   **kwargs) -> Any:
+    def get_object(
+        self, name: str, func: Optional[Callable] = None, binary: bool = True, **kwargs
+    ) -> Any:
         """
         Load object from blob storage using pickle.loads()
 
         Parameters
         ----------
         name : str
             Object name
         func : Optional[Callable], default None
             Function to be called to prepare object after load. If None, then pickle.loads() is used
         binary : bool, default True
             Whether to use binary (True) stream io.BytesIO or text (False) stream io.StringIO
         """
-        file_obj = self.get_file(name, format='bytes', **kwargs)
-        if func and hasattr(func, '__call__'):
+        file_obj = self.get_file(name, format="bytes", **kwargs)
+        if func and hasattr(func, "__call__"):
             return func(file_obj, **kwargs)
         if binary:
             return pickle.loads(file_obj)
         return json.load(io.BytesIO(file_obj), **kwargs)
 
     # upload object
-    def upload_object(self,
-                      obj: Any,
-                      name: str,
-                      func: Optional[Callable] = None,
-                      binary: bool = True,
-                      **kwargs) -> Any:
+    def upload_object(
+        self,
+        obj: Any,
+        name: str,
+        func: Optional[Callable] = None,
+        binary: bool = True,
+        **kwargs,
+    ) -> Any:
         """
         Upload object to blob storage using pickle.dumps()
 
         Parameters
         ----------
         obj : Any
             Object
@@ -175,15 +183,15 @@
             Object name
         func : Optional[Callable], default None
             Function to be called to prepare object for upload. If None, then pickle.dumps() is used
         binary : bool, default True
             Whether to use binary (True) stream io.BytesIO or text (False) stream io.StringIO
         """
         # upload file by full path
-        if func and hasattr(func, '__call__'):
+        if func and hasattr(func, "__call__"):
             file = func(obj, **kwargs)
         elif binary:
             file = pickle.dumps(obj)
         else:
             file = json.dumps(obj, **kwargs)
         # binary stream
         if binary:
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/items.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/items.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,20 +56,22 @@
         item_type : str
             Item type
         name : str
             Item name
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_item(): "
-                             f"unknown item type: '{item_type}'. "
-                             f"Known item types: {list(self.ItemRoutes.keys())}")
-        if route == 'Units' and name == ' ':
-            name = '_'
-        return self.get(f'{route}/{self.encode(name)}', **kwargs)
+            raise ValueError(
+                f"PetroVisor::get_item(): "
+                f"unknown item type: '{item_type}'. "
+                f"Known item types: {list(self.ItemRoutes.keys())}"
+            )
+        if route == "Units" and name == " ":
+            name = "_"
+        return self.get(f"{route}/{self.encode(name)}", **kwargs)
 
     # delete item
     def delete_item(self, item_type: str, item: Union[str, Dict], **kwargs) -> Any:
         """
         Delete item
 
         Parameters
@@ -77,19 +79,21 @@
         item_type : str
             Item type
         item : str, dict
             Item object or Item name
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::delete_item(): "
-                             f"unknown item type: '{item_type}'. "
-                             f"Known item types: {list(self.ItemRoutes.keys())}")
+            raise ValueError(
+                f"PetroVisor::delete_item(): "
+                f"unknown item type: '{item_type}'. "
+                f"Known item types: {list(self.ItemRoutes.keys())}"
+            )
         name = self.get_item_name(item, **kwargs)
-        return self.delete(f'{route}/{self.encode(name)}', **kwargs)
+        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
 
     # add or edit item
     def add_item(self, item_type: str, item: Dict, **kwargs) -> Any:
         """
         Add or edit item
 
         Parameters
@@ -97,19 +101,21 @@
         item_type : str
             Item type
         item : dict
             Item object
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::add_item(): "
-                             f"unknown item type: '{item_type}'. "
-                             f"Known item types: {list(self.ItemRoutes.keys())}")
+            raise ValueError(
+                f"PetroVisor::add_item(): "
+                f"unknown item type: '{item_type}'. "
+                f"Known item types: {list(self.ItemRoutes.keys())}"
+            )
         name = self.get_item_name(item, **kwargs)
-        return self.put(f'{route}/{self.encode(name)}', data=item, **kwargs)
+        return self.put(f"{route}/{self.encode(name)}", data=item, **kwargs)
 
     # update item metadata
     def update_item_metadata(self, item_type: str, item: Dict, **kwargs) -> Any:
         """
         Update item metadata
 
         Parameters
@@ -117,125 +123,145 @@
         item_type : str
             Item type
         item : dict
             Item object
         """
         route = self.get_petrovisor_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::update_item_metadata(): "
-                             f"unknown 'PetroVisor' item type: '{item_type}'. "
-                             f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}")
+            raise ValueError(
+                f"PetroVisor::update_item_metadata(): "
+                f"unknown 'PetroVisor' item type: '{item_type}'. "
+                f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}"
+            )
         name = self.get_item_name(item, **kwargs)
-        return self.put(f'{route}/{self.encode(name)}/Metadata', data=item, **kwargs)
+        return self.put(f"{route}/{self.encode(name)}/Metadata", data=item, **kwargs)
 
     # get items
     def get_items(self, item_type: str, **kwargs) -> List:
         """
         Get items of given type
 
         Parameters
         ----------
         item_type : str
             Item type
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_items(): "
-                             f"unknown item type: '{item_type}'. "
-                             f"Known item types: {list(self.ItemRoutes.keys())}")
-        return self.get(f'{route}/All', **kwargs)
+            raise ValueError(
+                f"PetroVisor::get_items(): "
+                f"unknown item type: '{item_type}'. "
+                f"Known item types: {list(self.ItemRoutes.keys())}"
+            )
+        return self.get(f"{route}/All", **kwargs)
 
     # get item paged
-    def get_items_paged(self, item_type: str, page: int = 1, page_size: int = 10, **kwargs) -> List:
+    def get_items_paged(
+        self, item_type: str, page: int = 1, page_size: int = 10, **kwargs
+    ) -> List:
         """
         Get items of given type in paged format
 
         Parameters
         ----------
         item_type : str
             Item type
         page : int, default 1
             Page number
         page_size : int, default 10
             Page size
         """
         route = self.get_petrovisor_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_items_paged(): "
-                             f"unknown 'PetroVisor' item type: '{item_type}'. "
-                             f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}")
-        return self.get(f'{route}/Paged', query={'Page': page, 'PageSize': page_size}, **kwargs)
+            raise ValueError(
+                f"PetroVisor::get_items_paged(): "
+                f"unknown 'PetroVisor' item type: '{item_type}'. "
+                f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}"
+            )
+        return self.get(
+            f"{route}/Paged", query={"Page": page, "PageSize": page_size}, **kwargs
+        )
 
     # get item names
     def get_item_names(self, item_type: str, **kwargs) -> List[str]:
         """
         Get item names of given type
 
         Parameters
         ----------
         item_type : str
             Item type
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_item_names(): "
-                             f"unknown item type: '{item_type}'. "
-                             f"Known item types: {list(self.ItemRoutes.keys())}")
-        return self.get(f'{route}', **kwargs)
+            raise ValueError(
+                f"PetroVisor::get_item_names(): "
+                f"unknown item type: '{item_type}'. "
+                f"Known item types: {list(self.ItemRoutes.keys())}"
+            )
+        return self.get(f"{route}", **kwargs)
 
     # get item labels
-    def get_item_labels(self, item_type: str, name: Optional[str] = None, **kwargs) -> List:
+    def get_item_labels(
+        self, item_type: str, name: Optional[str] = None, **kwargs
+    ) -> List:
         """
         Get item labels of given type
 
         Parameters
         ----------
         item_type : str
             Item type
         name : str
             Item name
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_item_labels(): "
-                             f"unknown 'PetroVisor' item type: '{item_type}'. "
-                             f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}")
+            raise ValueError(
+                f"PetroVisor::get_item_labels(): "
+                f"unknown 'PetroVisor' item type: '{item_type}'. "
+                f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}"
+            )
         if self.is_petrovisor_item(item_type, **kwargs):
             if name:
                 item = self.get_item(item_type, name, **kwargs)
-                return item['Labels']
-            items = self.get(f'{route}/PetroVisorItems', **kwargs)
-            return [{item['Name']: item['Labels']} for item in items]
+                return item["Labels"]
+            items = self.get(f"{route}/PetroVisorItems", **kwargs)
+            return [{item["Name"]: item["Labels"]} for item in items]
         return []
 
     # get item infos
-    def get_item_infos(self, item_type: str, name: Optional[str] = None, **kwargs) -> Union[List, Dict]:
+    def get_item_infos(
+        self, item_type: str, name: Optional[str] = None, **kwargs
+    ) -> Union[List, Dict]:
         """
         Get item infos of given type
 
         Parameters
         ----------
         item_type : str
             Item type
         name : str
             Item name
         """
         route = self.get_item_route(item_type, **kwargs)
         if not route:
-            raise ValueError(f"PetroVisor::get_item_infos(): "
-                             f"unknown 'PetroVisor' item type: '{item_type}'. "
-                             f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}")
+            raise ValueError(
+                f"PetroVisor::get_item_infos(): "
+                f"unknown 'PetroVisor' item type: '{item_type}'. "
+                f"Known 'PetroVisor' item types: {list(self.PetroVisorItemRoutes.keys())}"
+            )
         if self.is_info_item(item_type, **kwargs):
             if name:
-                return self.get(f'{route}/{self.encode(name)}/Info', **kwargs)
-            return self.get(f'{route}/Info', **kwargs)
+                return self.get(f"{route}/{self.encode(name)}/Info", **kwargs)
+            return self.get(f"{route}/Info", **kwargs)
         elif self.is_petrovisor_item(item_type, **kwargs):
             if name:
-                return self.get(f'{route}/{self.encode(name)}/PetroVisorItem', **kwargs)
-            return self.get(f'{route}/PetroVisorItems', **kwargs)
+                return self.get(f"{route}/{self.encode(name)}/PetroVisorItem", **kwargs)
+            return self.get(f"{route}/PetroVisorItems", **kwargs)
         return {} if name else []
 
     # get item name
     def get_item_name(self, item: Union[str, Dict], **kwargs) -> str:
         """
         Get item name
 
@@ -243,15 +269,21 @@
         ----------
         item : dict
             Item object
         """
         return ApiHelper.get_object_name(item)
 
     # get item field
-    def get_item_field(self, item_type: Optional[str], item: Union[str, Dict], field_name: str, **kwargs) -> Any:
+    def get_item_field(
+        self,
+        item_type: Optional[str],
+        item: Union[str, Dict],
+        field_name: str,
+        **kwargs,
+    ) -> Any:
         """
         Get item field value
 
         Parameters
         ----------
         item_type : str
             Item type
@@ -260,19 +292,22 @@
         field_name : str
             Field name
         """
         if isinstance(item, str) and item_type:
             item_name = ApiHelper.get_object_name(item)
             item = self.get_item(item_type, item_name, **kwargs)
         if not item:
-            raise ValueError(f"PetroVisor::get_item_field(): "
-                             f"item '{item}' cannot be found!")
+            raise ValueError(
+                f"PetroVisor::get_item_field(): item '{item}' cannot be found!"
+            )
         elif not ApiHelper.has_field(item, field_name):
-            raise ValueError(f"PetroVisor::get_item_field(): "
-                             f"item '{item}' doesn't not have '{field_name}' field!")
+            raise ValueError(
+                f"PetroVisor::get_item_field(): "
+                f"item '{item}' doesn't not have '{field_name}' field!"
+            )
         return item[field_name]
 
     # get 'NamedItem' route
     def get_item_route(self, data_type: str, **kwargs) -> str:
         """
         Get route for corresponding NamedItem type
 
@@ -357,86 +392,96 @@
 
     # get item routes
     @staticmethod
     def get_item_routes() -> Dict:
         """
         Get all item routes
         """
-        return dict(**ItemsMixinHelper.get_named_item_routes(), **ItemsMixinHelper.get_petrovisor_item_routes())
+        return dict(
+            **ItemsMixinHelper.get_named_item_routes(),
+            **ItemsMixinHelper.get_petrovisor_item_routes(),
+        )
 
     # get 'NamedItem' routes
     @staticmethod
     def get_named_item_routes() -> Dict:
         """
         Get routes of NamedItems
         """
         return {
-            ItemType.Unit: 'Units',
-            ItemType.UnitMeasurement: 'UnitMeasurements',
-            ItemType.Entity: 'Entities',
-            ItemType.EntityType: 'EntityTypes',
-            ItemType.Signal: 'Signals',
-            ItemType.Tag: 'Tags',
-            ItemType.Label: 'Labels',
-            ItemType.MessageEntry: 'MessageEntries',
-            ItemType.Ticket: 'Tickets',
-            ItemType.ProcessTemplate: 'ProcessTemplates',
-            ItemType.UserSetting: 'UserSettings',
-            ItemType.EventSubscription: 'EventSubscriptions',
+            ItemType.Unit: "Units",
+            ItemType.UnitMeasurement: "UnitMeasurements",
+            ItemType.Entity: "Entities",
+            ItemType.EntityType: "EntityTypes",
+            ItemType.Signal: "Signals",
+            ItemType.Tag: "Tags",
+            ItemType.Label: "Labels",
+            ItemType.MessageEntry: "MessageEntries",
+            ItemType.Ticket: "Tickets",
+            ItemType.ProcessTemplate: "ProcessTemplates",
+            ItemType.UserSetting: "UserSettings",
+            ItemType.EventSubscription: "EventSubscriptions",
         }
 
     # get 'PetroVisorItem' routes
     @staticmethod
     def get_info_item_routes() -> Dict:
         """
         Get routes of InfoItems
         """
-        return dict(**{
-            ItemType.MLModel: 'MLModels',
-            ItemType.DataGrid: 'DataGrids',
-            ItemType.DataConnection: 'DataConnections',
-            ItemType.DataSourceMapping: 'DataSourceMappings',
-            ItemType.DataIntegrationSession: 'DataIntegrationSessions',
-            ItemType.Scenario: 'Scenarios',
-        }, **{  # alias
-            ItemType.MachineLearningModel: 'MLModels',  # alias MLModel
-        })
+        return dict(
+            **{
+                ItemType.MLModel: "MLModels",
+                ItemType.DataGrid: "DataGrids",
+                ItemType.DataConnection: "DataConnections",
+                ItemType.DataSourceMapping: "DataSourceMappings",
+                ItemType.DataIntegrationSession: "DataIntegrationSessions",
+                ItemType.Scenario: "Scenarios",
+            },
+            **{  # alias
+                ItemType.MachineLearningModel: "MLModels",  # alias MLModel
+            },
+        )
 
     # get 'PetroVisorItem' routes
     @staticmethod
     def get_petrovisor_item_routes() -> Dict:
         """
         Get routes of PetroVisorItems
         """
-        return dict(**{
-            ItemType.ConfigurationSettings: 'ConfigurationSettings',
-            ItemType.RefTable: 'RefTables',
-            ItemType.PivotTable: 'PivotTables',
-            ItemType.Hierarchy: 'Hierarchies',
-            ItemType.Scope: 'Scopes',
-            ItemType.EntitySet: 'EntitySets',
-            ItemType.Context: 'Contexts',
-            ItemType.TableCalculation: 'TableCalculations',
-            ItemType.EventCalculation: 'EventCalculations',
-            ItemType.CleansingCalculation: 'CleansingCalculations',
-            ItemType.PSharpScript: 'PSharpScripts',
-            ItemType.CleansingScript: 'CleansingScripts',
-            ItemType.Plot: 'Plots',
-            ItemType.Chart: 'Charts',
-            ItemType.Filter: 'Filters',
-            ItemType.Workflow: 'Workflows',
-            ItemType.WorkflowSchedule: 'WorkflowSchedules',
-            ItemType.CustomWorkflowActivity: 'CustomWorkflowActivities',
-            ItemType.RWorkflowActivity: 'RWorkflowActivities',
-            ItemType.PythonWorkflowActivity: 'PythonWorkflowActivities',
-            ItemType.WebWorkflowActivity: 'WebWorkflowActivities',
-            ItemType.DataIntegrationSet: 'DataIntegrationSets',
-            ItemType.WorkspacePackage: 'WorkspacePackages',
-            ItemType.DCA: 'DCA',
-            ItemType.PowerBIItem: 'PowerBIItems',
-            ItemType.Dashboard: 'Dashboards',
-        }, **{  # alias
-            ItemType.ConfigurationSettingValue: 'ConfigurationSettings',  # alias ConfigurationSettings
-            ItemType.PivotTableDefinition: 'PivotTables',  # alias PivotTable
-            ItemType.ChartDefinition: 'Charts',  # alias Chart
-            ItemType.FilterDefinition: 'Filters',  # alias Filter
-        }, **ItemsMixinHelper.get_info_item_routes())
+        return dict(
+            **{
+                ItemType.ConfigurationSettings: "ConfigurationSettings",
+                ItemType.RefTable: "RefTables",
+                ItemType.PivotTable: "PivotTables",
+                ItemType.Hierarchy: "Hierarchies",
+                ItemType.Scope: "Scopes",
+                ItemType.EntitySet: "EntitySets",
+                ItemType.Context: "Contexts",
+                ItemType.TableCalculation: "TableCalculations",
+                ItemType.EventCalculation: "EventCalculations",
+                ItemType.CleansingCalculation: "CleansingCalculations",
+                ItemType.PSharpScript: "PSharpScripts",
+                ItemType.CleansingScript: "CleansingScripts",
+                ItemType.Plot: "Plots",
+                ItemType.Chart: "Charts",
+                ItemType.Filter: "Filters",
+                ItemType.Workflow: "Workflows",
+                ItemType.WorkflowSchedule: "WorkflowSchedules",
+                ItemType.CustomWorkflowActivity: "CustomWorkflowActivities",
+                ItemType.RWorkflowActivity: "RWorkflowActivities",
+                ItemType.PythonWorkflowActivity: "PythonWorkflowActivities",
+                ItemType.WebWorkflowActivity: "WebWorkflowActivities",
+                ItemType.DataIntegrationSet: "DataIntegrationSets",
+                ItemType.WorkspacePackage: "WorkspacePackages",
+                ItemType.DCA: "DCA",
+                ItemType.PowerBIItem: "PowerBIItems",
+                ItemType.Dashboard: "Dashboards",
+            },
+            **{  # alias
+                ItemType.ConfigurationSettingValue: "ConfigurationSettings",  # alias ConfigurationSettings
+                ItemType.PivotTableDefinition: "PivotTables",  # alias PivotTable
+                ItemType.ChartDefinition: "Charts",  # alias Chart
+                ItemType.FilterDefinition: "Filters",  # alias Filter
+            },
+            **ItemsMixinHelper.get_info_item_routes(),
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/logs.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,38 +24,40 @@
             'messagedetails','directory'
         Parameters
         ----------
         message : str
             Log message
         """
         log_entry = {
-            'Timestamp': None,
-            'Message': message,
-            'Category': None,
-            'UserName': None,
-            'Severity': None,
-            'Workspace': None,
-            'Schedule': None,
-            'Workflow': None,
-            'StartTime': None,
-            'EndTime': None,
-            'Script': None,
-            'Entity': None,
-            'Signal': None,
-            'Unit': None,
-            'Tag': None,
-            'NumberOfItems': None,
-            'ValueBefore': None,
-            'ValueAfter': None,
-            'ElapsedTime': None,
-            'MessageDetails': None,
-            'Directory': None
+            "Timestamp": None,
+            "Message": message,
+            "Category": None,
+            "UserName": None,
+            "Severity": None,
+            "Workspace": None,
+            "Schedule": None,
+            "Workflow": None,
+            "StartTime": None,
+            "EndTime": None,
+            "Script": None,
+            "Entity": None,
+            "Signal": None,
+            "Unit": None,
+            "Tag": None,
+            "NumberOfItems": None,
+            "ValueBefore": None,
+            "ValueAfter": None,
+            "ElapsedTime": None,
+            "MessageDetails": None,
+            "Directory": None,
         }
         log_entry = ApiHelper.update_dict(log_entry, **kwargs)
-        return self.post('LogEntries', data=ApiHelper.get_non_empty_fields(log_entry), **kwargs)
+        return self.post(
+            "LogEntries", data=ApiHelper.get_non_empty_fields(log_entry), **kwargs
+        )
 
     # add workflow log entry
     def add_workflow_log_entry(self, message: str, workflow: str, **kwargs):
         """
         Add log entry message to tge running workflow.
         Use keyword arguments to pass other information.
         Known fields are:
@@ -69,12 +71,14 @@
         Parameters
         ----------
         message : str
             Log message
         workflow : str
             Workflow name
         """
-        return self.add_log_entry(message,
-                                  Workflow=workflow,
-                                  Category='Workflow Execution',
-                                  UserName='WorkflowService',
-                                  **kwargs)
+        return self.add_log_entry(
+            message,
+            Workflow=workflow,
+            Category="Workflow Execution",
+            UserName="WorkflowService",
+            **kwargs,
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/ml.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,46 +63,52 @@
         model_name : str
             ML Model name
         attribute : str
             ML Model attribute
         """
         ml_model = self.ml_model(model_name, **kwargs)
         if ml_model is None or not ml_model:
-            raise ValueError(f"PetroVisor::ml_model_attribute(): "
-                             f"ML Model '{model_name}' cannot be found!")
+            raise ValueError(
+                f"PetroVisor::ml_model_attribute(): "
+                f"ML Model '{model_name}' cannot be found!"
+            )
         if attribute in ml_model:
             return ml_model[attribute]
-        raise ValueError(f"PetroVisor::ml_model_attribute(): "
-                         f"unknown ML Model attribute '{attribute}'!")
+        raise ValueError(
+            f"PetroVisor::ml_model_attribute(): "
+            f"unknown ML Model attribute '{attribute}'!"
+        )
 
     # get ML model type
     def ml_model_type(self, model_name: str, **kwargs) -> Any:
         """
         Get ML Model type
 
         Parameters
         ----------
         model_name : str
             ML Model name
         """
-        return self.ml_model_attribute(model_name, 'Type', **kwargs)
+        return self.ml_model_attribute(model_name, "Type", **kwargs)
 
     # get ML model features and label
     def ml_model_features_and_label(self, model_name: str, **kwargs) -> Any:
         """
         Get ML Model features and label
 
         Parameters
         ----------
         model_name : str
             ML Model name
         """
         features = {}
-        features_script = self.ml_model_attribute(model_name, 'TableFormula', **kwargs)
-        feature_tables = self.get_psharp_script_columns_and_signals(features_script, **kwargs)
+        features_script = self.ml_model_attribute(model_name, "TableFormula", **kwargs)
+        feature_tables = self.get_psharp_script_columns_and_signals(
+            features_script, **kwargs
+        )
         if feature_tables:
             for table_name, table in feature_tables.items():
                 if table:
                     return table
         return features
 
     # get ML model features
@@ -112,15 +118,15 @@
 
         Parameters
         ----------
         model_name : str
             ML Model name
         """
         features = self.ml_model_features_and_label(model_name, **kwargs)
-        label = self.ml_model_attribute(model_name, 'LabelColumnName', **kwargs)
+        label = self.ml_model_attribute(model_name, "LabelColumnName", **kwargs)
         return {k: v for k, v in features.items() if k != label}
 
     # get ML model feature names
     def ml_model_feature_names(self, model_name: str, **kwargs) -> Any:
         """
         Get ML Model feature names
 
@@ -138,15 +144,15 @@
         Get ML Model label
 
         Parameters
         ----------
         model_name : str
             ML Model name
         """
-        label = self.ml_model_attribute(model_name, 'LabelColumnName', **kwargs)
+        label = self.ml_model_attribute(model_name, "LabelColumnName", **kwargs)
         features = self.ml_model_features_and_label(model_name, **kwargs)
         for k, v in features.items():
             if k == label:
                 return label, v
         return label, None
 
     # get ML model label name
@@ -155,31 +161,33 @@
         Get ML Model label name
 
         Parameters
         ----------
         model_name : str
             ML Model name
         """
-        return self.ml_model_attribute(model_name, 'LabelColumnName', **kwargs)
+        return self.ml_model_attribute(model_name, "LabelColumnName", **kwargs)
 
     # get ML trainers and metrics
-    def ml_trainers_and_metrics(self, model_type: Union[str, MLModelType], **kwargs) -> Any:
+    def ml_trainers_and_metrics(
+        self, model_type: Union[str, MLModelType], **kwargs
+    ) -> Any:
         """
         Get ML trainers and metrics
 
         Parameters
         ----------
         model_type : str, MLModelType
             ML Model type:
             'Regression', 'BinaryClassification', 'MultipleClassification', 'Clustering',
             'NaiveBayes', 'NaiveBayesCategorical'
         """
-        route = 'MLModels/TrainersAndMetrics'
+        route = "MLModels/TrainersAndMetrics"
         model_type = self.get_ml_model_type_enum(model_type, **kwargs).name
-        return self.get(route, query={'ModelType': model_type}, **kwargs)
+        return self.get(route, query={"ModelType": model_type}, **kwargs)
 
     # get ML trainers
     def ml_trainers(self, model_type: Union[str, MLModelType], **kwargs) -> Any:
         """
         Get ML trainers
 
         Parameters
@@ -188,17 +196,18 @@
             ML Model type:
             'Regression', 'BinaryClassification', 'MultipleClassification', 'Clustering',
             'NaiveBayes', 'NaiveBayesCategorical'
         """
         model_type = self.get_ml_model_type_enum(model_type, **kwargs).name
         ml_trainers_and_metrics = self.ml_trainers_and_metrics(model_type, **kwargs)
         if not ml_trainers_and_metrics:
-            raise ValueError(f"PetroVisor::ml_trainers(): "
-                             f"unknown ML Model type: '{model_type}'!")
-        return ml_trainers_and_metrics['Trainers']
+            raise ValueError(
+                f"PetroVisor::ml_trainers(): unknown ML Model type: '{model_type}'!"
+            )
+        return ml_trainers_and_metrics["Trainers"]
 
     # get ML metrics
     def ml_metrics(self, model_type: Union[str, MLModelType], **kwargs) -> Any:
         """
         Get ML metrics
 
         Parameters
@@ -207,102 +216,113 @@
             ML Model type:
             'Regression', 'BinaryClassification', 'MultipleClassification', 'Clustering',
             'NaiveBayes', 'NaiveBayesCategorical'
         """
         model_type = self.get_ml_model_type_enum(model_type, **kwargs).name
         ml_trainers_and_metrics = self.ml_trainers_and_metrics(model_type, **kwargs)
         if not ml_trainers_and_metrics:
-            raise ValueError(f"PetroVisor::ml_trainers(): "
-                             f"unknown ML Model type: '{model_type}'!")
-        return ml_trainers_and_metrics['Metrics']
+            raise ValueError(
+                f"PetroVisor::ml_trainers(): unknown ML Model type: '{model_type}'!"
+            )
+        return ml_trainers_and_metrics["Metrics"]
 
     # get ML pre-training statistics
-    def ml_pre_training_statistics(self, model_name: str, skip_pre_processing: bool = True, **kwargs) -> Any:
+    def ml_pre_training_statistics(
+        self, model_name: str, skip_pre_processing: bool = True, **kwargs
+    ) -> Any:
         """
         Get ML pre-training statistics
 
         Parameters
         ----------
         model_name : str
             ML Model name
         skip_pre_processing : bool, default True
             Skip pre-processing of the data
         """
-        route = 'MLModels/PreTrainingStatistics'
-        return self.post(route, data={
-            'ModelName': model_name,
-            'SkipPreProcessing': skip_pre_processing,
-        }, **kwargs)
+        route = "MLModels/PreTrainingStatistics"
+        return self.post(
+            route,
+            data={
+                "ModelName": model_name,
+                "SkipPreProcessing": skip_pre_processing,
+            },
+            **kwargs,
+        )
 
     # get ML post-training statistics
-    def ml_post_training_statistics(self, model_name: str, entity: Optional[Union[str, dict]] = None, **kwargs) -> Any:
+    def ml_post_training_statistics(
+        self, model_name: str, entity: Optional[Union[str, dict]] = None, **kwargs
+    ) -> Any:
         """
         Get ML post-training statistics
 
         Parameters
         ----------
         model_name : str
             ML Model name
         entity : str | dict | None, default None
             Entity object or Entity name
         """
-        route = 'MLModels/PostTrainingStatistics'
+        route = "MLModels/PostTrainingStatistics"
         if entity:
-            request = {
-                'ModelName': model_name
-            }
+            request = {"ModelName": model_name}
             entity_name = ApiHelper.get_object_name(entity)
-            request['EntityName'] = entity_name
+            request["EntityName"] = entity_name
             return self.post(route, data=request, **kwargs)
-        return self.post(route, data={'ModelName': model_name}, **kwargs)
+        return self.post(route, data={"ModelName": model_name}, **kwargs)
 
     # predict ML model
-    def ml_predict(self, model_name: str, entity: Union[str, dict], data: dict, **kwargs) -> Any:
+    def ml_predict(
+        self, model_name: str, entity: Union[str, dict], data: dict, **kwargs
+    ) -> Any:
         """
         Get ML post-training statistics
 
         Parameters
         ----------
         model_name : str
             ML Model name
         entity : str, dict
             Entity object or Entity name
         data : dict
             ML Model data
         """
-        route = 'MLModels/Predict'
+        route = "MLModels/Predict"
         entity_name = ApiHelper.get_object_name(entity)
         request = {
-            'ModelName': model_name,
-            'EntityName': entity_name,
-            'SourceData': data,
+            "ModelName": model_name,
+            "EntityName": entity_name,
+            "SourceData": data,
         }
         request = ApiHelper.update_dict(request, **kwargs)
         return self.post(route, data=request, **kwargs)
 
     # train ML model
-    def ml_train(self,
-                 model_name: str,
-                 time_to_train: int = 5,
-                 complete_case_only: bool = True,
-                 per_entity: bool = False,
-                 normalization: str = 'Auto',
-                 trainers: Optional[Union[str, List[str]]] = None,
-                 optimization_metric: str = '',
-                 validation_fraction: float = 0.1,
-                 cross_folds: int = 0,
-                 clusters: int = 0,
-                 test_fraction: float = 0.0,
-                 test_latin_hypercube: bool = True,
-                 entity_set: Optional[Union[str, Dict]] = None,
-                 scope: Optional[Union[str, Dict]] = None,
-                 as_request: bool = False,
-                 request_source: Optional[str] = 'manually by user',
-                 activity: Optional[str] = None,
-                 **kwargs) -> Any:
+    def ml_train(
+        self,
+        model_name: str,
+        time_to_train: int = 5,
+        complete_case_only: bool = True,
+        per_entity: bool = False,
+        normalization: str = "Auto",
+        trainers: Optional[Union[str, List[str]]] = None,
+        optimization_metric: str = "",
+        validation_fraction: float = 0.1,
+        cross_folds: int = 0,
+        clusters: int = 0,
+        test_fraction: float = 0.0,
+        test_latin_hypercube: bool = True,
+        entity_set: Optional[Union[str, Dict]] = None,
+        scope: Optional[Union[str, Dict]] = None,
+        as_request: bool = False,
+        request_source: Optional[str] = "manually by user",
+        activity: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Get ML post-training statistics
 
         Parameters
         ----------
         model_name : str
             ML Model name
@@ -335,197 +355,225 @@
         as_request : bool, default True
             Send train request
         request_source : str, default 'manually by user'
             Source of request
         activity : str
             Name of workflow activity to select best ML Model
         """
-        route = 'MLModels/Train'
+        route = "MLModels/Train"
         request = {
-            'ModelName': model_name,
-            'Options': {
-                'EntitySet': None,
-                'Scope': None,
-                'TestFraction': test_fraction,
-                'TestLatinHypercube': test_latin_hypercube,
-                'ValidationFraction': validation_fraction,
-                'OptimizationMetric': optimization_metric,
-                'TimeToTrain': time_to_train,
-                'NumberOfClusters': clusters,
-                'NumberOfCrossValidationFolds': cross_folds,
-                'TrainersToExclude': [],
-                'NormalizationType': self.get_ml_normalization_type_enum(normalization, **kwargs).name,
-                'CompleteCasesOnly': complete_case_only,
+            "ModelName": model_name,
+            "Options": {
+                "EntitySet": None,
+                "Scope": None,
+                "TestFraction": test_fraction,
+                "TestLatinHypercube": test_latin_hypercube,
+                "ValidationFraction": validation_fraction,
+                "OptimizationMetric": optimization_metric,
+                "TimeToTrain": time_to_train,
+                "NumberOfClusters": clusters,
+                "NumberOfCrossValidationFolds": cross_folds,
+                "TrainersToExclude": [],
+                "NormalizationType": self.get_ml_normalization_type_enum(
+                    normalization, **kwargs
+                ).name,
+                "CompleteCasesOnly": complete_case_only,
             },
-            'IsModelPerEntity': per_entity
+            "IsModelPerEntity": per_entity,
         }
         # define trainers
         if trainers:
             # get trainers for current model type
             ml_model_type = self.ml_model_type(model_name, **kwargs)
             ml_trainers = self.ml_trainers(ml_model_type, **kwargs)
             # define trainers to exclude
             if not isinstance(trainers, list):
                 trainers = ApiHelper.to_list(trainers)
-            request['TrainersToExclude'] = [t for t in ml_trainers if t in trainers]
+            request["TrainersToExclude"] = [t for t in ml_trainers if t in trainers]
         # define training 'EntitySet'
         if entity_set:
             if isinstance(entity_set, str):
                 entity_set = self.get_item(ItemType.EntitySet, entity_set, **kwargs)
-            request['EntitySet'] = entity_set
+            request["EntitySet"] = entity_set
         # define training 'Scope'
         if scope:
             if isinstance(scope, str):
                 scope = self.get_item(ItemType.Scope, scope, **kwargs)
-            request['Scope'] = scope
+            request["Scope"] = scope
         # update options
-        request['Options'] = ApiHelper.update_dict(request['Options'], **kwargs)
+        request["Options"] = ApiHelper.update_dict(request["Options"], **kwargs)
         if as_request:
-            request['WorkspaceName'] = self.Workspace
-            request['Source'] = request_source
+            request["WorkspaceName"] = self.Workspace
+            request["Source"] = request_source
             if activity:
-                request['Activity'] = activity
-            self.post(f'{route}/AddRequest', data=request, **kwargs)
+                request["Activity"] = activity
+            self.post(f"{route}/AddRequest", data=request, **kwargs)
         return self.post(route, data=request, **kwargs)
 
     # check whether ML service is idle
     def ml_is_service_idle(self, **kwargs) -> Any:
         """
         Is ML service idle
 
         Parameters
         ----------
         """
-        route = 'ModelTraining/Idle'
+        route = "ModelTraining/Idle"
         return self.get(route, **kwargs)
 
     # get ML model training states
-    def ml_get_model_training_states(self, exclude_processed: bool = False, **kwargs) -> Any:
+    def ml_get_model_training_states(
+        self, exclude_processed: bool = False, **kwargs
+    ) -> Any:
         """
         Get ML model training states
 
         Parameters
         ----------
         exclude_processed : bool, default False
             Exclude processed states
         """
-        route = 'ModelTraining'
+        route = "ModelTraining"
         if exclude_processed:
             self.get(f"{route}/NoProcessed", **kwargs)
         return self.get(route, **kwargs)
 
     # get ML model id
-    def ml_get_model_training_id(self, model_name_or_id: Union[str, UUID], **kwargs) -> Any:
+    def ml_get_model_training_id(
+        self, model_name_or_id: Union[str, UUID], **kwargs
+    ) -> Any:
         """
         Get ML model training id
 
         Parameters
         ----------
         model_name_or_id : str, UUID
             ML Model name or ML Model Training Process UUID
         """
         mid = model_name_or_id
         if isinstance(model_name_or_id, str):
-            ml_training_states = self.ml_get_model_training_states(exclude_processed=False, **kwargs)
+            ml_training_states = self.ml_get_model_training_states(
+                exclude_processed=False, **kwargs
+            )
             mid = None
             for state in ml_training_states:
-                if state['ModelName'].lower() == model_name_or_id.lower():
-                    mid = state['Id']
+                if state["ModelName"].lower() == model_name_or_id.lower():
+                    mid = state["Id"]
         if mid is None:
-            raise ValueError(f"PetroVisor::ml_get_model_training_id(): "
-                             f"couldn't find '{model_name_or_id}' in the training list!")
+            raise ValueError(
+                f"PetroVisor::ml_get_model_training_id(): "
+                f"couldn't find '{model_name_or_id}' in the training list!"
+            )
         return ApiHelper.get_uuid(mid)
 
     # get ML model training state
-    def ml_get_model_training_state(self, model_name_or_id: Union[str, UUID], **kwargs) -> Any:
+    def ml_get_model_training_state(
+        self, model_name_or_id: Union[str, UUID], **kwargs
+    ) -> Any:
         """
         Get ML model training state
 
         Parameters
         ----------
         model_name_or_id : str, UUId
             ML Model name or ML Model Training Process UUID
         """
-        route = 'ModelTraining'
+        route = "ModelTraining"
         uuid = self.ml_get_model_training_id(model_name_or_id, **kwargs)
         return self.get(f"{route}/{self.encode(uuid)}", **kwargs)
 
     # get ML model training results
-    def ml_get_model_training_results(self, model_name_or_id: Union[str, UUID], **kwargs) -> Any:
+    def ml_get_model_training_results(
+        self, model_name_or_id: Union[str, UUID], **kwargs
+    ) -> Any:
         """
         Get ML model training results
 
         Parameters
         ----------
         model_name_or_id : str, UUId
             ML Model name or ML Model Training Process UUID
         """
-        route = 'ModelTraining/Results'
+        route = "ModelTraining/Results"
         uuid = self.ml_get_model_training_id(model_name_or_id, **kwargs)
         return self.get(f"{route}/{self.encode(uuid)}", **kwargs)
 
     # get ML Model Type enum
-    def get_ml_model_type_enum(self, type: Union[str, MLModelType], **kwargs) -> MLModelType:
+    def get_ml_model_type_enum(
+        self, type: Union[str, MLModelType], **kwargs
+    ) -> MLModelType:
         """
         Get ML Model Type
 
         Parameters
         ----------
         type : str, MLModelType
             ML Model type
         """
         if isinstance(type, MLModelType):
             return type
         # prepare name for comparison
         type = ApiHelper.get_comparison_string(type, **kwargs)
-        if type in ('regression', 'reg'):
+        if type in ("regression", "reg"):
             return MLModelType.Regression
-        elif type in ('binaryclassification', 'binaryclass', 'binclass', 'bin'):
+        elif type in ("binaryclassification", "binaryclass", "binclass", "bin"):
             return MLModelType.BinaryClassification
-        elif type in ('multipleclassification', 'multiclassification', 'multipleclass',
-                      'multiclass', 'multiple', 'multi'):
+        elif type in (
+            "multipleclassification",
+            "multiclassification",
+            "multipleclass",
+            "multiclass",
+            "multiple",
+            "multi",
+        ):
             return MLModelType.MultipleClassification
-        elif type in ('clustering', 'cluster'):
+        elif type in ("clustering", "cluster"):
             return MLModelType.Clustering
-        elif type in ('naivebayes', 'bayes'):
+        elif type in ("naivebayes", "bayes"):
             return MLModelType.NaiveBayes
-        elif type in ('naivebayescategorical', 'bayescategorical'):
+        elif type in ("naivebayescategorical", "bayescategorical"):
             return MLModelType.NaiveBayesCategorical
-        raise ValueError(f"PetroVisor::get_ml_model_enum(): "
-                         f"unknown data type: '{type}'! "
-                         f"Should be one of: {[t.name for t in MLModelType]}")
+        raise ValueError(
+            f"PetroVisor::get_ml_model_enum(): "
+            f"unknown data type: '{type}'! "
+            f"Should be one of: {[t.name for t in MLModelType]}"
+        )
 
     # get ML Normalization Type enum
-    def get_ml_normalization_type_enum(self, type: Union[str, MLNormalizationType], **kwargs) -> MLNormalizationType:
+    def get_ml_normalization_type_enum(
+        self, type: Union[str, MLNormalizationType], **kwargs
+    ) -> MLNormalizationType:
         """
         Get ML Normalization Type
 
         Parameters
         ----------
         type : str, MLNormalizationType
             ML Normalization type
         """
         if isinstance(type, MLNormalizationType):
             return type
         # prepare name for comparison
         type = ApiHelper.get_comparison_string(type, **kwargs)
-        if type in ('auto', 'automatic'):
+        if type in ("auto", "automatic"):
             return MLNormalizationType.Auto
-        elif type in ('minmax',):
+        elif type in ("minmax",):
             return MLNormalizationType.MinMax
-        elif type in ('meanvariance', 'meanvar'):
+        elif type in ("meanvariance", "meanvar"):
             return MLNormalizationType.MeanVariance
-        elif type in ('logmeanvariance', 'logmeanvar'):
+        elif type in ("logmeanvariance", "logmeanvar"):
             return MLNormalizationType.LogMeanVariance
-        elif type in ('binning', 'bin'):
+        elif type in ("binning", "bin"):
             return MLNormalizationType.Binning
-        elif type in ('supervisedbinning', 'supervisedbin', 'superbin'):
+        elif type in ("supervisedbinning", "supervisedbin", "superbin"):
             return MLNormalizationType.SupervisedBinning
-        elif type in ('robustscaling', 'robust'):
+        elif type in ("robustscaling", "robust"):
             return MLNormalizationType.RobustScaling
-        elif type in ('lpnorm', 'lp'):
+        elif type in ("lpnorm", "lp"):
             return MLNormalizationType.LpNorm
-        elif type in ('globalcontrast', 'contrast'):
+        elif type in ("globalcontrast", "contrast"):
             return MLNormalizationType.GlobalContrast
-        raise ValueError(f"PetroVisor::get_ml_normalization_enum(): "
-                         f"unknown data type: '{type}'! "
-                         f"Should be one of: {[t.name for t in MLNormalizationType]}")
+        raise ValueError(
+            f"PetroVisor::get_ml_normalization_enum(): "
+            f"unknown data type: '{type}'! "
+            f"Should be one of: {[t.name for t in MLNormalizationType]}"
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/pivot_tables.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/pivot_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     SupportsItemRequests,
     SupportsSignalsRequests,
     SupportsDataFrames,
 )
 
 
 # Pivot Table API calls
-class PivotTableMixin(SupportsDataFrames, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests):
+class PivotTableMixin(
+    SupportsDataFrames, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests
+):
     """
     Pivot Table API calls
     """
 
     # get pivot table names
     def get_pivot_table_names(self, **kwargs) -> Any:
         """
@@ -39,22 +41,24 @@
         ----------
         name : str
             Pivot table name
         """
         return self.get_item(ItemType.PivotTable, name, **kwargs)
 
     # load pivot table data
-    def load_pivot_table_data(self,
-                              name: str,
-                              entity_set: Optional[Union[str, Dict]] = None,
-                              scope: Optional[Union[str, Dict]] = None,
-                              num_rows: Optional[int] = 0,
-                              generate: bool = False,
-                              groupby_entity: bool = False,
-                              **kwargs) -> Any:
+    def load_pivot_table_data(
+        self,
+        name: str,
+        entity_set: Optional[Union[str, Dict]] = None,
+        scope: Optional[Union[str, Dict]] = None,
+        num_rows: Optional[int] = 0,
+        generate: bool = False,
+        groupby_entity: bool = False,
+        **kwargs,
+    ) -> Any:
         """
         Load pivot table and return DataFrame
 
         Parameters
         ----------
         name : str
             Pivot table name
@@ -65,94 +69,117 @@
         num_rows : int, default 0
             Number of rows to load
         generate : bool, default False
             Generate pivot table, otherwise load saved
         groupby_entity : bool, default False
             Return dictionary of DataFrames grouped by entity name
         """
-        route = 'PivotTables'
+        route = "PivotTables"
         if generate or entity_set or scope:
             options = {}
             if entity_set:
                 entity_set_name = ApiHelper.get_object_name(entity_set, **kwargs)
-                options['OverrideEntitySet'] = self.get_item(ItemType.EntitySet, entity_set_name, **kwargs)
+                options["OverrideEntitySet"] = self.get_item(
+                    ItemType.EntitySet, entity_set_name, **kwargs
+                )
             if scope:
                 scope_name = ApiHelper.get_object_name(scope, **kwargs)
-                options['OverrideScope'] = self.get_item(ItemType.Scope, scope_name, **kwargs)
+                options["OverrideScope"] = self.get_item(
+                    ItemType.Scope, scope_name, **kwargs
+                )
             if options:
-                pivot_table_data = self.get(f'{route}/{self.encode(name)}/Generated/Options', data=options, **kwargs)
+                pivot_table_data = self.get(
+                    f"{route}/{self.encode(name)}/Generated/Options",
+                    data=options,
+                    **kwargs,
+                )
             else:
-                pivot_table_data = self.get(f'{route}/{self.encode(name)}/Generated', **kwargs)
+                pivot_table_data = self.get(
+                    f"{route}/{self.encode(name)}/Generated", **kwargs
+                )
         else:
-            pivot_table_data = self.get(f'{route}/{self.encode(name)}/Saved',
-                                        query={
-                                            'RowCount': self.get_json_valid_value(num_rows, 'numeric')
-                                        },
-                                        **kwargs)
+            pivot_table_data = self.get(
+                f"{route}/{self.encode(name)}/Saved",
+                query={"RowCount": self.get_json_valid_value(num_rows, "numeric")},
+                **kwargs,
+            )
         if pivot_table_data:
-            return self.convert_pivot_table_to_dataframe(pivot_table_data, groupby_entity=groupby_entity, **kwargs)
-
-        warnings.warn(f"PetroVisor::load_pivot_table_data(): "
-                      f"Pivot table '{name}' might be not saved, please try to generate data instead.",
-                      RuntimeWarning, stacklevel=1)
+            return self.convert_pivot_table_to_dataframe(
+                pivot_table_data, groupby_entity=groupby_entity, **kwargs
+            )
+
+        warnings.warn(
+            f"PetroVisor::load_pivot_table_data(): "
+            f"Pivot table '{name}' might be not saved, please try to generate data instead.",
+            RuntimeWarning,
+            stacklevel=1,
+        )
 
         return None
 
     # save pivot table data
-    def save_pivot_table_data(self,
-                              name: str,
-                              entity_set: Optional[str] = None,
-                              scope: Optional[str] = None,
-                              **kwargs) -> Any:
+    def save_pivot_table_data(
+        self,
+        name: str,
+        entity_set: Optional[str] = None,
+        scope: Optional[str] = None,
+        **kwargs,
+    ) -> Any:
         """
         Save pivot table data
 
         Parameters
         ----------
         name : str
             Pivot table name
         entity_set : str, dict, default None
             EntitySet object or EntitySet name. If None, the EntitySet from PivotTable definition is used.
         scope : str, dict, default None
             Scope object or Scope name. If None, the Scope from PivotTable definition is used.
         """
-        route = 'PivotTables'
+        route = "PivotTables"
         options = {}
         if entity_set:
             entity_set_name = ApiHelper.get_object_name(entity_set, **kwargs)
-            options['OverrideEntitySet'] = self.get_item(ItemType.EntitySet, entity_set_name, **kwargs)
+            options["OverrideEntitySet"] = self.get_item(
+                ItemType.EntitySet, entity_set_name, **kwargs
+            )
         if scope:
             scope_name = ApiHelper.get_object_name(scope, **kwargs)
-            options['OverrideScope'] = self.get_item(ItemType.Scope, scope_name, **kwargs)
+            options["OverrideScope"] = self.get_item(
+                ItemType.Scope, scope_name, **kwargs
+            )
         if options:
-            self.post(f'{route}/{self.encode(name)}/Save/Options', data=options, **kwargs)
-        return self.get(f'{route}/{self.encode(name)}/Save', **kwargs)
+            self.post(
+                f"{route}/{self.encode(name)}/Save/Options", data=options, **kwargs
+            )
+        return self.get(f"{route}/{self.encode(name)}/Save", **kwargs)
 
     # delete pivot table data
     def delete_pivot_table_data(self, name: str, **kwargs) -> Any:
         """
         Delete pivot table data
 
         Parameters
         ----------
         name : str
             Reference table name
         """
-        route = 'PivotTables'
+        route = "PivotTables"
         if not self.item_exists(ItemType.PivotTable, name):
             return ApiRequests.success()
-        return self.get(f'{route}/{self.encode(name)}/Delete', **kwargs)
+        return self.get(f"{route}/{self.encode(name)}/Delete", **kwargs)
 
     # delete pivot table
     def delete_pivot_table(self, name: str, **kwargs) -> Any:
         """
         Delete pivot table
 
         Parameters
         ----------
         name : str
             Pivot table name
         """
-        route = 'PivotTables'
+        route = "PivotTables"
         if not self.item_exists(ItemType.PivotTable, name):
             return ApiRequests.success()
-        return self.delete(f'{route}/{self.encode(name)}', **kwargs)
+        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/psharp.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/psharp.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,37 +14,43 @@
     SupportsDataFrames,
     SupportsPsharpRequests,
     SupportsItemRequests,
 )
 
 
 # P# API class
-class PsharpMixin(SupportsDataFrames, SupportsPsharpRequests, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests):
+class PsharpMixin(
+    SupportsDataFrames,
+    SupportsPsharpRequests,
+    SupportsSignalsRequests,
+    SupportsItemRequests,
+    SupportsRequests,
+):
     """
     P# API class
     """
 
     # get P# script names
     def get_psharp_script_names(self, **kwargs) -> List[str]:
         """
         Get P# script names
         """
-        return self.get_item_names('PSharpScript', **kwargs)
+        return self.get_item_names("PSharpScript", **kwargs)
 
     # get P# script
     def get_psharp_script(self, name: str, **kwargs) -> Dict:
         """
         Get P# script
 
         Parameters
         ----------
         name : str
             P# script name
         """
-        return self.get(f'PSharpScripts/{self.encode(name)}', **kwargs)
+        return self.get(f"PSharpScripts/{self.encode(name)}", **kwargs)
 
     # get P# script content
     def get_psharp_script_content(self, script: Union[str, Dict], **kwargs) -> str:
         """
         Get P# script content
 
         Parameters
@@ -53,128 +59,138 @@
             P# script object or P# script name
         """
         # get P# script content
         if isinstance(script, str):
             script_content = script
             # check is script is the name of P# script
             script_names = self.get_psharp_script_names(**kwargs)
-            script = self.get_psharp_script(script, **kwargs) if script in script_names else None
+            script = (
+                self.get_psharp_script(script, **kwargs)
+                if script in script_names
+                else None
+            )
         else:
             script_content = None
         if script is None and script_content:
             pass
-        elif 'Content' in script:
-            script_content = script['Content']
+        elif "Content" in script:
+            script_content = script["Content"]
         else:
-            raise ValueError(f"PetroVisor::get_psharp_script_content(): "
-                             f"couldn't get content of P# script '{script}'.")
+            raise ValueError(
+                f"PetroVisor::get_psharp_script_content(): "
+                f"couldn't get content of P# script '{script}'."
+            )
         return script_content
 
     # parse P# script
-    def parse_psharp_script(self,
-                            script: Union[str, Dict],
-                            options: Optional[Dict] = None,
-                            **kwargs) -> Dict:
+    def parse_psharp_script(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> Dict:
         """
         Parse P# script
 
         Parameters
         ----------
         script : str, dict
             P# script object or P# script name
         options : dict, default None
             P# script parse options
         """
         # get P# script content
         script_content = self.get_psharp_script_content(script, **kwargs)
         # define options
         if not options:
-            options = {
-                'TreatScriptContentAsScriptName': False,
-                'NoMissedObjects': True
-            }
+            options = {"TreatScriptContentAsScriptName": False, "NoMissedObjects": True}
             options = ApiHelper.update_dict(options, **kwargs)
-        return self.post('Parsing/Parsed', data={'ScriptContent': script_content, 'Options': options}, **kwargs)
+        return self.post(
+            "Parsing/Parsed",
+            data={"ScriptContent": script_content, "Options": options},
+            **kwargs,
+        )
 
     # get P# script table names
-    def get_psharp_script_table_names(self,
-                                      script: Union[str, Dict],
-                                      options: Optional[Dict] = None,
-                                      **kwargs) -> List[str]:
+    def get_psharp_script_table_names(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> List[str]:
         """
         Get P# script table names
 
         Parameters
         ----------
         script : str, dict
             P# script object or P# script name
         options : dict, default None
             P# script parse options
         """
-        if isinstance(script, str) or 'TableCalculations' not in script:
-            psharp_script_parsed = self.parse_psharp_script(script, options=options, **kwargs)
+        if isinstance(script, str) or "TableCalculations" not in script:
+            psharp_script_parsed = self.parse_psharp_script(
+                script, options=options, **kwargs
+            )
         else:
             psharp_script_parsed = script
-        if 'TableCalculations' in psharp_script_parsed:
-            table_names = [t['Name'] for t in psharp_script_parsed['TableCalculations']]
+        if "TableCalculations" in psharp_script_parsed:
+            table_names = [t["Name"] for t in psharp_script_parsed["TableCalculations"]]
         else:
             table_names = []
         return table_names
 
     # get P# script tables, columns and signals
-    def get_psharp_script_columns_and_signals(self,
-                                              script: Union[str, Dict],
-                                              options: Optional[Dict] = None,
-                                              **kwargs) -> Dict:
+    def get_psharp_script_columns_and_signals(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> Dict:
         """
         Get P# script columns and signals
 
         Parameters
         ----------
         script : str, dict
             P# script object or P# script name
         options : dict, default None
             P# script parse options
         """
-        if isinstance(script, str) or 'TableCalculations' not in script:
-            psharp_script_parsed = self.parse_psharp_script(script, options=options, **kwargs)
+        if isinstance(script, str) or "TableCalculations" not in script:
+            psharp_script_parsed = self.parse_psharp_script(
+                script, options=options, **kwargs
+            )
         else:
             psharp_script_parsed = script
         # get psharp script signals
         table_signals = {}
-        if 'TableCalculations' in psharp_script_parsed:
-            for t in psharp_script_parsed['TableCalculations']:
-                table_name = t['Name']
-                table_columns = t['Columns']
+        if "TableCalculations" in psharp_script_parsed:
+            for t in psharp_script_parsed["TableCalculations"]:
+                table_name = t["Name"]
+                table_columns = t["Columns"]
                 table_signals[table_name] = {}
                 for col in table_columns:
-                    col_name = col['Name']
-                    unit_name = col['Unit']['Name']
+                    col_name = col["Name"]
+                    unit_name = col["Unit"]["Name"]
                     # full_column_name = col_name + ' ' + '[' + unit_name + ']'
-                    col_formula = col['Formula']
+                    col_formula = col["Formula"]
                     col_signal = col_formula.split('"')
-                    signal_name = col_signal[1] if len(col_signal) > 1 else ''
-                    signal_unit_name = col_signal[3] if len(col_signal) > 3 else ' '
+                    signal_name = col_signal[1] if len(col_signal) > 1 else ""
+                    signal_unit_name = col_signal[3] if len(col_signal) > 3 else " "
                     # table_signals[table_name][full_column_name] = {'Signal': signal_name, 'Unit': signal_unit_name}
                     table_signals[table_name][col_name] = {
-                        'Unit': unit_name,
-                        'Signal': signal_name,
-                        'SignalUnit': signal_unit_name
+                        "Unit": unit_name,
+                        "Signal": signal_name,
+                        "SignalUnit": signal_unit_name,
                     }
         return table_signals
 
     # load P# table
-    def load_psharp_table(self,
-                          script_name: str,
-                          table: Optional[str] = None,
-                          dropna: bool = True,
-                          with_entity_column: bool = True,
-                          groupby_entity: bool = False,
-                          load_full_table_info: bool = False,
-                          **kwargs) -> Optional[Union[pd.DataFrame, List[pd.DataFrame], Dict[str, pd.DataFrame]]]:
+    def load_psharp_table(
+        self,
+        script_name: str,
+        table: Optional[str] = None,
+        dropna: bool = True,
+        with_entity_column: bool = True,
+        groupby_entity: bool = False,
+        load_full_table_info: bool = False,
+        **kwargs,
+    ) -> Optional[Union[pd.DataFrame, List[pd.DataFrame], Dict[str, pd.DataFrame]]]:
         """
         Load P# table and return DataFrame
 
         Parameters
         ----------
         script_name : str
             P# script name
@@ -202,87 +218,111 @@
             if table_name not in table_names:
                 return None
         else:
             # get table id
             try:
                 table_id = int(table)
             except BaseException:
-                raise ValueError(f"PetroVisor::load_table_from_psharp(): "
-                                 f"{table} should be either 'string'(table name), 'integer'(table id) "
-                                 f"or 'None'(all tables) !")
+                raise ValueError(
+                    f"PetroVisor::load_table_from_psharp(): "
+                    f"{table} should be either 'string'(table name), 'integer'(table id) "
+                    f"or 'None'(all tables) !"
+                )
             # return None if table id is out of range
             num_tables = len(table_names)
             if table_id >= num_tables or (num_tables + table_id) < 0:
-                raise ValueError(f"PetroVisor::load_table_from_psharp(): "
-                                 f"table id '{table}' is out of range. "
-                                 f"There are {num_tables} tables in current P# script!")
+                raise ValueError(
+                    f"PetroVisor::load_table_from_psharp(): "
+                    f"table id '{table}' is out of range. "
+                    f"There are {num_tables} tables in current P# script!"
+                )
             # get table name
             table_name = table_names[table_id]
 
         # read single table from P# script
         if table_name and dropna:
             if with_entity_column:
-                psharp_table = self.get(f'PSharpScripts/{self.encode(script_name)}/ExecuteAsBITable',
-                                        query={'Table': table_name}, **kwargs)
+                psharp_table = self.get(
+                    f"PSharpScripts/{self.encode(script_name)}/ExecuteAsBITable",
+                    query={"Table": table_name},
+                    **kwargs,
+                )
             else:
-                psharp_table = self.get(f'PSharpScripts/{self.encode(script_name)}/ExecuteAsTable',
-                                        query={'Table': table_name}, **kwargs)
+                psharp_table = self.get(
+                    f"PSharpScripts/{self.encode(script_name)}/ExecuteAsTable",
+                    query={"Table": table_name},
+                    **kwargs,
+                )
             if psharp_table is not None:
-                return self.convert_psharp_table_to_dataframe(psharp_table,
-                                                              with_entity_column=with_entity_column,
-                                                              groupby_entity=groupby_entity,
-                                                              dropna=dropna,
-                                                              **kwargs)
+                return self.convert_psharp_table_to_dataframe(
+                    psharp_table,
+                    with_entity_column=with_entity_column,
+                    groupby_entity=groupby_entity,
+                    dropna=dropna,
+                    **kwargs,
+                )
         else:
             psharp_table = None
 
         # read multiple tables from P# script
         # if with_entity_column:
         #     psharp_tables = [self.get(f'PSharpScripts/{script_name}/ExecuteAsBITable',
         #                               query={'Table': table_name}, **kwargs)
         #                      for table_name in table_names]
         # else:
         #     psharp_tables = [self.get(f'PSharpScripts/{script_name}/ExecuteAsTable',
         #                               query={'Table': table_name}, **kwargs)
         #                      for table_name in table_names]
         script_content = self.get_psharp_script_content(script_name, **kwargs)
         if load_full_table_info:
-            psharp_tables = self.post('PSharpScripts/ExecuteScript',
-                                      data={'ScriptContent': script_content}, **kwargs)
+            psharp_tables = self.post(
+                "PSharpScripts/ExecuteScript",
+                data={"ScriptContent": script_content},
+                **kwargs,
+            )
         else:
-            psharp_tables = self.post('PSharpScripts/Execute',
-                                      data={'ScriptContent': script_content}, **kwargs)
+            psharp_tables = self.post(
+                "PSharpScripts/Execute",
+                data={"ScriptContent": script_content},
+                **kwargs,
+            )
 
         # return single table
         if table_name:
-            return self.convert_psharp_table_to_dataframe(psharp_tables[table_names.index(table_name)],
-                                                          with_entity_column=with_entity_column,
-                                                          groupby_entity=groupby_entity,
-                                                          dropna=dropna,
-                                                          **kwargs)
+            return self.convert_psharp_table_to_dataframe(
+                psharp_tables[table_names.index(table_name)],
+                with_entity_column=with_entity_column,
+                groupby_entity=groupby_entity,
+                dropna=dropna,
+                **kwargs,
+            )
         # return multiple tables
         return {
-            table_name: self.convert_psharp_table_to_dataframe(t,
-                                                               with_entity_column=with_entity_column,
-                                                               groupby_entity=groupby_entity,
-                                                               dropna=dropna,
-                                                               **kwargs)
+            table_name: self.convert_psharp_table_to_dataframe(
+                t,
+                with_entity_column=with_entity_column,
+                groupby_entity=groupby_entity,
+                dropna=dropna,
+                **kwargs,
+            )
             for table_name, t in zip(table_names, psharp_tables)
         }
 
     # save data from table to PetroVisor
-    def save_table_data(self,
-                        df: pd.DataFrame,
-                        delimiter: str = '\t',
-                        signals: Optional[Dict] = None,
-                        chunksize: int = 10000,
-                        only_existing_entities: bool = True,
-                        entity_type: str = '',
-                        entities: Optional[Dict] = None,
-                        **kwargs) -> None:
+    def save_table_data(
+        self,
+        df: pd.DataFrame,
+        delimiter: str = "\t",
+        signals: Optional[Dict] = None,
+        chunksize: int = 10000,
+        only_existing_entities: bool = True,
+        entity_type: str = "",
+        entities: Optional[Dict] = None,
+        **kwargs,
+    ) -> None:
         """
         Save DataFrame data to corresponding signals
 
         Parameters
         ----------
         df : DataFrame, str
             Table or filename. Table should contain necessary columns 'Entity', 'Date' or 'Depth',
@@ -299,28 +339,44 @@
             Save data only if entity exist in workspace
         entity_type : str, default None
             Save data only for specified entity type
         """
         # read table
         if isinstance(df, str):
             ext = ApiHelper.get_file_extension(df, **kwargs)
-            if ext.lower() in ['.xlsx', '.xls']:
+            if ext.lower() in [".xlsx", ".xls"]:
                 df = pd.read_excel(df)
             else:  # elif(ext.lower() in ['.csv']):
                 df = pd.read_csv(df, delimiter=delimiter)
         if df is not None:
             if chunksize and (df.shape[0] > chunksize):
                 for start in range(0, df.shape[0], chunksize):
                     end = min(start + chunksize, df.shape[0])
-                    self.save_table_data(df[start:end], delimiter=delimiter, signals=signals, chunksize=chunksize,
-                                         only_existing_entities=only_existing_entities, entity_type=entity_type,
-                                         entities=entities, **kwargs)
+                    self.save_table_data(
+                        df[start:end],
+                        delimiter=delimiter,
+                        signals=signals,
+                        chunksize=chunksize,
+                        only_existing_entities=only_existing_entities,
+                        entity_type=entity_type,
+                        entities=entities,
+                        **kwargs,
+                    )
                 return None
             # get PetroVisor data from DataFrame
-            data_to_save = self.get_signal_data_from_dataframe(df, signals=signals,
-                                                               only_existing_entities=only_existing_entities,
-                                                               entity_type=entity_type, entities=entities, **kwargs)
+            data_to_save = self.get_signal_data_from_dataframe(
+                df,
+                signals=signals,
+                only_existing_entities=only_existing_entities,
+                entity_type=entity_type,
+                entities=entities,
+                **kwargs,
+            )
             # save data
             for data_type, data in data_to_save.items():
                 if data:
-                    self.post(f'{self.get_signal_type_route(data_type)}/Save', data=data, **kwargs)
+                    self.post(
+                        f"{self.get_signal_type_route(data_type)}/Save",
+                        data=data,
+                        **kwargs,
+                    )
         return None
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/reference_tables.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/reference_tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,37 @@
     Dict,
 )
 
 from datetime import datetime
 import time
 import pandas as pd
 import numpy as np
-from pandas.api.types import is_bool_dtype, is_numeric_dtype, is_string_dtype, is_datetime64_dtype
+from pandas.api.types import (
+    is_bool_dtype,
+    is_numeric_dtype,
+    is_string_dtype,
+    is_datetime64_dtype,
+)
 
 from petrovisor.api.dtypes.internal_dtypes import RefTableColumnType
 from petrovisor.api.utils.helper import ApiHelper
 from petrovisor.api.utils.requests import ApiRequests
 from petrovisor.api.dtypes.items import ItemType
 from petrovisor.api.protocols.protocols import (
     SupportsRequests,
     SupportsItemRequests,
     SupportsSignalsRequests,
     SupportsDataFrames,
 )
 
 
 # Reference Table API calls
-class RefTableMixin(SupportsDataFrames, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests):
+class RefTableMixin(
+    SupportsDataFrames, SupportsSignalsRequests, SupportsItemRequests, SupportsRequests
+):
     """
     Reference Table API calls
     """
 
     # get reference table names
     def get_ref_table_names(self, **kwargs) -> Any:
         """
@@ -46,23 +53,26 @@
         ----------
         name : str
             Reference table name
         """
         return self.get_item(ItemType.RefTable, name, **kwargs)
 
     # add reference table
-    def add_ref_table(self, name: str,
-                      df: Union[pd.DataFrame, Dict],
-                      description: Optional[str] = None,
-                      key_col: Optional[str] = 'Key',
-                      date_col: Optional[str] = None,
-                      entity_col: Optional[str] = 'Entity',
-                      skip_existing_data=False,
-                      chunksize=None,
-                      **kwargs) -> Any:
+    def add_ref_table(
+        self,
+        name: str,
+        df: Union[pd.DataFrame, Dict],
+        description: Optional[str] = None,
+        key_col: Optional[str] = "Key",
+        date_col: Optional[str] = None,
+        entity_col: Optional[str] = "Entity",
+        skip_existing_data=False,
+        chunksize=None,
+        **kwargs,
+    ) -> Any:
         """
         Add reference table from provided DataFrame.
         If reference table already exists the provided DataFrame should follow the exact same schema.
 
         Parameters
         ----------
         name : str
@@ -87,98 +97,113 @@
 
         # add definition if it doesn't exists
         is_empty = df.empty
         if not self.item_exists(ItemType.RefTable, name):
 
             # date column
             df_date_cols = set()
-            for col in RefTableMixinHelper.get_set(date_col, default={'Date', 'Timestamp', 'Time'}):
+            for col in RefTableMixinHelper.get_set(
+                date_col, default={"Date", "Timestamp", "Time"}
+            ):
                 if col in df.columns:
                     df_date_cols.add(col)
-            if 'Timestamp' in df_date_cols:
-                df_date_col = 'Timestamp'
-            elif 'Date' in df_date_cols:
-                df_date_col = 'Date'
-            elif 'Time' in df_date_cols:
-                df_date_col = 'Time'
+            if "Timestamp" in df_date_cols:
+                df_date_col = "Timestamp"
+            elif "Date" in df_date_cols:
+                df_date_col = "Date"
+            elif "Time" in df_date_cols:
+                df_date_col = "Time"
             else:
                 df_date_col = df_date_cols.pop() if df_date_cols else None
 
             # entity column
             df_entity_cols = set()
-            for col in RefTableMixinHelper.get_set(entity_col, default='Entity'):
+            for col in RefTableMixinHelper.get_set(entity_col, default="Entity"):
                 if col in df.columns:
                     df_entity_cols.add(col)
-            if 'Entity' in df_entity_cols:
-                df_entity_col = 'Entity'
+            if "Entity" in df_entity_cols:
+                df_entity_col = "Entity"
             else:
                 df_entity_col = df_entity_cols.pop() if df_entity_cols else None
 
             # key column
             df_key_cols = set()
-            for col in RefTableMixinHelper.get_set(key_col, default='Key'):
+            for col in RefTableMixinHelper.get_set(key_col, default="Key"):
                 if col in df.columns:
                     df_key_cols.add(col)
-            if 'Key' in df_key_cols:
-                df_key_col = 'Key'
+            if "Key" in df_key_cols:
+                df_key_col = "Key"
             elif df_key_cols:
                 df_key_col = df_key_cols.pop()
             else:
-                raise ValueError("PetroVisor::add_ref_table(): "
-                                 "'Key' column is not specified")
+                raise ValueError(
+                    "PetroVisor::add_ref_table(): " "'Key' column is not specified"
+                )
 
             # reserved column names: "ID", "Timestamp", "Entity"
-            reserved_columns = {'ID', 'Entity', 'Timestamp'}
+            reserved_columns = {"ID", "Entity", "Timestamp"}
             if df_date_col:
                 reserved_columns = reserved_columns.union({df_date_col})
             if df_entity_col:
                 reserved_columns = reserved_columns.union({df_entity_col})
             reserved_columns = reserved_columns.union({df_key_col})
             value_columns = [col for col in df.columns if col not in reserved_columns]
             column_types = df.dtypes
             options = {
-                'Name': name,
-                'Description': description or "",
-                'Key': {
-                    'Name': df_key_col,
-                    'UnitName': self.get_column_unit(df_key_col) or ' ',
-                    'ColumnType': RefTableMixinHelper.get_ref_table_column_type(column_types[df_key_col]),
+                "Name": name,
+                "Description": description or "",
+                "Key": {
+                    "Name": df_key_col,
+                    "UnitName": self.get_column_unit(df_key_col) or " ",
+                    "ColumnType": RefTableMixinHelper.get_ref_table_column_type(
+                        column_types[df_key_col]
+                    ),
                 },
-                'Values': [{'Name': col,
-                            'UnitName': self.get_column_unit(col) or ' ',
-                            'ColumnType': RefTableMixinHelper.get_ref_table_column_type(column_types[col]),
-                            } for col in value_columns],
+                "Values": [
+                    {
+                        "Name": col,
+                        "UnitName": self.get_column_unit(col) or " ",
+                        "ColumnType": RefTableMixinHelper.get_ref_table_column_type(
+                            column_types[col]
+                        ),
+                    }
+                    for col in value_columns
+                ],
             }
             options = ApiHelper.update_dict(options, **kwargs)
             result = self.add_item(ItemType.RefTable, options, **kwargs)
             if is_empty:
                 return result
         if is_empty:
             return ApiRequests.success()
         # save data to already exists RefTable
         waiting_time = 3  # in seconds
         while not self.item_exists(ItemType.RefTable, name):
             time.sleep(waiting_time)
-        return self.save_ref_table_data(name,
-                                        df,
-                                        skip_existing_data=skip_existing_data,
-                                        chunksize=chunksize,
-                                        **kwargs)
+        return self.save_ref_table_data(
+            name,
+            df,
+            skip_existing_data=skip_existing_data,
+            chunksize=chunksize,
+            **kwargs,
+        )
 
     # load reference table data
-    def load_ref_table_data(self,
-                            name: str,
-                            entity: Optional[Union[str, Dict, List[str], List[Dict]]] = None,
-                            date_start: Optional[Union[datetime, str]] = None,
-                            date_end: Optional[Union[datetime, str]] = None,
-                            where_expression: Optional[str] = None,
-                            date_col: Optional[str] = 'Timestamp',
-                            entity_col: Optional[str] = 'Entity',
-                            options: Optional[Dict] = None,
-                            **kwargs) -> pd.DataFrame:
+    def load_ref_table_data(
+        self,
+        name: str,
+        entity: Optional[Union[str, Dict, List[str], List[Dict]]] = None,
+        date_start: Optional[Union[datetime, str]] = None,
+        date_end: Optional[Union[datetime, str]] = None,
+        where_expression: Optional[str] = None,
+        date_col: Optional[str] = "Timestamp",
+        entity_col: Optional[str] = "Entity",
+        options: Optional[Dict] = None,
+        **kwargs,
+    ) -> pd.DataFrame:
         """
         Load reference table data
 
         Parameters
         ----------
         name : str
             Reference table name
@@ -193,66 +218,81 @@
         date_col : str, default 'Date'
             Date column name. Default names 'Date' (compatible with date column in P# table), 'Timestamp' (compatible with the internal time column name in RefTable), 'Time' (typically used as displayed name)
         entity_col : str, default 'Entity'
             Entity column name
         options : dict, None, default Noe
             Options to retrieve data
         """
-        route = 'RefTables'
+        route = "RefTables"
         filter_options = options if options else {}
         if entity:
-            if isinstance(entity, (list, tuple, set, )):
-                filter_options['Entities'] = [ApiHelper.get_object_name(entity) for e in entity]
+            if isinstance(
+                entity,
+                (
+                    list,
+                    tuple,
+                    set,
+                ),
+            ):
+                filter_options["Entities"] = [
+                    ApiHelper.get_object_name(entity) for e in entity
+                ]
             else:
-                filter_options['Entity'] = ApiHelper.get_object_name(entity)
+                filter_options["Entity"] = ApiHelper.get_object_name(entity)
         if date_start and date_end:
-            date_start = self.get_json_valid_value(date_start, 'time', **kwargs) or ''
-            date_end = self.get_json_valid_value(date_start, 'time', **kwargs) or ''
+            date_start = self.get_json_valid_value(date_start, "time", **kwargs) or ""
+            date_end = self.get_json_valid_value(date_start, "time", **kwargs) or ""
             if date_start and not date_end:
-                filter_options['Timestamp'] = date_end
+                filter_options["Timestamp"] = date_end
             elif not date_start and date_end:
-                filter_options['Timestamp'] = date_end
+                filter_options["Timestamp"] = date_end
             elif date_start and date_end:
-                filter_options['StartTimestamp'] = date_start
-                filter_options['EndTimestamp'] = date_end
+                filter_options["StartTimestamp"] = date_start
+                filter_options["EndTimestamp"] = date_end
         if where_expression:
-            filter_options['WhereExpression'] = where_expression
+            filter_options["WhereExpression"] = where_expression
         filter_options = ApiHelper.update_dict(filter_options, **kwargs)
 
         # get filtered data
-        data = self.post(f'{route}/{self.encode(name)}/Data', data=filter_options, **kwargs)
+        data = self.post(
+            f"{route}/{self.encode(name)}/Data", data=filter_options, **kwargs
+        )
         ref_table_info = self.get_ref_table_data_info(name)
-        columns = [f"{d['Name']} [{d['UnitName']}]" for d in ref_table_info['Values']]
-        key_column = f"{ref_table_info['Key']['Name']} [{ref_table_info['Key']['UnitName']}]"
-        columns = [entity_col or 'Entity', date_col or 'Date', key_column, *columns]
+        columns = [f"{d['Name']} [{d['UnitName']}]" for d in ref_table_info["Values"]]
+        key_column = (
+            f"{ref_table_info['Key']['Name']} [{ref_table_info['Key']['UnitName']}]"
+        )
+        columns = [entity_col or "Entity", date_col or "Date", key_column, *columns]
         df = pd.DataFrame(data=data, columns=columns)
         return df
 
     # save data to reference table
-    def save_ref_table_data(self,
-                            name: str,
-                            df: pd.DataFrame,
-                            skip_existing_data: Optional[bool] = False,
-                            chunksize: Optional[int] = None,
-                            **kwargs):
+    def save_ref_table_data(
+        self,
+        name: str,
+        df: pd.DataFrame,
+        skip_existing_data: Optional[bool] = False,
+        chunksize: Optional[int] = None,
+        **kwargs,
+    ):
         """
         Save reference table data
 
         Parameters
         ----------
         name : str
             Reference table name
         df : DataFrame, dict
             DataFrame or dictionary, where keys are column names and values are column values or predefined types, such as 'str', 'float', 'bool', 'datetime64[s]'.
         skip_existing_data : bool, default False
             Whether to skip or overwrite existing data that has same combination of 'Entity', 'Timestamp', 'Key'
         chunksize : int, default None
             Chunk size for splitting request into multiple smaller requests.
         """
-        route = 'RefTables'
+        route = "RefTables"
 
         # create DataFrame in case if it is passed as dictionary
         def create_dataframe(d: Dict):
             df = pd.DataFrame()
             for c, d in d.items():
                 if isinstance(d, (str, type)):
                     df[c] = pd.Series(dtype=d)
@@ -268,80 +308,88 @@
                 # num_chunks = int(math.ceil(df.shape[0] / chunksize))
                 # step = max(1, int(math.floor(0.1 * df.shape[0] / chunksize)))
                 i = 0
 
                 for start in range(0, df.shape[0], chunksize):
                     end = min(start + chunksize, df.shape[0])
 
-                    self.save_ref_table_data(name,
-                                             df[start:end],
-                                             skip_existing_data=skip_existing_data,
-                                             chunksize=chunksize,
-                                             **kwargs)
+                    self.save_ref_table_data(
+                        name,
+                        df[start:end],
+                        skip_existing_data=skip_existing_data,
+                        chunksize=chunksize,
+                        **kwargs,
+                    )
                     i += 1
                 return ApiRequests.success()
             # save data
-            data = df.astype('string').to_json(orient='values')
-            return self.put(f"{route}/{self.encode(name)}/Data/String",
-                            query={'skipExistingData': skip_existing_data},
-                            data=data)
+            data = df.astype("string").to_json(orient="values")
+            return self.put(
+                f"{route}/{self.encode(name)}/Data/String",
+                query={"skipExistingData": skip_existing_data},
+                data=data,
+            )
         return ApiRequests.success()
 
     # delete reference table data
-    def delete_ref_table_data(self,
-                              name: str,
-                              date_start: Optional[Union[datetime, float]] = None,
-                              date_end: Optional[Union[datetime, float]] = None,
-                              **kwargs) -> Any:
+    def delete_ref_table_data(
+        self,
+        name: str,
+        date_start: Optional[Union[datetime, float]] = None,
+        date_end: Optional[Union[datetime, float]] = None,
+        **kwargs,
+    ) -> Any:
         """
         Delete reference table data
 
         Parameters
         ----------
         name : str
             Reference table name
         date_start : str, datetime, None
             Start Date or None
         date_end : str, datetime, None
             End Date or None
         """
-        route = 'RefTables'
+        route = "RefTables"
         if date_start or date_end:
-            date_start = self.get_json_valid_value(date_start, 'time', **kwargs) or ''
-            date_end = self.get_json_valid_value(date_start, 'time', **kwargs) or ''
+            date_start = self.get_json_valid_value(date_start, "time", **kwargs) or ""
+            date_end = self.get_json_valid_value(date_start, "time", **kwargs) or ""
             if date_start and not date_end:
                 date_end = date_start
             elif not date_start and date_end:
                 date_start = date_end
             if date_start and date_end:
                 options = {
-                    'TimestampStart': date_start,
-                    'TimestampEnd': date_end,
-                    'IncludeWithNoTimestamp': False,  # Whether rows without timestamps should be deleted
+                    "TimestampStart": date_start,
+                    "TimestampEnd": date_end,
+                    "IncludeWithNoTimestamp": False,  # Whether rows without timestamps should be deleted
                 }
                 options = ApiHelper.update_dict(options, **kwargs)
-                return self.delete(f'{route}/{self.encode(name)}/Data/Timestamp', query=options, **kwargs)
-        return self.delete(f'{route}/{self.encode(name)}/Data', **kwargs)
+                return self.delete(
+                    f"{route}/{self.encode(name)}/Data/Timestamp",
+                    query=options,
+                    **kwargs,
+                )
+        return self.delete(f"{route}/{self.encode(name)}/Data", **kwargs)
 
     # delete reference table
-    def delete_ref_table(self,
-                         name: str,
-                         **kwargs) -> Any:
+    def delete_ref_table(self, name: str, **kwargs) -> Any:
         """
         Delete reference table
 
         Parameters
         ----------
         name : str
             Reference table name
         """
-        route = 'RefTables'
+        route = "RefTables"
         if not self.item_exists(ItemType.RefTable, name):
             return ApiRequests.success()
-        return self.delete(f'{route}/{self.encode(name)}', **kwargs)
+        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
 
 
 # Reference table mixin helper
 class RefTableMixinHelper:
 
     # create DataFrame in case if it is passed as dictionary
     @staticmethod
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/workflows.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/workflows.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 # Workflows API calls
 class WorkflowsMixin(SupportsRequests):
     """
     Workflows API calls
     """
 
     # run 'Workflow'
-    def run_workflow(self,
-                     workflow: str,
-                     contexts: Optional[List[str]] = None,
-                     scope: str = None,
-                     entity_set: str = None,
-                     schedule_name: str = 'Now',
-                     source: str = 'by Activity service',
-                     **kwargs) -> Any:
+    def run_workflow(
+        self,
+        workflow: str,
+        contexts: Optional[List[str]] = None,
+        scope: str = None,
+        entity_set: str = None,
+        schedule_name: str = "Now",
+        source: str = "by Activity service",
+        **kwargs,
+    ) -> Any:
         """
         Run workflow
 
         Parameters
         ----------
         workflow : str
             Workflow name
@@ -40,25 +42,25 @@
             EntitySet name
         schedule_name : str, default 'Now'
             Schedule name
         source : str, default 'by Activity service'
             Source name
         """
         data = {
-            'WorkflowName': workflow,
-            'WorkspaceName': self.Workspace,
-            'Source': source,
-            'ScheduleName': schedule_name,
-            'ProcessingContexts': contexts if contexts else [],
+            "WorkflowName": workflow,
+            "WorkspaceName": self.Workspace,
+            "Source": source,
+            "ScheduleName": schedule_name,
+            "ProcessingContexts": contexts if contexts else [],
         }
         if scope:
-            data['ProcessingScopeName'] = scope
+            data["ProcessingScopeName"] = scope
         if entity_set:
-            data['ProcessingEntitySet'] = entity_set
-        return self.post('WorkflowExecution/AddRequest', data=data, **kwargs)
+            data["ProcessingEntitySet"] = entity_set
+        return self.post("WorkflowExecution/AddRequest", data=data, **kwargs)
 
     # get 'Workflow' execution state
     def get_workflow_execution_state(self, uid: UUID, **kwargs):
         """
         Get workflow execution state
 
         Parameters
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/methods/workspace_values.py` & `petrovisor-0.1.3/src/petrovisor/api/methods/workspace_values.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,172 +18,194 @@
     """
 
     # get workspace value names
     def get_workspace_value_names(self, **kwargs) -> List[str]:
         """
         Get all workspace value names
         """
-        route = 'ConfigurationSettings'
-        return self.get(f'{route}', **kwargs)
+        route = "ConfigurationSettings"
+        return self.get(f"{route}", **kwargs)
 
     # get workspace values
-    def get_workspace_values(self, value_type: Optional[str] = None, **kwargs) -> Dict[str, Any]:
+    def get_workspace_values(
+        self, value_type: Optional[str] = None, **kwargs
+    ) -> Dict[str, Any]:
         """
         Get all workspace values
 
         Parameters
         ----------
         value_type : str, default None
             Value type: 'Numeric', 'NumericWithUnit', 'String', 'List', 'Dictionary', 'Enumeration'
         """
-        route = 'ConfigurationSettings'
+        route = "ConfigurationSettings"
         if value_type:
             t = ApiHelper.get_comparison_string(value_type)
-            if t in {'numeric'}:
-                value_type = 'Numeric'
-            elif t in {'numericwithunit'}:
-                value_type = 'NumericWithUnit'
-            elif t in {'string', 'str'}:
-                value_type = 'String'
-            elif t in {'list'}:
-                value_type = 'List'
-            elif t in {'dictionary', 'dict'}:
-                value_type = 'Dictionary'
-            elif t in {'enumeration', 'enum'}:
-                value_type = 'Enumeration'
+            if t in {"numeric"}:
+                value_type = "Numeric"
+            elif t in {"numericwithunit"}:
+                value_type = "NumericWithUnit"
+            elif t in {"string", "str"}:
+                value_type = "String"
+            elif t in {"list"}:
+                value_type = "List"
+            elif t in {"dictionary", "dict"}:
+                value_type = "Dictionary"
+            elif t in {"enumeration", "enum"}:
+                value_type = "Enumeration"
             else:
-                raise ValueError(f"PetroVisor::get_workspace_values(): "
-                                 f"unknown workspace value type: '{value_type}'. "
-                                 f"Known workspace value types: "
-                                 f"{WorkspaceValueMixinHelper.get_workspace_value_types()}")
-            values = self.get(f'{route}/{value_type}/{route}', **kwargs)
+                raise ValueError(
+                    f"PetroVisor::get_workspace_values(): "
+                    f"unknown workspace value type: '{value_type}'. "
+                    f"Known workspace value types: "
+                    f"{WorkspaceValueMixinHelper.get_workspace_value_types()}"
+                )
+            values = self.get(f"{route}/{value_type}/{route}", **kwargs)
         else:
-            values = self.get(f'{route}/All', **kwargs)
-        return {value['Name']: WorkspaceValueMixinHelper.get_workspace_value(value, **kwargs) for value in values}
+            values = self.get(f"{route}/All", **kwargs)
+        return {
+            value["Name"]: WorkspaceValueMixinHelper.get_workspace_value(
+                value, **kwargs
+            )
+            for value in values
+        }
 
     # get workspace value
     def get_workspace_value(self, name: str, **kwargs) -> Tuple[Any, str]:
         """
         Get workspace value
 
         Parameters
         ----------
         name : str
             Variable name
         """
-        route = 'ConfigurationSettings'
+        route = "ConfigurationSettings"
         # get workspace value
-        value = self.get(f'{route}/{self.encode(name)}', **kwargs)
+        value = self.get(f"{route}/{self.encode(name)}", **kwargs)
         return WorkspaceValueMixinHelper.get_workspace_value(value, **kwargs)
 
     # add workspace value
-    def add_workspace_value(self,
-                            name: str,
-                            value: Union[str, List[Any], Dict[str, Any], Tuple, float, int],
-                            unit: Union[Dict, str] = '',
-                            description: Optional[str] = '',
-                            **kwargs) -> Any:
+    def add_workspace_value(
+        self,
+        name: str,
+        value: Union[str, List[Any], Dict[str, Any], Tuple, float, int],
+        unit: Union[Dict, str] = "",
+        description: Optional[str] = "",
+        **kwargs,
+    ) -> Any:
         """
         Add or edit workspace value
 
         Parameters
         ----------
         name : str
             Variable name
         value : str | dict | list | enum | float | int
             Variable value
         unit : str
             Unit object or Unit name
         description : str
             Description
         """
-        route = 'ConfigurationSettings'
+        route = "ConfigurationSettings"
         # value specs
-        value_specs = WorkspaceValueMixinHelper.get_workspace_value_specs(name,
-                                                                          value,
-                                                                          unit=unit,
-                                                                          description=description,
-                                                                          **kwargs)
+        value_specs = WorkspaceValueMixinHelper.get_workspace_value_specs(
+            name, value, unit=unit, description=description, **kwargs
+        )
         # get existing workspace values names
         workspace_value_names = self.get_workspace_value_names(**kwargs)
         if name in workspace_value_names:
-            return self.put(f'{route}/{self.encode(name)}', data=value_specs, **kwargs)
-        return self.post(f'{route}', data=value_specs, **kwargs)
+            return self.put(f"{route}/{self.encode(name)}", data=value_specs, **kwargs)
+        return self.post(f"{route}", data=value_specs, **kwargs)
 
     # rename workspace value
     def rename_workspace_value(self, old_name: str, new_name: str, **kwargs) -> Dict:
         """
         Rename workspace value
 
         Parameters
         ----------
         old_name : str
             Old variable name
         new_name : str
             New variable name
         """
-        route = 'ConfigurationSettings'
-        return self.post(f'{route}/Rename', query={
-            'OldName': old_name,
-            'NewName': new_name,
-        }, **kwargs)
+        route = "ConfigurationSettings"
+        return self.post(
+            f"{route}/Rename",
+            query={
+                "OldName": old_name,
+                "NewName": new_name,
+            },
+            **kwargs,
+        )
 
     # delete workspace value
     def delete_workspace_value(self, name: str, **kwargs) -> Dict:
         """
         Delete workspace value
 
         Parameters
         ----------
         name : str
             Variable name
         """
-        route = 'ConfigurationSettings'
-        return self.delete(f'{route}/{self.encode(name)}', **kwargs)
+        route = "ConfigurationSettings"
+        return self.delete(f"{route}/{self.encode(name)}", **kwargs)
 
 
 # Workspace value mixin Helper
 class WorkspaceValueMixinHelper:
     """
     Workspace value mixin Helper
     """
 
     # get known workspace value types
     @staticmethod
     def get_workspace_value_types():
-        return ['Numeric', 'NumericWithUnit', 'String', 'List', 'Dictionary', 'Enumeration']
+        return [
+            "Numeric",
+            "NumericWithUnit",
+            "String",
+            "List",
+            "Dictionary",
+            "Enumeration",
+        ]
 
     # get workspace value
     @staticmethod
     def get_workspace_value(value: Dict, **kwargs) -> Any:
         """
         Get workspace value
 
         Parameters
         ----------
         value : dict
             Value specs
         """
 
-        if value and 'ValueType' in value and value['ValueType']:
-            value_type = value['ValueType']
-            if value_type == 'NumericWithUnit':
-                return value['NumericValue'], value['UnitName']
-            for vtype in ['Numeric', 'String', 'List', 'Dictionary', 'Enumeration']:
+        if value and "ValueType" in value and value["ValueType"]:
+            value_type = value["ValueType"]
+            if value_type == "NumericWithUnit":
+                return value["NumericValue"], value["UnitName"]
+            for vtype in ["Numeric", "String", "List", "Dictionary", "Enumeration"]:
                 if value_type == vtype:
-                    return value[f'{vtype}Value']
+                    return value[f"{vtype}Value"]
         return None
 
     # get workspace value specs
     @staticmethod
-    def get_workspace_value_specs(name: str,
-                                  value: Union[str, List[Any], Dict[str, Any], Tuple],
-                                  unit: Union[Dict, str] = '',
-                                  description: Optional[str] = '',
-                                  **kwargs) -> Dict[str, Any]:
+    def get_workspace_value_specs(
+        name: str,
+        value: Union[str, List[Any], Dict[str, Any], Tuple],
+        unit: Union[Dict, str] = "",
+        description: Optional[str] = "",
+        **kwargs,
+    ) -> Dict[str, Any]:
         """
         Add or edit workspace value
 
         Parameters
         ----------
         name : str
             Variable name
@@ -193,46 +215,48 @@
             Unit object or Unit name
         description : str
             Description
         """
         # get value type, unit
 
         value_type = None
-        value_unit: str = ''
+        value_unit: str = ""
         if isinstance(value, list):
-            value_type = 'List'
+            value_type = "List"
             valid_value = [str(v) for v in value]
         elif isinstance(value, dict):
-            value_type = 'Dictionary'
+            value_type = "Dictionary"
             valid_value = {str(k): str(v) for k, v in value.items()}
         elif isinstance(value, tuple):
-            value_type = 'Enumeration'
+            value_type = "Enumeration"
             valid_value = {}
             eid = -1
             for v in value:
                 if isinstance(v, (tuple, list)) and len(v) > 1:
                     eid = int(v[1])
                     valid_value[str(v[0])] = eid
                 else:
                     eid += 1
                     valid_value[str(v)] = eid
         else:
             valid_value = value
             if isinstance(value, str):
-                value_type = 'String'
+                value_type = "String"
             elif ApiHelper.is_float(value) or ApiHelper.is_int(value):
-                value_unit = ApiHelper.get_object_name(unit, **kwargs) if unit else ''
-                value_type = 'NumericWithUnit' if value_unit else 'Numeric'
+                value_unit = ApiHelper.get_object_name(unit, **kwargs) if unit else ""
+                value_type = "NumericWithUnit" if value_unit else "Numeric"
 
         # get value field name
-        value_field_name = 'NumericValue' if value_type == 'NumericWithUnit' else f'{value_type}Value'
+        value_field_name = (
+            "NumericValue" if value_type == "NumericWithUnit" else f"{value_type}Value"
+        )
 
         # value specs
         value_specs = {
-            'Name': name,
+            "Name": name,
             value_field_name: valid_value,
-            'Description': description,
-            'ValueType': value_type,
+            "Description": description,
+            "ValueType": value_type,
         }
         if value_unit:
-            value_specs['UnitName'] = value_unit
+            value_specs["UnitName"] = value_unit
         return value_specs
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/protocols/protocols.py` & `petrovisor-0.1.3/src/petrovisor/api/protocols/protocols.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import (
     Any,
     Optional,
     Union,
     List,
     Dict,
 )
+
 try:
     from typing import Protocol
 except BaseException:
     from typing_extensions import Protocol
 
 import pandas as pd
+from datetime import datetime
 
 from petrovisor.api.dtypes.internal_dtypes import SignalType
+from petrovisor.api.dtypes.increments import (
+    TimeIncrement,
+    DepthIncrement,
+)
 
 
 # PetroVisor requests protocol
 class SupportsRequests(Protocol):
     @property
     def Api(self) -> str: ...
 
@@ -63,15 +69,17 @@
     def put(self, rqst: str, **kwargs) -> Any: ...
 
     # delete method
     def delete(self, rqst: str, **kwargs) -> Any: ...
 
     # encode url component
     @staticmethod
-    def encode(url_component: str, safe: Optional[Union[str, bytes]] = '~', **kwargs) -> str: ...
+    def encode(
+        url_component: str, safe: Optional[Union[str, bytes]] = "~", **kwargs
+    ) -> str: ...
 
 
 # PetroVisor Items requests protocol
 class SupportsItemRequests(Protocol):
     # get item types
     def get_item_types(self, **kwargs): ...
 
@@ -90,31 +98,35 @@
     # get items
     def get_items(self, item_type: str, **kwargs) -> List: ...
 
     # get item names
     def get_item_names(self, item_type: str, **kwargs) -> List[str]: ...
 
     # get item paged
-    def get_items_paged(self, item_type: str, page: int = 1, page_size: int = 10, **kwargs) -> List: ...
+    def get_items_paged(
+        self, item_type: str, page: int = 1, page_size: int = 10, **kwargs
+    ) -> List: ...
 
     # get item labels
     def get_item_labels(self, item_type: str, **kwargs) -> List[str]: ...
 
     # get item infos
     def get_item_infos(self, item_type: str, **kwargs) -> List: ...
 
     # get item name
     def get_item_name(self, item: Union[str, Dict], **kwargs) -> str: ...
 
     # get item field
-    def get_item_field(self,
-                       item_type: Optional[str],
-                       item: Union[str, Dict],
-                       field_name: str,
-                       **kwargs) -> Any: ...
+    def get_item_field(
+        self,
+        item_type: Optional[str],
+        item: Union[str, Dict],
+        field_name: str,
+        **kwargs,
+    ) -> Any: ...
 
     # get 'NamedItem' route
     def get_item_route(self, data_type: str, **kwargs) -> str: ...
 
     # get 'PetroVisorItems' route
     def get_petrovisor_item_route(self, data_type: str, **kwargs) -> str: ...
 
@@ -133,21 +145,25 @@
     # items exists
     def item_exists(self, item_type: str, item: Union[str, Dict], **kwargs) -> bool: ...
 
 
 # PetroVisor Entities requests protocol
 class SupportsEntitiesRequests(Protocol):
     # get entity
-    def get_entity(self, name: str, alias: Optional[str] = '', **kwargs) -> Dict: ...
+    def get_entity(self, name: str, alias: Optional[str] = "", **kwargs) -> Dict: ...
 
     # get entities
-    def get_entities(self, entity_type: Optional[str] = '', signal: Optional[str] = '', **kwargs) -> List[Dict]: ...
+    def get_entities(
+        self, entity_type: Optional[str] = "", signal: Optional[str] = "", **kwargs
+    ) -> List[Dict]: ...
 
     # get entity names
-    def get_entity_names(self, entity_type: Optional[str] = '', signal: Optional[str] = '', **kwargs) -> List[str]: ...
+    def get_entity_names(
+        self, entity_type: Optional[str] = "", signal: Optional[str] = "", **kwargs
+    ) -> List[str]: ...
 
     # add entities
     def add_entities(self, entities: List, **kwargs) -> Any: ...
 
     # rename entity type
     def rename_entity_type(self, old_name: str, new_name: str, **kwargs) -> Any: ...
 
@@ -155,74 +171,139 @@
     def rename_entity(self, old_name: str, new_name: str, **kwargs) -> Any: ...
 
 
 # Signals requests protocol
 class SupportsSignalsRequests(Protocol):
 
     # get 'Signal'
-    def get_signal(self, name: str, short_name: Optional[str] = '', **kwargs) -> Optional[Dict]: ...
+    def get_signal(
+        self, name: str, short_name: Optional[str] = "", **kwargs
+    ) -> Optional[Dict]: ...
 
     # get 'Signal' names
-    def get_signal_names(self,
-                         signal_type: Optional[str] = '',
-                         entity: Optional[Union[Any, str]] = None,
-                         **kwargs) -> List[str]: ...
+    def get_signal_names(
+        self,
+        signal_type: Optional[str] = "",
+        entity: Optional[Union[Any, str]] = None,
+        **kwargs,
+    ) -> List[str]: ...
 
     # get valid signal type name
-    def get_signal_type_enum(self, signal_type: Union[str, SignalType], **kwargs) -> SignalType: ...
+    def get_signal_type_enum(
+        self, signal_type: Union[str, SignalType], **kwargs
+    ) -> SignalType: ...
 
     # get signal type route
-    def get_signal_type_route(self, signal_type: Union[str, SignalType], **kwargs) -> str: ...
+    def get_signal_type_route(
+        self, signal_type: Union[str, SignalType], **kwargs
+    ) -> str: ...
+
+
+# PetroVisor Contex requests protocol
+class SupportsContextRequests(Protocol):
+    # get 'Context'
+    def get_context(
+        self,
+        name: Union[str, Dict],
+        entity_set: Union[str, Dict] = None,
+        scope: Union[str, Dict] = None,
+        hierarchy: Union[str, Dict] = None,
+        relationship: Dict[str, str] = None,
+        entity_type: Union[str, List[str]] = None,
+        entities: Union[Union[str, Dict], List[Union[str, Dict]]] = None,
+        time_start: Union[str, datetime] = None,
+        time_end: Union[str, datetime] = None,
+        time_step: Union[str, TimeIncrement] = None,
+        depth_start: float = None,
+        depth_end: float = None,
+        depth_step: Union[str, DepthIncrement] = None,
+        **kwargs,
+    ) -> Optional[Dict]: ...
+
+    # get 'Scope'
+    def get_scope(
+        self,
+        name: Union[str, Dict],
+        time_start: Union[str, datetime] = None,
+        time_end: Union[str, datetime] = None,
+        time_step: Union[str, TimeIncrement] = None,
+        depth_start: float = None,
+        depth_end: float = None,
+        depth_step: Union[str, DepthIncrement] = None,
+        **kwargs,
+    ) -> Optional[Dict]: ...
+
+    # get 'EntitySet'
+    def get_entity_set(
+        self,
+        name: Union[str, Dict],
+        entities: List[str] = None,
+        entity_type: Union[str, List[str]] = None,
+        **kwargs,
+    ) -> Optional[Dict]: ...
+
+    # get 'Hierarchy'
+    def get_hierarchy(
+        self, name: Union[str, Dict], relationship: Dict[str, str] = None, **kwargs
+    ) -> Optional[Dict]: ...
 
 
 # P# requests protocol
 class SupportsPsharpRequests(Protocol):
     # get P# script
     def get_psharp_script(self, name: str, **kwargs) -> Dict: ...
 
     # parse P# script
-    def parse_psharp_script(self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs) -> Dict: ...
+    def parse_psharp_script(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> Dict: ...
 
     # get P# script content
     def get_psharp_script_content(self, script: Union[str, Dict], **kwargs) -> str: ...
 
     # get P# script table names
-    def get_psharp_script_table_names(self,
-                                      script: Union[str, Dict],
-                                      options: Optional[Dict] = None,
-                                      **kwargs) -> List[str]: ...
+    def get_psharp_script_table_names(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> List[str]: ...
 
     # get P# script tables, columns and signals
-    def get_psharp_script_columns_and_signals(self,
-                                              script: Union[str, Dict],
-                                              options: Optional[Dict] = None,
-                                              **kwargs) -> Dict: ...
+    def get_psharp_script_columns_and_signals(
+        self, script: Union[str, Dict], options: Optional[Dict] = None, **kwargs
+    ) -> Dict: ...
 
 
 # DataFrames handling protocol
 class SupportsDataFrames(Protocol):
     # get valid json value
-    def get_json_valid_value(self, value: Any, dtype: Union[str, SignalType] = 'unknown', **kwargs) -> Any: ...
+    def get_json_valid_value(
+        self, value: Any, dtype: Union[str, SignalType] = "unknown", **kwargs
+    ) -> Any: ...
 
     # convert PivotTable to DataFrame
-    def convert_pivot_table_to_dataframe(self, data: List, groupby_entity: bool = False, **kwargs): ...
+    def convert_pivot_table_to_dataframe(
+        self, data: List, groupby_entity: bool = False, **kwargs
+    ): ...
 
     # Get signal data from DataFrame
 
-    def get_signal_data_from_dataframe(self,
-                                       df: pd.DataFrame,
-                                       signals: Optional[Dict] = None,
-                                       only_existing_entities: bool = True,
-                                       entity_type: str = '',
-                                       entities: Optional[Dict] = None,
-                                       **kwargs) -> Dict[str, Any]: ...
+    def get_signal_data_from_dataframe(
+        self,
+        df: pd.DataFrame,
+        signals: Optional[Dict] = None,
+        only_existing_entities: bool = True,
+        entity_type: str = "",
+        entities: Optional[Dict] = None,
+        **kwargs,
+    ) -> Dict[str, Any]: ...
 
     # convert P# table to DataFrame
-    def convert_psharp_table_to_dataframe(self,
-                                          psharp_table: Union[Dict, List],
-                                          dropna: bool = True,
-                                          with_entity_column: bool = True,
-                                          groupby_entity: bool = False,
-                                          **kwargs) -> Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]: ...
+    def convert_psharp_table_to_dataframe(
+        self,
+        psharp_table: Union[Dict, List],
+        dropna: bool = True,
+        with_entity_column: bool = True,
+        groupby_entity: bool = False,
+        **kwargs,
+    ) -> Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]: ...
 
     # get column unit
     def get_column_unit(self, column_name: str, **kwargs) -> str: ...
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/utils/datastructs.py` & `petrovisor-0.1.3/src/petrovisor/api/utils/datastructs.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,45 +4,52 @@
 # string constants
 def strconstants(cls=None, supress_warnings=False):
     """
     Decorator to create string constants class
     which returns field as is if it doesn't exist
     and sends warning if supress_warnings is set to False
     """
+
     def wrap(cls):
 
         # static class
         class StaticClass:
             """
             Static class which raises error if instance of the class is created
             """
 
             def __new__(cls, *args, **kwargs):
-                raise TypeError(f"Instances of static class '{cls.__name__}' cannot be created.")
+                raise TypeError(
+                    f"Instances of static class '{cls.__name__}' cannot be created."
+                )
 
         # metaclass with customized __getattr___
         class StrConstantsMeta(type):
             """
             String constants metaclass which sends warning if field doesn't exist
             """
 
             def __getattr__(cls, attr):
                 if attr in cls.__dict__:
                     return cls.__dict__[attr]
                 if not supress_warnings:
-                    warnings.warn(f"Field '{attr}' does not exist in '{cls.__name__}'."
-                                  "Returning attribute as is.",
-                                  RuntimeWarning, stacklevel=1)
+                    warnings.warn(
+                        f"Field '{attr}' does not exist in '{cls.__name__}'."
+                        "Returning attribute as is.",
+                        RuntimeWarning,
+                        stacklevel=1,
+                    )
                 return attr
 
         # static string constants
         class StrConstants(cls, StaticClass, metaclass=StrConstantsMeta):
             """
             Static string constants class which sends warning if field doesn't exist
             """
+
             pass
 
         return StrConstants
 
     # See if decorator is called with or without parentheses.
     if cls is None:
         # decorator is called with parentheses.
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/utils/helper.py` & `petrovisor-0.1.3/src/petrovisor/api/utils/helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,35 +22,41 @@
     # get default discovery urls
     @staticmethod
     def get_discovery_urls() -> List[str]:
         """
         Get known discovery urls
         """
         return [
-            r'https://identity-latest.eu1.petrovisor.com',
-            r'https://identity.eu1.petrovisor.com',
-            r'https://identity-latest.us1.petrovisor.com',
-            r'https://identity.us1.petrovisor.com']
+            r"https://identity-latest.eu1.petrovisor.com",
+            r"https://identity.eu1.petrovisor.com",
+            r"https://identity-latest.us1.petrovisor.com",
+            r"https://identity.us1.petrovisor.com",
+        ]
 
     # get object name
     @staticmethod
-    def get_object_name(obj: Any, **kwargs) -> str:
+    def get_object_name(obj: Any, field: str = "Name", **kwargs) -> str:
         """
         Get object name
 
         Parameters
         ----------
         obj : Any
             Object
+        field : str, default 'Name'
+            Field name
         """
         if isinstance(obj, str):
             return obj
-        elif ApiHelper.has_field(obj, 'Name'):
-            return obj['Name']
-        return str(obj)
+        elif obj is None:
+            return ""
+        try:
+            return ApiHelper.get_field(obj, field, ignore_case=True) or ""
+        except:
+            return str(obj)
 
     # update dictionary
     @staticmethod
     def update_dict(d: Dict, **kwargs) -> Dict:
         """
         Update dictionary fields with keyword argument values
 
@@ -80,28 +86,93 @@
         keys: str | list[str]
             Dictionary keys
         """
         if not isinstance(keys, list):
             keys = [keys]
         return {k: v for k, v in d.items() if k not in keys}
 
-    # check if object has field/attribute
+    # check if object has field or attribute
     @staticmethod
-    def has_field(obj: Any, field: str, **kwargs):
+    def has_field(obj: Any, field: str, ignore_case: bool = False, **kwargs):
         """
         Check whether object/dict has provided field/attribute
 
         Parameters
         ----------
         obj : Any
             Object
         field : str
             Field name
+        ignore_case : bool, default False
+            Whether to ignore field/attribute name case
+        """
+        if isinstance(obj, dict):
+            if field in obj:
+                return True
+            elif ignore_case:
+                if field.casefold() in obj:
+                    return True
+                return any(k.casefold() == field.casefold() for k in obj.keys())
+            else:
+                return False
+        else:
+            if hasattr(obj, field):
+                return True
+            elif ignore_case:
+                if hasattr(obj, field.casefold()):
+                    return True
+                else:
+                    return any(attr.casefold() == field.casefold() for attr in dir(obj))
+            else:
+                return False
+
+    # get object field value or default
+    @staticmethod
+    def get_field(obj: Any, field: str, ignore_case: bool = False, **kwargs):
         """
-        return hasattr(obj, field) or (isinstance(obj, dict) and field in obj)
+        Get object's field/attribute values
+
+        Parameters
+        ----------
+        obj : Any
+            Object
+        field : str
+            Field name
+        ignore_case : bool, default False
+            Whether to ignore field/attribute name case
+        kwargs: keyword arguments
+            Keyword argument among which if 'default' is present then it is used as default value,
+            when field does not exist.
+        """
+        if isinstance(obj, dict):
+            if field in obj:
+                return obj[field]
+            elif ignore_case:
+                if field.casefold() in obj:
+                    return obj[field.casefold()]
+                else:
+                    for k in obj.keys():
+                        if k.casefold() == field.casefold():
+                            return obj[k]
+        else:
+            if hasattr(obj, field):
+                return getattr(obj, field)
+            elif ignore_case:
+                if hasattr(obj, field.casefold()):
+                    return getattr(obj, field.casefold())
+                else:
+                    for attr in dir(obj):
+                        if attr.casefold() == field.casefold():
+                            return getattr(obj, attr)
+        # could not find object field/attribute
+        if "default" in kwargs:
+            return kwargs["default"]
+        raise AttributeError(
+            f"'{type(obj).__name__}' object has no attribute '{field}'"
+        )
 
     # get non-empty fields
     @staticmethod
     def get_non_empty_fields(d: Dict) -> Dict:
         """
         Get non-empty(is not None) fields of dictionary
 
@@ -114,23 +185,25 @@
 
     # get default characters to ignore
     @staticmethod
     def get_default_ignore_characters() -> List[str]:
         """
         Get list of default characters to ignore when comparing string names
         """
-        return [' ', '_', '-', '.', ',']
+        return [" ", "_", "-", ".", ","]
 
     # get comparison string
     @staticmethod
-    def get_comparison_string(s: str,
-                              ignore_characters: Union[List[str], str, bool] = True,
-                              ignore_case: bool = True,
-                              strip: bool = True,
-                              **kwargs):
+    def get_comparison_string(
+        s: str,
+        ignore_characters: Union[List[str], str, bool] = True,
+        ignore_case: bool = True,
+        strip: bool = True,
+        **kwargs,
+    ):
         """
         Get string preprocessed for comparison
 
         Parameters
         ----------
         s : str
             String
@@ -143,27 +216,29 @@
         """
         if ignore_characters:
             if isinstance(ignore_characters, bool):
                 ignore_characters = ApiHelper.get_default_ignore_characters()
             elif isinstance(ignore_characters, str):
                 ignore_characters = [ignore_characters]
             for c in ignore_characters:
-                s = s.replace(c, '')
+                s = s.replace(c, "")
         if ignore_case:
             s = s.lower()
         return s.strip() if strip else s
 
     # get dictionary value
     @staticmethod
-    def get_dict_value(d: Dict,
-                       key: Union[str, Any],
-                       ignore_characters: Union[List[str], str, bool] = True,
-                       ignore_case: bool = True,
-                       strip: bool = True,
-                       **kwargs) -> Optional[str]:
+    def get_dict_value(
+        d: Dict,
+        key: Union[str, Any],
+        ignore_characters: Union[List[str], str, bool] = True,
+        ignore_case: bool = True,
+        strip: bool = True,
+        **kwargs,
+    ) -> Optional[str]:
         """
         Get dictionary value
 
         Parameters
         ----------
         d : str
             String
@@ -178,39 +253,43 @@
         """
         if d:
             if not isinstance(key, str):
                 key = str(key)
             if key in d:
                 return d[key]
             else:
-                key_to_compare = \
-                    ApiHelper.get_comparison_string(key,
-                                                    ignore_characters=ignore_characters,
-                                                    ignore_case=ignore_case,
-                                                    strip=strip,
-                                                    **kwargs)
+                key_to_compare = ApiHelper.get_comparison_string(
+                    key,
+                    ignore_characters=ignore_characters,
+                    ignore_case=ignore_case,
+                    strip=strip,
+                    **kwargs,
+                )
                 for k, v in d.items():
-                    k_to_compare = \
-                        ApiHelper.get_comparison_string(k,
-                                                        ignore_characters=ignore_characters,
-                                                        ignore_case=ignore_case,
-                                                        strip=strip,
-                                                        **kwargs)
+                    k_to_compare = ApiHelper.get_comparison_string(
+                        k,
+                        ignore_characters=ignore_characters,
+                        ignore_case=ignore_case,
+                        strip=strip,
+                        **kwargs,
+                    )
                     if k_to_compare == key_to_compare:
                         return v
         return None
 
     # check whether dict/list contains key
     @staticmethod
-    def contains(d: Union[Dict, List],
-                 key: Union[str, Any],
-                 ignore_characters:  Union[List[str], str, bool] = True,
-                 ignore_case: bool = True,
-                 strip: bool = True,
-                 **kwargs) -> bool:
+    def contains(
+        d: Union[Dict, List],
+        key: Union[str, Any],
+        ignore_characters: Union[List[str], str, bool] = True,
+        ignore_case: bool = True,
+        strip: bool = True,
+        **kwargs,
+    ) -> bool:
         """
         Check whether dictionary contains field/key
 
         Parameters
         ----------
         d : str
             String
@@ -224,27 +303,29 @@
             Strip/Trim string.
         """
         if not isinstance(key, str):
             key = str(key)
         if key in d:
             return True
         else:
-            key_to_compare = \
-                ApiHelper.get_comparison_string(key,
-                                                ignore_characters=ignore_characters,
-                                                ignore_case=ignore_case,
-                                                strip=strip,
-                                                **kwargs)
+            key_to_compare = ApiHelper.get_comparison_string(
+                key,
+                ignore_characters=ignore_characters,
+                ignore_case=ignore_case,
+                strip=strip,
+                **kwargs,
+            )
             for k in d:
-                k_to_compare = \
-                    ApiHelper.get_comparison_string(k,
-                                                    ignore_characters=ignore_characters,
-                                                    ignore_case=ignore_case,
-                                                    strip=strip,
-                                                    **kwargs)
+                k_to_compare = ApiHelper.get_comparison_string(
+                    k,
+                    ignore_characters=ignore_characters,
+                    ignore_case=ignore_case,
+                    strip=strip,
+                    **kwargs,
+                )
                 if k_to_compare == key_to_compare:
                     return True
         return False
 
     # check whether convertible to integer
     @staticmethod
     def is_int(value: Any, **kwargs) -> bool:
@@ -286,15 +367,15 @@
         Get UUID value
 
         Parameters
         ----------
         value : Any
             Value
         """
-        return UUID(value) if ApiHelper.is_uuid(value) else UUID(value['Id'])
+        return UUID(value) if ApiHelper.is_uuid(value) else UUID(value["Id"])
 
     # is uuid
     @staticmethod
     def is_uuid(value: Any, **kwargs) -> bool:
         """
         Is UUID value
 
@@ -316,15 +397,15 @@
         Is iterable object
 
         Parameters
         ----------
         x : Any
             Object
         """
-        if hasattr(x, '__len__'):
+        if hasattr(x, "__len__"):
             return True
         return False
 
     # is empty
     @staticmethod
     def is_empty(x: Any, **kwargs) -> bool:
         """
@@ -350,15 +431,15 @@
         Parameters
         ----------
         x : Any
             Object
         """
         if isinstance(x, (np.ndarray, pd.DataFrame, pd.Series)):
             return x.shape[0]
-        elif hasattr(x, '__len__'):
+        elif hasattr(x, "__len__"):
             return len(x)
         return None
 
     # get number of columns
     @staticmethod
     def get_num_cols(x: Any, **kwargs) -> Optional[int]:
         """
@@ -442,25 +523,25 @@
         Get Windows-like file path
 
         Parameters
         ----------
         path : str
             File path.
         """
-        if '/' in path:
-            path = path.replace('/', '\\')
+        if "/" in path:
+            path = path.replace("/", "\\")
         return path
 
     # get Unix-like file path
     @staticmethod
     def get_unix_like_path(path: str, **kwargs) -> str:
         """
         Get Unix-like file path
 
         Parameters
         ----------
         path : str
             File path.
         """
-        if '\\' in path:
-            path = path.replace('\\', '/')
+        if "\\" in path:
+            path = path.replace("\\", "/")
         return path
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/utils/login.py` & `petrovisor-0.1.3/src/petrovisor/api/utils/login.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,23 @@
     """
 
     def __init__(self, **kwargs):
         pass
 
     # get access token
     @staticmethod
-    def get_access_token(key: str = '',
-                         username: str = '',
-                         password: str = '',
-                         refresh_token: str = '',
-                         discovery_url: str = '',
-                         token_endpoint: str = '',
-                         **kwargs) -> Dict:
+    def get_access_token(
+        key: str = "",
+        username: str = "",
+        password: str = "",
+        refresh_token: str = "",
+        discovery_url: str = "",
+        token_endpoint: str = "",
+        **kwargs,
+    ) -> Dict:
         """
         Get access token response
 
         Parameters
         ----------
         key : str, default None
             Access key generated from username and password
@@ -47,60 +49,73 @@
         password : str, default None
             Password
         token_endpoint : str, default None
             Token endpoint
         """
         access_response = None
         if key:
-            access_response = ApiLogin.get_access_token_from_key(key,
-                                                                 discovery_url=discovery_url,
-                                                                 token_endpoint=token_endpoint,
-                                                                 **kwargs)
+            access_response = ApiLogin.get_access_token_from_key(
+                key,
+                discovery_url=discovery_url,
+                token_endpoint=token_endpoint,
+                **kwargs,
+            )
         if not access_response and username and password:
-            access_response = ApiLogin.get_access_token_from_credentials(username, password,
-                                                                         discovery_url=discovery_url,
-                                                                         token_endpoint=token_endpoint,
-                                                                         **kwargs)
+            access_response = ApiLogin.get_access_token_from_credentials(
+                username,
+                password,
+                discovery_url=discovery_url,
+                token_endpoint=token_endpoint,
+                **kwargs,
+            )
         if not access_response and refresh_token:
-            access_response = ApiLogin.get_access_token_from_refresh_token(refresh_token,
-                                                                           discovery_url=discovery_url,
-                                                                           token_endpoint=token_endpoint,
-                                                                           **kwargs)
+            access_response = ApiLogin.get_access_token_from_refresh_token(
+                refresh_token,
+                discovery_url=discovery_url,
+                token_endpoint=token_endpoint,
+                **kwargs,
+            )
         return access_response
 
     # get access token from key
     @staticmethod
-    def get_access_token_from_key(key: str,
-                                  discovery_url: str = '',
-                                  token_endpoint: str = '', **kwargs) -> Dict:
+    def get_access_token_from_key(
+        key: str, discovery_url: str = "", token_endpoint: str = "", **kwargs
+    ) -> Dict:
         """
         Get access token response from key
 
         Parameters
         ----------
         key : str
             Access key generated from username and password
         discovery_url : str, default None
             Discovery url
         token_endpoint : str, default None
             Token endpoint
         """
         credentials = ApiLogin.get_credentials_from_key(key)
-        username = credentials['username']
-        password = credentials['password']
-        return ApiLogin.get_access_token_from_credentials(username, password,
-                                                          discovery_url=discovery_url,
-                                                          token_endpoint=token_endpoint)
+        username = credentials["username"]
+        password = credentials["password"]
+        return ApiLogin.get_access_token_from_credentials(
+            username,
+            password,
+            discovery_url=discovery_url,
+            token_endpoint=token_endpoint,
+        )
 
     # get access token from username and password
     @staticmethod
-    def get_access_token_from_credentials(username: str,
-                                          password: str,
-                                          discovery_url: str = '',
-                                          token_endpoint: str = '', **kwargs) -> Dict:
+    def get_access_token_from_credentials(
+        username: str,
+        password: str,
+        discovery_url: str = "",
+        token_endpoint: str = "",
+        **kwargs,
+    ) -> Dict:
         """
         Get access token response from credentials
 
         Parameters
         ----------
         username : str
             Username
@@ -109,65 +124,68 @@
         discovery_url : str, default None
             Discovery url
         token_endpoint : str, default None
             Token endpoint
         """
         if not token_endpoint:
             token_endpoint = ApiLogin.get_token_endpoint(discovery_url=discovery_url)
-        grant_type = 'password'
-        client_id = 'petrovisor.python.client'
-        scope = 'petrovisor.api'
+        grant_type = "password"
+        client_id = "petrovisor.python.client"
+        scope = "petrovisor.api"
         requests_headers = {
-            'Content-Type': 'application/x-www-form-urlencoded',
+            "Content-Type": "application/x-www-form-urlencoded",
         }
         request_data = {
-            'username': username,
-            'password': password,
-            'client_id': client_id,
-            'grant_type': grant_type,
-            'scope': scope,
+            "username": username,
+            "password": password,
+            "client_id": client_id,
+            "grant_type": grant_type,
+            "scope": scope,
         }
-        response = requests.post(token_endpoint, headers=requests_headers, data=request_data)
+        response = requests.post(
+            token_endpoint, headers=requests_headers, data=request_data
+        )
         # get response content
         access_response = json.loads(response.content)
         return access_response
 
     # get access token from refresh token
     @staticmethod
-    def get_access_token_from_refresh_token(refresh_token: str,
-                                            discovery_url: str = '',
-                                            token_endpoint: str = '',
-                                            **kwargs) -> Dict:
+    def get_access_token_from_refresh_token(
+        refresh_token: str, discovery_url: str = "", token_endpoint: str = "", **kwargs
+    ) -> Dict:
         """
         Get access token response from refresh token
 
         Parameters
         ----------
         refresh_token : str, default None
             Refresh Token
         discovery_url : str, default None
             Discovery url
         token_endpoint : str, default None
             Token endpoint
         """
         if not token_endpoint:
             token_endpoint = ApiLogin.get_token_endpoint(discovery_url=discovery_url)
-        grant_type = 'refresh_token'
-        client_id = 'petrovisor.python.client'
-        scope = 'petrovisor.api'
+        grant_type = "refresh_token"
+        client_id = "petrovisor.python.client"
+        scope = "petrovisor.api"
         requests_headers = {
-            'Content-Type': 'application/x-www-form-urlencoded',
+            "Content-Type": "application/x-www-form-urlencoded",
         }
         request_data = {
-            'refresh_token': refresh_token,
-            'client_id': client_id,
-            'grant_type': grant_type,
-            'scope': scope,
+            "refresh_token": refresh_token,
+            "client_id": client_id,
+            "grant_type": grant_type,
+            "scope": scope,
         }
-        response = requests.post(token_endpoint, headers=requests_headers, data=request_data)
+        response = requests.post(
+            token_endpoint, headers=requests_headers, data=request_data
+        )
         # get response content
         access_response = json.loads(response.content)
         return access_response
 
     # get credentials structure with username and password from key
     @staticmethod
     def get_credentials_from_key(key: str, **kwargs) -> Dict:
@@ -176,25 +194,25 @@
 
         Parameters
         ----------
         key : str
             Access key generated from username and password
         """
         valid_credentials = {
-            'username': '',
-            'password': '',
+            "username": "",
+            "password": "",
         }
         if key and isinstance(key, str):
             # decode the key
             auth = ApiLogin.decode_base64(key)
             if auth:
-                s = str(auth).split(':')
+                s = str(auth).split(":")
                 if s and len(s) > 1:
-                    valid_credentials['username'] = s[0]
-                    valid_credentials['password'] = ':'.join(s[1:])
+                    valid_credentials["username"] = s[0]
+                    valid_credentials["password"] = ":".join(s[1:])
         return valid_credentials
 
     # get credentials structure with username and password
     @staticmethod
     def get_credentials(username: str, password: str) -> Dict:
         """
         Get credentials from username and password
@@ -203,164 +221,188 @@
         ----------
         username : str
             Username
         password : str
             Password
         """
         valid_credentials = {
-            'username': username,
-            'password': password,
+            "username": username,
+            "password": password,
         }
         return valid_credentials
 
     # generate credentials key from username and password
     @staticmethod
-    def generate_credentials_key(username: str = '', password: str = '', **kwargs) -> str:
+    def generate_credentials_key(
+        username: str = "", password: str = "", **kwargs
+    ) -> str:
         """
         Get credentials key
 
         Parameters
         ----------
         username : str, default None
             Username
         password : str, default None
             Password
         """
         if username and password:
             # decode the key
-            key = ApiLogin.encode_base64(username + ':' + password)
+            key = ApiLogin.encode_base64(username + ":" + password)
         else:
-            key = ''
+            key = ""
         return key
 
     # get token endpoint
     @staticmethod
-    def get_token_endpoint(discovery_url: str = '', **kwargs) -> str:
+    def get_token_endpoint(discovery_url: str = "", **kwargs) -> str:
         """
         Get token endpoint
 
         Parameters
         ----------
         discovery_url : str, default None
             Discovery url
         """
-        return ApiLogin.get_endpoint('token_endpoint', discovery_url=discovery_url)
+        return ApiLogin.get_endpoint("token_endpoint", discovery_url=discovery_url)
 
     # get web api endpoint
     @staticmethod
-    def get_web_api_endpoint(discovery_url: str = '', **kwargs) -> str:
+    def get_web_api_endpoint(discovery_url: str = "", **kwargs) -> str:
         """
         Get web api endpoint
 
         Parameters
         ----------
         discovery_url : str, default None
             Discovery url
         """
-        return ApiLogin.get_endpoint('petrovisor_webapi_endpoint', discovery_url=discovery_url)
+        return ApiLogin.get_endpoint(
+            "petrovisor_webapi_endpoint", discovery_url=discovery_url
+        )
 
     # get endpoint
     @staticmethod
-    def get_endpoint(endpoint_name: str, discovery_url: str = '', **kwargs) -> str:
+    def get_endpoint(endpoint_name: str, discovery_url: str = "", **kwargs) -> str:
         """
         Get endpoint
 
         Parameters
         ----------
         endpoint_name : str
             Endpoint name
         discovery_url : str, default None
             Discovery url
         """
         endpoints = ApiLogin.get_discovery_document(discovery_url)
         if endpoints and endpoint_name in endpoints:
             return endpoints[endpoint_name]
-        return ''
+        return ""
 
     # get discovery document
     @staticmethod
-    def get_discovery_document(discovery_url: str = '', **kwargs) -> Any:
+    def get_discovery_document(discovery_url: str = "", **kwargs) -> Any:
         """
         Get discovery document
 
         Parameters
         ----------
         discovery_url : str, default None
             Discovery url
         """
         if not discovery_url:
-            raise ValueError("PetroVisorLogin::get_discovery_document(): "
-                             "'discovery_url' is undefined!")
-        if not discovery_url.endswith('/'):
-            discovery_url += '/'
-        well_known_url = f'{discovery_url}.well-known/openid-configuration'
+            raise ValueError(
+                "PetroVisorLogin::get_discovery_document(): "
+                "'discovery_url' is undefined!"
+            )
+        if not discovery_url.endswith("/"):
+            discovery_url += "/"
+        well_known_url = f"{discovery_url}.well-known/openid-configuration"
         endpoints = requests.get(well_known_url).json()
         return endpoints
 
     # encode base64 message
     @staticmethod
-    def decode_base64(base64_message: Union[bytes, str],
-                      fmt: str = 'ascii',
-                      altchars: Optional[str] = None,
-                      **kwargs) -> str:
+    def decode_base64(
+        base64_message: Union[bytes, str],
+        fmt: str = "ascii",
+        altchars: Optional[str] = None,
+        **kwargs,
+    ) -> str:
         """
         Decode base64 string
 
         Parameters
         ----------
         base64_message : bytes, str
             Base64 message
         fmt : str, default 'ascii'
             Format
         altchars : str
             Alternative characters encoded instead of + or / characters.
             altchars is a byte-like object and must have a minimum length of 2.
         """
-        base64_bytes = base64_message if isinstance(base64_message, bytes) else str(base64_message).encode(fmt)
+        base64_bytes = (
+            base64_message
+            if isinstance(base64_message, bytes)
+            else str(base64_message).encode(fmt)
+        )
         # altchars = b'+/'
         # base64_bytes = re.sub(rb'[^a-zA-Z0-9%s]+' % altchars, b'', base64_bytes)  # normalize
         missing_padding = (4 - len(base64_bytes) % 4) % 4
         if missing_padding:
-            base64_bytes += b'=' * missing_padding
+            base64_bytes += b"=" * missing_padding
         # num_bytes = len(base64_bytes)
         # message_bytes = base64.b64decode(base64_bytes, altchars)
-        has_dash_underscore = True if (b'-' in base64_bytes or b'_' in base64_bytes) else False
+        has_dash_underscore = (
+            True if (b"-" in base64_bytes or b"_" in base64_bytes) else False
+        )
         if has_dash_underscore:
-            altchars = b'-_'
+            altchars = b"-_"
         message_bytes = None
         try:
             if altchars:
                 message_bytes = base64.b64decode(base64_bytes, altchars)
             else:
                 message_bytes = base64.b64decode(base64_bytes)
         except ValueError:
             pass
         finally:
             if message_bytes:
-                message = message_bytes if ApiLogin.is_binary_string(message_bytes) else message_bytes.decode(
-                    fmt)
+                message = (
+                    message_bytes
+                    if ApiLogin.is_binary_string(message_bytes)
+                    else message_bytes.decode(fmt)
+                )
             else:
-                message = ''
+                message = ""
         return message
 
     # encode base64 message
     @staticmethod
-    def encode_base64(base64_message: Union[bytes, str], fmt: str = 'ascii', **kwargs) -> str:
+    def encode_base64(
+        base64_message: Union[bytes, str], fmt: str = "ascii", **kwargs
+    ) -> str:
         """
         Encode base64 string
 
         Parameters
         ----------
         base64_message : bytes, str
             Base64 message
         fmt : str, default 'ascii'
             Format
         """
         import base64
-        base64_bytes = base64_message if isinstance(base64_message, bytes) else str(base64_message).encode(fmt)
+
+        base64_bytes = (
+            base64_message
+            if isinstance(base64_message, bytes)
+            else str(base64_message).encode(fmt)
+        )
         message_bytes = base64.b64encode(base64_bytes)
         message = message_bytes.decode(fmt)
         return message
 
     # check whether string is binary
     @staticmethod
     def is_binary_string(bytes_str: bytes, **kwargs) -> bool:
@@ -368,9 +410,11 @@
         Check whether string is binary
 
         Parameters
         ----------
         bytes_str : bytes
             Bytes string
         """
-        textchars = bytearray({7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7f})
+        textchars = bytearray(
+            {7, 8, 9, 10, 12, 13, 27} | set(range(0x20, 0x100)) - {0x7F}
+        )
         return bool(bytes_str.translate(None, textchars))
```

### Comparing `petrovisor-0.1.2/src/petrovisor/api/utils/requests.py` & `petrovisor-0.1.3/src/petrovisor/api/utils/requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,26 @@
     """
 
     def __init__(self):
         pass
 
     # 'GET' request
     @staticmethod
-    def get(api: str,
-            rqst: str,
-            workspace: str = '',
-            data: Optional[Any] = None,
-            query: Optional[Any] = None,
-            files: Optional[Any] = None,
-            token: str = '',
-            route: str = 'PetroVisor/API/',
-            format: str = 'json',
-            **kwargs) -> Any:
+    def get(
+        api: str,
+        rqst: str,
+        workspace: str = "",
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        token: str = "",
+        route: str = "PetroVisor/API/",
+        format: str = "json",
+        **kwargs,
+    ) -> Any:
         """
         Get request
 
         Parameters
         ----------
         api : str
             Api endpoint
@@ -53,29 +55,42 @@
         token : str, default None
             Token
         route : str, default 'PetroVisor/API/'
             Route
         format : str, default 'json'
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         """
-        return ApiRequests.get_response('GET', api, rqst, workspace=workspace, data=data, query=query,
-                                        files=files, token=token, route=route, format=format, **kwargs)
+        return ApiRequests.get_response(
+            "GET",
+            api,
+            rqst,
+            workspace=workspace,
+            data=data,
+            query=query,
+            files=files,
+            token=token,
+            route=route,
+            format=format,
+            **kwargs,
+        )
 
     # 'POST' request
     @staticmethod
-    def post(api: str,
-             rqst: str,
-             workspace: str = '',
-             data: Optional[Any] = None,
-             query: Optional[Any] = None,
-             files: Optional[Any] = None,
-             token: str = '',
-             route: str = 'PetroVisor/API/',
-             format: str = 'json',
-             **kwargs) -> Any:
+    def post(
+        api: str,
+        rqst: str,
+        workspace: str = "",
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        token: str = "",
+        route: str = "PetroVisor/API/",
+        format: str = "json",
+        **kwargs,
+    ) -> Any:
         """
         Post request
 
         Parameters
         ----------
         api : str
             Api endpoint
@@ -92,29 +107,42 @@
         token : str, default None
             Token
         route : str, default 'PetroVisor/API/'
             Route
         format : str, default 'json'
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         """
-        return ApiRequests.get_response('POST', api, rqst, workspace=workspace, data=data, query=query,
-                                        files=files, token=token, route=route, format=format, **kwargs)
+        return ApiRequests.get_response(
+            "POST",
+            api,
+            rqst,
+            workspace=workspace,
+            data=data,
+            query=query,
+            files=files,
+            token=token,
+            route=route,
+            format=format,
+            **kwargs,
+        )
 
     # 'PUT' request
     @staticmethod
-    def put(api: str,
-            rqst: str,
-            workspace: str = '',
-            data: Optional[Any] = None,
-            query: Optional[Any] = None,
-            files: Optional[Any] = None,
-            token: str = '',
-            route: str = 'PetroVisor/API/',
-            format: str = 'json',
-            **kwargs) -> Any:
+    def put(
+        api: str,
+        rqst: str,
+        workspace: str = "",
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        token: str = "",
+        route: str = "PetroVisor/API/",
+        format: str = "json",
+        **kwargs,
+    ) -> Any:
         """
         Put request
 
         Parameters
         ----------
         api : str
             Api endpoint
@@ -131,29 +159,42 @@
         token : str, default None
             Token
         route : str, default 'PetroVisor/API/'
             Route
         format : str, default 'json'
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         """
-        return ApiRequests.get_response('PUT', api, rqst, workspace=workspace, data=data, query=query,
-                                        files=files, token=token, route=route, format=format, **kwargs)
+        return ApiRequests.get_response(
+            "PUT",
+            api,
+            rqst,
+            workspace=workspace,
+            data=data,
+            query=query,
+            files=files,
+            token=token,
+            route=route,
+            format=format,
+            **kwargs,
+        )
 
     # 'DELETE' request
     @staticmethod
-    def delete(api: str,
-               rqst: str,
-               workspace: str = '',
-               data: Optional[Any] = None,
-               query: Optional[Any] = None,
-               files: Optional[Any] = None,
-               token: str = '',
-               route: str = 'PetroVisor/API/',
-               format: str = 'json',
-               **kwargs) -> Any:
+    def delete(
+        api: str,
+        rqst: str,
+        workspace: str = "",
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        token: str = "",
+        route: str = "PetroVisor/API/",
+        format: str = "json",
+        **kwargs,
+    ) -> Any:
         """
         Delete request
 
         Parameters
         ----------
         api : str
             Api endpoint
@@ -170,32 +211,45 @@
         token : str, default None
             Token
         route : str, default 'PetroVisor/API/'
             Route
         format : str, default 'json'
             Response format: 'json', 'text', 'content', 'raw', 'bytes', 'binary'
         """
-        return ApiRequests.get_response('DELETE', api, rqst, workspace=workspace, data=data, query=query,
-                                        files=files, token=token, route=route, format=format, **kwargs)
+        return ApiRequests.get_response(
+            "DELETE",
+            api,
+            rqst,
+            workspace=workspace,
+            data=data,
+            query=query,
+            files=files,
+            token=token,
+            route=route,
+            format=format,
+            **kwargs,
+        )
 
     # get REST API response
     @staticmethod
-    def get_response(method: str,
-                     api: str,
-                     rqst: str,
-                     workspace: str = '',
-                     data: Optional[Any] = None,
-                     query: Optional[Any] = None,
-                     files: Optional[Any] = None,
-                     token: str = '',
-                     route: str = 'PetroVisor/API/',
-                     format: str = 'json',
-                     retry_on_unauthorized: bool = True,
-                     errors: str = 'coerce',
-                     **kwargs) -> Any:
+    def get_response(
+        method: str,
+        api: str,
+        rqst: str,
+        workspace: str = "",
+        data: Optional[Any] = None,
+        query: Optional[Any] = None,
+        files: Optional[Any] = None,
+        token: str = "",
+        route: str = "PetroVisor/API/",
+        format: str = "json",
+        retry_on_unauthorized: bool = True,
+        errors: str = "coerce",
+        **kwargs,
+    ) -> Any:
         """
         Get response from request
 
         Parameters
         ----------
         method : str
             'GET', 'PUT', 'POST', 'DELETE'
@@ -221,149 +275,203 @@
             Retry if request was unauthorized(401)
         errors : str, default 'coerce'
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
         """
         request_headers = {
-            'accept': 'application/json',
+            "accept": "application/json",
         }
         # add access token to headers
         if token:
-            request_headers['authorization'] = f'Bearer {token}'
+            request_headers["authorization"] = f"Bearer {token}"
         # content type to headers
         if data or isinstance(data, dict):
-            request_headers['content-type'] = 'application/json'
+            request_headers["content-type"] = "application/json"
             if not data:
                 data = json.dumps(data)
         # elif(files):
         #     request_headers['content-type'] = 'multipart/form-data'
         # add workspace
         if workspace:
-            rqst = workspace + '/' + rqst
+            rqst = workspace + "/" + rqst
         if query:
             if isinstance(query, str):
-                rqst = rqst + '?' + query
+                rqst = rqst + "?" + query
             elif isinstance(query, list):
-                rqst = rqst + '?' + '&'.join([f'{v}' for v in query])
+                rqst = rqst + "?" + "&".join([f"{v}" for v in query])
             # generalized dictionary
-            elif callable(getattr(query, 'items', None)):
-                rqst = rqst + '?' + '&'.join([f'{k}={ApiRequests.encode(v)}' for k, v in query.items()])
+            elif callable(getattr(query, "items", None)):
+                rqst = (
+                    rqst
+                    + "?"
+                    + "&".join(
+                        [f"{k}={ApiRequests.encode(v)}" for k, v in query.items()]
+                    )
+                )
         # get request url
         request_url = ApiRequests.get_request_url(route, api, rqst)
 
         # method name
         method_name = method.upper().strip()
 
         # convert data to json string
         if data and not isinstance(data, str):
             data = json.dumps(data)
 
         # request secs
         timeout = 59 * 60  # time out limit in seconds (3540)
-        max_retries = 1  # increased to 3 times in case of 400 Bad Request or 4004 Not Found
+        max_retries = (
+            1  # increased to 3 times in case of 400 Bad Request or 4004 Not Found
+        )
         waiting_time = 5  # in seconds
 
         # get response
         response = None
         attempt = 0
         while attempt < max_retries:
             attempt += 1
             try:
                 # GET: read resource
                 # The GET method requests a representation of the specified resource.
                 # Requests using GET should only retrieve data.
-                if method_name == 'GET':
-                    response = requests.get(request_url,
-                                            headers=request_headers, data=data, files=files, timeout=timeout)
+                if method_name == "GET":
+                    response = requests.get(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # POST: create resource
                 # The POST method submits an entity to the specified resource,
                 # often causing a change in state or side effects on the server.
-                elif method_name == 'POST':
-                    response = requests.post(request_url,
-                                             headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "POST":
+                    response = requests.post(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # PUT: update resource
                 # The PUT method replaces all current representations of the target resource with the request payload.
-                elif method_name == 'PUT':
-                    response = requests.put(request_url,
-                                            headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "PUT":
+                    response = requests.put(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # DELETE: delete resource
                 # The DELETE method deletes the specified resource.
-                elif method_name == 'DELETE':
-                    response = requests.delete(request_url,
-                                               headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "DELETE":
+                    response = requests.delete(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # PATCH: modify resource
                 # The PATCH method applies partial modifications to a resource.
-                elif method_name == 'PATCH':
-                    response = requests.patch(request_url,
-                                              headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "PATCH":
+                    response = requests.patch(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # HEAD: read resource, response without body
                 # The HEAD method asks for a response identical to a GET request, but without the response body.
-                elif method_name == 'HEAD':
-                    response = requests.head(request_url,
-                                             headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "HEAD":
+                    response = requests.head(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # OPTIONS: specify communication options
                 # The OPTIONS method describes the communication options for the target resource.
-                elif method_name == 'OPTIONS':
-                    response = requests.options(request_url,
-                                                headers=request_headers, data=data, files=files, timeout=timeout)
+                elif method_name == "OPTIONS":
+                    response = requests.options(
+                        request_url,
+                        headers=request_headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout,
+                    )
                 # CONNECT:
                 # The CONNECT method establishes a tunnel to the server identified by the target resource.
-                elif method_name == 'CONNECT':
+                elif method_name == "CONNECT":
                     pass
                 # TRACE:
                 # The TRACE method performs a message loop-back test along the path to the target resource.
-                elif method_name == 'TRACE':
+                elif method_name == "TRACE":
                     pass
                 # raise exception if error occurred
                 response.raise_for_status()
             except requests.exceptions.HTTPError as err:
 
                 # check if unauthorized request (401)
-                if retry_on_unauthorized and response.status_code == requests.codes.unauthorized:
+                if (
+                    retry_on_unauthorized
+                    and response.status_code == requests.codes.unauthorized
+                ):
                     return response
 
-                if response.status_code in {requests.codes.bad_request, requests.codes.not_found}:
+                if response.status_code in {
+                    requests.codes.bad_request,
+                    requests.codes.not_found,
+                }:
                     max_retries = 3
 
                 # retry request
                 if attempt < max_retries:
                     time.sleep(waiting_time)
                     response = None
                     continue
 
                 # get more informative error message
-                response_content = getattr(err.response, 'text', getattr(err.response, 'content', None)) or None
+                response_content = (
+                    getattr(
+                        err.response, "text", getattr(err.response, "content", None)
+                    )
+                    or None
+                )
                 if response_content:
                     err.args = (f"{err.args[0]}, Response: \n{response_content}",)
 
                 def issue_warning(error):
                     error_message = f"{error}"
                     # print(error_message, file=sys.stderr)
                     warnings.warn(error_message, RuntimeWarning, stacklevel=1)
 
                 if isinstance(errors, str):
                     error_type = errors.lower()
-                    if error_type == 'coerce':
+                    if error_type == "coerce":
                         issue_warning(err)
                         return None
-                    elif error_type == 'ignore':
+                    elif error_type == "ignore":
                         return response
                 raise err
             break
 
         if response is not None:
             try:
-                if format in ('json',):
+                if format in ("json",):
                     return response.json()
-                elif format in ('bytes', 'binary', 'content'):
+                elif format in ("bytes", "binary", "content"):
                     return response.content
-                elif format in ('text',):
+                elif format in ("text",):
                     return response.text
-                elif format in ('raw',):
+                elif format in ("raw",):
                     return response.raw
                 elif not format:
                     return response
                 return response.content
             except (AttributeError, requests.exceptions.JSONDecodeError):
                 return response
         return None
@@ -381,16 +489,16 @@
         api : str
             Api endpoint
         rqst : str
             Request
         """
         # get web api service url
         web_api_service_url = api
-        if not web_api_service_url.endswith('/'):
-            web_api_service_url += '/'
+        if not web_api_service_url.endswith("/"):
+            web_api_service_url += "/"
         # form request url
         request_url = route + rqst.strip()
         # validate request url
         request_url = ApiRequests.validate_url(request_url)
         return web_api_service_url + request_url
 
     # validate request url
@@ -404,15 +512,15 @@
         request : str
             Request
         """
         return requote_uri(request)
 
     # encode url component
     @staticmethod
-    def encode(url_component: str, safe: Union[str, bytes] = '~', **kwargs) -> str:
+    def encode(url_component: str, safe: Union[str, bytes] = "~", **kwargs) -> str:
         """
         Encode url component
 
         Parameters
         ----------
         url_component : str
             URL component
@@ -427,9 +535,9 @@
     @staticmethod
     def success():
         """
         Return success response
         """
         response = Response()
         response.status_code = 200
-        response._content = json.dumps({"message": "Success!"}).encode('utf-8')
+        response._content = json.dumps({"message": "Success!"}).encode("utf-8")
         return response
```

### Comparing `petrovisor-0.1.2/src/petrovisor/petrovisor.py` & `petrovisor-0.1.3/src/petrovisor/petrovisor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from typing import Optional
 
 # import api methods
 from petrovisor.api.base import RequestsMixin
 from petrovisor.api.methods.items import ItemsMixin
 from petrovisor.api.methods.entities import EntitiesMixin
+from petrovisor.api.methods.contexts import ContextMixin
 from petrovisor.api.methods.signals import SignalsMixin
 from petrovisor.api.methods.workspace_values import WorkspaceValuesMixin
 from petrovisor.api.methods.psharp import PsharpMixin
 from petrovisor.api.methods.reference_tables import RefTableMixin
 from petrovisor.api.methods.pivot_tables import PivotTableMixin
 from petrovisor.api.methods.dataframes import DataFrameMixin
 from petrovisor.api.methods.ml import MLMixin
 from petrovisor.api.methods.workflows import WorkflowsMixin
 from petrovisor.api.methods.files import FilesMixin
 from petrovisor.api.methods.logs import LogsMixin
 
 
 # PetroVisor API calls
-class PetroVisor(RequestsMixin,
-                 ItemsMixin,
-                 EntitiesMixin,
-                 SignalsMixin,
-                 WorkspaceValuesMixin,
-                 PsharpMixin,
-                 RefTableMixin,
-                 PivotTableMixin,
-                 MLMixin,
-                 WorkflowsMixin,
-                 FilesMixin,
-                 LogsMixin,
-                 DataFrameMixin, ):
+class PetroVisor(
+    RequestsMixin,
+    ItemsMixin,
+    EntitiesMixin,
+    ContextMixin,
+    SignalsMixin,
+    WorkspaceValuesMixin,
+    PsharpMixin,
+    RefTableMixin,
+    PivotTableMixin,
+    MLMixin,
+    WorkflowsMixin,
+    FilesMixin,
+    LogsMixin,
+    DataFrameMixin,
+):
     """
     PetroVisor API class
     """
 
-    def __init__(self,
-                 workspace: Optional[str] = '',
-                 api: Optional[str] = '',
-                 token: Optional[str] = '',
-                 discovery_url: Optional[str] = '',
-                 key: Optional[str] = '',
-                 username: Optional[str] = '',
-                 password: Optional[str] = '',
-                 errors: Optional[str] = 'coerce',
-                 **kwargs):
+    def __init__(
+        self,
+        workspace: Optional[str] = "",
+        api: Optional[str] = "",
+        token: Optional[str] = "",
+        discovery_url: Optional[str] = "",
+        key: Optional[str] = "",
+        username: Optional[str] = "",
+        password: Optional[str] = "",
+        errors: Optional[str] = "coerce",
+        **kwargs,
+    ):
         """
         Parameters
         ----------
         workspace : str, default None
             Workspace name
         api : str, default None
             Web api endpoint
@@ -63,16 +69,18 @@
             Password
         errors : str, default 'coerce'
             If ‘raise’, then invalid request will raise an exception.
             If ‘coerce’, then invalid request will issue a warning and return None.
             If ‘ignore’, then invalid request will return the response.
         """
 
-        super().__init__(workspace=workspace,
-                         api=api,
-                         token=token,
-                         discovery_url=discovery_url,
-                         key=key,
-                         username=username,
-                         password=password,
-                         errors=errors,
-                         **kwargs)
+        super().__init__(
+            workspace=workspace,
+            api=api,
+            token=token,
+            discovery_url=discovery_url,
+            key=key,
+            username=username,
+            password=password,
+            errors=errors,
+            **kwargs,
+        )
```

### Comparing `petrovisor-0.1.2/src/petrovisor.egg-info/PKG-INFO` & `petrovisor-0.1.3/src/petrovisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petrovisor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for PetroVisor platform.
 Home-page: https://github.com/Datagration/petrovisor-python-api
 Author: Datagration Solutions Inc.
 Author-email: "Datagration Solutions Inc." <developers@datagration.com>
 License: MIT License
         
         Copyright (c) 2021 Datagration Solutions Inc.
```

### Comparing `petrovisor-0.1.2/src/petrovisor.egg-info/SOURCES.txt` & `petrovisor-0.1.3/src/petrovisor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/petrovisor/api/dtypes/__init__.py
 src/petrovisor/api/dtypes/data_grids.py
 src/petrovisor/api/dtypes/increments.py
 src/petrovisor/api/dtypes/internal_dtypes.py
 src/petrovisor/api/dtypes/items.py
 src/petrovisor/api/dtypes/ml.py
 src/petrovisor/api/methods/__init__.py
+src/petrovisor/api/methods/contexts.py
 src/petrovisor/api/methods/data_grids.py
 src/petrovisor/api/methods/dataframes.py
 src/petrovisor/api/methods/entities.py
 src/petrovisor/api/methods/files.py
 src/petrovisor/api/methods/items.py
 src/petrovisor/api/methods/logs.py
 src/petrovisor/api/methods/ml.py
```

### Comparing `petrovisor-0.1.2/tests/test_entities_and_signals.py` & `petrovisor-0.1.3/tests/test_entities_and_signals.py`

 * *Files identical despite different names*

### Comparing `petrovisor-0.1.2/tests/test_reference_tables.py` & `petrovisor-0.1.3/tests/test_reference_tables.py`

 * *Files identical despite different names*

