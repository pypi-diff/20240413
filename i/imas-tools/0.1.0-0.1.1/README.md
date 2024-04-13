# Comparing `tmp/imas_tools-0.1.0.tar.gz` & `tmp/imas_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.1.0.tar", max compression
+gzip compressed data, was "imas_tools-0.1.1.tar", max compression
```

## Comparing `imas_tools-0.1.0.tar` & `imas_tools-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.1.0/imas_tools/__init__.py
--rw-r--r--   0        0        0     4124 2024-04-13 08:31:37.334472 imas_tools-0.1.0/imas_tools/recochoku.py
--rw-r--r--   0        0        0      416 2024-04-13 09:29:40.840900 imas_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.1.0/README.md
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 imas_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.1.1/imas_tools/__init__.py
+-rw-r--r--   0        0        0     4124 2024-04-13 08:31:37.334472 imas_tools-0.1.1/imas_tools/recochoku.py
+-rw-r--r--   0        0        0      416 2024-04-13 11:39:07.485442 imas_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 imas_tools-0.1.1/PKG-INFO
```

### Comparing `imas_tools-0.1.0/imas_tools/recochoku.py` & `imas_tools-0.1.1/imas_tools/recochoku.py`

 * *Files identical despite different names*

