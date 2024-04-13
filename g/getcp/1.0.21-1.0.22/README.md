# Comparing `tmp/getcp-1.0.21.tar.gz` & `tmp/getcp-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getcp-1.0.21.tar", last modified: Sat Apr 13 09:01:23 2024, max compression
+gzip compressed data, was "getcp-1.0.22.tar", last modified: Sat Apr 13 11:20:55 2024, max compression
```

## Comparing `getcp-1.0.21.tar` & `getcp-1.0.22.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 09:01:23.837359 getcp-1.0.21/
--rw-rw-rw-   0        0        0     1090 2024-04-12 16:54:47.000000 getcp-1.0.21/LICENSE
--rw-rw-rw-   0        0        0     1914 2024-04-13 09:01:23.828793 getcp-1.0.21/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-12 20:26:25.000000 getcp-1.0.21/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 09:01:23.809749 getcp-1.0.21/getcp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:46:43.000000 getcp-1.0.21/getcp/__init__.py
--rw-rw-rw-   0        0        0     1543 2024-04-13 08:49:37.000000 getcp-1.0.21/getcp/cc.py
--rw-rw-rw-   0        0        0     1242 2024-04-12 16:48:04.000000 getcp-1.0.21/getcp/cf.py
-drwxrwxrwx   0        0        0        0 2024-04-13 09:01:23.826381 getcp-1.0.21/getcp.egg-info/
--rw-rw-rw-   0        0        0     1914 2024-04-13 09:01:23.000000 getcp-1.0.21/getcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-13 09:01:23.000000 getcp-1.0.21/getcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 09:01:23.000000 getcp-1.0.21/getcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-13 09:01:23.000000 getcp-1.0.21/getcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-13 09:01:23.000000 getcp-1.0.21/getcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 09:01:23.837359 getcp-1.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1485 2024-04-13 09:00:40.000000 getcp-1.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 11:20:55.551908 getcp-1.0.22/
+-rw-rw-rw-   0        0        0     1090 2024-04-12 16:54:47.000000 getcp-1.0.22/LICENSE
+-rw-rw-rw-   0        0        0     2032 2024-04-13 11:20:55.550911 getcp-1.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-04-13 11:20:15.000000 getcp-1.0.22/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 11:20:55.543511 getcp-1.0.22/getcp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:46:43.000000 getcp-1.0.22/getcp/__init__.py
+-rw-rw-rw-   0        0        0     1543 2024-04-13 08:49:37.000000 getcp-1.0.22/getcp/cc.py
+-rw-rw-rw-   0        0        0     1242 2024-04-12 16:48:04.000000 getcp-1.0.22/getcp/cf.py
+-rw-rw-rw-   0        0        0     1843 2024-04-13 11:13:47.000000 getcp-1.0.22/getcp/github.py
+drwxrwxrwx   0        0        0        0 2024-04-13 11:20:55.549911 getcp-1.0.22/getcp.egg-info/
+-rw-rw-rw-   0        0        0     2032 2024-04-13 11:20:55.000000 getcp-1.0.22/getcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2024-04-13 11:20:55.000000 getcp-1.0.22/getcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 11:20:55.000000 getcp-1.0.22/getcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-13 11:20:55.000000 getcp-1.0.22/getcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-13 11:20:55.000000 getcp-1.0.22/getcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 11:20:55.552944 getcp-1.0.22/setup.cfg
+-rw-rw-rw-   0        0        0     1485 2024-04-13 11:20:37.000000 getcp-1.0.22/setup.py
```

### Comparing `getcp-1.0.21/LICENSE` & `getcp-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `getcp-1.0.21/PKG-INFO` & `getcp-1.0.22/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getcp
-Version: 1.0.21
+Version: 1.0.22
 Summary: getcp is a Python package that provides functions to retrieve stats from Competitive Programming platforms. Currently, it supports fetching stats from CodeChef and Codeforces.
 Home-page: https://github.com/UD11/getcp-pkg
 Author: Uddalak Seal
 Author-email: hidan84@duck.com
 License: MIT
 Project-URL: Documentation, https://ud11.github.io/getcp-docs/
 Project-URL: Source, https://github.com/UD11/getcp-pkg?tab=readme-ov-file
@@ -45,21 +45,24 @@
 
 ```bash
 pip install getcp
 ```
 
 ## Usage
 
-```bash
-    from getcp import cc, cf
+```py
+    from getcp import cc, cf, github
     
     codechef_stats = cc.get_codechef_stats('username')
     codeforces_stats = cf.get_codeforces_stats('username')
+    github_info = github.get_github_stats('username')
     
     print("CodeChef Stats:")
     print(codechef_stats)
     
-    print("\nCodeforces )Stats:")
-    print(codeforces_stats
-
+    print("\nCodeforces Stats:")
+    print(codeforces_stats)
+    
+    print("\nGithub Info:")
+    print(github_info)
 
 ```
```

### Comparing `getcp-1.0.21/README.md` & `getcp-1.0.22/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 
 ```bash
 pip install getcp
 ```
 
 ## Usage
 
-```bash
-    from getcp import cc, cf
+```py
+    from getcp import cc, cf, github
     
     codechef_stats = cc.get_codechef_stats('username')
     codeforces_stats = cf.get_codeforces_stats('username')
+    github_info = github.get_github_stats('username')
     
     print("CodeChef Stats:")
     print(codechef_stats)
     
-    print("\nCodeforces )Stats:")
-    print(codeforces_stats
-
+    print("\nCodeforces Stats:")
+    print(codeforces_stats)
+    
+    print("\nGithub Info:")
+    print(github_info)
 
 ```
```

### Comparing `getcp-1.0.21/getcp/cc.py` & `getcp-1.0.22/getcp/cc.py`

 * *Files identical despite different names*

### Comparing `getcp-1.0.21/getcp/cf.py` & `getcp-1.0.22/getcp/cf.py`

 * *Files identical despite different names*

### Comparing `getcp-1.0.21/getcp.egg-info/PKG-INFO` & `getcp-1.0.22/getcp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getcp
-Version: 1.0.21
+Version: 1.0.22
 Summary: getcp is a Python package that provides functions to retrieve stats from Competitive Programming platforms. Currently, it supports fetching stats from CodeChef and Codeforces.
 Home-page: https://github.com/UD11/getcp-pkg
 Author: Uddalak Seal
 Author-email: hidan84@duck.com
 License: MIT
 Project-URL: Documentation, https://ud11.github.io/getcp-docs/
 Project-URL: Source, https://github.com/UD11/getcp-pkg?tab=readme-ov-file
@@ -45,21 +45,24 @@
 
 ```bash
 pip install getcp
 ```
 
 ## Usage
 
-```bash
-    from getcp import cc, cf
+```py
+    from getcp import cc, cf, github
     
     codechef_stats = cc.get_codechef_stats('username')
     codeforces_stats = cf.get_codeforces_stats('username')
+    github_info = github.get_github_stats('username')
     
     print("CodeChef Stats:")
     print(codechef_stats)
     
-    print("\nCodeforces )Stats:")
-    print(codeforces_stats
-
+    print("\nCodeforces Stats:")
+    print(codeforces_stats)
+    
+    print("\nGithub Info:")
+    print(github_info)
 
 ```
```

### Comparing `getcp-1.0.21/setup.py` & `getcp-1.0.22/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='getcp',
-    version='1.0.21',
+    version='1.0.22',
     description='getcp is a Python package that provides functions to retrieve stats from Competitive Programming platforms. Currently, it supports fetching stats from CodeChef and Codeforces.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UD11/getcp-pkg",
     author='Uddalak Seal',
     author_email='hidan84@duck.com',
     license='MIT',
```

