# Comparing `tmp/baypy-1.2.1.tar.gz` & `tmp/baypy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baypy-1.2.1.tar", last modified: Thu Apr 11 13:14:01 2024, max compression
+gzip compressed data, was "baypy-1.3.0.tar", last modified: Sat Apr 13 14:40:50 2024, max compression
```

## Comparing `baypy-1.2.1.tar` & `baypy-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.677600 baypy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:13:52.000000 baypy-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46879 2024-04-11 13:14:01.677600 baypy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-11 13:13:52.000000 baypy-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/analysis/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/diagnostics/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/model/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46879 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-11 13:13:52.000000 baypy-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:14:01.677600 baypy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 13:13:52.000000 baypy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.478768 baypy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 14:40:42.000000 baypy-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-04-13 14:40:50.478768 baypy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-13 14:40:42.000000 baypy-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.470769 baypy-1.3.0/baypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.474768 baypy-1.3.0/baypy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/analysis/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.474768 baypy-1.3.0/baypy/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/diagnostics/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.474768 baypy-1.3.0/baypy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/model/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.474768 baypy-1.3.0/baypy/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/regression/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-13 14:40:42.000000 baypy-1.3.0/baypy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:40:50.474768 baypy-1.3.0/baypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-04-13 14:40:50.000000 baypy-1.3.0/baypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 14:40:50.000000 baypy-1.3.0/baypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:40:50.000000 baypy-1.3.0/baypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-13 14:40:50.000000 baypy-1.3.0/baypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 14:40:50.000000 baypy-1.3.0/baypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-13 14:40:42.000000 baypy-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:40:50.478768 baypy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 14:40:42.000000 baypy-1.3.0/setup.py
```

### Comparing `baypy-1.2.1/LICENSE` & `baypy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/PKG-INFO` & `baypy-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baypy
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python library for solving bayesian regression models through a Monte Carlo Markov chain sampling
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,33 +679,34 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/baypy
 Project-URL: Documentation, https://baypy.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/baypy/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/baypy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: numpy==1.26.1
-Requires-Dist: pandas==2.0.3
-Requires-Dist: scipy==1.11.3
+Requires-Dist: matplotlib>=3.6
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy!=1.11.0,>=1.6
 Provides-Extra: doc
 Requires-Dist: furo==2023.8.19; extra == "doc"
 Requires-Dist: m2r2==0.3.3.post2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.3; extra == "test"
@@ -724,15 +725,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -746,15 +747,19 @@
    :target: https://pypi.org/project/baypy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `baypy-1.2.1/README.rst` & `baypy-1.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -31,15 +31,19 @@
    :target: https://pypi.org/project/baypy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `baypy-1.2.1/baypy/analysis/functions.py` & `baypy-1.3.0/baypy/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/diagnostics/functions.py` & `baypy-1.3.0/baypy/diagnostics/functions.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/model/linear_model.py` & `baypy-1.3.0/baypy/model/linear_model.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/model/model.py` & `baypy-1.3.0/baypy/model/model.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/regression/functions.py` & `baypy-1.3.0/baypy/regression/functions.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/regression/linear_regression.py` & `baypy-1.3.0/baypy/regression/linear_regression.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/regression/regression.py` & `baypy-1.3.0/baypy/regression/regression.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy/utils.py` & `baypy-1.3.0/baypy/utils.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/baypy.egg-info/PKG-INFO` & `baypy-1.3.0/baypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baypy
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python library for solving bayesian regression models through a Monte Carlo Markov chain sampling
 Author-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 Maintainer-email: Andrea Blengino <ing.andrea.blengino@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -679,33 +679,34 @@
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/AndreaBlengino/baypy
 Project-URL: Documentation, https://baypy.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/AndreaBlengino/baypy/issues
 Project-URL: Repository, https://github.com/AndreaBlengino/baypy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: numpy==1.26.1
-Requires-Dist: pandas==2.0.3
-Requires-Dist: scipy==1.11.3
+Requires-Dist: matplotlib>=3.6
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=2.0
+Requires-Dist: scipy!=1.11.0,>=1.6
 Provides-Extra: doc
 Requires-Dist: furo==2023.8.19; extra == "doc"
 Requires-Dist: m2r2==0.3.3.post2; extra == "doc"
 Requires-Dist: sphinx==7.2.6; extra == "doc"
 Provides-Extra: test
 Requires-Dist: coverage==7.3.2; extra == "test"
 Requires-Dist: hypothesis==6.88.3; extra == "test"
@@ -724,15 +725,15 @@
 
 .. list-table::
    :stub-columns: 1
    :widths: auto
    :width: 100%
 
    * - PyPI
-     - |pypi_release| |supported_python_versions| |build|
+     - |pypi_release| |supported_python_versions| |build| |dependencies|
    * - Tests
      - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
    * - Documentation
      - |docs|
    * - Code Quality
      - |codefactor_grade| |codacy_grade| |issues|
    * - License
@@ -746,15 +747,19 @@
    :target: https://pypi.org/project/baypy/
    :alt: PyPI - Supported Python Versions
 
 .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/release.yml.svg?logo=github
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/release.yml
    :alt: Package Build
 
-.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&label=Linux
+.. |dependencies| image:: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy/badge.svg
+   :target: https://dependency-dash.repo-helper.uk/github/AndreaBlengino/baypy
+   :alt: Dependencies Status
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&logoColor=white&label=Linux
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/linux_test.yml
    :alt: Linux Tests
 
 .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/macos_test.yml.svg?logo=apple&label=macOS
    :target: https://github.com/AndreaBlengino/baypy/actions/workflows/macos_test.yml
    :alt: macOS Tests
```

### Comparing `baypy-1.2.1/baypy.egg-info/SOURCES.txt` & `baypy-1.3.0/baypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baypy-1.2.1/pyproject.toml` & `baypy-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baypy"
 dynamic = ["version"]
-requires-python = ">=3.9,<3.13"
+requires-python = ">=3.9"
 dependencies = [
-  "matplotlib==3.7.2",
-  "numpy==1.26.1",
-  "pandas==2.0.3",
-  "scipy==1.11.3",
+  "matplotlib>=3.6",
+  "numpy>=1.20",
+  "pandas>=2.0",
+  "scipy>=1.6,!=1.11.0",
 ]
 authors = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 maintainers = [
   {name = "Andrea Blengino", email = "ing.andrea.blengino@protonmail.com"},
 ]
 description = "Python library for solving bayesian regression models through a Monte Carlo Markov chain sampling"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
+  "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Education",
   "Intended Audience :: Manufacturing",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
```

