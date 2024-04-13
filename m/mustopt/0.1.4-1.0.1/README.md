# Comparing `tmp/mustopt-0.1.4.tar.gz` & `tmp/mustopt-1.0.1.tar.gz`

## Comparing `mustopt-0.1.4.tar` & `mustopt-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 mustopt-0.1.4/coverage.toml
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 mustopt-0.1.4/ruff.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/__about__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/__init__.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/model.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mustopt-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mustopt-0.1.4/tests/test_model.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 mustopt-0.1.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mustopt-0.1.4/LICENSE
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mustopt-0.1.4/README.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 mustopt-0.1.4/hatch.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 mustopt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 mustopt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 mustopt-1.0.1/coverage.toml
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 mustopt-1.0.1/ruff.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/__about__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/__init__.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/_container.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/_errors.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/_meta.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mustopt-1.0.1/src/mustopt/py.typed
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mustopt-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 mustopt-1.0.1/tests/test_logic.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 mustopt-1.0.1/tests/test_types.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 mustopt-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mustopt-1.0.1/LICENSE
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mustopt-1.0.1/README.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 mustopt-1.0.1/hatch.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 mustopt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 mustopt-1.0.1/PKG-INFO
```

### Comparing `mustopt-0.1.4/ruff.toml` & `mustopt-1.0.1/ruff.toml`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.4/.gitignore` & `mustopt-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.4/LICENSE` & `mustopt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.4/hatch.toml` & `mustopt-1.0.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.4/pyproject.toml` & `mustopt-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.4/PKG-INFO` & `mustopt-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mustopt
-Version: 0.1.4
+Version: 1.0.1
 Dynamic: Summary
 Project-URL: Home, https://github.com/MemberWave/MustOpt
 Project-URL: Issues, https://github.com/MemberWave/MustOpt/issues
 Project-URL: Source, https://github.com/MemberWave/MustOpt
 Author-email: Dmitry Starov <dmitry.staroff@gmail.com>
 License: MIT License
```

