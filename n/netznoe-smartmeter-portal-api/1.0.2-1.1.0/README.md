# Comparing `tmp/netznoe-smartmeter-portal-api-1.0.2.tar.gz` & `tmp/netznoe_smartmeter_portal_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netznoe-smartmeter-portal-api-1.0.2.tar", last modified: Tue May 23 07:35:11 2023, max compression
+gzip compressed data, was "netznoe_smartmeter_portal_api-1.1.0.tar", last modified: Sat Apr 13 13:58:15 2024, max compression
```

## Comparing `netznoe-smartmeter-portal-api-1.0.2.tar` & `netznoe_smartmeter_portal_api-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.359799 netznoe-smartmeter-portal-api-1.0.2/
--rw-r--r--   0 schue     (1000) schue     (1000)     1073 2023-04-16 11:53:11.000000 netznoe-smartmeter-portal-api-1.0.2/LICENSE
--rw-r--r--   0 schue     (1000) schue     (1000)     4732 2023-05-23 07:35:11.360799 netznoe-smartmeter-portal-api-1.0.2/PKG-INFO
--rw-r--r--   0 schue     (1000) schue     (1000)     3843 2023-04-16 20:40:16.000000 netznoe-smartmeter-portal-api-1.0.2/README.md
--rw-r--r--   0 schue     (1000) schue     (1000)       98 2023-04-16 15:15:10.000000 netznoe-smartmeter-portal-api-1.0.2/pyproject.toml
--rw-r--r--   0 schue     (1000) schue     (1000)     1148 2023-05-23 07:35:11.360799 netznoe-smartmeter-portal-api-1.0.2/setup.cfg
--rw-r--r--   0 schue     (1000) schue     (1000)       37 2023-04-16 15:09:50.000000 netznoe-smartmeter-portal-api-1.0.2/setup.py
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.356799 netznoe-smartmeter-portal-api-1.0.2/src/
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.358799 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/
--rw-r--r--   0 schue     (1000) schue     (1000)      193 2023-04-16 10:39:28.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/__init__.py
--rw-r--r--   0 schue     (1000) schue     (1000)     6395 2023-04-25 19:25:10.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/api.py
--rw-r--r--   0 schue     (1000) schue     (1000)     1033 2023-04-16 20:45:06.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api/models.py
-drwxr-xr-x   0 schue     (1000) schue     (1000)        0 2023-05-23 07:35:11.359799 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/
--rw-r--r--   0 schue     (1000) schue     (1000)     4732 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
--rw-r--r--   0 schue     (1000) schue     (1000)      466 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
--rw-r--r--   0 schue     (1000) schue     (1000)        1 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
--rw-r--r--   0 schue     (1000) schue     (1000)       33 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
--rw-r--r--   0 schue     (1000) schue     (1000)       30 2023-05-23 07:35:11.000000 netznoe-smartmeter-portal-api-1.0.2/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
```

### Comparing `netznoe-smartmeter-portal-api-1.0.2/LICENSE` & `netznoe_smartmeter_portal_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netznoe-smartmeter-portal-api-1.0.2/setup.cfg` & `netznoe_smartmeter_portal_api-1.1.0/setup.cfg`

 * *Files identical despite different names*

