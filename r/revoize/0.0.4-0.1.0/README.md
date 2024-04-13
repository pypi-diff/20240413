# Comparing `tmp/revoize-0.0.4.tar.gz` & `tmp/revoize-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revoize-0.0.4.tar", max compression
+gzip compressed data, was "revoize-0.1.0.tar", max compression
```

## Comparing `revoize-0.0.4.tar` & `revoize-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0     1068 2024-03-29 12:09:31.970271 revoize-0.0.4/LICENSE
--rw-r--r--   0        0        0      580 2024-03-29 12:46:58.826784 revoize-0.0.4/README.md
--rw-r--r--   0        0        0     2923 2024-03-29 12:47:33.388375 revoize-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       53 2024-03-29 11:54:54.106847 revoize-0.0.4/revoize/main.py
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 revoize-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 09:42:11.101682 revoize-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3243 2024-04-13 18:06:07.965047 revoize-0.1.0/README.md
+-rw-r--r--   0        0        0     3431 2024-04-13 18:06:59.142753 revoize-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-04-11 09:42:11.103545 revoize-0.1.0/revoize/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:42:11.103593 revoize-0.1.0/revoize/api/__init__.py
+-rw-r--r--   0        0        0    10299 2024-04-11 09:42:11.104027 revoize-0.1.0/revoize/api/client.py
+-rw-r--r--   0        0        0      209 2024-04-11 09:42:11.104307 revoize-0.1.0/revoize/api/exceptions.py
+-rw-r--r--   0        0        0     1186 2024-04-11 09:42:11.104589 revoize-0.1.0/revoize/api/utils.py
+-rw-r--r--   0        0        0       45 2024-04-11 09:42:11.104871 revoize-0.1.0/revoize/auth/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-11 09:42:11.105060 revoize-0.1.0/revoize/auth/auth.py
+-rw-r--r--   0        0        0      103 2024-04-11 09:42:11.105306 revoize-0.1.0/revoize/auth/exceptions.py
+-rw-r--r--   0        0        0      143 2024-04-11 09:42:11.105495 revoize-0.1.0/revoize/defaults.py
+-rw-r--r--   0        0        0      555 2024-04-11 09:42:11.105770 revoize-0.1.0/revoize/schema/__init__.py
+-rw-r--r--   0        0        0     2996 2024-04-11 09:42:11.106046 revoize-0.1.0/revoize/schema/schema.py
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 revoize-0.1.0/PKG-INFO
```

### Comparing `revoize-0.0.4/LICENSE` & `revoize-0.1.0/LICENSE`

 * *Files identical despite different names*

