# Comparing `tmp/vietqr-generator-0.0.4.tar.gz` & `tmp/vietqr-generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vietqr-generator-0.0.4.tar", last modified: Sat Mar 30 17:09:04 2024, max compression
+gzip compressed data, was "vietqr-generator-0.0.5.tar", last modified: Sat Apr 13 00:17:18 2024, max compression
```

## Comparing `vietqr-generator-0.0.4.tar` & `vietqr-generator-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 17:09:04.044130 vietqr-generator-0.0.4/
--rw-rw-rw-   0        0        0    35801 2024-03-30 16:10:28.000000 vietqr-generator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3735 2024-03-30 17:09:04.043129 vietqr-generator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2920 2024-03-30 16:10:28.000000 vietqr-generator-0.0.4/README.md
--rw-rw-rw-   0        0        0      908 2024-03-30 17:08:49.000000 vietqr-generator-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 17:09:04.044130 vietqr-generator-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 17:09:04.026129 vietqr-generator-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 17:09:04.028129 vietqr-generator-0.0.4/src/vietqr/
--rw-rw-rw-   0        0        0    15753 2024-03-30 17:07:15.000000 vietqr-generator-0.0.4/src/vietqr/VietQR.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:09:04.043129 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/
--rw-rw-rw-   0        0        0     3735 2024-03-30 17:09:04.000000 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-03-30 17:09:04.000000 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 17:09:04.000000 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-30 17:09:04.000000 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 17:09:04.000000 vietqr-generator-0.0.4/src/vietqr_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 00:17:18.849201 vietqr-generator-0.0.5/
+-rw-rw-rw-   0        0        0    35801 2024-03-30 16:10:28.000000 vietqr-generator-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3735 2024-04-13 00:17:18.848201 vietqr-generator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2920 2024-03-30 16:10:28.000000 vietqr-generator-0.0.5/README.md
+-rw-rw-rw-   0        0        0      910 2024-04-13 00:17:09.000000 vietqr-generator-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 00:17:18.849201 vietqr-generator-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 00:17:18.833152 vietqr-generator-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 00:17:18.835152 vietqr-generator-0.0.5/src/vietqr/
+-rw-rw-rw-   0        0        0    15753 2024-03-30 17:07:15.000000 vietqr-generator-0.0.5/src/vietqr/VietQR.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:17:18.847201 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/
+-rw-rw-rw-   0        0        0     3735 2024-04-13 00:17:18.000000 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-13 00:17:18.000000 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 00:17:18.000000 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 00:17:18.000000 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-13 00:17:18.000000 vietqr-generator-0.0.5/src/vietqr_generator.egg-info/top_level.txt
```

### Comparing `vietqr-generator-0.0.4/LICENSE` & `vietqr-generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vietqr-generator-0.0.4/PKG-INFO` & `vietqr-generator-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vietqr-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is the VietQR library which help to generate the VietQR Data String, which align with VietQR specifications. (The current VietQR Specification was announced by Napas on 21 Apr 2021)
 Author-email: Jean Nguyen <community@unicube.me>
 Project-URL: Homepage, https://github.com/unicubevn/vietqr
 Project-URL: Bug Tracker, https://github.com/unicubevn/vietqr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: qrcode[pil]
 
 # VietQR Generation Library
 
 This is a VietQR generation library.
```

### Comparing `vietqr-generator-0.0.4/README.md` & `vietqr-generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vietqr-generator-0.0.4/pyproject.toml` & `vietqr-generator-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=40.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vietqr-generator"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Jean Nguyen", email="community@unicube.me" },
 ]
 description = """
     This is the VietQR library which help to generate the VietQR Data String, which align with VietQR specifications. (The current VietQR Specification was announced by Napas on 21 Apr 2021)
 """
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 dependencies = [
   "qrcode[pil]",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `vietqr-generator-0.0.4/src/vietqr/VietQR.py` & `vietqr-generator-0.0.5/src/vietqr/VietQR.py`

 * *Files identical despite different names*

### Comparing `vietqr-generator-0.0.4/src/vietqr_generator.egg-info/PKG-INFO` & `vietqr-generator-0.0.5/src/vietqr_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: vietqr-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is the VietQR library which help to generate the VietQR Data String, which align with VietQR specifications. (The current VietQR Specification was announced by Napas on 21 Apr 2021)
 Author-email: Jean Nguyen <community@unicube.me>
 Project-URL: Homepage, https://github.com/unicubevn/vietqr
 Project-URL: Bug Tracker, https://github.com/unicubevn/vietqr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: qrcode[pil]
 
 # VietQR Generation Library
 
 This is a VietQR generation library.
```

