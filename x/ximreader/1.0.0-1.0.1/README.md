# Comparing `tmp/ximreader-1.0.0.tar.gz` & `tmp/ximreader-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ximreader-1.0.0.tar", last modified: Wed Apr 10 23:32:33 2024, max compression
+gzip compressed data, was "ximreader-1.0.1.tar", last modified: Sat Apr 13 21:14:26 2024, max compression
```

## Comparing `ximreader-1.0.0.tar` & `ximreader-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-10 23:32:33.371056 ximreader-1.0.0/
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1301 2024-04-09 23:49:10.000000 ximreader-1.0.0/LICENSE
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)       25 2024-04-10 00:38:13.000000 ximreader-1.0.0/MANIFEST.in
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1046 2024-04-10 23:32:33.371056 ximreader-1.0.0/PKG-INFO
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)      549 2024-04-10 20:47:31.000000 ximreader-1.0.0/README.md
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)      622 2024-04-10 00:33:11.000000 ximreader-1.0.0/pyproject.toml
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)       15 2024-04-09 23:49:30.000000 ximreader-1.0.0/requirements.txt
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)       38 2024-04-10 23:32:33.371056 ximreader-1.0.0/setup.cfg
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1840 2024-04-10 20:39:02.000000 ximreader-1.0.0/setup.py
-drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-10 23:32:33.367723 ximreader-1.0.0/src/
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)     4034 2024-04-09 23:49:10.000000 ximreader-1.0.0/src/ximreader.cpp
-drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-10 23:32:33.367723 ximreader-1.0.0/ximreader/
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)       33 2024-04-09 23:49:10.000000 ximreader-1.0.0/ximreader/__init__.py
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)      444 2024-04-10 20:46:53.000000 ximreader-1.0.0/ximreader/ximReader.py
-drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-10 23:32:33.371056 ximreader-1.0.0/ximreader.egg-info/
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1046 2024-04-10 23:32:33.000000 ximreader-1.0.0/ximreader.egg-info/PKG-INFO
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)      297 2024-04-10 23:32:33.000000 ximreader-1.0.0/ximreader.egg-info/SOURCES.txt
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)        1 2024-04-10 23:32:33.000000 ximreader-1.0.0/ximreader.egg-info/dependency_links.txt
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)        6 2024-04-10 23:32:33.000000 ximreader-1.0.0/ximreader.egg-info/requires.txt
--rw-r--r--   0 dkumar    (1000) dkumar    (1000)       10 2024-04-10 23:32:33.000000 ximreader-1.0.0/ximreader.egg-info/top_level.txt
+drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-13 21:14:26.661187 ximreader-1.0.1/
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1301 2024-04-09 23:49:10.000000 ximreader-1.0.1/LICENSE
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)       25 2024-04-10 00:38:13.000000 ximreader-1.0.1/MANIFEST.in
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1125 2024-04-13 21:14:26.661187 ximreader-1.0.1/PKG-INFO
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)      628 2024-04-11 00:37:07.000000 ximreader-1.0.1/README.md
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)      622 2024-04-13 21:14:21.000000 ximreader-1.0.1/pyproject.toml
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)       15 2024-04-09 23:49:30.000000 ximreader-1.0.1/requirements.txt
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)       38 2024-04-13 21:14:26.661187 ximreader-1.0.1/setup.cfg
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1840 2024-04-13 21:13:23.000000 ximreader-1.0.1/setup.py
+drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-13 21:14:26.661187 ximreader-1.0.1/src/
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)     4034 2024-04-09 23:49:10.000000 ximreader-1.0.1/src/ximreader.cpp
+drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-13 21:14:26.661187 ximreader-1.0.1/ximreader/
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)       33 2024-04-09 23:49:10.000000 ximreader-1.0.1/ximreader/__init__.py
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)      444 2024-04-13 21:09:50.000000 ximreader-1.0.1/ximreader/ximReader.py
+drwxr-xr-x   0 dkumar    (1000) dkumar    (1000)        0 2024-04-13 21:14:26.661187 ximreader-1.0.1/ximreader.egg-info/
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)     1125 2024-04-13 21:14:26.000000 ximreader-1.0.1/ximreader.egg-info/PKG-INFO
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)      297 2024-04-13 21:14:26.000000 ximreader-1.0.1/ximreader.egg-info/SOURCES.txt
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)        1 2024-04-13 21:14:26.000000 ximreader-1.0.1/ximreader.egg-info/dependency_links.txt
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)        6 2024-04-13 21:14:26.000000 ximreader-1.0.1/ximreader.egg-info/requires.txt
+-rw-r--r--   0 dkumar    (1000) dkumar    (1000)       10 2024-04-13 21:14:26.000000 ximreader-1.0.1/ximreader.egg-info/top_level.txt
```

### Comparing `ximreader-1.0.0/LICENSE` & `ximreader-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ximreader-1.0.0/PKG-INFO` & `ximreader-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: ximreader
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python extension for reading xim files
 Author: Dinesh Kumar
 Author-email: Dinesh Kumar <dkumar@lbl.gov>
 Project-URL: Homepage, https://github.com/aryabhatt/ximreader
 Project-URL: Issues, https://github.com/aryabhatt/ximreader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 ## ximReader Python package for loading xim files
 
-ximReader is an open-source tool for reading xim files as numpy arrays. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
+ximReader is an open-source tool for reading xim files as NumPy array. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
 
 ## Installation
 
-ximReader can installed via pip
+ximReader can be installed via pip
 
-`` pip install git+https://github.com/aryabhatt/ximreader.git ``
+    pip install git+https://github.com/aryabhatt/ximreader.git
 
-Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the installation.
+Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the source installation.
 
 
 ## Usage
 
     from ximreader import ximReader
-    image = ximReader(<full path to xim>)
+
+    def awesone_function(..., ximfilename, ...)
+        ...
+
+        image = ximReader(ximfilename)
+
+        ...
```

### Comparing `ximreader-1.0.0/README.md` & `ximreader-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 ## ximReader Python package for loading xim files
 
-ximReader is an open-source tool for reading xim files as numpy arrays. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
+ximReader is an open-source tool for reading xim files as NumPy array. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
 
 ## Installation
 
-ximReader can installed via pip
+ximReader can be installed via pip
 
-`` pip install git+https://github.com/aryabhatt/ximreader.git ``
+    pip install git+https://github.com/aryabhatt/ximreader.git
 
-Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the installation.
+Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the source installation.
 
 
 ## Usage
 
     from ximreader import ximReader
-    image = ximReader(<full path to xim>)
+
+    def awesone_function(..., ximfilename, ...)
+        ...
+
+        image = ximReader(ximfilename)
+
+        ...
```

### Comparing `ximreader-1.0.0/pyproject.toml` & `ximreader-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "pybind11"
     ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ximreader"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name="Dinesh Kumar", email="dkumar@lbl.gov"},
     ]
 description = "Python extension for reading xim files"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.8"
```

### Comparing `ximreader-1.0.0/setup.py` & `ximreader-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     include_dirs=[get_pybind11_headers()],
     extra_compile_args = ['-std=c++17']
 )
 extensions.append(ext)
 
 setup(
     name='ximreader',
-    version= "1.0.0",
+    version= "1.0.1",
     description="Python Extension for reading XIM files",
     long_description=readme,
     author="Dinesh Kumar",
     author_email="dkumar@lbl.gov",
     packages=[ "ximreader" ],
     install_requires=requirements,
     license="BSD (2-clause)",
```

### Comparing `ximreader-1.0.0/src/ximreader.cpp` & `ximreader-1.0.1/src/ximreader.cpp`

 * *Files identical despite different names*

### Comparing `ximreader-1.0.0/ximreader.egg-info/PKG-INFO` & `ximreader-1.0.1/ximreader.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: ximreader
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python extension for reading xim files
 Author: Dinesh Kumar
 Author-email: Dinesh Kumar <dkumar@lbl.gov>
 Project-URL: Homepage, https://github.com/aryabhatt/ximreader
 Project-URL: Issues, https://github.com/aryabhatt/ximreader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 ## ximReader Python package for loading xim files
 
-ximReader is an open-source tool for reading xim files as numpy arrays. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
+ximReader is an open-source tool for reading xim files as NumPy array. It is based on XimReader (https://bitbucket.org/dmoderesearchtools/ximreader/src/master/). 
 
 ## Installation
 
-ximReader can installed via pip
+ximReader can be installed via pip
 
-`` pip install git+https://github.com/aryabhatt/ximreader.git ``
+    pip install git+https://github.com/aryabhatt/ximreader.git
 
-Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the installation.
+Alternatively, it can be installed from the source. It is recommended that a virtual environment be used for the source installation.
 
 
 ## Usage
 
     from ximreader import ximReader
-    image = ximReader(<full path to xim>)
+
+    def awesone_function(..., ximfilename, ...)
+        ...
+
+        image = ximReader(ximfilename)
+
+        ...
```

