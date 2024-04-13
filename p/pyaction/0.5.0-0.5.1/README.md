# Comparing `tmp/pyaction-0.5.0.tar.gz` & `tmp/pyaction-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.5.0.tar", last modified: Sat Apr 13 10:59:56 2024, max compression
+gzip compressed data, was "pyaction-0.5.1.tar", last modified: Sat Apr 13 12:11:39 2024, max compression
```

## Comparing `pyaction-0.5.0.tar` & `pyaction-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:56.339787 pyaction-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-13 10:59:52.000000 pyaction-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-13 10:59:56.339787 pyaction-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-13 10:59:52.000000 pyaction-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:56.335787 pyaction-0.5.0/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:56.339787 pyaction-0.5.0/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyaction/issues/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:59:56.339787 pyaction-0.5.0/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 10:59:56.000000 pyaction-0.5.0/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-13 10:59:52.000000 pyaction-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:59:56.339787 pyaction-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-13 12:11:35.000000 pyaction-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 12:11:35.000000 pyaction-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-13 12:11:39.901695 pyaction-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-13 12:11:35.000000 pyaction-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.897695 pyaction-0.5.1/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/issues/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.897695 pyaction-0.5.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:11:39.901695 pyaction-0.5.1/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 12:11:39.000000 pyaction-0.5.1/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-13 12:11:35.000000 pyaction-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 12:11:39.901695 pyaction-0.5.1/setup.cfg
```

### Comparing `pyaction-0.5.0/LICENSE` & `pyaction-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.0/PKG-INFO` & `pyaction-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.0
+Version: 0.5.1
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml) [![main](https://github.com/lnxpy/pyaction/actions/workflows/main.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/main.yml) ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version)
+## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.0/README.md` & `pyaction-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## PyAction [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml) [![main](https://github.com/lnxpy/pyaction/actions/workflows/main.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/main.yml) ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version)
+## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.0/pyaction/auth.py` & `pyaction-0.5.1/pyaction/auth.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.0/pyaction/cli.py` & `pyaction-0.5.1/pyaction/cli.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.0/pyaction/io.py` & `pyaction-0.5.1/pyaction/io.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.0/pyaction/issues/connector.py` & `pyaction-0.5.1/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.0/pyaction.egg-info/PKG-INFO` & `pyaction-0.5.1/pyaction.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.0
+Version: 0.5.1
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml) [![main](https://github.com/lnxpy/pyaction/actions/workflows/main.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/main.yml) ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version)
+## PyAction ![version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![docs ci](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.0/pyproject.toml` & `pyaction-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.5.0"
+version = "0.5.1"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
     "pygithub >= 2.3.0",
@@ -25,15 +25,15 @@
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.5.1"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```

