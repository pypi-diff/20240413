# Comparing `tmp/ortfodb-0.3.1.tar.gz` & `tmp/ortfodb-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-0.3.1.tar", max compression
+gzip compressed data, was "ortfodb-0.3.2.tar", max compression
```

## Comparing `ortfodb-0.3.1.tar` & `ortfodb-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-0.3.1/README.md
--rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-0.3.1/ortfodb/__init__.py
--rw-r--r--   0        0        0     6923 2024-04-12 22:14:06.276685 ortfodb-0.3.1/ortfodb/configuration.py
--rw-r--r--   0        0        0     1666 2024-04-12 22:14:07.123383 ortfodb-0.3.1/ortfodb/database.py
--rw-r--r--   0        0        0     2791 2024-04-12 22:14:07.933413 ortfodb-0.3.1/ortfodb/tags.py
--rw-r--r--   0        0        0     2311 2024-04-12 22:14:08.740110 ortfodb-0.3.1/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-12 22:14:09.383468 ortfodb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-0.3.2/README.md
+-rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-0.3.2/ortfodb/__init__.py
+-rw-r--r--   0        0        0     6923 2024-04-12 22:45:43.206325 ortfodb-0.3.2/ortfodb/configuration.py
+-rw-r--r--   0        0        0    14616 2024-04-12 22:45:44.073024 ortfodb-0.3.2/ortfodb/database.py
+-rw-r--r--   0        0        0     2791 2024-04-12 22:45:44.903055 ortfodb-0.3.2/ortfodb/tags.py
+-rw-r--r--   0        0        0     2311 2024-04-12 22:45:45.693084 ortfodb-0.3.2/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-12 22:45:46.336441 ortfodb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-0.3.2/PKG-INFO
```

### Comparing `ortfodb-0.3.1/ortfodb/configuration.py` & `ortfodb-0.3.2/ortfodb/configuration.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.1/ortfodb/tags.py` & `ortfodb-0.3.2/ortfodb/tags.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.1/ortfodb/technologies.py` & `ortfodb-0.3.2/ortfodb/technologies.py`

 * *Files identical despite different names*

### Comparing `ortfodb-0.3.1/PKG-INFO` & `ortfodb-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 0.3.1
+Version: 0.3.2
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

