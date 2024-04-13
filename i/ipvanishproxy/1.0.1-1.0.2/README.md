# Comparing `tmp/ipvanishproxy-1.0.1.tar.gz` & `tmp/ipvanishproxy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipvanishproxy-1.0.1.tar", last modified: Sat Apr 13 19:39:59 2024, max compression
+gzip compressed data, was "ipvanishproxy-1.0.2.tar", last modified: Sat Apr 13 19:52:46 2024, max compression
```

## Comparing `ipvanishproxy-1.0.1.tar` & `ipvanishproxy-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 19:39:59.078997 ipvanishproxy-1.0.1/
--rw-rw-rw-   0        0        0      549 2024-04-13 19:39:59.076996 ipvanishproxy-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 19:39:59.005996 ipvanishproxy-1.0.1/app/
-drwxrwxrwx   0        0        0        0 2024-04-13 19:39:59.071998 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/
--rw-rw-rw-   0        0        0      549 2024-04-13 19:39:58.000000 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-13 19:39:58.000000 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:39:58.000000 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-13 19:39:58.000000 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:39:58.000000 ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 19:39:59.079996 ipvanishproxy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      869 2024-04-13 19:39:39.000000 ipvanishproxy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:52:46.329297 ipvanishproxy-1.0.2/
+-rw-rw-rw-   0        0        0      529 2024-04-13 19:52:46.326295 ipvanishproxy-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 19:52:46.295297 ipvanishproxy-1.0.2/ipvanishproxy/
+-rw-rw-rw-   0        0        0       24 2024-04-13 17:05:39.000000 ipvanishproxy-1.0.2/ipvanishproxy/__init__.py
+-rw-rw-rw-   0        0        0     5235 2024-04-13 17:10:59.000000 ipvanishproxy-1.0.2/ipvanishproxy/proxy.py
+drwxrwxrwx   0        0        0        0 2024-04-13 19:52:46.323295 ipvanishproxy-1.0.2/ipvanishproxy.egg-info/
+-rw-rw-rw-   0        0        0      529 2024-04-13 19:52:46.000000 ipvanishproxy-1.0.2/ipvanishproxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-04-13 19:52:46.000000 ipvanishproxy-1.0.2/ipvanishproxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 19:52:46.000000 ipvanishproxy-1.0.2/ipvanishproxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-13 19:52:46.000000 ipvanishproxy-1.0.2/ipvanishproxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 19:52:46.329297 ipvanishproxy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-13 19:52:42.000000 ipvanishproxy-1.0.2/setup.py
```

### Comparing `ipvanishproxy-1.0.1/PKG-INFO` & `ipvanishproxy-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: ipvanishproxy
-Version: 1.0.1
+Version: 1.0.2
 Summary: ipVanish proxy dictionary package
 Author: Nahom Dereje
 Author-email: dev@nahom.eu.org
 Keywords: IpVanish,Proxy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: app
 
 ipVanish proxy dictionary package which returns simple froxy dictionary given username and password
```

### Comparing `ipvanishproxy-1.0.1/app/ipvanishproxy.egg-info/PKG-INFO` & `ipvanishproxy-1.0.2/ipvanishproxy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: ipvanishproxy
-Version: 1.0.1
+Version: 1.0.2
 Summary: ipVanish proxy dictionary package
 Author: Nahom Dereje
 Author-email: dev@nahom.eu.org
 Keywords: IpVanish,Proxy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Dist: app
 
 ipVanish proxy dictionary package which returns simple froxy dictionary given username and password
```

### Comparing `ipvanishproxy-1.0.1/setup.py` & `ipvanishproxy-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'ipVanish proxy dictionary package'
 LONG_DESCRIPTION = 'ipVanish proxy dictionary package which returns simple froxy dictionary given username and password'
 
 setup(
     name='ipvanishproxy',
     version=VERSION,
     author='Nahom Dereje',
     author_email='dev@nahom.eu.org',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    package_dir={"":"app"},
-    packages=[],
-    install_requires=find_packages(),
+    packages=find_packages(),
+    install_requires=[],
     keywords=['IpVanish', "Proxy"],
     classifiers= [
                 "Development Status :: 3 - Alpha",
                 "Intended Audience :: Education",
                 "Programming Language :: Python :: 3",
                 "Operating System :: MacOS :: MacOS X",
                 "Operating System :: Microsoft :: Windows"
```

