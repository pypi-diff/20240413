# Comparing `tmp/emo_market_base-0.0.3.tar.gz` & `tmp/emo_market_base-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emo_market_base-0.0.3.tar", last modified: Mon Apr  8 21:20:38 2024, max compression
+gzip compressed data, was "emo_market_base-0.0.4.tar", last modified: Sat Apr 13 14:52:48 2024, max compression
```

## Comparing `emo_market_base-0.0.3.tar` & `emo_market_base-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 21:20:38.694719 emo_market_base-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.686720 emo_market_base-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/emo_market_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 21:20:38.000000 emo_market_base-0.0.3/src/emo_market_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/market_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/filesytem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:38.690719 emo_market_base-0.0.3/src/market_base/webdriver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/category_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/list_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/product_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-08 21:20:33.000000 emo_market_base-0.0.3/src/market_base/webdriver/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:48.262597 emo_market_base-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/src/emo_market_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-13 14:52:48.000000 emo_market_base-0.0.4/src/emo_market_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-13 14:52:48.000000 emo_market_base-0.0.4/src/emo_market_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:52:48.000000 emo_market_base-0.0.4/src/emo_market_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-13 14:52:48.000000 emo_market_base-0.0.4/src/emo_market_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 14:52:48.000000 emo_market_base-0.0.4/src/emo_market_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/src/market_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/filesytem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:48.266597 emo_market_base-0.0.4/src/market_base/webdriver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/category_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/list_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/product_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-13 14:52:40.000000 emo_market_base-0.0.4/src/market_base/webdriver/url.py
```

### Comparing `emo_market_base-0.0.3/LICENSE` & `emo_market_base-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/PKG-INFO` & `emo_market_base-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emo_market_base
-Version: 0.0.3
+Version: 0.0.4
 Summary: Marketlerden ürünleri kazıma işlemleri için temel pakettir
 Home-page: https://github.com/erenmustafaozdal/market-base
 Author: Eren Mustafa Özdal
 Author-email: eren.060737@gmail.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `emo_market_base-0.0.3/setup.py` & `emo_market_base-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="emo_market_base",
-    version="v0.0.3",
+    version="v0.0.4",
     author="Eren Mustafa Özdal",
     author_email="eren.060737@gmail.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     description="Marketlerden ürünleri kazıma işlemleri için temel pakettir",
     long_description=description,
     long_description_content_type="text/markdown",
```

### Comparing `emo_market_base-0.0.3/src/emo_market_base.egg-info/PKG-INFO` & `emo_market_base-0.0.4/src/emo_market_base.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emo_market_base
-Version: 0.0.3
+Version: 0.0.4
 Summary: Marketlerden ürünleri kazıma işlemleri için temel pakettir
 Home-page: https://github.com/erenmustafaozdal/market-base
 Author: Eren Mustafa Özdal
 Author-email: eren.060737@gmail.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `emo_market_base-0.0.3/src/emo_market_base.egg-info/SOURCES.txt` & `emo_market_base-0.0.4/src/emo_market_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/date.py` & `emo_market_base-0.0.4/src/market_base/date.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/db.py` & `emo_market_base-0.0.4/src/market_base/db.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/filesytem.py` & `emo_market_base-0.0.4/src/market_base/filesytem.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/category_page.py` & `emo_market_base-0.0.4/src/market_base/webdriver/category_page.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/list_product.py` & `emo_market_base-0.0.4/src/market_base/webdriver/list_product.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/market.py` & `emo_market_base-0.0.4/src/market_base/webdriver/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,16 @@
             self.driver.execute_script(self.remove_element_script, el)
 
     def scroll_to_element(self, el: Union[WebElement, Tuple[str, str]]):
         # eğer gönderilen bir web elemanı değilse seç
         if not isinstance(el, WebElement):
             el = self.driver.find_element(*el)
 
+        self.driver.execute_script(self.scroll_to_element_script, el)
+
     def scroll_to_bottom(self):
         self.driver.execute_script(self.scroll_to_bottom_script)
 
     def get_next_date(self, excludes: List, locator: Tuple[str, str]) -> Dict:
         els = self.driver.find_elements(*locator)
         dates = Date.get_dates(els, excludes)
         return Date.next_date(dates)
```

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/product.py` & `emo_market_base-0.0.4/src/market_base/webdriver/product.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/product_page.py` & `emo_market_base-0.0.4/src/market_base/webdriver/product_page.py`

 * *Files identical despite different names*

### Comparing `emo_market_base-0.0.3/src/market_base/webdriver/url.py` & `emo_market_base-0.0.4/src/market_base/webdriver/url.py`

 * *Files identical despite different names*

