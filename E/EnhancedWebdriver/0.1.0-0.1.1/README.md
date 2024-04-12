# Comparing `tmp/enhancedwebdriver-0.1.tar.gz` & `tmp/enhancedwebdriver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedwebdriver-0.1.tar", last modified: Fri Apr 12 20:25:48 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.1.tar", last modified: Fri Apr 12 22:25:40 2024, max compression
```

## Comparing `enhancedwebdriver-0.1.tar` & `enhancedwebdriver-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 20:25:48.390948 enhancedwebdriver-0.1/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 20:25:48.390948 enhancedwebdriver-0.1/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      695 2024-04-12 20:25:48.394948 enhancedwebdriver-0.1/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 20:25:48.386948 enhancedwebdriver-0.1/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 20:25:48.390948 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 20:25:48.000000 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      335 2024-04-12 20:25:48.000000 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-12 20:25:48.000000 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       17 2024-04-12 20:25:48.000000 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-12 20:25:48.000000 enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 20:25:48.390948 enhancedwebdriver-0.1/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    13749 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.1/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.1/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      695 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.149917 enhancedwebdriver-0.1.1/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)      563 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      335 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       17 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-12 22:25:40.000000 enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-12 22:25:40.153917 enhancedwebdriver-0.1.1/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    13883 2024-04-12 22:23:59.000000 enhancedwebdriver-0.1.1/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.1/src/enhanced_webdriver/__init__.py
```

### Comparing `enhancedwebdriver-0.1/LICENSE` & `enhancedwebdriver-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedwebdriver-0.1/PKG-INFO` & `enhancedwebdriver-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1/setup.cfg` & `enhancedwebdriver-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.0
+version = 0.1.1
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls =
```

### Comparing `enhancedwebdriver-0.1/src/EnhancedWebdriver.egg-info/PKG-INFO` & `enhancedwebdriver-0.1.1/src/EnhancedWebdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.0
+Version: 0.1.1
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1/src/enhanced_webdriver/EnhancedWebdriver.py` & `enhancedwebdriver-0.1.1/src/enhanced_webdriver/EnhancedWebdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 import shutil
 import subprocess
 from pathlib import Path
 from time import sleep
 from typing import Optional
 
-import undetected_chromedriver as uc
 from download import download
 from selenium import webdriver
 from selenium.common.exceptions import (
     StaleElementReferenceException,
     NoSuchElementException,
     TimeoutException,
     WebDriverException,
@@ -63,18 +62,20 @@
         """
         instance = object.__new__(EnhancedWebdriver)
         if web_driver is None:
             try:
                 if not undetected:
                     web_driver = webdriver.Chrome(options, service, keep_alive)
                 elif service is not None:
+                    import undetected_chromedriver as uc
                     web_driver = uc.Chrome(
                         options, driver_executable_path=service._path
                     )
                 else:
+                    import undetected_chromedriver as uc
                     web_driver = uc.Chrome(
                         options,
                         driver_executable_path=next(
                             Path(__file__).parent.glob(cls._driver_name.format("*"))
                         ),
                     )
             except (SessionNotCreatedException, NoSuchDriverException, StopIteration) as e:
@@ -90,14 +91,15 @@
                 for executable_file in Path(__file__).parent.glob(
                     cls._driver_name.format("*")
                 ):
                     if executable_file.name == executable_path.name:
                         continue
                     os.remove(executable_file)
                 if undetected:
+                    import undetected_chromedriver as uc
                     web_driver = uc.Chrome(driver_executable_path=executable_path)
                 else:
                     service = Service(executable_path=str(executable_path))
                     web_driver = webdriver.Chrome(service=service)
         instance.__dict__ = web_driver.__dict__
         return instance
```

