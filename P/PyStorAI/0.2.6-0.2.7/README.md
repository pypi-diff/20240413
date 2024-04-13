# Comparing `tmp/PyStorAI-0.2.6.tar.gz` & `tmp/PyStorAI-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorAI-0.2.6.tar", last modified: Fri Apr 12 18:57:03 2024, max compression
+gzip compressed data, was "PyStorAI-0.2.7.tar", last modified: Fri Apr 12 21:02:42 2024, max compression
```

## Comparing `PyStorAI-0.2.6.tar` & `PyStorAI-0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.813655 PyStorAI-0.2.6/PyStorAI/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 18:54:20.000000 PyStorAI-0.2.6/PyStorAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6103 2024-04-12 18:54:59.000000 PyStorAI-0.2.6/PyStorAI/storyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.814655 PyStorAI-0.2.6/PyStorAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      933 2024-04-12 18:53:55.000000 PyStorAI-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:02:42.003987 PyStorAI-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 21:02:42.003987 PyStorAI-0.2.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:02:42.002987 PyStorAI-0.2.7/PyStorAI/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 20:59:47.000000 PyStorAI-0.2.7/PyStorAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2024-04-12 21:02:17.000000 PyStorAI-0.2.7/PyStorAI/storyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 21:02:42.003987 PyStorAI-0.2.7/PyStorAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 21:02:41.000000 PyStorAI-0.2.7/PyStorAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-12 21:02:41.000000 PyStorAI-0.2.7/PyStorAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 21:02:41.000000 PyStorAI-0.2.7/PyStorAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 21:02:41.000000 PyStorAI-0.2.7/PyStorAI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 21:02:42.003987 PyStorAI-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-12 21:01:41.000000 PyStorAI-0.2.7/setup.py
```

### Comparing `PyStorAI-0.2.6/PKG-INFO` & `PyStorAI-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.6
+Version: 0.2.7
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Your Name
 Author-email: your@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.6/PyStorAI/storyboard.py` & `PyStorAI-0.2.7/PyStorAI/storyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
                     f.write(response.content)
                     print(f"Image {i} download successful.")
 
                 # Rename file to remove "?raw=true"
                 os.rename(file_name, f"image{i}.png")
                 print(f"Image {i} filename changed.")
 
-                # Add indice to downloaded images
-                downloaded_images.add(i)
+                # Update download index
+                downloaded_images.add(i)
+                # Count images downloaded
                 num_images += 1
             else:
                 print(f"Failed to download image {i}. Status code: {response.status_code}")
     
     global image_files # debugging
     image_files = [f"image{index}.png" for index in indices]
 
@@ -142,26 +143,28 @@
 
             # Rename file to remove "?raw=true"
             os.rename(file_name, f"image{i}.png")
             print(f"Image {i} filename changed.")
 
             # Count images downloaded
             num_images +=1
-
         else:
             print(f"Failed to download image {i}. Status code: {response.status_code}")
             break  # Stop downloading
+
+
 
     # Read captions from file
     captions = []
     with open('captions.txt', 'r') as captions_file:
         captions = captions_file.read().splitlines()
 
     global image_files # debugging
     image_files = [f"image{i}.png" for i in range(1, num_images + 1)]
+
 
     # Determine display layout
     global num_cols # debugging
     global num_rows # debugging
     num_cols = min(num_images, 4)
     num_rows = -(-num_images // num_cols)
```

### Comparing `PyStorAI-0.2.6/PyStorAI.egg-info/PKG-INFO` & `PyStorAI-0.2.7/PyStorAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.6
+Version: 0.2.7
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Your Name
 Author-email: your@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.6/setup.py` & `PyStorAI-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyStorAI',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
     ],
     include_package_data=True,
     author='Your Name',
     author_email='your@email.com',
```

