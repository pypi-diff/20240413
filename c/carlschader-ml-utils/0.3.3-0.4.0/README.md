# Comparing `tmp/carlschader_ml_utils-0.3.3.tar.gz` & `tmp/carlschader_ml_utils-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carlschader_ml_utils-0.3.3.tar", last modified: Thu Apr 11 16:29:17 2024, max compression
+gzip compressed data, was "carlschader_ml_utils-0.4.tar", last modified: Fri Apr 12 21:34:45 2024, max compression
```

## Comparing `carlschader_ml_utils-0.3.3.tar` & `carlschader_ml_utils-0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:29:17.970713 carlschader_ml_utils-0.3.3/
--rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.3.3/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-11 16:29:17.970713 carlschader_ml_utils-0.3.3/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.3.3/README.md
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:29:17.970713 carlschader_ml_utils-0.3.3/carlschader_ml_utils/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4621 2024-04-11 16:28:23.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils/image_utils.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1764 2024-04-02 16:02:55.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils/train.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-11 16:29:17.970713 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-11 16:29:17.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      350 2024-04-11 16:29:17.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-11 16:29:17.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-11 16:29:17.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-04-11 16:29:17.000000 carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-04-11 16:29:01.000000 carlschader_ml_utils-0.3.3/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-11 16:29:17.970713 carlschader_ml_utils-0.3.3/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 21:34:45.263493 carlschader_ml_utils-0.4/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-03-25 18:47:30.000000 carlschader_ml_utils-0.4/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-12 21:34:45.263493 carlschader_ml_utils-0.4/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 18:48:53.000000 carlschader_ml_utils-0.4/README.md
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 21:34:45.263493 carlschader_ml_utils-0.4/carlschader_ml_utils/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-03-25 20:37:15.000000 carlschader_ml_utils-0.4/carlschader_ml_utils/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4944 2024-04-12 21:33:47.000000 carlschader_ml_utils-0.4/carlschader_ml_utils/image_utils.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-12 21:34:45.263493 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      605 2024-04-12 21:34:45.000000 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      320 2024-04-12 21:34:45.000000 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-12 21:34:45.000000 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-12 21:34:45.000000 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       26 2024-04-12 21:34:45.000000 carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      872 2024-04-12 21:34:00.000000 carlschader_ml_utils-0.4/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-12 21:34:45.263493 carlschader_ml_utils-0.4/setup.cfg
```

### Comparing `carlschader_ml_utils-0.3.3/LICENSE` & `carlschader_ml_utils-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `carlschader_ml_utils-0.3.3/PKG-INFO` & `carlschader_ml_utils-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.3.3
+Version: 0.4.0
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.3.3/carlschader_ml_utils/image_utils.py` & `carlschader_ml_utils-0.4/carlschader_ml_utils/image_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,19 @@
                         current_count = 0
                         current_label = label
                     class_average += emb
                 else:
                     if label != current_label:
                         class_name = dataset.classes[current_label]
                         class_stack = torch.stack(class_stack, dim=0)
-                        torch.save(class_stack, os.path.join(save_dir, f'{class_name}.pth'))
+                        if not os.path.exists(os.path.join(save_dir, class_name)):
+                            os.mkdir(os.path.join(save_dir, class_name))
+                        for k in range(class_stack.shape[0]):
+                            torch.save(class_stack[k], os.path.join(save_dir, class_name, f'{k}.pth'))
+                        # torch.save(class_stack, os.path.join(save_dir, f'{class_name}.pth'))
                         class_stack = []
                         current_count = 0
                         current_label = label
                     class_stack.append(emb)
 
                 current_count += 1
```

### Comparing `carlschader_ml_utils-0.3.3/carlschader_ml_utils.egg-info/PKG-INFO` & `carlschader_ml_utils-0.4/carlschader_ml_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carlschader_ml_utils
-Version: 0.3.3
+Version: 0.4.0
 Summary: A collection of utilities for machine learning projects
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ml-utils
 Project-URL: Issues, https://github.com/carlschader/ml-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `carlschader_ml_utils-0.3.3/pyproject.toml` & `carlschader_ml_utils-0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "carlschader_ml_utils"
-version = "0.3.3"
+version = "0.4.0"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "A collection of utilities for machine learning projects"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

