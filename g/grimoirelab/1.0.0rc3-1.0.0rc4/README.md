# Comparing `tmp/grimoirelab-1.0.0rc3.tar.gz` & `tmp/grimoirelab-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab-1.0.0rc3.tar", max compression
+gzip compressed data, was "grimoirelab-1.0.0rc4.tar", max compression
```

## Comparing `grimoirelab-1.0.0rc3.tar` & `grimoirelab-1.0.0rc4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2024-04-11 11:34:01.686269 grimoirelab-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     8685 2024-04-11 11:34:01.686269 grimoirelab-1.0.0rc3/README.md
--rw-r--r--   0        0        0       34 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/__init__.py
--rw-r--r--   0        0        0       91 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/_version.py
--rwxr-xr-x   0        0        0     1844 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/grimoirelab.py
--rw-r--r--   0        0        0     1882 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 grimoirelab-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-04-12 16:19:40.057178 grimoirelab-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     8685 2024-04-12 16:19:40.061178 grimoirelab-1.0.0rc4/README.md
+-rw-r--r--   0        0        0       34 2024-04-12 16:19:40.125178 grimoirelab-1.0.0rc4/grimoirelab/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-12 16:19:40.125178 grimoirelab-1.0.0rc4/grimoirelab/_version.py
+-rwxr-xr-x   0        0        0     1844 2024-04-12 16:19:40.125178 grimoirelab-1.0.0rc4/grimoirelab/grimoirelab.py
+-rw-r--r--   0        0        0     1882 2024-04-12 16:19:40.129178 grimoirelab-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 grimoirelab-1.0.0rc4/PKG-INFO
```

### Comparing `grimoirelab-1.0.0rc3/LICENSE` & `grimoirelab-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc3/README.md` & `grimoirelab-1.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc3/grimoirelab/grimoirelab.py` & `grimoirelab-1.0.0rc4/grimoirelab/grimoirelab.py`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc3/pyproject.toml` & `grimoirelab-1.0.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab"
-version = "1.0.0-rc.3"
+version = "1.0.0-rc.4"
 description = "Tool set for software development analytics"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -39,19 +39,19 @@
 python = "^3.8"
 
 grimoirelab-toolkit = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 perceval-mozilla = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 perceval-opnfv = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 perceval-puppet = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 perceval-weblate = {version = ">=1.0.0-rc.2", allow-prereleases = true}
-sortinghat = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+sortinghat = {version = ">=1.0.0-rc.3", allow-prereleases = true}
 kidash = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 grimoirelab-panels = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-grimoire-elk = {version = ">=1.0.0-rc.2", allow-prereleases = true}
-sirmordred = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+grimoire-elk = {version = ">=1.0.0-rc.3", allow-prereleases = true}
+sirmordred = {version = ">=1.0.0-rc.3", allow-prereleases = true}
 cereslib = {version = ">=1.0.0-rc.1", allow-prereleases = true}
 graal = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 perceval = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `grimoirelab-1.0.0rc3/PKG-INFO` & `grimoirelab-1.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Tool set for software development analytics
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: cereslib (>=1.0.0-rc.1)
 Requires-Dist: graal (>=1.0.0-rc.2)
-Requires-Dist: grimoire-elk (>=1.0.0-rc.2)
+Requires-Dist: grimoire-elk (>=1.0.0-rc.3)
 Requires-Dist: grimoirelab-panels (>=1.0.0-rc.1)
 Requires-Dist: grimoirelab-toolkit (>=1.0.0-rc.2)
 Requires-Dist: kidash (>=1.0.0-rc.2)
 Requires-Dist: perceval (>=1.0.0-rc.2)
 Requires-Dist: perceval-mozilla (>=1.0.0-rc.2)
 Requires-Dist: perceval-opnfv (>=1.0.0-rc.2)
 Requires-Dist: perceval-puppet (>=1.0.0-rc.2)
 Requires-Dist: perceval-weblate (>=1.0.0-rc.2)
-Requires-Dist: sirmordred (>=1.0.0-rc.2)
-Requires-Dist: sortinghat (>=1.0.0-rc.2)
+Requires-Dist: sirmordred (>=1.0.0-rc.3)
+Requires-Dist: sortinghat (>=1.0.0-rc.3)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab
 Description-Content-Type: text/markdown
 
 # GrimoireLab
 
 [![grimoirelab-showcase](https://user-images.githubusercontent.com/25265451/84442403-30dcce80-ac5b-11ea-9f5b-60266d875ebd.png "GrimoireLab | CHAOSS Bitergia Analytics")](https://chaoss.biterg.io/app/kibana#/dashboard/Overview)
```

