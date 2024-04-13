# Comparing `tmp/py_static_dtm-1.0.0a3.tar.gz` & `tmp/py_static_dtm-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_static_dtm-1.0.0a3.tar", last modified: Sat Apr 13 17:47:50 2024, max compression
+gzip compressed data, was "py_static_dtm-1.0.0a4.tar", last modified: Sat Apr 13 18:38:02 2024, max compression
```

## Comparing `py_static_dtm-1.0.0a3.tar` & `py_static_dtm-1.0.0a4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.019037 py_static_dtm-1.0.0a3/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.011037 py_static_dtm-1.0.0a3/.github/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.011037 py_static_dtm-1.0.0a3/.github/workflows/
--rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/.github/workflows/lint.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/.github/workflows/test.yaml
--rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/.gitignore
--rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a3/.pre-commit-config.yaml
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.011037 py_static_dtm-1.0.0a3/.vscode/
--rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/.vscode/settings.json
--rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:47:50.015037 py_static_dtm-1.0.0a3/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a3/README.md
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.015037 py_static_dtm-1.0.0a3/docs/
--rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/docs/Haifa Sea With Tests Points.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      986 2024-04-13 17:46:30.000000 py_static_dtm-1.0.0a3/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 17:47:50.019037 py_static_dtm-1.0.0a3/setup.cfg
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.011037 py_static_dtm-1.0.0a3/src/
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.015037 py_static_dtm-1.0.0a3/src/py_static_dtm/
--rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/src/py_static_dtm/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/src/py_static_dtm/kml_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1161 2024-04-13 16:49:18.000000 py_static_dtm-1.0.0a3/src/py_static_dtm/polygon_utils.py
--rw-rw-r--   0 ben       (1000) ben       (1000)        6 2024-04-13 17:46:11.000000 py_static_dtm-1.0.0a3/src/py_static_dtm/py.typed
--rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a3/src/py_static_dtm/static_dtm.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.015037 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 17:47:49.000000 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      693 2024-04-13 17:47:50.000000 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 17:47:49.000000 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 17:47:49.000000 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 17:47:49.000000 py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/top_level.txt
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 17:47:50.015037 py_static_dtm-1.0.0a3/tests/
--rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/tests/HaifaSea.kml
--rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a3/tests/conftest.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/tests/haifa_points.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      370 2024-04-13 16:50:43.000000 py_static_dtm-1.0.0a3/tests/test_example_simple_usage.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a3/tests/test_fastkml_poc.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a3/tests/test_stress_static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.842959 py_static_dtm-1.0.0a4/.github/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/.github/workflows/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      264 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.github/workflows/lint.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      282 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.github/workflows/test.yaml
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3078 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.gitignore
+-rw-rw-r--   0 ben       (1000) ben       (1000)      945 2024-04-13 16:33:21.000000 py_static_dtm-1.0.0a4/.pre-commit-config.yaml
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/.vscode/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      124 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/.vscode/settings.json
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      849 2024-04-13 16:18:18.000000 py_static_dtm-1.0.0a4/README.md
+-rwxrwxr-x   0 ben       (1000) ben       (1000)      374 2024-04-13 18:37:19.000000 py_static_dtm-1.0.0a4/build_and_publish.sh
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/docs/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     8620 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/docs/Haifa Sea With Tests Points.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      986 2024-04-13 17:46:30.000000 py_static_dtm-1.0.0a4/pyproject.toml
+-rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/setup.cfg
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/src/
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.846959 py_static_dtm-1.0.0a4/src/py_static_dtm/
+-rw-rw-r--   0 ben       (1000) ben       (1000)      123 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/__init__.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1318 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/kml_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1161 2024-04-13 16:49:18.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/polygon_utils.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)        6 2024-04-13 17:46:11.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/py.typed
+-rw-rw-r--   0 ben       (1000) ben       (1000)      989 2024-04-13 16:34:22.000000 py_static_dtm-1.0.0a4/src/py_static_dtm/static_dtm.py
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)     1557 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1000) ben       (1000)      714 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       41 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1000) ben       (1000)       14 2024-04-13 18:38:02.000000 py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/top_level.txt
+drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-04-13 18:38:02.850959 py_static_dtm-1.0.0a4/tests/
+-rw-rw-r--   0 ben       (1000) ben       (1000)     3804 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/HaifaSea.kml
+-rw-rw-r--   0 ben       (1000) ben       (1000)      785 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a4/tests/conftest.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1084 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/haifa_points.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)      370 2024-04-13 16:50:43.000000 py_static_dtm-1.0.0a4/tests/test_example_simple_usage.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1548 2024-04-13 16:08:57.000000 py_static_dtm-1.0.0a4/tests/test_fastkml_poc.py
+-rw-rw-r--   0 ben       (1000) ben       (1000)     1956 2024-04-13 16:21:21.000000 py_static_dtm-1.0.0a4/tests/test_stress_static_dtm.py
```

### Comparing `py_static_dtm-1.0.0a3/.gitignore` & `py_static_dtm-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/.pre-commit-config.yaml` & `py_static_dtm-1.0.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/LICENSE` & `py_static_dtm-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/PKG-INFO` & `py_static_dtm-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a3/README.md` & `py_static_dtm-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/docs/Haifa Sea With Tests Points.kml` & `py_static_dtm-1.0.0a4/docs/Haifa Sea With Tests Points.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/pyproject.toml` & `py_static_dtm-1.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/src/py_static_dtm/kml_utils.py` & `py_static_dtm-1.0.0a4/src/py_static_dtm/kml_utils.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/src/py_static_dtm/polygon_utils.py` & `py_static_dtm-1.0.0a4/src/py_static_dtm/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/src/py_static_dtm/static_dtm.py` & `py_static_dtm-1.0.0a4/src/py_static_dtm/static_dtm.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/PKG-INFO` & `py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-static-dtm
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: A custom DTM object that returns a constant value in a certain polygon
 Author-email: Ben Sembira <classified@classified.classified>
 Project-URL: Homepage, https://github.com/ben-sembira-1/py-static-dtm
 Project-URL: Issues, https://github.com/ben-sembira-1/py-static-dtm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py_static_dtm-1.0.0a3/src/py_static_dtm.egg-info/SOURCES.txt` & `py_static_dtm-1.0.0a4/src/py_static_dtm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+build_and_publish.sh
 pyproject.toml
 .github/workflows/lint.yaml
 .github/workflows/test.yaml
 .vscode/settings.json
 docs/Haifa Sea With Tests Points.kml
 src/py_static_dtm/__init__.py
 src/py_static_dtm/kml_utils.py
```

### Comparing `py_static_dtm-1.0.0a3/tests/HaifaSea.kml` & `py_static_dtm-1.0.0a4/tests/HaifaSea.kml`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/tests/conftest.py` & `py_static_dtm-1.0.0a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/tests/haifa_points.py` & `py_static_dtm-1.0.0a4/tests/haifa_points.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/tests/test_fastkml_poc.py` & `py_static_dtm-1.0.0a4/tests/test_fastkml_poc.py`

 * *Files identical despite different names*

### Comparing `py_static_dtm-1.0.0a3/tests/test_stress_static_dtm.py` & `py_static_dtm-1.0.0a4/tests/test_stress_static_dtm.py`

 * *Files identical despite different names*

