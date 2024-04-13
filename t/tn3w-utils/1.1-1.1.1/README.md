# Comparing `tmp/tn3w_utils-1.1.tar.gz` & `tmp/tn3w_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tn3w_utils-1.1.tar", last modified: Fri Feb 16 14:13:21 2024, max compression
+gzip compressed data, was "tn3w_utils-1.1.1.tar", last modified: Sat Apr 13 13:41:20 2024, max compression
```

## Comparing `tn3w_utils-1.1.tar` & `tn3w_utils-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:13:21.698744 tn3w_utils-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-16 14:13:13.000000 tn3w_utils-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-02-16 14:13:21.698744 tn3w_utils-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-16 14:13:13.000000 tn3w_utils-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 14:13:21.698744 tn3w_utils-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-16 14:13:13.000000 tn3w_utils-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:13:21.694743 tn3w_utils-1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:13:21.694743 tn3w_utils-1.1/src/tn3w_utils/
--rw-r--r--   0 runner    (1001) docker     (127)   245600 2024-02-16 14:13:13.000000 tn3w_utils-1.1/src/tn3w_utils/Comic_Sans_MS.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   117072 2024-02-16 14:13:13.000000 tn3w_utils-1.1/src/tn3w_utils/Droid_Sans_Mono.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-02-16 14:13:13.000000 tn3w_utils-1.1/src/tn3w_utils/Helvetica.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    70479 2024-02-16 14:13:13.000000 tn3w_utils-1.1/src/tn3w_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115893 2024-02-16 14:13:13.000000 tn3w_utils-1.1/src/tn3w_utils/languages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:13:21.698744 tn3w_utils-1.1/src/tn3w_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-02-16 14:13:21.000000 tn3w_utils-1.1/src/tn3w_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-16 14:13:21.000000 tn3w_utils-1.1/src/tn3w_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 14:13:21.000000 tn3w_utils-1.1/src/tn3w_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-16 14:13:21.000000 tn3w_utils-1.1/src/tn3w_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-16 14:13:21.000000 tn3w_utils-1.1/src/tn3w_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:20.878221 tn3w_utils-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-13 13:41:20.874221 tn3w_utils-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:41:20.878221 tn3w_utils-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:20.870221 tn3w_utils-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:20.874221 tn3w_utils-1.1.1/src/tn3w_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)   245600 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/src/tn3w_utils/Comic_Sans_MS.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   117072 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/src/tn3w_utils/Droid_Sans_Mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/src/tn3w_utils/Helvetica.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    70479 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/src/tn3w_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115893 2024-04-13 13:41:12.000000 tn3w_utils-1.1.1/src/tn3w_utils/languages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:20.874221 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-13 13:41:20.000000 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-13 13:41:20.000000 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:41:20.000000 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 13:41:20.000000 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 13:41:20.000000 tn3w_utils-1.1.1/src/tn3w_utils.egg-info/top_level.txt
```

### Comparing `tn3w_utils-1.1/LICENSE` & `tn3w_utils-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/PKG-INFO` & `tn3w_utils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn3w_utils
-Version: 1.1
+Version: 1.1.1
 Summary: A consolidation of all tools created so far as a Python package
 Home-page: https://github.com/tn3w/tn3w_utils
 Author: TN3W
 Author-email: tn3wA8xxfuVMs2@proton.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: ipaddress
 Requires-Dist: requests
 Requires-Dist: googletrans==3.1.0a0
 Requires-Dist: bs4
-Requires-Dist: pillow>=10.2.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: python-magic
 Requires-Dist: distro
 Requires-Dist: captcha
 
 # TN3W_Utils
 A consolidation of all tools created so far as a Python package
```

### Comparing `tn3w_utils-1.1/README.md` & `tn3w_utils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/setup.py` & `tn3w_utils-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requirements = [str(requirement.requirement) for requirement in list(parse_requirements("requirements.txt", session=False))]
 
 with open('README.md', 'r', encoding='utf-8') as readable_file:
     long_description = readable_file.read()
 
 setup(
     name='tn3w_utils',
-    version='1.1',
+    version='1.1.1',
     description='A consolidation of all tools created so far as a Python package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TN3W',
     author_email='tn3wA8xxfuVMs2@proton.me',
     url='https://github.com/tn3w/tn3w_utils',
     packages=find_packages(where = 'src'),
```

### Comparing `tn3w_utils-1.1/src/tn3w_utils/Comic_Sans_MS.ttf` & `tn3w_utils-1.1.1/src/tn3w_utils/Comic_Sans_MS.ttf`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/src/tn3w_utils/Droid_Sans_Mono.ttf` & `tn3w_utils-1.1.1/src/tn3w_utils/Droid_Sans_Mono.ttf`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/src/tn3w_utils/Helvetica.ttf` & `tn3w_utils-1.1.1/src/tn3w_utils/Helvetica.ttf`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/src/tn3w_utils/__init__.py` & `tn3w_utils-1.1.1/src/tn3w_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/src/tn3w_utils/languages.json` & `tn3w_utils-1.1.1/src/tn3w_utils/languages.json`

 * *Files identical despite different names*

### Comparing `tn3w_utils-1.1/src/tn3w_utils.egg-info/PKG-INFO` & `tn3w_utils-1.1.1/src/tn3w_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn3w_utils
-Version: 1.1
+Version: 1.1.1
 Summary: A consolidation of all tools created so far as a Python package
 Home-page: https://github.com/tn3w/tn3w_utils
 Author: TN3W
 Author-email: tn3wA8xxfuVMs2@proton.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: ipaddress
 Requires-Dist: requests
 Requires-Dist: googletrans==3.1.0a0
 Requires-Dist: bs4
-Requires-Dist: pillow>=10.2.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: python-magic
 Requires-Dist: distro
 Requires-Dist: captcha
 
 # TN3W_Utils
 A consolidation of all tools created so far as a Python package
```

