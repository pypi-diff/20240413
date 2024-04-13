# Comparing `tmp/HapooDB-0.0.1.tar.gz` & `tmp/HapooDB-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HapooDB-0.0.1.tar", last modified: Sat Apr 13 17:13:30 2024, max compression
+gzip compressed data, was "HapooDB-0.0.2.tar", last modified: Sat Apr 13 18:09:32 2024, max compression
```

## Comparing `HapooDB-0.0.1.tar` & `HapooDB-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 17:13:30.702859 HapooDB-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-13 17:13:30.679908 HapooDB-0.0.1/HapooDB/
--rw-rw-rw-   0        0        0     3778 2024-04-13 17:02:36.000000 HapooDB-0.0.1/HapooDB/HapooDB.py
--rw-rw-rw-   0        0        0       27 2024-04-13 17:02:14.000000 HapooDB-0.0.1/HapooDB/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 17:13:30.699855 HapooDB-0.0.1/HapooDB.egg-info/
--rw-rw-rw-   0        0        0      451 2024-04-13 17:13:30.000000 HapooDB-0.0.1/HapooDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-04-13 17:13:30.000000 HapooDB-0.0.1/HapooDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 17:13:30.000000 HapooDB-0.0.1/HapooDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 17:13:30.000000 HapooDB-0.0.1/HapooDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2024-04-13 17:13:30.700852 HapooDB-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 17:13:30.702859 HapooDB-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-04-13 17:12:04.000000 HapooDB-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.482910 HapooDB-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.463960 HapooDB-0.0.2/HapooDB/
+-rw-rw-rw-   0        0        0     3778 2024-04-13 17:02:36.000000 HapooDB-0.0.2/HapooDB/HapooDB.py
+-rw-rw-rw-   0        0        0       28 2024-04-13 18:08:23.000000 HapooDB-0.0.2/HapooDB/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:09:32.478919 HapooDB-0.0.2/HapooDB.egg-info/
+-rw-rw-rw-   0        0        0      451 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 18:09:32.000000 HapooDB-0.0.2/HapooDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2024-04-13 18:09:32.480914 HapooDB-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 18:09:32.482910 HapooDB-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-04-13 18:06:25.000000 HapooDB-0.0.2/setup.py
```

### Comparing `HapooDB-0.0.1/HapooDB/HapooDB.py` & `HapooDB-0.0.2/HapooDB/HapooDB.py`

 * *Files identical despite different names*

### Comparing `HapooDB-0.0.1/setup.py` & `HapooDB-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Hapoo DB'
 
 
 # Setting up
 setup(
     name="HapooDB",
     version=VERSION,
```

