# Comparing `tmp/my_playground-0.1.0.tar.gz` & `tmp/my_playground-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_playground-0.1.0.tar", last modified: Sat Apr 13 14:59:19 2024, max compression
+gzip compressed data, was "my_playground-0.1.1.tar", last modified: Sat Apr 13 15:09:50 2024, max compression
```

## Comparing `my_playground-0.1.0.tar` & `my_playground-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       13 2024-04-13 14:59:06.115665 my_playground-0.1.0/README.md
--rw-r--r--   0        0        0      413 2024-04-13 14:59:19.119698 my_playground-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 14:59:06.115665 my_playground-0.1.0/src/playground/__init__.py
--rw-r--r--   0        0        0       22 2024-04-13 14:59:06.115665 my_playground-0.1.0/src/playground/hello.py
--rw-r--r--   0        0        0        0 2024-04-13 14:59:06.115665 my_playground-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-13 15:09:38.741021 my_playground-0.1.1/README.md
+-rw-r--r--   0        0        0      413 2024-04-13 15:09:50.133053 my_playground-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 15:09:38.745020 my_playground-0.1.1/src/playground/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-13 15:09:38.745020 my_playground-0.1.1/src/playground/hello.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:09:38.745020 my_playground-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.1/PKG-INFO
```

