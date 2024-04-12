# Comparing `tmp/facialfinder-0.0.2.tar.gz` & `tmp/facialfinder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facialfinder-0.0.2.tar", last modified: Fri Apr 12 20:06:28 2024, max compression
+gzip compressed data, was "facialfinder-0.0.3.tar", last modified: Fri Apr 12 22:06:34 2024, max compression
```

## Comparing `facialfinder-0.0.2.tar` & `facialfinder-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 20:06:28.406720 facialfinder-0.0.2/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-12 18:33:09.000000 facialfinder-0.0.2/LICENSE.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 20:06:28.406532 facialfinder-0.0.2/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3180 2024-04-12 18:48:05.000000 facialfinder-0.0.2/README.md
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 20:06:28.405541 facialfinder-0.0.2/facialfinder/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 18:59:26.000000 facialfinder-0.0.2/facialfinder/__init__.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       96 2024-04-12 18:58:20.000000 facialfinder-0.0.2/facialfinder/_path.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-12 20:04:58.000000 facialfinder-0.0.2/facialfinder/image.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-12 20:04:58.000000 facialfinder-0.0.2/facialfinder/video.py
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 20:06:28.406342 facialfinder-0.0.2/facialfinder.egg-info/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 20:06:28.000000 facialfinder-0.0.2/facialfinder.egg-info/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      300 2024-04-12 20:06:28.000000 facialfinder-0.0.2/facialfinder.egg-info/SOURCES.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 20:06:28.000000 facialfinder-0.0.2/facialfinder.egg-info/dependency_links.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-12 20:06:28.000000 facialfinder-0.0.2/facialfinder.egg-info/requires.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-12 20:06:28.000000 facialfinder-0.0.2/facialfinder.egg-info/top_level.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-12 20:06:28.406754 facialfinder-0.0.2/setup.cfg
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      683 2024-04-12 20:05:50.000000 facialfinder-0.0.2/setup.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:06:34.202828 facialfinder-0.0.3/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-12 18:33:09.000000 facialfinder-0.0.3/LICENSE.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 22:06:34.202629 facialfinder-0.0.3/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3180 2024-04-12 18:48:05.000000 facialfinder-0.0.3/README.md
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:06:34.201678 facialfinder-0.0.3/facialfinder/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 18:59:26.000000 facialfinder-0.0.3/facialfinder/__init__.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      129 2024-04-12 22:06:08.000000 facialfinder-0.0.3/facialfinder/_path.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:06:34.202242 facialfinder-0.0.3/facialfinder/datasets/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:05:38.000000 facialfinder-0.0.3/facialfinder/datasets/__init__.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-12 20:04:58.000000 facialfinder-0.0.3/facialfinder/image.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-12 20:04:58.000000 facialfinder-0.0.3/facialfinder/video.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:06:34.202395 facialfinder-0.0.3/facialfinder.egg-info/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 22:06:34.000000 facialfinder-0.0.3/facialfinder.egg-info/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      334 2024-04-12 22:06:34.000000 facialfinder-0.0.3/facialfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 22:06:34.000000 facialfinder-0.0.3/facialfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-12 22:06:34.000000 facialfinder-0.0.3/facialfinder.egg-info/requires.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-12 22:06:34.000000 facialfinder-0.0.3/facialfinder.egg-info/top_level.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-12 22:06:34.202880 facialfinder-0.0.3/setup.cfg
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      683 2024-04-12 22:06:23.000000 facialfinder-0.0.3/setup.py
```

### Comparing `facialfinder-0.0.2/LICENSE.txt` & `facialfinder-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.2/PKG-INFO` & `facialfinder-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
```

### Comparing `facialfinder-0.0.2/README.md` & `facialfinder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.2/facialfinder/image.py` & `facialfinder-0.0.3/facialfinder/image.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.2/facialfinder/video.py` & `facialfinder-0.0.3/facialfinder/video.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.2/facialfinder.egg-info/PKG-INFO` & `facialfinder-0.0.3/facialfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
```

### Comparing `facialfinder-0.0.2/setup.py` & `facialfinder-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 core_dir = Path(__file__).parent
 
 long_description = (core_dir / "README.md").read_text()
 
 setup(
     name="facialfinder",
-    version="0.0.2",
+    version="0.0.3",
     url="https://github.com/Anonimous05/FacialFinder",
     author="Airas Tolonov",
     author_email="airastolonov05@gmail.com",
     description="Simple tool for Face Detection on Image or Video, realtime detection support.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

