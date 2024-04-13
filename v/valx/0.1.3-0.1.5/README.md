# Comparing `tmp/valx-0.1.3.tar.gz` & `tmp/valx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valx-0.1.3.tar", last modified: Thu Apr 11 12:42:53 2024, max compression
+gzip compressed data, was "valx-0.1.5.tar", last modified: Sat Apr 13 07:20:12 2024, max compression
```

## Comparing `valx-0.1.3.tar` & `valx-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:53.973686 valx-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 12:42:49.000000 valx-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 12:42:53.973686 valx-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-11 12:42:49.000000 valx-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:42:53.973686 valx-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 12:42:53.000000 valx-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:53.973686 valx-0.1.3/valx/
--rw-r--r--   0 runner    (1001) docker     (127)    42515 2024-04-11 12:42:49.000000 valx-0.1.3/valx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:42:53.973686 valx-0.1.3/valx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 12:42:53.000000 valx-0.1.3/valx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 12:42:53.000000 valx-0.1.3/valx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:42:53.000000 valx-0.1.3/valx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 12:42:53.000000 valx-0.1.3/valx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:20:12.269870 valx-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-13 07:20:09.000000 valx-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-13 07:20:12.269870 valx-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-13 07:20:09.000000 valx-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:20:12.269870 valx-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-13 07:20:12.000000 valx-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:20:12.265870 valx-0.1.5/valx/
+-rw-r--r--   0 runner    (1001) docker     (127)    42515 2024-04-13 07:20:09.000000 valx-0.1.5/valx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:20:12.265870 valx-0.1.5/valx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-13 07:20:12.000000 valx-0.1.5/valx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 07:20:12.000000 valx-0.1.5/valx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:20:12.000000 valx-0.1.5/valx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 07:20:12.000000 valx-0.1.5/valx.egg-info/top_level.txt
```

### Comparing `valx-0.1.3/LICENSE` & `valx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `valx-0.1.3/PKG-INFO` & `valx-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valx
-Version: 0.1.3
+Version: 0.1.5
 Summary: An open-source Python library for text cleaning tasks.
 Home-page: https://github.com/infinitode/valx
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `valx-0.1.3/README.md` & `valx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `valx-0.1.3/setup.py` & `valx-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='valx',
-    version='0.1.3',
+    version='0.1.5',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='An open-source Python library for text cleaning tasks.',
     long_description='An open-source Python library for data cleaning tasks. Includes profanity detection, and removal.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/valx',
     packages=find_packages(),
```

### Comparing `valx-0.1.3/valx/__init__.py` & `valx-0.1.5/valx/__init__.py`

 * *Files identical despite different names*

### Comparing `valx-0.1.3/valx.egg-info/PKG-INFO` & `valx-0.1.5/valx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valx
-Version: 0.1.3
+Version: 0.1.5
 Summary: An open-source Python library for text cleaning tasks.
 Home-page: https://github.com/infinitode/valx
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

