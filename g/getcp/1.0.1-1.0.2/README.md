# Comparing `tmp/getcp-1.0.1.tar.gz` & `tmp/getcp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getcp-1.0.1.tar", last modified: Fri Apr 12 17:12:45 2024, max compression
+gzip compressed data, was "getcp-1.0.2.tar", last modified: Fri Apr 12 17:30:46 2024, max compression
```

## Comparing `getcp-1.0.1.tar` & `getcp-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:12:45.023274 getcp-1.0.1/
--rw-rw-rw-   0        0        0     1090 2024-04-12 16:54:47.000000 getcp-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1055 2024-04-12 17:12:45.020315 getcp-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      625 2024-04-12 17:03:29.000000 getcp-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 17:12:44.973573 getcp-1.0.1/getcp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:46:43.000000 getcp-1.0.1/getcp/__init__.py
--rw-rw-rw-   0        0        0     1547 2024-04-12 16:47:46.000000 getcp-1.0.1/getcp/cc.py
--rw-rw-rw-   0        0        0     1242 2024-04-12 16:48:04.000000 getcp-1.0.1/getcp/cf.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:12:45.019125 getcp-1.0.1/getcp.egg-info/
--rw-rw-rw-   0        0        0     1055 2024-04-12 17:12:44.000000 getcp-1.0.1/getcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-12 17:12:44.000000 getcp-1.0.1/getcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:12:44.000000 getcp-1.0.1/getcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-12 17:12:44.000000 getcp-1.0.1/getcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 17:12:44.000000 getcp-1.0.1/getcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 17:12:45.023274 getcp-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-04-12 17:12:34.000000 getcp-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:30:46.976903 getcp-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-04-12 16:54:47.000000 getcp-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1007 2024-04-12 17:30:46.974197 getcp-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2024-04-12 17:29:21.000000 getcp-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 17:30:46.931874 getcp-1.0.2/getcp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:46:43.000000 getcp-1.0.2/getcp/__init__.py
+-rw-rw-rw-   0        0        0     1547 2024-04-12 16:47:46.000000 getcp-1.0.2/getcp/cc.py
+-rw-rw-rw-   0        0        0     1242 2024-04-12 16:48:04.000000 getcp-1.0.2/getcp/cf.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:30:46.971588 getcp-1.0.2/getcp.egg-info/
+-rw-rw-rw-   0        0        0     1007 2024-04-12 17:30:46.000000 getcp-1.0.2/getcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-12 17:30:46.000000 getcp-1.0.2/getcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:30:46.000000 getcp-1.0.2/getcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-12 17:30:46.000000 getcp-1.0.2/getcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 17:30:46.000000 getcp-1.0.2/getcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 17:30:46.978167 getcp-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-12 17:26:39.000000 getcp-1.0.2/setup.py
```

### Comparing `getcp-1.0.1/LICENSE` & `getcp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getcp-1.0.1/PKG-INFO` & `getcp-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getcp
-Version: 1.0.1
+Version: 1.0.2
 Summary: getcp is a Python package that provides functions to retrieve stats from CP platforms. Currently, it supports fetching stats from CodeChef and Codeforces.
 Author: Uddalak Seal
 Author-email: hidan84@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -26,18 +26,18 @@
 ```bash
 pip install getcp
 ```
 
 ## Usage
 
 ```bash
-    from getcp import get_codechef_stats, get_codeforces_stats
-
-    codechef_stats = get_codechef_stats('my_codechef_username')
-    codeforces_stats = get_codeforces_stats('my_codeforces_handle')
+    from getcp import cc, cf
+    
+    codechef_stats = cc.get_codechef_stats('username')
+    codeforces_stats = cf.get_codeforces_stats('username')
     
     print("CodeChef Stats:")
     print(codechef_stats)
     
     print("\nCodeforces Stats:")
     print(codeforces_stats)
```

### Comparing `getcp-1.0.1/getcp/cc.py` & `getcp-1.0.2/getcp/cc.py`

 * *Files identical despite different names*

### Comparing `getcp-1.0.1/getcp/cf.py` & `getcp-1.0.2/getcp/cf.py`

 * *Files identical despite different names*

### Comparing `getcp-1.0.1/getcp.egg-info/PKG-INFO` & `getcp-1.0.2/getcp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getcp
-Version: 1.0.1
+Version: 1.0.2
 Summary: getcp is a Python package that provides functions to retrieve stats from CP platforms. Currently, it supports fetching stats from CodeChef and Codeforces.
 Author: Uddalak Seal
 Author-email: hidan84@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -26,18 +26,18 @@
 ```bash
 pip install getcp
 ```
 
 ## Usage
 
 ```bash
-    from getcp import get_codechef_stats, get_codeforces_stats
-
-    codechef_stats = get_codechef_stats('my_codechef_username')
-    codeforces_stats = get_codeforces_stats('my_codeforces_handle')
+    from getcp import cc, cf
+    
+    codechef_stats = cc.get_codechef_stats('username')
+    codeforces_stats = cf.get_codeforces_stats('username')
     
     print("CodeChef Stats:")
     print(codechef_stats)
     
     print("\nCodeforces Stats:")
     print(codeforces_stats)
```

### Comparing `getcp-1.0.1/setup.py` & `getcp-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='getcp',
-    version='1.0.1',
+    version='1.0.2',
     description='getcp is a Python package that provides functions to retrieve stats from CP platforms. Currently, it supports fetching stats from CodeChef and Codeforces.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Uddalak Seal',
     author_email='hidan84@duck.com',
     packages=setuptools.find_packages(),
     install_requires=[
```

