# Comparing `tmp/bmt-1.3.0.tar.gz` & `tmp/bmt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmt-1.3.0.tar", max compression
+gzip compressed data, was "bmt-1.4.0.tar", max compression
```

## Comparing `bmt-1.3.0.tar` & `bmt-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1544 2024-04-08 21:22:55.826008 bmt-1.3.0/LICENSE
--rw-r--r--   0        0        0     1110 2024-04-08 21:22:55.826008 bmt-1.3.0/README.md
--rw-r--r--   0        0        0       31 2024-04-08 21:22:55.826008 bmt-1.3.0/bmt/__init__.py
--rw-r--r--   0        0        0    74545 2024-04-08 21:22:55.826008 bmt-1.3.0/bmt/toolkit.py
--rw-r--r--   0        0        0     3843 2024-04-08 21:22:55.826008 bmt-1.3.0/bmt/utils.py
--rw-r--r--   0        0        0     1585 2024-04-08 21:23:09.274010 bmt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 bmt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-04-13 01:02:48.592183 bmt-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1110 2024-04-13 01:02:48.592183 bmt-1.4.0/README.md
+-rw-r--r--   0        0        0       31 2024-04-13 01:02:48.592183 bmt-1.4.0/bmt/__init__.py
+-rw-r--r--   0        0        0    74545 2024-04-13 01:02:48.592183 bmt-1.4.0/bmt/toolkit.py
+-rw-r--r--   0        0        0     3843 2024-04-13 01:02:48.592183 bmt-1.4.0/bmt/utils.py
+-rw-r--r--   0        0        0     1585 2024-04-13 01:02:59.852199 bmt-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 bmt-1.4.0/PKG-INFO
```

### Comparing `bmt-1.3.0/LICENSE` & `bmt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bmt-1.3.0/README.md` & `bmt-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bmt-1.3.0/bmt/toolkit.py` & `bmt-1.4.0/bmt/toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     SlotDefinition,
 )
 from bmt.utils import format_element, parse_name
 
 Url = str
 Path = str
 
-LATEST_BIOLINK_RELEASE = "4.1.6"
+LATEST_BIOLINK_RELEASE = "4.2.0"
 
 REMOTE_PATH = f"https://raw.githubusercontent.com/biolink/biolink-model/v{LATEST_BIOLINK_RELEASE}/biolink-model.yaml"
 PREDICATE_MAP = f"https://raw.githubusercontent.com/biolink/biolink-model/v{LATEST_BIOLINK_RELEASE}/predicate_mapping.yaml"
 
 
 NODE_PROPERTY = "node property"
 ASSOCIATION_SLOT = "association slot"
```

### Comparing `bmt-1.3.0/bmt/utils.py` & `bmt-1.4.0/bmt/utils.py`

 * *Files identical despite different names*

### Comparing `bmt-1.3.0/pyproject.toml` & `bmt-1.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmt"
-version = "1.3.0"
+version = "1.4.0"
 description = "Biolink Model Toolkit: A Python API for working with the Biolink Model"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "BSD"
 
 readme = "README.md"
 repository = "https://github.com/biolink/biolink-model-toolkit"
 documentation = "https://biolink.github.io/biolink-model-toolkit/"
```

### Comparing `bmt-1.3.0/PKG-INFO` & `bmt-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmt
-Version: 1.3.0
+Version: 1.4.0
 Summary: Biolink Model Toolkit: A Python API for working with the Biolink Model
 Home-page: https://github.com/biolink/biolink-model-toolkit
 License: BSD
 Keywords: schema,linked data,data modeling,biolink,api
 Author: Sierra Taylor Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<4.0
```

