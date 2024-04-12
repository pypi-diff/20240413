# Comparing `tmp/g2papi-1.0.2.tar.gz` & `tmp/g2papi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2papi-1.0.2.tar", last modified: Fri Apr 12 21:48:02 2024, max compression
+gzip compressed data, was "g2papi-1.0.3.tar", last modified: Fri Apr 12 21:51:22 2024, max compression
```

## Comparing `g2papi-1.0.2.tar` & `g2papi-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.166732 g2papi-1.0.2/
--rw-r--r--   0 jsafer     (503) staff       (20)     1072 2024-04-12 21:04:13.000000 g2papi-1.0.2/LICENSE
--rw-r--r--   0 jsafer     (503) staff       (20)     4191 2024-04-12 21:48:02.165767 g2papi-1.0.2/PKG-INFO
--rw-r--r--   0 jsafer     (503) staff       (20)     3910 2024-04-12 21:04:13.000000 g2papi-1.0.2/README.md
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.158943 g2papi-1.0.2/g2papi/
--rw-r--r--   0 jsafer     (503) staff       (20)       85 2024-03-28 16:40:25.000000 g2papi-1.0.2/g2papi/__init__.py
--rw-r--r--   0 jsafer     (503) staff       (20)      844 2024-03-28 18:16:13.000000 g2papi-1.0.2/g2papi/api.py
--rw-r--r--   0 jsafer     (503) staff       (20)     1340 2024-03-28 18:00:11.000000 g2papi-1.0.2/g2papi/cli.py
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.164802 g2papi-1.0.2/g2papi.egg-info/
--rw-r--r--   0 jsafer     (503) staff       (20)     4191 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/PKG-INFO
--rw-r--r--   0 jsafer     (503) staff       (20)      255 2024-04-12 21:48:02.000000 g2papi-1.0.2/g2papi.egg-info/SOURCES.txt
--rw-r--r--   0 jsafer     (503) staff       (20)        1 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/dependency_links.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       43 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/entry_points.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       16 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/requires.txt
--rw-r--r--   0 jsafer     (503) staff       (20)        7 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/top_level.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       38 2024-04-12 21:48:02.167212 g2papi-1.0.2/setup.cfg
--rw-r--r--   0 jsafer     (503) staff       (20)      625 2024-04-12 21:47:47.000000 g2papi-1.0.2/setup.py
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:51:22.969262 g2papi-1.0.3/
+-rw-r--r--   0 jsafer     (503) staff       (20)     1072 2024-04-12 21:04:13.000000 g2papi-1.0.3/LICENSE
+-rw-r--r--   0 jsafer     (503) staff       (20)     4313 2024-04-12 21:51:22.968731 g2papi-1.0.3/PKG-INFO
+-rw-r--r--   0 jsafer     (503) staff       (20)     3910 2024-04-12 21:04:13.000000 g2papi-1.0.3/README.md
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:51:22.961754 g2papi-1.0.3/g2papi/
+-rw-r--r--   0 jsafer     (503) staff       (20)       85 2024-03-28 16:40:25.000000 g2papi-1.0.3/g2papi/__init__.py
+-rw-r--r--   0 jsafer     (503) staff       (20)      844 2024-03-28 18:16:13.000000 g2papi-1.0.3/g2papi/api.py
+-rw-r--r--   0 jsafer     (503) staff       (20)     1340 2024-03-28 18:00:11.000000 g2papi-1.0.3/g2papi/cli.py
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:51:22.967648 g2papi-1.0.3/g2papi.egg-info/
+-rw-r--r--   0 jsafer     (503) staff       (20)     4313 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/PKG-INFO
+-rw-r--r--   0 jsafer     (503) staff       (20)      255 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/SOURCES.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)        1 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/dependency_links.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       43 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/entry_points.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       16 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/requires.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)        7 2024-04-12 21:51:22.000000 g2papi-1.0.3/g2papi.egg-info/top_level.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       38 2024-04-12 21:51:22.969491 g2papi-1.0.3/setup.cfg
+-rw-r--r--   0 jsafer     (503) staff       (20)      772 2024-04-12 21:51:08.000000 g2papi-1.0.3/setup.py
```

### Comparing `g2papi-1.0.2/LICENSE` & `g2papi-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.2/PKG-INFO` & `g2papi-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: g2papi
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python client and CLI for easy access to G2P portal APIs
 Author: Jordan Safer
 Author-email: genomics2proteins@gmail.com
 License: UNKNOWN
+Project-URL: GitHub, https://www.github.com/broadinstitute/g2papi
+Project-URL: G2P portal, https://g2p.broadinstitute.org
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # g2papi
 
 `g2papi` is a Python library and command-line tool designed to interact with the G2P API provided by the Broad Institute. It allows users to retrieve mappings between protein isoforms, transcripts, and PDB structures for a gene, as well as protein feature tables for a gene.
```

### Comparing `g2papi-1.0.2/README.md` & `g2papi-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.2/g2papi/api.py` & `g2papi-1.0.3/g2papi/api.py`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.2/g2papi/cli.py` & `g2papi-1.0.3/g2papi/cli.py`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.2/g2papi.egg-info/PKG-INFO` & `g2papi-1.0.3/g2papi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: g2papi
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python client and CLI for easy access to G2P portal APIs
 Author: Jordan Safer
 Author-email: genomics2proteins@gmail.com
 License: UNKNOWN
+Project-URL: GitHub, https://www.github.com/broadinstitute/g2papi
+Project-URL: G2P portal, https://g2p.broadinstitute.org
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # g2papi
 
 `g2papi` is a Python library and command-line tool designed to interact with the G2P API provided by the Broad Institute. It allows users to retrieve mappings between protein isoforms, transcripts, and PDB structures for a gene, as well as protein feature tables for a gene.
```

### Comparing `g2papi-1.0.2/setup.py` & `g2papi-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='g2papi',
-    version='1.0.2',
+    version='1.0.3',
     author='Jordan Safer',
     author_email='genomics2proteins@gmail.com',
     description='A python client and CLI for easy access to G2P portal APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    project_urls={
+        "GitHub": "https://www.github.com/broadinstitute/g2papi",
+        "G2P portal": "https://g2p.broadinstitute.org"
+    },
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas'
     ],
     entry_points={
         'console_scripts': [
```

