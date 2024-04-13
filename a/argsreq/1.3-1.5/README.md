# Comparing `tmp/argsreq-1.3.tar.gz` & `tmp/argsreq-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argsreq-1.3.tar", last modified: Sat Apr 13 08:50:40 2024, max compression
+gzip compressed data, was "argsreq-1.5.tar", last modified: Sat Apr 13 09:07:57 2024, max compression
```

## Comparing `argsreq-1.3.tar` & `argsreq-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 08:50:40.646761 argsreq-1.3/
--rw-rw-rw-   0        0        0      311 2024-04-13 08:50:40.646761 argsreq-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 08:50:40.643799 argsreq-1.3/argsreq.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-13 08:50:40.000000 argsreq-1.3/argsreq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-13 08:50:40.000000 argsreq-1.3/argsreq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 08:50:40.000000 argsreq-1.3/argsreq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 08:50:40.000000 argsreq-1.3/argsreq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-13 08:50:40.645770 argsreq-1.3/reqargs/
--rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:08.000000 argsreq-1.3/reqargs/__init__.py
--rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.3/reqargs/__main__.py
--rw-rw-rw-   0        0        0    15372 2024-04-13 08:50:18.000000 argsreq-1.3/reqargs/colorls.py
--rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:22.000000 argsreq-1.3/reqargs/reqargs.py
--rw-rw-rw-   0        0        0       42 2024-04-13 08:50:40.647789 argsreq-1.3/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-04-13 08:50:33.000000 argsreq-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.902454 argsreq-1.5/
+-rw-rw-rw-   0        0        0      311 2024-04-13 09:07:57.901434 argsreq-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.898553 argsreq-1.5/argsreq.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 09:07:57.000000 argsreq-1.5/argsreq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 09:07:57.901434 argsreq-1.5/reqargs/
+-rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:08.000000 argsreq-1.5/reqargs/__init__.py
+-rw-rw-rw-   0        0        0       34 2022-11-18 04:36:49.000000 argsreq-1.5/reqargs/__main__.py
+-rw-rw-rw-   0        0        0    15372 2024-04-13 08:50:18.000000 argsreq-1.5/reqargs/colorls.py
+-rw-rw-rw-   0        0        0    15786 2024-04-13 08:50:22.000000 argsreq-1.5/reqargs/reqargs.py
+-rw-rw-rw-   0        0        0       42 2024-04-13 09:07:57.903463 argsreq-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      641 2024-04-13 09:07:49.000000 argsreq-1.5/setup.py
```

### Comparing `argsreq-1.3/reqargs/__init__.py` & `argsreq-1.5/reqargs/__init__.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.3/reqargs/colorls.py` & `argsreq-1.5/reqargs/colorls.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.3/reqargs/reqargs.py` & `argsreq-1.5/reqargs/reqargs.py`

 * *Files identical despite different names*

### Comparing `argsreq-1.3/setup.py` & `argsreq-1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3'
+VERSION = '1.5'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="argsreq",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
+    package_data={'colorls': ['config/colorls.toml']},
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

