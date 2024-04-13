# Comparing `tmp/pulumi_eks-2.4a1712955188.tar.gz` & `tmp/pulumi_eks-2.4a1712956359.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-2.4a1712955188.tar", last modified: Fri Apr 12 20:59:40 2024, max compression
+gzip compressed data, was "pulumi_eks-2.4a1712956359.tar", last modified: Fri Apr 12 21:31:05 2024, max compression
```

## Comparing `pulumi_eks-2.4a1712955188.tar` & `pulumi_eks-2.4a1712956359.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:59:40.443694 pulumi_eks-2.4a1712955188/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-12 20:59:40.443694 pulumi_eks-2.4a1712955188/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:59:40.439695 pulumi_eks-2.4a1712955188/pulumi_eks/
--rw-------   0 runner    (1001) docker     (127)     1150 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (127)    85348 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9222 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (127)    94098 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (127)     4860 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (127)    30218 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (127)    46243 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (127)     8405 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (127)    49155 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (127)    38606 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2715 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (127)       40 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (127)    39043 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:59:40.443694 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-12 20:59:40.000000 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 20:59:40.000000 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:59:40.000000 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 20:59:40.000000 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 20:59:40.000000 pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      720 2024-04-12 20:59:34.000000 pulumi_eks-2.4a1712955188/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:59:40.443694 pulumi_eks-2.4a1712955188/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:05.038008 pulumi_eks-2.4a1712956359/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-12 21:31:05.038008 pulumi_eks-2.4a1712956359/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:05.038008 pulumi_eks-2.4a1712956359/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (127)     1150 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    85348 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9222 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)    94098 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (127)     4860 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (127)    30218 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (127)    46243 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (127)     8405 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (127)    49155 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (127)    38606 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2715 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (127)       40 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (127)    39043 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:05.038008 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-12 21:31:05.000000 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 21:31:05.000000 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:31:05.000000 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 21:31:05.000000 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 21:31:05.000000 pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      720 2024-04-12 21:30:58.000000 pulumi_eks-2.4a1712956359/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:31:05.038008 pulumi_eks-2.4a1712956359/setup.cfg
```

### Comparing `pulumi_eks-2.4a1712955188/PKG-INFO` & `pulumi_eks-2.4a1712956359/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1712955188
+Version: 2.4.0a1712956359
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1712955188 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1712956359 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4a1712955188/README.md` & `pulumi_eks-2.4a1712956359/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/__init__.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/_inputs.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/_utilities.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/cluster.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/cluster_creation_role_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/managed_node_group.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/node_group.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/node_group_security_group.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/node_group_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/node_group_v2.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/node_group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/outputs.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/provider.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks/vpc_cni.py` & `pulumi_eks-2.4a1712956359/pulumi_eks/vpc_cni.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1712955188
+Version: 2.4.0a1712956359
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1712955188 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1712956359 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4a1712955188/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-2.4a1712956359/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4a1712955188/pyproject.toml` & `pulumi_eks-2.4a1712956359/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_eks"
   description = "Pulumi Amazon Web Services (AWS) EKS Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-aws>=6.0.0,<7.0.0", "pulumi-kubernetes>=4.0.0,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "eks"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1712955188"
+  version = "2.4.0a1712956359"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-eks"
 
 [build-system]
```

