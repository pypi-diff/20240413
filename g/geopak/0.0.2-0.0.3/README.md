# Comparing `tmp/geopak-0.0.2.tar.gz` & `tmp/geopak-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopak-0.0.2.tar", last modified: Tue Apr  2 19:09:44 2024, max compression
+gzip compressed data, was "geopak-0.0.3.tar", last modified: Sat Apr 13 12:07:21 2024, max compression
```

## Comparing `geopak-0.0.2.tar` & `geopak-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 19:09:30.000000 geopak-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.890041 geopak-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 19:09:30.000000 geopak-0.0.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-02 19:09:30.000000 geopak-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:09:30.000000 geopak-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:09:30.000000 geopak-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 19:09:44.898041 geopak-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 19:09:30.000000 geopak-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.894041 geopak-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/csv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/iris.csv
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/sample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/examples/vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/geopak.md
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:09:30.000000 geopak-0.0.2/docs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/geopak/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/geopak.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 19:09:30.000000 geopak-0.0.2/geopak/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/geopak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 19:09:44.000000 geopak-0.0.2/geopak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-02 19:09:30.000000 geopak-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 19:09:30.000000 geopak-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:09:30.000000 geopak-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 19:09:30.000000 geopak-0.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:09:44.898041 geopak-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:44.898041 geopak-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:09:30.000000 geopak-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 19:09:30.000000 geopak-0.0.2/tests/test_geopak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.763816 geopak-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-13 12:07:05.000000 geopak-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.755817 geopak-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.755817 geopak-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.759817 geopak-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-13 12:07:05.000000 geopak-0.0.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-13 12:07:05.000000 geopak-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:07:05.000000 geopak-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-13 12:07:05.000000 geopak-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 12:07:21.763816 geopak-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 12:07:05.000000 geopak-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.759817 geopak-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.759817 geopak-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/sample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/geopak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.759817 geopak-0.0.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-13 12:07:05.000000 geopak-0.0.3/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.759817 geopak-0.0.3/geopak/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 12:07:05.000000 geopak-0.0.3/geopak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 12:07:05.000000 geopak-0.0.3/geopak/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-04-13 12:07:05.000000 geopak-0.0.3/geopak/geopak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 12:07:05.000000 geopak-0.0.3/geopak/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.763816 geopak-0.0.3/geopak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 12:07:21.000000 geopak-0.0.3/geopak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-13 12:07:05.000000 geopak-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 12:07:05.000000 geopak-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 12:07:05.000000 geopak-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-13 12:07:05.000000 geopak-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 12:07:21.763816 geopak-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:07:21.763816 geopak-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-13 12:07:05.000000 geopak-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-13 12:07:05.000000 geopak-0.0.3/tests/test_geopak.py
```

### Comparing `geopak-0.0.2/.github/workflows/docs-build.yml` & `geopak-0.0.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/docs.yml` & `geopak-0.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/installation.yml` & `geopak-0.0.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/macos.yml` & `geopak-0.0.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/pypi.yml` & `geopak-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/ubuntu.yml` & `geopak-0.0.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.github/workflows/windows.yml` & `geopak-0.0.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/.gitignore` & `geopak-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/PKG-INFO` & `geopak-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopak
-Version: 0.0.2
+Version: 0.0.3
 Summary: python package demo for geodpatial analysis
 Author-email: Albert Tandoh <atandoh004@St.ug.edu.gh>
 License: MIT License
 Project-URL: Homepage, https://github.com/Tandoh004/geopak
 Keywords: geopak
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geopak-0.0.2/docs/contributing.md` & `geopak-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/docs/examples/csv.ipynb` & `geopak-0.0.3/docs/examples/csv.ipynb`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/docs/examples/iris.csv` & `geopak-0.0.3/docs/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/docs/examples/sample.ipynb` & `geopak-0.0.3/docs/examples/sample.ipynb`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/docs/examples/vector.ipynb` & `geopak-0.0.3/docs/examples/vector.ipynb`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/docs/installation.md` & `geopak-0.0.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/geopak.egg-info/PKG-INFO` & `geopak-0.0.3/geopak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopak
-Version: 0.0.2
+Version: 0.0.3
 Summary: python package demo for geodpatial analysis
 Author-email: Albert Tandoh <atandoh004@St.ug.edu.gh>
 License: MIT License
 Project-URL: Homepage, https://github.com/Tandoh004/geopak
 Keywords: geopak
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geopak-0.0.2/geopak.egg-info/SOURCES.txt` & `geopak-0.0.3/geopak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/mkdocs.yml` & `geopak-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `geopak-0.0.2/pyproject.toml` & `geopak-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geopak"
-version = "0.0.2"
+version = "0.0.3"
 dynamic = [
     "dependencies",
 ]
 description = "python package demo for geodpatial analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.2"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

