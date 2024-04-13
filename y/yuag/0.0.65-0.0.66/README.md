# Comparing `tmp/yuag-0.0.65.tar.gz` & `tmp/yuag-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.65.tar", last modified: Sat Apr  6 19:53:40 2024, max compression
+gzip compressed data, was "yuag-0.0.66.tar", last modified: Sat Apr 13 21:15:27 2024, max compression
```

## Comparing `yuag-0.0.65.tar` & `yuag-0.0.66.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:53:40.417967 yuag-0.0.65/
--rw-rw-rw-   0        0        0       52 2024-04-06 19:53:40.411991 yuag-0.0.65/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-06 19:53:40.418970 yuag-0.0.65/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-06 19:53:22.000000 yuag-0.0.65/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:53:40.285194 yuag-0.0.65/yuag/
--rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.65/yuag/__init__.py
--rw-rw-rw-   0        0        0    42581 2024-04-06 19:44:14.000000 yuag-0.0.65/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:53:40.409993 yuag-0.0.65/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-06 19:53:39.000000 yuag-0.0.65/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-06 19:53:39.000000 yuag-0.0.65/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:53:39.000000 yuag-0.0.65/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-06 19:53:39.000000 yuag-0.0.65/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.084455 yuag-0.0.66/
+-rw-rw-rw-   0        0        0       52 2024-04-13 21:15:27.081457 yuag-0.0.66/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 21:15:27.084455 yuag-0.0.66/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-13 21:15:04.000000 yuag-0.0.66/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.049478 yuag-0.0.66/yuag/
+-rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.66/yuag/__init__.py
+-rw-rw-rw-   0        0        0    42525 2024-04-13 21:14:57.000000 yuag-0.0.66/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-13 21:15:27.079461 yuag-0.0.66/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-13 21:15:26.000000 yuag-0.0.66/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.65/yuag/__init__.py` & `yuag-0.0.66/yuag/__init__.py`

 * *Files identical despite different names*

### Comparing `yuag-0.0.65/yuag/yuag.py` & `yuag-0.0.66/yuag/yuag.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,17 +848,15 @@
     key = "number 5"
 
     ==> -1
     ```
     """
     
     if key in the_object:
-        for i, item in enumerate(the_object.keys()):
-            if key == item:
-                return i
+        return getObjectKeys(the_object).index(key)
     else:
         return -1
 
 def delete_key(the_object: dict, key: str): # {"n1":10, "n2":20, "n3":30}, key = "n1" ==> {"n2":20, "n3":30}
     """
     اللهم صل على سيدنا محمد ﷺ\n
     مثال
```

