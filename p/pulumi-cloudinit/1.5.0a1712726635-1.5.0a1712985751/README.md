# Comparing `tmp/pulumi_cloudinit-1.5.0a1712726635.tar.gz` & `tmp/pulumi_cloudinit-1.5.0a1712985751.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.5.0a1712726635.tar", last modified: Wed Apr 10 05:28:19 2024, max compression
+gzip compressed data, was "pulumi_cloudinit-1.5.0a1712985751.tar", last modified: Sat Apr 13 05:26:41 2024, max compression
```

## Comparing `pulumi_cloudinit-1.5.0a1712726635.tar` & `pulumi_cloudinit-1.5.0a1712985751.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:28:19.235444 pulumi_cloudinit-1.5.0a1712726635/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-10 05:28:19.235444 pulumi_cloudinit-1.5.0a1712726635/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:28:19.235444 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:28:19.235444 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-10 05:28:19.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-10 05:28:19.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:28:19.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 05:28:19.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 05:28:19.000000 pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 05:28:12.000000 pulumi_cloudinit-1.5.0a1712726635/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:28:19.235444 pulumi_cloudinit-1.5.0a1712726635/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:26:41.972562 pulumi_cloudinit-1.5.0a1712985751/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-13 05:26:41.972562 pulumi_cloudinit-1.5.0a1712985751/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:26:41.972562 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:26:41.972562 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-13 05:26:41.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 05:26:41.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:26:41.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 05:26:41.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 05:26:41.000000 pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 05:26:35.000000 pulumi_cloudinit-1.5.0a1712985751/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:26:41.972562 pulumi_cloudinit-1.5.0a1712985751/setup.cfg
```

### Comparing `pulumi_cloudinit-1.5.0a1712726635/PKG-INFO` & `pulumi_cloudinit-1.5.0a1712985751/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1712726635
+Version: 1.5.0a1712985751
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1712726635/README.md` & `pulumi_cloudinit-1.5.0a1712985751/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.5.0a1712985751/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1712726635
+Version: 1.5.0a1712985751
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1712726635/pyproject.toml` & `pulumi_cloudinit-1.5.0a1712985751/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_cloudinit"
   description = "A Pulumi package for creating and managing cloudinit cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "cloudinit"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.5.0a1712726635"
+  version = "1.5.0a1712985751"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-cloudinit"
 
 [build-system]
```

