# Comparing `tmp/rack-0.0.2.tar.gz` & `tmp/rack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rack-0.0.2.tar", last modified: Sat Apr 13 05:28:37 2024, max compression
+gzip compressed data, was "rack-0.0.3.tar", last modified: Sat Apr 13 05:36:24 2024, max compression
```

## Comparing `rack-0.0.2.tar` & `rack-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:28:37.778361 rack-0.0.2/
--rw-rw-r--   0 cJ        (1000) cJ        (1000)        0 2024-04-13 01:18:37.000000 rack-0.0.2/LICENSE
--rw-r--r--   0 cJ        (1000) cJ        (1000)      696 2024-04-13 05:28:37.778361 rack-0.0.2/PKG-INFO
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      202 2024-04-13 05:28:30.000000 rack-0.0.2/README.rst
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      108 2024-04-13 00:59:20.000000 rack-0.0.2/__init__.py
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      584 2024-04-13 05:27:02.000000 rack-0.0.2/pyproject.toml
-drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:28:37.778361 rack-0.0.2/rack.egg-info/
--rw-r--r--   0 cJ        (1000) cJ        (1000)      696 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/PKG-INFO
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      168 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/SOURCES.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)        1 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/dependency_links.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)        5 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/top_level.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)       38 2024-04-13 05:28:37.778361 rack-0.0.2/setup.cfg
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      425 2024-04-13 05:25:37.000000 rack-0.0.2/setup.py
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.637436 rack-0.0.3/
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.636436 rack-0.0.3/LICENSES/
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)     1078 2024-04-13 05:32:55.000000 rack-0.0.3/LICENSES/MIT.txt
+-rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 05:36:24.637436 rack-0.0.3/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      260 2024-04-13 05:29:52.000000 rack-0.0.3/README.rst
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      227 2024-04-13 05:35:08.000000 rack-0.0.3/__init__.py
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      593 2024-04-13 05:33:17.000000 rack-0.0.3/pyproject.toml
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.637436 rack-0.0.3/rack.egg-info/
+-rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      177 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        1 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        5 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/top_level.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)       38 2024-04-13 05:36:24.637436 rack-0.0.3/setup.cfg
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      425 2024-04-13 05:25:37.000000 rack-0.0.3/setup.py
```

### Comparing `rack-0.0.2/pyproject.toml` & `rack-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 readme = {file = "README.rst", content-type = "text/x-rst"}
 
 authors = [
     { name = "Jérôme Carretero" },
 ]
 
-license = { file = "LICENSE" }
+license = { file = "LICENSES/MIT.txt" }
 
 keywords = ["persistent"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
```

