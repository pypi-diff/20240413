# Comparing `tmp/rollplayerlib-0.2.0.tar.gz` & `tmp/rollplayerlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rollplayerlib-0.2.0.tar", last modified: Sat Apr 13 18:26:49 2024, max compression
+gzip compressed data, was "rollplayerlib-0.3.0.tar", last modified: Sat Apr 13 18:39:21 2024, max compression
```

## Comparing `rollplayerlib-0.2.0.tar` & `rollplayerlib-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:26:49.761603 rollplayerlib-0.2.0/
--rw-r--r--   0 infernity  (1000) infernity  (1000)     1068 2024-04-13 17:49:32.000000 rollplayerlib-0.2.0/LICENSE
--rw-r--r--   0 infernity  (1000) infernity  (1000)     3853 2024-04-13 18:26:49.761603 rollplayerlib-0.2.0/PKG-INFO
--rw-r--r--   0 infernity  (1000) infernity  (1000)     3218 2024-04-13 18:25:40.000000 rollplayerlib-0.2.0/README.md
--rw-r--r--   0 infernity  (1000) infernity  (1000)      669 2024-04-13 18:18:11.000000 rollplayerlib-0.2.0/pyproject.toml
--rw-r--r--   0 infernity  (1000) infernity  (1000)       38 2024-04-13 18:26:49.761603 rollplayerlib-0.2.0/setup.cfg
-drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:26:49.758270 rollplayerlib-0.2.0/src/
-drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:26:49.758270 rollplayerlib-0.2.0/src/rollplayerlib/
--rw-r--r--   0 infernity  (1000) infernity  (1000)      262 2024-04-13 18:25:55.000000 rollplayerlib-0.2.0/src/rollplayerlib/__init__.py
--rw-r--r--   0 infernity  (1000) infernity  (1000)     6073 2024-04-13 18:05:36.000000 rollplayerlib-0.2.0/src/rollplayerlib/bonuses.py
--rw-r--r--   0 infernity  (1000) infernity  (1000)     9563 2024-04-13 18:17:51.000000 rollplayerlib-0.2.0/src/rollplayerlib/dice.py
--rw-r--r--   0 infernity  (1000) infernity  (1000)      543 2024-04-13 18:15:45.000000 rollplayerlib-0.2.0/src/rollplayerlib/enums.py
--rw-r--r--   0 infernity  (1000) infernity  (1000)      139 2024-04-13 18:00:19.000000 rollplayerlib-0.2.0/src/rollplayerlib/exceptions.py
--rw-r--r--   0 infernity  (1000) infernity  (1000)     3330 2024-04-13 18:09:08.000000 rollplayerlib-0.2.0/src/rollplayerlib/formatting.py
-drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:26:49.761603 rollplayerlib-0.2.0/src/rollplayerlib.egg-info/
--rw-r--r--   0 infernity  (1000) infernity  (1000)     3853 2024-04-13 18:26:49.000000 rollplayerlib-0.2.0/src/rollplayerlib.egg-info/PKG-INFO
--rw-r--r--   0 infernity  (1000) infernity  (1000)      372 2024-04-13 18:26:49.000000 rollplayerlib-0.2.0/src/rollplayerlib.egg-info/SOURCES.txt
--rw-r--r--   0 infernity  (1000) infernity  (1000)        1 2024-04-13 18:26:49.000000 rollplayerlib-0.2.0/src/rollplayerlib.egg-info/dependency_links.txt
--rw-r--r--   0 infernity  (1000) infernity  (1000)       14 2024-04-13 18:26:49.000000 rollplayerlib-0.2.0/src/rollplayerlib.egg-info/top_level.txt
+drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     1068 2024-04-13 17:49:32.000000 rollplayerlib-0.3.0/LICENSE
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     3853 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/PKG-INFO
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     3218 2024-04-13 18:25:40.000000 rollplayerlib-0.3.0/README.md
+-rw-r--r--   0 infernity  (1000) infernity  (1000)      669 2024-04-13 18:39:18.000000 rollplayerlib-0.3.0/pyproject.toml
+-rw-r--r--   0 infernity  (1000) infernity  (1000)       38 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/setup.cfg
+drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/src/
+drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/src/rollplayerlib/
+-rw-r--r--   0 infernity  (1000) infernity  (1000)      268 2024-04-13 18:36:17.000000 rollplayerlib-0.3.0/src/rollplayerlib/__init__.py
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     6073 2024-04-13 18:05:36.000000 rollplayerlib-0.3.0/src/rollplayerlib/bonuses.py
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     9563 2024-04-13 18:17:51.000000 rollplayerlib-0.3.0/src/rollplayerlib/dice.py
+-rw-r--r--   0 infernity  (1000) infernity  (1000)      543 2024-04-13 18:15:45.000000 rollplayerlib-0.3.0/src/rollplayerlib/enums.py
+-rw-r--r--   0 infernity  (1000) infernity  (1000)      139 2024-04-13 18:00:19.000000 rollplayerlib-0.3.0/src/rollplayerlib/exceptions.py
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     3330 2024-04-13 18:09:08.000000 rollplayerlib-0.3.0/src/rollplayerlib/formatting.py
+drwxr-xr-x   0 infernity  (1000) infernity  (1000)        0 2024-04-13 18:39:21.660485 rollplayerlib-0.3.0/src/rollplayerlib.egg-info/
+-rw-r--r--   0 infernity  (1000) infernity  (1000)     3853 2024-04-13 18:39:21.000000 rollplayerlib-0.3.0/src/rollplayerlib.egg-info/PKG-INFO
+-rw-r--r--   0 infernity  (1000) infernity  (1000)      372 2024-04-13 18:39:21.000000 rollplayerlib-0.3.0/src/rollplayerlib.egg-info/SOURCES.txt
+-rw-r--r--   0 infernity  (1000) infernity  (1000)        1 2024-04-13 18:39:21.000000 rollplayerlib-0.3.0/src/rollplayerlib.egg-info/dependency_links.txt
+-rw-r--r--   0 infernity  (1000) infernity  (1000)       14 2024-04-13 18:39:21.000000 rollplayerlib-0.3.0/src/rollplayerlib.egg-info/top_level.txt
```

### Comparing `rollplayerlib-0.2.0/LICENSE` & `rollplayerlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/PKG-INFO` & `rollplayerlib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rollplayerlib
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to roll dice in a simple way, but with advanced functionality.
 Author-email: whirlingstars <infernity@infernity.dev>
 License: MIT
 Keywords: DICE,ROLL,RANDOM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rollplayerlib-0.2.0/README.md` & `rollplayerlib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/pyproject.toml` & `rollplayerlib-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rollplayerlib"
-version = "0.2.0"
+version = "0.3.0"
 license = {text = "MIT"}
 authors = [{name = "whirlingstars", email = "infernity@infernity.dev"}]
 keywords = ["DICE", "ROLL", "RANDOM"]
 classifiers = ["Development Status :: 4 - Beta", "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Programming Language :: Python :: 3.12"]
 description = "A library to roll dice in a simple way, but with advanced functionality."
 readme = "README.md"
```

### Comparing `rollplayerlib-0.2.0/src/rollplayerlib/bonuses.py` & `rollplayerlib-0.3.0/src/rollplayerlib/bonuses.py`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/src/rollplayerlib/dice.py` & `rollplayerlib-0.3.0/src/rollplayerlib/dice.py`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/src/rollplayerlib/enums.py` & `rollplayerlib-0.3.0/src/rollplayerlib/enums.py`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/src/rollplayerlib/formatting.py` & `rollplayerlib-0.3.0/src/rollplayerlib/formatting.py`

 * *Files identical despite different names*

### Comparing `rollplayerlib-0.2.0/src/rollplayerlib.egg-info/PKG-INFO` & `rollplayerlib-0.3.0/src/rollplayerlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rollplayerlib
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to roll dice in a simple way, but with advanced functionality.
 Author-email: whirlingstars <infernity@infernity.dev>
 License: MIT
 Keywords: DICE,ROLL,RANDOM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

