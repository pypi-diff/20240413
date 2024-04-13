# Comparing `tmp/restx-0.1.1.tar.gz` & `tmp/restx-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restx-0.1.1.tar", max compression
+gzip compressed data, was "restx-0.1.4.tar", max compression
```

## Comparing `restx-0.1.1.tar` & `restx-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-04-13 08:36:11.424182 restx-0.1.1/LICENSE
--rw-r--r--   0        0        0       83 2024-04-13 10:09:24.428188 restx-0.1.1/README.md
--rw-r--r--   0        0        0      592 2024-04-13 10:20:06.376250 restx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 08:02:36.161963 restx-0.1.1/restx/__init__.py
--rw-r--r--   0        0        0      364 2024-04-13 08:40:43.514130 restx-0.1.1/restx/cli.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 restx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-13 08:36:11.424182 restx-0.1.4/LICENSE
+-rw-r--r--   0        0        0       83 2024-04-13 10:09:24.428188 restx-0.1.4/README.md
+-rw-r--r--   0        0        0     1160 2024-04-13 17:15:01.061193 restx-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 08:02:36.161963 restx-0.1.4/restx/__init__.py
+-rwxr-xr-x   0        0        0     1834 2024-04-13 16:41:40.187903 restx-0.1.4/restx/cli.py
+-rw-r--r--   0        0        0      140 2024-04-13 16:17:32.113654 restx-0.1.4/restx/enums.py
+-rw-r--r--   0        0        0     2780 2024-04-13 16:51:00.611191 restx-0.1.4/restx/utils.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 restx-0.1.4/PKG-INFO
```

### Comparing `restx-0.1.1/LICENSE` & `restx-0.1.4/LICENSE`

 * *Files identical despite different names*

