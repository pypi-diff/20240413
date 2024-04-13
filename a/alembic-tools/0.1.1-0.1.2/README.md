# Comparing `tmp/alembic_tools-0.1.1.tar.gz` & `tmp/alembic_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_tools-0.1.1.tar", max compression
+gzip compressed data, was "alembic_tools-0.1.2.tar", max compression
```

## Comparing `alembic_tools-0.1.1.tar` & `alembic_tools-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 alembic_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0       15 2024-04-11 15:49:10.635624 alembic_tools-0.1.1/README.md
--rw-r--r--   0        0        0       70 2022-07-27 17:35:59.280000 alembic_tools-0.1.1/alembic_tools/__init__.py
--rw-r--r--   0        0        0    11733 2022-07-27 17:35:59.352000 alembic_tools-0.1.1/alembic_tools/commands.py
--rw-r--r--   0        0        0     2345 2022-07-27 17:35:59.310000 alembic_tools-0.1.1/alembic_tools/env.py
--rw-r--r--   0        0        0      494 2022-06-29 18:23:14.701000 alembic_tools-0.1.1/alembic_tools/script.py.mako
--rw-r--r--   0        0        0      512 2022-06-29 18:23:14.701000 alembic_tools-0.1.1/alembic_tools/utils.py
--rw-r--r--   0        0        0      409 2022-07-27 17:35:59.289000 alembic_tools-0.1.1/alembic_tools/version.py
--rw-r--r--   0        0        0      334 2024-04-13 13:12:08.360114 alembic_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 alembic_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 alembic_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0       15 2024-04-11 15:49:10.635624 alembic_tools-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2022-07-27 17:35:59.280000 alembic_tools-0.1.2/alembic_tools/__init__.py
+-rw-r--r--   0        0        0    11733 2022-07-27 17:35:59.352000 alembic_tools-0.1.2/alembic_tools/commands.py
+-rw-r--r--   0        0        0     2345 2022-07-27 17:35:59.310000 alembic_tools-0.1.2/alembic_tools/env.py
+-rw-r--r--   0        0        0      494 2022-06-29 18:23:14.701000 alembic_tools-0.1.2/alembic_tools/script.py.mako
+-rw-r--r--   0        0        0      512 2022-06-29 18:23:14.701000 alembic_tools-0.1.2/alembic_tools/utils.py
+-rw-r--r--   0        0        0      409 2022-07-27 17:35:59.289000 alembic_tools-0.1.2/alembic_tools/version.py
+-rw-r--r--   0        0        0      334 2024-04-13 13:13:25.126403 alembic_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 alembic_tools-0.1.2/PKG-INFO
```

### Comparing `alembic_tools-0.1.1/LICENSE` & `alembic_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_tools-0.1.1/alembic_tools/commands.py` & `alembic_tools-0.1.2/alembic_tools/commands.py`

 * *Files identical despite different names*

### Comparing `alembic_tools-0.1.1/alembic_tools/env.py` & `alembic_tools-0.1.2/alembic_tools/env.py`

 * *Files identical despite different names*

### Comparing `alembic_tools-0.1.1/alembic_tools/utils.py` & `alembic_tools-0.1.2/alembic_tools/utils.py`

 * *Files identical despite different names*

