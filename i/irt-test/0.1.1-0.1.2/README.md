# Comparing `tmp/irt_test-0.1.1.tar.gz` & `tmp/irt_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irt_test-0.1.1.tar", max compression
+gzip compressed data, was "irt_test-0.1.2.tar", max compression
```

## Comparing `irt_test-0.1.1.tar` & `irt_test-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-04-12 16:35:12.647211 irt_test-0.1.1/LICENSE
--rw-r--r--   0        0        0     2942 2024-04-13 03:42:24.153078 irt_test-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-13 03:42:24.153078 irt_test-0.1.1/irt_test/__init__.py
--rw-r--r--   0        0        0    10028 2024-04-13 03:42:24.153078 irt_test-0.1.1/irt_test/irt.py
--rw-r--r--   0        0        0      399 2024-04-13 03:43:20.703175 irt_test-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 irt_test-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 16:35:12.647211 irt_test-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2123 2024-04-13 15:11:42.709453 irt_test-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 03:42:24.153078 irt_test-0.1.2/irt_test/__init__.py
+-rw-r--r--   0        0        0    10028 2024-04-13 03:42:24.153078 irt_test-0.1.2/irt_test/irt.py
+-rw-r--r--   0        0        0      399 2024-04-13 15:12:00.580461 irt_test-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 irt_test-0.1.2/PKG-INFO
```

### Comparing `irt_test-0.1.1/LICENSE` & `irt_test-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irt_test-0.1.1/irt_test/irt.py` & `irt_test-0.1.2/irt_test/irt.py`

 * *Files identical despite different names*

