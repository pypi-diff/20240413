# Comparing `tmp/pyserato-0.0.1.tar.gz` & `tmp/pyserato-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserato-0.0.1.tar", last modified: Mon Jan  8 09:35:27 2024, max compression
+gzip compressed data, was "pyserato-0.0.2.tar", last modified: Sat Apr 13 16:43:29 2024, max compression
```

## Comparing `pyserato-0.0.1.tar` & `pyserato-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.650512 pyserato-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.646512 pyserato-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.646512 pyserato-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-08 09:35:21.000000 pyserato-0.0.1/.github/workflows/main_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-08 09:35:21.000000 pyserato-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-08 09:35:21.000000 pyserato-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-08 09:35:27.650512 pyserato-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-08 09:35:21.000000 pyserato-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-08 09:35:21.000000 pyserato-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 09:35:27.650512 pyserato-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.646512 pyserato-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.650512 pyserato-0.0.1/src/pyserato/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:21.000000 pyserato-0.0.1/src/pyserato/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-01-08 09:35:21.000000 pyserato-0.0.1/src/pyserato/crate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:21.000000 pyserato-0.0.1/src/pyserato/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-08 09:35:21.000000 pyserato-0.0.1/src/pyserato/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.650512 pyserato-0.0.1/src/pyserato.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-08 09:35:27.000000 pyserato-0.0.1/src/pyserato.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-08 09:35:27.000000 pyserato-0.0.1/src/pyserato.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 09:35:27.000000 pyserato-0.0.1/src/pyserato.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-08 09:35:27.000000 pyserato-0.0.1/src/pyserato.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-08 09:35:27.000000 pyserato-0.0.1/src/pyserato.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 09:35:27.650512 pyserato-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-01-08 09:35:21.000000 pyserato-0.0.1/tests/test_crate.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-08 09:35:21.000000 pyserato-0.0.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:22.000000 pyserato-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.067403 pyserato-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-13 16:43:22.000000 pyserato-0.0.2/.github/workflows/main_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 16:43:22.000000 pyserato-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-13 16:43:22.000000 pyserato-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-13 16:43:29.071403 pyserato-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-13 16:43:22.000000 pyserato-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-13 16:43:22.000000 pyserato-0.0.2/examples/create_crates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-13 16:43:22.000000 pyserato-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:43:29.071403 pyserato-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.067403 pyserato-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/src/pyserato/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:22.000000 pyserato-0.0.2/src/pyserato/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-13 16:43:22.000000 pyserato-0.0.2/src/pyserato/crate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:22.000000 pyserato-0.0.2/src/pyserato/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-13 16:43:22.000000 pyserato-0.0.2/src/pyserato/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/src/pyserato.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-13 16:43:29.000000 pyserato-0.0.2/src/pyserato.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 16:43:29.000000 pyserato-0.0.2/src/pyserato.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:43:29.000000 pyserato-0.0.2/src/pyserato.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 16:43:29.000000 pyserato-0.0.2/src/pyserato.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 16:43:29.000000 pyserato-0.0.2/src/pyserato.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:43:29.071403 pyserato-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-13 16:43:22.000000 pyserato-0.0.2/tests/test_crate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-13 16:43:22.000000 pyserato-0.0.2/tests/test_util.py
```

### Comparing `pyserato-0.0.1/.github/workflows/main_test.yaml` & `pyserato-0.0.2/.github/workflows/main_test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
           pip install -e .
           pip install -e .[test]
       - name: Test with pytest
         run: |
           flake8 --max-line-length=120 src tests
           mypy src tests
           coverage run -m pytest tests
-          coverage report --fail-under=95
+          coverage report --fail-under=98
```

### Comparing `pyserato-0.0.1/LICENSE` & `pyserato-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserato-0.0.1/pyproject.toml` & `pyserato-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pyserato"
 description = "PySerato API."
 readme = "README.md"
-version = '0.0.1'
+version = '0.0.2'
 authors = [
     { name = "Luke Purnell", email = "luke.a.purnell@gmail.com" }
 ]
 
 
 [project.optional-dependencies]
 dev = [
```

