# Comparing `tmp/mergoo-0.0.6.tar.gz` & `tmp/mergoo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergoo-0.0.6.tar", last modified: Mon Apr  8 11:16:25 2024, max compression
+gzip compressed data, was "mergoo-0.0.7.tar", last modified: Sat Apr 13 19:04:46 2024, max compression
```

## Comparing `mergoo-0.0.6.tar` & `mergoo-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 11:16:25.060763 mergoo-0.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2024-04-08 10:00:06.000000 mergoo-0.0.6/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14892 2024-04-08 11:16:25.060763 mergoo-0.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5185 2024-04-08 11:15:50.000000 mergoo-0.0.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 11:16:25.056763 mergoo-0.0.6/mergoo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8276 2024-04-08 11:04:33.000000 mergoo-0.0.6/mergoo/compose_experts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2688 2024-04-08 10:00:06.000000 mergoo-0.0.6/mergoo/compose_layers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9649 2024-04-08 10:00:06.000000 mergoo-0.0.6/mergoo/safe_saving.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 11:16:25.060763 mergoo-0.0.6/mergoo.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14892 2024-04-08 11:16:25.000000 mergoo-0.0.6/mergoo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2024-04-08 11:16:25.000000 mergoo-0.0.6/mergoo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-08 11:16:25.000000 mergoo-0.0.6/mergoo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      163 2024-04-08 11:16:25.000000 mergoo-0.0.6/mergoo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-08 11:16:25.000000 mergoo-0.0.6/mergoo.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2024-04-08 11:16:18.000000 mergoo-0.0.6/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-08 11:16:25.060763 mergoo-0.0.6/setup.cfg
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     7651 2024-04-13 18:59:15.000000 mergoo-0.0.7/LICENSE
+-rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)     9732 2024-04-13 19:04:46.463332 mergoo-0.0.7/PKG-INFO
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/mergoo/
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     1412 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/compose_experts.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9272 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/compose_layers.py
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)     9649 2024-04-13 18:59:15.000000 mergoo-0.0.7/mergoo/safe_saving.py
+drwxrwxr-x   0 alirezamsh  (1000) alirezamsh  (1000)        0 2024-04-13 19:04:46.463332 mergoo-0.0.7/mergoo.egg-info/
+-rw-r--r--   0 alirezamsh  (1000) alirezamsh  (1000)     9732 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/PKG-INFO
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      244 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        1 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      163 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/requires.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)        7 2024-04-13 19:04:46.000000 mergoo-0.0.7/mergoo.egg-info/top_level.txt
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)      978 2024-04-13 19:00:36.000000 mergoo-0.0.7/pyproject.toml
+-rw-rw-r--   0 alirezamsh  (1000) alirezamsh  (1000)       38 2024-04-13 19:04:46.463332 mergoo-0.0.7/setup.cfg
```

### Comparing `mergoo-0.0.6/LICENSE` & `mergoo-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.6/mergoo/safe_saving.py` & `mergoo-0.0.7/mergoo/safe_saving.py`

 * *Files identical despite different names*

### Comparing `mergoo-0.0.6/pyproject.toml` & `mergoo-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mergoo"
-version = "0.0.6"
+version = "0.0.7"
 description = "Impelementation of Leeroo LLM composer."
 authors = [{ name = "Leeroo Team", email = "support@leeroo.com" }]
 readme = "README.md"
-keywords = ["LLM", "compose", "MoE", "router"]
+keywords = ["LLM", "compose", "MoE", "router", "mixture-of-adapters", "merge"]
 license = {file = "LICENSE"}
 dependencies = [
     "torch>=2.0.0",
     "tqdm==4.66.2",
     "safetensors~=0.4.2",
     "accelerate~=0.27.2",
     "transformers",
@@ -27,15 +27,15 @@
 [project.urls]
 homepage = "https://github.com/Leeroo-AI/mergoo"
 repository = "https://github.com/Leeroo-AI/mergoo"
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
 python_version = "3.10"
-strict = true
+strict = false
 
 [project.optional-dependencies]
 dev = ["super-lint"]
 
 [tool.setuptools]
 packages = ["mergoo"]
```

