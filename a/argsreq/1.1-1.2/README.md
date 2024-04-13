# Comparing `tmp/argsreq-1.1.tar.gz` & `tmp/argsreq-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsreq-1.1.tar", last modified: Sat Apr 13 08:33:21 2024, max compression
+gzip compressed data, was "argsreq-1.2.tar", last modified: Sat Apr 13 08:45:31 2024, max compression
```

## Comparing `argsreq-1.1.tar` & `argsreq-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 08:33:21.075887 argsreq-1.1/
--rw-rw-rw-   0        0        0      311 2024-04-13 08:33:21.074818 argsreq-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 08:33:21.070911 argsreq-1.1/argsreq.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-13 08:33:20.000000 argsreq-1.1/argsreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-13 08:33:21.000000 argsreq-1.1/argsreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 08:33:20.000000 argsreq-1.1/argsreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 08:33:20.000000 argsreq-1.1/argsreq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 08:33:21.073807 argsreq-1.1/reqargs/
--rw-rw-rw-   0        0        0    15826 2024-04-13 08:28:17.000000 argsreq-1.1/reqargs/__init__.py
--rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.1/reqargs/__main__.py
--rw-rw-rw-   0        0        0    15412 2024-04-13 08:28:50.000000 argsreq-1.1/reqargs/colorls.py
--rw-rw-rw-   0        0        0    15826 2024-04-13 08:28:29.000000 argsreq-1.1/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-13 08:33:21.075887 argsreq-1.1/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-04-13 08:33:17.000000 argsreq-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:45:31.797775 argsreq-1.2/
+-rw-rw-rw-   0        0        0      311 2024-04-13 08:45:31.796768 argsreq-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 08:45:31.793889 argsreq-1.2/argsreq.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-13 08:45:31.000000 argsreq-1.2/argsreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-13 08:45:31.000000 argsreq-1.2/argsreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 08:45:31.000000 argsreq-1.2/argsreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 08:45:31.000000 argsreq-1.2/argsreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 08:45:31.796768 argsreq-1.2/reqargs/
+-rw-rw-rw-   0        0        0    15826 2024-04-13 08:28:17.000000 argsreq-1.2/reqargs/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.2/reqargs/__main__.py
+-rw-rw-rw-   0        0        0    15412 2024-04-13 08:28:50.000000 argsreq-1.2/reqargs/colorls.py
+-rw-rw-rw-   0        0        0    15826 2024-04-13 08:28:29.000000 argsreq-1.2/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 08:45:31.797775 argsreq-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      585 2024-04-13 08:45:27.000000 argsreq-1.2/setup.py
```

### Comparing `argsreq-1.1/reqargs/__init__.py` & `argsreq-1.2/reqargs/__init__.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.1/reqargs/colorls.py` & `argsreq-1.2/reqargs/colorls.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.1/reqargs/reqargs.py` & `argsreq-1.2/reqargs/reqargs.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.1/setup.py` & `argsreq-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="argsreq",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
```

