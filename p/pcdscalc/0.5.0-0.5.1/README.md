# Comparing `tmp/pcdscalc-0.5.0.tar.gz` & `tmp/pcdscalc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdscalc-0.5.0.tar", last modified: Fri Sep 15 19:04:58 2023, max compression
+gzip compressed data, was "pcdscalc-0.5.1.tar", last modified: Fri Apr 12 22:10:43 2024, max compression
```

## Comparing `pcdscalc-0.5.0.tar` & `pcdscalc-0.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/source/be_lens_calcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs/source/pmps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.559876 pcdscalc-0.5.0/pcdscalc/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    37830 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/be_lens_calcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15319 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/diffraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/pmps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/pcdscalc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19199 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/test_be_lens_calcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/test_diffraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/pcdscalc/tests/test_lens_sets/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/test_lens_sets/lens_set
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/tests/test_pmps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pcdscalc/xray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/pcdscalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-15 19:04:58.000000 pcdscalc-0.5.0/pcdscalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-15 19:04:37.000000 pcdscalc-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 19:04:58.563876 pcdscalc-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.146473 pcdscalc-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.146473 pcdscalc-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.146473 pcdscalc-0.5.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.146473 pcdscalc-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.146473 pcdscalc-0.5.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/source/be_lens_calcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs/source/pmps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/pcdscalc/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37832 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15319 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/diffraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/pmps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/pcdscalc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19199 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/test_be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/test_diffraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/pcdscalc/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/test_lens_sets/lens_set
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/tests/test_pmps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pcdscalc/xray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/pcdscalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 22:10:43.000000 pcdscalc-0.5.1/pcdscalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 22:10:31.000000 pcdscalc-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:10:43.150473 pcdscalc-0.5.1/setup.cfg
```

### Comparing `pcdscalc-0.5.0/.flake8` & `pcdscalc-0.5.1/.flake8`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/.github/ISSUE_TEMPLATE.md` & `pcdscalc-0.5.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `pcdscalc-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/.github/workflows/standard.yml` & `pcdscalc-0.5.1/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/.gitignore` & `pcdscalc-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/.pre-commit-config.yaml` & `pcdscalc-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/CONTRIBUTING.rst` & `pcdscalc-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/LICENSE` & `pcdscalc-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/PKG-INFO` & `pcdscalc-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdscalc
-Version: 0.5.0
+Version: 0.5.1
 Summary: PCDS Calculation Routines
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pcdscalc-0.5.0/README.rst` & `pcdscalc-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/conda-recipe/meta.yaml` & `pcdscalc-0.5.1/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/docs/Makefile` & `pcdscalc-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/docs/make.bat` & `pcdscalc-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/docs/source/be_lens_calcs.rst` & `pcdscalc-0.5.1/docs/source/be_lens_calcs.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/docs/source/conf.py` & `pcdscalc-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/docs/source/index.rst` & `pcdscalc-0.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/be_lens_calcs.py` & `pcdscalc-0.5.1/pcdscalc/be_lens_calcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         except json.decoder.JSONDecodeError as err:
             logger.error('When getting the lens set: %s', err)
             raise err
 
         if get_all:
             return sets
 
-        if set_number_top_to_bot not in range(1, len(sets)):
+        if set_number_top_to_bot not in range(1, len(sets)+1):
             err_msg = ('Provided an invalid set_number_top_to_bottom: '
                        f'{set_number_top_to_bot}, please provide a number '
                        f'from 1 to {len(sets)}')
             logger.error(err_msg)
             raise ValueError(err_msg)
     # if only one set in the list, return the list
     if not isinstance(sets[0], list):
```

### Comparing `pcdscalc-0.5.0/pcdscalc/common.py` & `pcdscalc-0.5.1/pcdscalc/common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/constants.py` & `pcdscalc-0.5.1/pcdscalc/constants.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/diffraction.py` & `pcdscalc-0.5.1/pcdscalc/diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/pmps.py` & `pcdscalc-0.5.1/pcdscalc/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/tests/test_be_lens_calcs.py` & `pcdscalc-0.5.1/pcdscalc/tests/test_be_lens_calcs.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/tests/test_common.py` & `pcdscalc-0.5.1/pcdscalc/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/tests/test_diffraction.py` & `pcdscalc-0.5.1/pcdscalc/tests/test_diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/tests/test_pmps.py` & `pcdscalc-0.5.1/pcdscalc/tests/test_pmps.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/version.py` & `pcdscalc-0.5.1/pcdscalc/version.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc/xray.py` & `pcdscalc-0.5.1/pcdscalc/xray.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pcdscalc.egg-info/PKG-INFO` & `pcdscalc-0.5.1/pcdscalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdscalc
-Version: 0.5.0
+Version: 0.5.1
 Summary: PCDS Calculation Routines
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pcdscalc-0.5.0/pcdscalc.egg-info/SOURCES.txt` & `pcdscalc-0.5.1/pcdscalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.5.0/pyproject.toml` & `pcdscalc-0.5.1/pyproject.toml`

 * *Files identical despite different names*

