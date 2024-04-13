# Comparing `tmp/noteshrunk-1.1.1.tar.gz` & `tmp/noteshrunk-1.2.0.tar.gz`

## Comparing `noteshrunk-1.1.1.tar` & `noteshrunk-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0    23123 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/src/noteshrunk.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/LICENSE
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    45710 2020-02-02 00:00:00.000000 noteshrunk-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0    23956 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/src/noteshrunk.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    45710 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/PKG-INFO
```

### Comparing `noteshrunk-1.1.1/src/noteshrunk.py` & `noteshrunk-1.2.0/src/noteshrunk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 
 import argparse
-import multiprocessing
+from concurrent.futures import ThreadPoolExecutor
 import os
 from pathlib import Path
 import random
 import re
 import string
 import subprocess
 import tempfile
@@ -195,35 +195,39 @@
         percentage (float): Percentage of pixels to sample
 
     Returns:
         np.array: The sampled pixels.
     """
     total_pixels = image.shape[0] * image.shape[1]
     sample_size = int(total_pixels * (percentage / 100))
-    np.random.seed(0)
-    indices = np.random.choice(total_pixels, size=sample_size, replace=False)
+    rng = np.random.default_rng(0)
+    indices = rng.choice(total_pixels, size=sample_size, replace=False)
     return image.reshape((-1, 3))[indices]
 
 
-def perform_kmeans(image, n_clusters):
+def perform_kmeans(image, n_clusters, args):
     """
     Performs k-means clustering on the image and return the cluster centers and the model.
 
     Args:
         image (np.array): The image to perform k-means clustering on.
         n_clusters (int): The number of clusters.
 
     Returns:
         tuple: The cluster centers and the fitted KMeans model.
     """
     flattened_image = image.reshape((-1, 3))
     kmeans = KMeans(
+        init = 'k-means++',
+        n_init=1,
         n_clusters=n_clusters,
-        n_init='auto',
-        random_state=0).fit(flattened_image)
+        copy_x = False,
+        random_state=np.random.RandomState(0),
+        verbose = args.verbose
+        ).fit(flattened_image)
     return kmeans.cluster_centers_, kmeans
 
 
 def pack_rgb(rgb):
     """
     Pack a 24-bit RGB triple into a single integer.
 
@@ -324,15 +328,15 @@
         sampled_pixels,
         background_color=background_color,
         threshold_saturation=args.threshold_saturation,
         threshold_value=args.threshold_value)
     foreground_pixels = sampled_pixels[foreground_mask]
 
     kmeans_colors, kmeans_model = perform_kmeans(
-        foreground_pixels, args.n_colors - 1)
+        foreground_pixels, args.n_colors - 1, args)
 
     if args.white_background:
         color_palette = np.vstack(
             [[255, 255, 255], kmeans_colors]).round(0).astype('uint8')
     else:
         color_palette = np.vstack(
             [background_color, kmeans_colors]).round(0).astype('uint8')
@@ -560,15 +564,15 @@
         filename (str): The filename to use for the output file.
     """
     file_path = Path(filename)
 
     if file_path.exists():
 
         while True:
-            choice = input("File exists. Overwrite? (y: yes; n: no and quit; r: rename) [ynR]: ").strip().lower()
+            choice = input('File "{}" exists. Overwrite? (y: yes; n: no and quit; r: rename) [ynR]: '.format(file_path)).strip().lower()
 
             if choice == 'y':
                 print(f"Overwriting the file: {filename}")
                 break
 
             elif choice == 'n':
                 print("Not overwriting the file. Exiting program.")
@@ -603,14 +607,15 @@
 
 
 def verbose_print(args, *message, conditions=[]):
     """
     Prints a <message> if all given <conditions> are True.
 
     Args:
+        args (argparse.Namespace): The command line arguments
         message (str): The message to be printed.
         conditions (list of bool): A list of boolean constraints that must all be True for the message to be printed.
 
     Returns:
         None
     """
     if args.verbose and all(conditions):
@@ -683,51 +688,70 @@
         color_palette, kmeans_model = create_palette(image, args)
 
     image = apply_color_palette(image, color_palette, kmeans_model, args)
 
     save_as_pdf(image, output_filename, args)
 
 
+def check_file_existence(files):
+    """
+    Checks if a file / a list of files exist and raises an error if any are missing.
+
+    Args:
+        files (str / pathlib.Path or list of str / pathlib.Path): Files to be tested for existence.
+
+    Raises:
+        FileNotFoundError: If at least one file does not exist.
+    """
+    # Ensure <files> is a list.
+    # In case <files> is neither str, nor Path, nor list, the error is raised by pathlib.Path below
+    if not isinstance(files, list):
+        files = [files]
+
+    for file in files:
+        path = Path(file)
+        if not path.exists():
+            raise FileNotFoundError(f"File not found: {file}")
+
+
 def main():
     """
     The main function of the program.
     """
     args = parse_args()
     file_paths = sort_filenames(args.files)
+    check_file_existence(file_paths)
 
     # Create a temporary folder at the output file location for storing intermediate PDFs.
     # This way the intermediate files are automatically deleted upon program exit.
     # Each image is converted to a single-page PDF before concatenation
     # afterwards, which reduces the memory footprint.
-    with tempfile.TemporaryDirectory(dir=args.output.parent, prefix='tmp_pdfs-', delete=(not args.keep_intermediate)) as temp_dir:
+    with tempfile.TemporaryDirectory(dir=os.getcwd(), prefix='tmp_pdfs-', delete=(not args.keep_intermediate)) as temp_dir:
 
         intermediate_pdf_paths = []
 
         if args.global_palette:
             color_palette, kmeans_model = create_palette(file_paths, args, use_global_palette=True)
 
-        with multiprocessing.Pool(args.jobs) as pool:
+        with ThreadPoolExecutor(max_workers=args.jobs) as executor:
 
             for idx, file in enumerate(file_paths):
 
                 output_filename = args.output.parent / temp_dir / Path(file.name).with_suffix('.pdf')
 
                 # E.g. the same input file multiple times
                 if output_filename in intermediate_pdf_paths or output_filename.exists():
                     output_filename = rename_with_random_string(output_filename)
 
-                # Apply asynchronously for potentially faster execution since the order is
-                # preserved via intermediate_pdf_paths
-                pool.apply_async(process_image, (file, output_filename, idx, args,
-                                 (color_palette, kmeans_model) if args.global_palette else None))
+                executor.submit(process_image, file=file, output_filename=output_filename, idx=idx, args=args,
+                                 global_palette=(color_palette, kmeans_model) if args.global_palette else None)
 
                 intermediate_pdf_paths.append(output_filename)
 
-            pool.close()
-            pool.join()
+            executor.shutdown(wait=True)
 
         verbose_print(
             args,
             'Skipping the deletion of intermediate PDFs (folder {}).'.format(temp_dir),
             conditions=[args.keep_intermediate]
         )
```

### Comparing `noteshrunk-1.1.1/.gitignore` & `noteshrunk-1.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,20 @@
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
 
-# misc
+# Vim
 *.un~
+*.swp
+
+# misc
+output.pdf
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
 #   intended to run in multiple environments; otherwise, check them in:
 # .python-version
 
 # pipenv
```

### Comparing `noteshrunk-1.1.1/LICENSE` & `noteshrunk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.1.1/README.md` & `noteshrunk-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.1.1/pyproject.toml` & `noteshrunk-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.1.1"
+version = "1.2.0"
 description = "Document Color Palette Compression"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
```

### Comparing `noteshrunk-1.1.1/PKG-INFO` & `noteshrunk-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.1.1
+Version: 1.2.0
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

