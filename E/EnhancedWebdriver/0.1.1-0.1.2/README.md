# Comparing `tmp/enhancedwebdriver-0.1.1.tar.gz` & `tmp/enhancedwebdriver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedwebdriver-0.1.1.tar", last modified: Fri Apr 12 22:25:40 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.2.tar", last modified: Fri Apr 12 22:31:01 2024, max compression
```

## Comparing `enhancedwebdriver-0.1.1.tar` & `enhancedwebdriver-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.1/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.1/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      695 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.149917 enhancedwebdriver-0.1.1/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      335 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       17 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    13883 2024-04-12 22:23:59.000000 enhancedwebdriver-0.1.1/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.1/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:31:01.729926 enhancedwebdriver-0.1.2/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.2/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)      594 2024-04-12 22:31:01.729926 enhancedwebdriver-0.1.2/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.2/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      712 2024-04-12 22:31:01.729926 enhancedwebdriver-0.1.2/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:31:01.725926 enhancedwebdriver-0.1.2/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:31:01.729926 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)      594 2024-04-12 22:31:01.000000 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      335 2024-04-12 22:31:01.000000 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-12 22:31:01.000000 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       33 2024-04-12 22:31:01.000000 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-12 22:31:01.000000 enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:31:01.729926 enhancedwebdriver-0.1.2/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    13883 2024-04-12 22:23:59.000000 enhancedwebdriver-0.1.2/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.2/src/enhanced_webdriver/__init__.py
```

### Comparing `enhancedwebdriver-0.1.1/LICENSE` & `enhancedwebdriver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedwebdriver-0.1.1/PKG-INFO` & `enhancedwebdriver-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.05
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.18.0
+Requires-Dist: download>=0.3.5
```

### Comparing `enhancedwebdriver-0.1.1/setup.cfg` & `enhancedwebdriver-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.1
+version = 0.1.2
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls = 
@@ -17,14 +17,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.05
 install_requires = 
 	selenium>=4.18.0
+	download>=0.3.5
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/PKG-INFO` & `enhancedwebdriver-0.1.2/src/EnhancedWebdriver.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.05
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium>=4.18.0
+Requires-Dist: download>=0.3.5
```

### Comparing `enhancedwebdriver-0.1.1/src/enhanced_webdriver/EnhancedWebdriver.py` & `enhancedwebdriver-0.1.2/src/enhanced_webdriver/EnhancedWebdriver.py`

 * *Files identical despite different names*

