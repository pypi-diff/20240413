# Comparing `tmp/pypar-0.0.5.tar.gz` & `tmp/pypar-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypar-0.0.5.tar", last modified: Thu Oct 26 22:21:57 2023, max compression
+gzip compressed data, was "pypar-0.0.6.tar", last modified: Fri Apr 12 22:54:50 2024, max compression
```

## Comparing `pypar-0.0.5.tar` & `pypar-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-10-26 22:21:57.837190 pypar-0.0.5/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1069 2023-10-26 20:34:22.000000 pypar-0.0.5/LICENSE
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    13843 2023-10-26 22:21:57.837190 pypar-0.0.5/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    13450 2023-10-26 22:21:35.000000 pypar-0.0.5/README.md
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-10-26 22:21:57.833190 pypar-0.0.5/pypar/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      152 2023-10-26 22:21:35.000000 pypar-0.0.5/pypar/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    18613 2023-10-26 22:21:35.000000 pypar-0.0.5/pypar/alignment.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2620 2023-10-26 20:34:22.000000 pypar-0.0.5/pypar/compare.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1693 2023-10-26 22:21:35.000000 pypar-0.0.5/pypar/phoneme.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5861 2023-10-26 20:34:22.000000 pypar-0.0.5/pypar/textgrid.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4035 2023-10-26 22:21:35.000000 pypar-0.0.5/pypar/word.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-10-26 22:21:57.837190 pypar-0.0.5/pypar.egg-info/
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    13843 2023-10-26 22:21:57.000000 pypar-0.0.5/pypar.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      317 2023-10-26 22:21:57.000000 pypar-0.0.5/pypar.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-10-26 22:21:57.000000 pypar-0.0.5/pypar.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        6 2023-10-26 22:21:57.000000 pypar-0.0.5/pypar.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        6 2023-10-26 22:21:57.000000 pypar-0.0.5/pypar.egg-info/top_level.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-10-26 22:21:57.837190 pypar-0.0.5/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      620 2023-10-26 22:21:35.000000 pypar-0.0.5/setup.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-10-26 22:21:57.837190 pypar-0.0.5/test/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2506 2023-10-26 20:34:22.000000 pypar-0.0.5/test/test_alignment.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1456 2023-10-26 20:34:22.000000 pypar-0.0.5/test/test_compare.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 22:54:50.534443 pypar-0.0.6/
+-rw-rw-r--   0 max       (1000) max       (1000)     1069 2024-04-12 22:46:10.000000 pypar-0.0.6/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)    13843 2024-04-12 22:54:50.534443 pypar-0.0.6/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)    13450 2024-04-12 22:46:10.000000 pypar-0.0.6/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 22:54:50.534443 pypar-0.0.6/pypar/
+-rw-rw-r--   0 max       (1000) max       (1000)      152 2024-04-12 22:46:10.000000 pypar-0.0.6/pypar/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    18717 2024-04-12 22:52:59.000000 pypar-0.0.6/pypar/alignment.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2620 2024-04-12 22:46:10.000000 pypar-0.0.6/pypar/compare.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1693 2024-04-12 22:46:10.000000 pypar-0.0.6/pypar/phoneme.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5861 2024-04-12 22:46:10.000000 pypar-0.0.6/pypar/textgrid.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4035 2024-04-12 22:46:10.000000 pypar-0.0.6/pypar/word.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 22:54:50.534443 pypar-0.0.6/pypar.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    13843 2024-04-12 22:54:50.000000 pypar-0.0.6/pypar.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      317 2024-04-12 22:54:50.000000 pypar-0.0.6/pypar.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2024-04-12 22:54:50.000000 pypar-0.0.6/pypar.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        6 2024-04-12 22:54:50.000000 pypar-0.0.6/pypar.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        6 2024-04-12 22:54:50.000000 pypar-0.0.6/pypar.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2024-04-12 22:54:50.534443 pypar-0.0.6/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      620 2024-04-12 22:54:34.000000 pypar-0.0.6/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 22:54:50.534443 pypar-0.0.6/test/
+-rw-rw-r--   0 max       (1000) max       (1000)     2506 2024-04-12 22:46:10.000000 pypar-0.0.6/test/test_alignment.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1456 2024-04-12 22:46:10.000000 pypar-0.0.6/test/test_compare.py
```

### Comparing `pypar-0.0.5/LICENSE` & `pypar-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/PKG-INFO` & `pypar-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypar
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python phoneme alignment representation
 Home-page: https://github.com/maxrmorrison/pypar
 Author: Max Morrison
 Author-email: maxrmorrison@gmail.com
 License: MIT
 Keywords: align,duration,phoneme,speech
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypar-0.0.5/README.md` & `pypar-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/pypar/alignment.py` & `pypar-0.0.6/pypar/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,16 @@
     def save(self, filename: Union[str, bytes, os.PathLike]) -> None:
         """Save alignment to json
 
         Arguments
             filename
                 The location on disk to save the phoneme alignment json
         """
+        if os.path.dirname(filename):
+            os.makedirs(os.path.dirname(filename), exist_ok=True)
         if isinstance(filename, Path):
             filename = str(filename)
         extension = filename.split('.')[-1]
         if extension == 'json':
             self.save_json(filename)
         elif extension.lower() == 'textgrid':
             self.save_textgrid(filename)
```

### Comparing `pypar-0.0.5/pypar/compare.py` & `pypar-0.0.6/pypar/compare.py`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/pypar/phoneme.py` & `pypar-0.0.6/pypar/phoneme.py`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/pypar/textgrid.py` & `pypar-0.0.6/pypar/textgrid.py`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/pypar/word.py` & `pypar-0.0.6/pypar/word.py`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/pypar.egg-info/PKG-INFO` & `pypar-0.0.6/pypar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypar
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python phoneme alignment representation
 Home-page: https://github.com/maxrmorrison/pypar
 Author: Max Morrison
 Author-email: maxrmorrison@gmail.com
 License: MIT
 Keywords: align,duration,phoneme,speech
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pypar-0.0.5/setup.py` & `pypar-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Description
 with open('README.md') as file:
     long_description = file.read()
 
 
 setup(
     name='pypar',
-    version='0.0.5',
+    version='0.0.6',
     description='Python phoneme alignment representation',
     author='Max Morrison',
     author_email='maxrmorrison@gmail.com',
     url='https://github.com/maxrmorrison/pypar',
     install_requires=['numpy'],
     packages=['pypar'],
     long_description=long_description,
```

### Comparing `pypar-0.0.5/test/test_alignment.py` & `pypar-0.0.6/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `pypar-0.0.5/test/test_compare.py` & `pypar-0.0.6/test/test_compare.py`

 * *Files identical despite different names*

