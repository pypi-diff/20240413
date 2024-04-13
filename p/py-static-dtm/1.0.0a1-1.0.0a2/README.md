# Comparing `tmp/py_static_dtm-1.0.0a1.tar.gz` & `tmp/py_static_dtm-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_static_dtm-1.0.0a1.tar", last modified: Sat Apr 13 17:12:19 2024, max compression
+gzip compressed data, was "py_static_dtm-1.0.0a2.tar", last modified: Sat Apr 13 17:39:29 2024, max compression
```

## Comparing `py_static_dtm-1.0.0a1.tar` & `py_static_dtm-1.0.0a2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.970260 py_static_dtm-1.0.0a1/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.942260 py_static_dtm-1.0.0a1/.github/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.954260 py_static_dtm-1.0.0a1/.github/workflows/
--rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/.github/workflows/lint.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/.github/workflows/test.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/.gitignore
--rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a1/.pre-commit-config.yaml
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.954260 py_static_dtm-1.0.0a1/.vscode/
--rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/.vscode/settings.json
--rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:12:19.970260 py_static_dtm-1.0.0a1/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a1/README.md
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.954260 py_static_dtm-1.0.0a1/docs/
--rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/docs/Haifa Sea With Tests Points.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      942 2024-04-13 17:10:41.000000 py_static_dtm-1.0.0a1/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 17:12:19.970260 py_static_dtm-1.0.0a1/setup.cfg
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.946260 py_static_dtm-1.0.0a1/src/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.958260 py_static_dtm-1.0.0a1/src/py_static_dtm/
--rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/src/py_static_dtm/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/src/py_static_dtm/kml_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1161 2024-04-13 16:49:18.000000 py_static_dtm-1.0.0a1/src/py_static_dtm/polygon_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)        0 2024-04-13 16:47:50.000000 py_static_dtm-1.0.0a1/src/py_static_dtm/py.typed
--rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a1/src/py_static_dtm/static_dtm.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.966260 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:12:19.000000 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      693 2024-04-13 17:12:19.000000 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 17:12:19.000000 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 17:12:19.000000 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 17:12:19.000000 py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/top_level.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:12:19.966260 py_static_dtm-1.0.0a1/tests/
--rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/tests/HaifaSea.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a1/tests/conftest.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/tests/haifa_points.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      370 2024-04-13 16:50:43.000000 py_static_dtm-1.0.0a1/tests/test_example_simple_usage.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a1/tests/test_fastkml_poc.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a1/tests/test_stress_static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.943857 py_static_dtm-1.0.0a2/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.923856 py_static_dtm-1.0.0a2/.github/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.935857 py_static_dtm-1.0.0a2/.github/workflows/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/.github/workflows/lint.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/.github/workflows/test.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/.gitignore
+-rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a2/.pre-commit-config.yaml
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.935857 py_static_dtm-1.0.0a2/.vscode/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/.vscode/settings.json
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:39:29.939857 py_static_dtm-1.0.0a2/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a2/README.md
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.935857 py_static_dtm-1.0.0a2/docs/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/docs/Haifa Sea With Tests Points.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      993 2024-04-13 17:37:44.000000 py_static_dtm-1.0.0a2/pyproject.toml
+-rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 17:39:29.943857 py_static_dtm-1.0.0a2/setup.cfg
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.927856 py_static_dtm-1.0.0a2/src/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.939857 py_static_dtm-1.0.0a2/src/py_static_dtm/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/src/py_static_dtm/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/src/py_static_dtm/kml_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1161 2024-04-13 16:49:18.000000 py_static_dtm-1.0.0a2/src/py_static_dtm/polygon_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)        0 2024-04-13 16:47:50.000000 py_static_dtm-1.0.0a2/src/py_static_dtm/py.typed
+-rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a2/src/py_static_dtm/static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.939857 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:39:29.000000 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      693 2024-04-13 17:39:29.000000 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 17:39:29.000000 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 17:39:29.000000 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 17:39:29.000000 py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/top_level.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:39:29.939857 py_static_dtm-1.0.0a2/tests/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/tests/HaifaSea.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a2/tests/conftest.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/tests/haifa_points.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      370 2024-04-13 16:50:43.000000 py_static_dtm-1.0.0a2/tests/test_example_simple_usage.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a2/tests/test_fastkml_poc.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a2/tests/test_stress_static_dtm.py
```

### Comparing `py_static_dtm-1.0.0a1/.gitignore` & `py_static_dtm-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/.pre-commit-config.yaml` & `py_static_dtm-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/LICENSE` & `py_static_dtm-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/PKG-INFO` & `py_static_dtm-1.0.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a1/README.md` & `py_static_dtm-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/docs/Haifa Sea With Tests Points.kml` & `py_static_dtm-1.0.0a2/docs/Haifa Sea With Tests Points.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/pyproject.toml` & `py_static_dtm-1.0.0a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm>=8.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+"*" = ["py.typed"]
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "py-static-dtm"
 dynamic = ["version"]
 authors = [
```

### Comparing `py_static_dtm-1.0.0a1/src/py_static_dtm/kml_utils.py` & `py_static_dtm-1.0.0a2/src/py_static_dtm/kml_utils.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/src/py_static_dtm/polygon_utils.py` & `py_static_dtm-1.0.0a2/src/py_static_dtm/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/src/py_static_dtm/static_dtm.py` & `py_static_dtm-1.0.0a2/src/py_static_dtm/static_dtm.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/PKG-INFO` & `py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a1/src/py_static_dtm.egg-info/SOURCES.txt` & `py_static_dtm-1.0.0a2/src/py_static_dtm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/tests/HaifaSea.kml` & `py_static_dtm-1.0.0a2/tests/HaifaSea.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/tests/conftest.py` & `py_static_dtm-1.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/tests/haifa_points.py` & `py_static_dtm-1.0.0a2/tests/haifa_points.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/tests/test_fastkml_poc.py` & `py_static_dtm-1.0.0a2/tests/test_fastkml_poc.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a1/tests/test_stress_static_dtm.py` & `py_static_dtm-1.0.0a2/tests/test_stress_static_dtm.py`

 * *Files identical despite different names*

