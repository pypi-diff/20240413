# Comparing `tmp/ogusa-0.1.4.tar.gz` & `tmp/ogusa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogusa-0.1.4.tar", last modified: Fri Apr  5 02:05:48 2024, max compression
+gzip compressed data, was "ogusa-0.1.5.tar", last modified: Fri Apr 12 23:38:47 2024, max compression
```

## Comparing `ogusa-0.1.4.tar` & `ogusa-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.396954 ogusa-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-05 02:05:44.000000 ogusa-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-05 02:05:48.396954 ogusa-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-05 02:05:44.000000 ogusa-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.392954 ogusa-0.1.4/ogusa/
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/bequest_transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/calibrate_chi_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/deterministic_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/estimate_beta_j.py
--rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/get_micro_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/labor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/macro_params.py
--rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/ogusa_default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/psid_data_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/psid_summ_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/transfer_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/wealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-04-05 02:05:44.000000 ogusa-0.1.4/ogusa/wealthinit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:05:48.396954 ogusa-0.1.4/ogusa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 02:05:48.000000 ogusa-0.1.4/ogusa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 02:05:44.000000 ogusa-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:05:48.396954 ogusa-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-05 02:05:44.000000 ogusa-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-12 23:38:43.000000 ogusa-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 23:38:47.534392 ogusa-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-12 23:38:43.000000 ogusa-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/ogusa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/bequest_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/calibrate_chi_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/deterministic_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/estimate_beta_j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/get_micro_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/labor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/macro_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2040787 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/ogusa_default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/psid_data_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/psid_summ_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/transfer_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/wealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-04-12 23:38:44.000000 ogusa-0.1.5/ogusa/wealthinit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:38:47.534392 ogusa-0.1.5/ogusa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 23:38:47.000000 ogusa-0.1.5/ogusa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 23:38:44.000000 ogusa-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:38:47.534392 ogusa-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-12 23:38:44.000000 ogusa-0.1.5/setup.py
```

### Comparing `ogusa-0.1.4/LICENSE` & `ogusa-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/PKG-INFO` & `ogusa-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.4
+Version: 0.1.5
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.4/README.md` & `ogusa-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/bequest_transmission.py` & `ogusa-0.1.5/ogusa/bequest_transmission.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/calibrate.py` & `ogusa-0.1.5/ogusa/calibrate.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/calibrate_chi_n.py` & `ogusa-0.1.5/ogusa/calibrate_chi_n.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/constants.py` & `ogusa-0.1.5/ogusa/constants.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/deterministic_profiles.py` & `ogusa-0.1.5/ogusa/deterministic_profiles.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/estimate_beta_j.py` & `ogusa-0.1.5/ogusa/estimate_beta_j.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/get_micro_data.py` & `ogusa-0.1.5/ogusa/get_micro_data.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/income.py` & `ogusa-0.1.5/ogusa/income.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/labor.py` & `ogusa-0.1.5/ogusa/labor.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/macro_params.py` & `ogusa-0.1.5/ogusa/macro_params.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/ogusa_default_parameters.json` & `ogusa-0.1.5/ogusa/ogusa_default_parameters.json`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/psid_data_setup.py` & `ogusa-0.1.5/ogusa/psid_data_setup.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/psid_summ_stats.py` & `ogusa-0.1.5/ogusa/psid_summ_stats.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/transfer_distribution.py` & `ogusa-0.1.5/ogusa/transfer_distribution.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/utils.py` & `ogusa-0.1.5/ogusa/utils.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/wealth.py` & `ogusa-0.1.5/ogusa/wealth.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa/wealthinit.py` & `ogusa-0.1.5/ogusa/wealthinit.py`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/ogusa.egg-info/PKG-INFO` & `ogusa-0.1.5/ogusa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogusa
-Version: 0.1.4
+Version: 0.1.5
 Summary: USA calibration for OG-Core
 Home-page: https://github.com/PSLmodels/OG-USA/
 Download-URL: https://github.com/PSLmodels/OG-USA/
 Author: Jason DeBacker and Richard W. Evans
 License: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Project-URL: Issue Tracker, https://github.com/PSLmodels/OG-USA/issues
 Keywords: USA calibration of large scale overlapping generations model of fiscal policy
```

### Comparing `ogusa-0.1.4/ogusa.egg-info/SOURCES.txt` & `ogusa-0.1.5/ogusa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogusa-0.1.4/setup.py` & `ogusa-0.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-"""This file contains the OG-USA package's metadata and dependencies."""
-
-from setuptools import find_packages, setup
+import setuptools
 
 with open("README.md", "r") as readme_file:
-    readme = readme_file.read()
+    longdesc = readme_file.read()
 
-setup(
+setuptools.setup(
     name="ogusa",
-    version="0.1.4",
+    version="0.1.5",
     author="Jason DeBacker and Richard W. Evans",
     license="CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     description="USA calibration for OG-Core",
-    long_description=readme,
     long_description_content_type="text/markdown",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Natural Language :: English",
-        "License :: OSI Approved :: Common Public License",
-        "Operating System :: POSIX",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
+    long_description=longdesc,
     keywords="USA calibration of large scale overlapping generations model of fiscal policy",
     url="https://github.com/PSLmodels/OG-USA/",
     download_url="https://github.com/PSLmodels/OG-USA/",
     project_urls={
         "Issue Tracker": "https://github.com/PSLmodels/OG-USA/issues",
     },
     packages=["ogusa"],
@@ -52,9 +37,22 @@
         "xlwt",
         "openpyxl>=3.1.2",
         "statsmodels",
         "linearmodels",
         "wheel",
         "ogcore",
     ],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "License :: OSI Approved :: Common Public License",
+        "Operating System :: POSIX",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
     tests_require=["pytest"],
 )
```

