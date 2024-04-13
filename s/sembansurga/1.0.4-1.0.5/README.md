# Comparing `tmp/sembansurga-1.0.4.tar.gz` & `tmp/sembansurga-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.4.tar", last modified: Sun Feb 18 17:42:26 2024, max compression
+gzip compressed data, was "sembansurga-1.0.5.tar", last modified: Sat Apr 13 20:35:43 2024, max compression
```

## Comparing `sembansurga-1.0.4.tar` & `sembansurga-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      405 2024-02-18 17:42:26.174029 sembansurga-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-25 08:55:36.000000 sembansurga-1.0.4/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-01-25 08:55:16.000000 sembansurga-1.0.4/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 17:42:26.174029 sembansurga-1.0.4/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-02-18 17:42:26.000000 sembansurga-1.0.4/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 17:42:26.174029 sembansurga-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      730 2024-02-18 17:42:08.000000 sembansurga-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.544648 sembansurga-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-13 20:35:43.544648 sembansurga-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.534648 sembansurga-1.0.5/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-13 20:34:57.000000 sembansurga-1.0.5/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2024-04-13 20:34:38.000000 sembansurga-1.0.5/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.544648 sembansurga-1.0.5/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 20:35:43.544648 sembansurga-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-13 20:35:11.000000 sembansurga-1.0.5/setup.py
```

### Comparing `sembansurga-1.0.4/setup.py` & `sembansurga-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.4',
+    version='1.0.5',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

