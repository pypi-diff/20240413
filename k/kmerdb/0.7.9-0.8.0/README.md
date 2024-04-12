# Comparing `tmp/kmerdb-0.7.9.tar.gz` & `tmp/kmerdb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerdb-0.7.9.tar", last modified: Tue Apr  9 19:42:40 2024, max compression
+gzip compressed data, was "kmerdb-0.8.0.tar", last modified: Fri Apr 12 23:25:40 2024, max compression
```

## Comparing `kmerdb-0.7.9.tar` & `kmerdb-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.7.9/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.7.9/MANIFEST.in
--rw-r--r--   0 matt      (1000) matt      (1000)    26600 2024-04-09 19:42:40.389017 kmerdb-0.7.9/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    10606 2024-04-06 05:32:04.000000 kmerdb-0.7.9/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/kmerdb/
--rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.7.9/kmerdb/CITATION.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)    95832 2024-04-09 19:12:35.000000 kmerdb-0.7.9/kmerdb/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.7.9/kmerdb/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    27137 2024-04-09 19:14:01.000000 kmerdb-0.7.9/kmerdb/appmap.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.7.9/kmerdb/banners.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    15992 2024-04-09 17:09:24.000000 kmerdb-0.7.9/kmerdb/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)  1166079 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb/distance.c
--rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.7.9/kmerdb/distance.pyx
--rw-rw-r--   0 matt      (1000) matt      (1000)    42776 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/fileutil.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    51253 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/graph.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.7.9/kmerdb/index.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22573 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/kmer.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.7.9/kmerdb/legacy.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    19206 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/parse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.7.9/kmerdb/probability.py
--rw-r-----   0 matt      (1000) matt      (1000)     5235 2022-05-01 17:20:48.000000 kmerdb-0.7.9/kmerdb/python_distances.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/kmerdb.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    26600 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      607 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      287 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4592 2024-04-09 19:42:27.000000 kmerdb-0.7.9/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-04-09 19:42:40.389017 kmerdb-0.7.9/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-04-09 17:08:02.000000 kmerdb-0.7.9/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/test/
--rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.7.9/test/test_kmer.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.0/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.0/MANIFEST.in
+-rw-r--r--   0 matt      (1000) matt      (1000)    26629 2024-04-12 23:25:40.515748 kmerdb-0.8.0/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    10606 2024-04-06 05:32:04.000000 kmerdb-0.8.0/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/kmerdb/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.0/kmerdb/CITATION.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)   106771 2024-04-12 23:19:22.000000 kmerdb-0.8.0/kmerdb/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.0/kmerdb/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    33281 2024-04-12 23:22:03.000000 kmerdb-0.8.0/kmerdb/appmap.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.0/kmerdb/banners.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13805 2024-04-12 23:22:17.000000 kmerdb-0.8.0/kmerdb/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)  1165266 2024-04-12 23:21:13.000000 kmerdb-0.8.0/kmerdb/distance.c
+-rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.0/kmerdb/distance.pyx
+-rw-rw-r--   0 matt      (1000) matt      (1000)    39346 2024-04-12 21:59:34.000000 kmerdb-0.8.0/kmerdb/fileutil.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    52230 2024-04-11 13:34:16.000000 kmerdb-0.8.0/kmerdb/graph.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.0/kmerdb/index.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-11 15:45:27.000000 kmerdb-0.8.0/kmerdb/kmer.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.0/kmerdb/legacy.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-12 23:09:24.000000 kmerdb-0.8.0/kmerdb/logger.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    19476 2024-04-12 01:25:50.000000 kmerdb-0.8.0/kmerdb/parse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.0/kmerdb/probability.py
+-rw-r-----   0 matt      (1000) matt      (1000)     5632 2024-04-11 00:22:28.000000 kmerdb-0.8.0/kmerdb/python_distances.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.0/kmerdb/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/kmerdb.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    26629 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4615 2024-04-12 23:16:02.000000 kmerdb-0.8.0/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-04-12 23:25:40.515748 kmerdb-0.8.0/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-04-12 23:15:53.000000 kmerdb-0.8.0/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/test/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.0/test/test_kmer.py
```

### Comparing `kmerdb-0.7.9/LICENSE.txt` & `kmerdb-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/PKG-INFO` & `kmerdb-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.7.9
+Version: 0.8.0
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
 Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
@@ -252,14 +252,15 @@
 Requires-Dist: jsonschema>=4.17.3
 Requires-Dist: psutil>=4.2.0
 Requires-Dist: Cython>=3.0.8
 Requires-Dist: biopython>=1.81
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: pandas>=2.2.2
 Requires-Dist: setuptools>=69.2.0
 Provides-Extra: dev
 Requires-Dist: auditwheel>=5.1.2; extra == "dev"
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: coverage>=4.5.4; extra == "dev"
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
```

### Comparing `kmerdb-0.7.9/README.md` & `kmerdb-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/__init__.py` & `kmerdb-0.8.0/kmerdb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,26 +20,49 @@
 import logging
 import argparse
 import os
 import sys
 import yaml
 import json
 import time
+import signal
+
+
+import pdb
+
 from multiprocessing import cpu_count
+
 from collections import OrderedDict
 
 
 from Bio import bgzf
 
 #import concurrent.futures
 
+from kmerdb import logger as kdbLogger
+
 global logger
 logger = None
 
 
+global step
+step = 0
+
+global feature
+feature = 0
+
+global exit_code
+exit_code = -1
+
+
+global exit_summary
+exit_summary = None
+
+
+
 def print_argv():
     argv = sys.argv
     sys.stderr.write(" ".join(argv[0:4]) + " ...\n")
 
 def citation():
 
     MODULE_ROOT = os.path.dirname(__file__)
@@ -168,15 +191,15 @@
         #kmerdb_appmap.print_shuf_header()
         raise ValueError("Unsupported method")
     elif arguments.method == "matrix":
         kmerdb_appmap.print_matrix_header()
     elif arguments.method == "distance":
         kmerdb_appmap.print_distance_header()
 
-
+    sys.stderr.write("\n\nUse --help for expanded usage\n")
 
 def distances(arguments):
     """
     An end-user function to provide CLI access to certain distances
     """
     from multiprocessing import Pool
     import multiprocessing as mp
@@ -185,285 +208,364 @@
     import numpy as np
     from scipy.spatial.distance import pdist, squareform
 
 
     from kmerdb import fileutil, config, util, distances
 
 
+
+
+
+    global feature
+    global step
+
+
+    
+
     has_cython = False
     try:
 
 
         from kmerdb.distance import pearson_correlation
         from kmerdb import python_distances as distance
-        logger.info("Correctly importing distance module")
+        
+        logger.log_it("Importing distance module...", "INFO")
         has_cython = True
     except ImportError as e:
-        logger.error(e)
-        logger.error("Could not import Cython distance submodule")
+        logger.log_it(e.__str__(), "ERROR")
+        logger.log_it("Could not import Cython distance submodule", "ERROR")
         raise RuntimeError("Cannot import pyx library")
 
     n = len(arguments.input)
 
     if len(arguments.input) > 1:
+
+        feature = 1
+        step = 1
+
+        
         file_reader = fileutil.FileReader()
         files = list(map(lambda f: fileutil.open(f, 'r', slurp=False), arguments.input))
         
-        logger.debug("Files: {0}".format(files))
+        logger.log_it("Files: {0}".format(files), "DEBUG")
+
+        
         if not all(os.path.splitext(kdb)[-1] == ".kdb" for kdb in arguments.input):
             raise IOError("One or more parseable .kdb filepaths did not end in '.kdb'")
         dtypes = [x.metadata["kmer_ids_dtype"] for x in files]
         suggested_dtype = dtypes[0]
 
-        logger.error(dtypes)
-        logger.error("Suggested dtype: {0}".format(suggested_dtype))
 
-        logger.info("\n\n\n\n{0}\n\n\n\n".format(suggested_dtype))
+        logger.log_it(", ".join(dtypes), "ERROR")
+        logger.log_it("Suggested dtype: {0}".format(suggested_dtype), "ERROR")
+
+        logger.log_it("\n\n\n\n{0}\n\n\n\n".format(suggested_dtype), "INFO")
+
         
         ks = [kdbrdr.k for kdbrdr in files]
         suggested_k = ks[0]
         if not all(kdbrdr.k == suggested_k for kdbrdr in files):
-            logger.error("Files: {0}".format(files))
-            logger.error("Choices of k: {0}".format(ks))
-            logger.error("By default the inferred value of k is used when k is not specified at the command line, which was {0}".format(suggested_k))
+            logger.log_it("Files: {0}".format(files), "ERROR")
+
+            logger.log_it("Choices of k: {0}".format(ks), "ERROR")
+            logger.log_it("By default the inferred value of k is used when k is not specified at the command line, which was {0}".format(suggested_k), "ERROR")
+
+            
             raise TypeError("One or more files did not have k set to be equal to {0}".format(arguments.k))
-        logger.debug("Files: {0}".format(files))
+
+
+        
+        logger.log_it("Files: {0}".format(files), "DEBUG")
+
         
         if not all(kdbrdr.dtype == suggested_dtype for kdbrdr in files):
             raise TypeError("One or more files did not have dtype = {0}".format(suggested_dtype))
         if arguments.parallel > 1:
             with Pool(processes=arguments.parallel) as pool:
                 files = pool.map(file_reader.load_file, arguments.input)
         else:
             files = list(map(lambda f: fileutil.open(f, 'r', slurp=True), arguments.input))
 
 
         data = [kdbrdr.slurp() for kdbrdr in files]
-        logger.info(data)
-        logger.error("Suggested dtype {0}".format(suggested_dtype))
-        logger.error(data)
-        pure_data = np.array(data, dtype=suggested_dtype)
-        profiles = np.transpose(pure_data)
+
+
+
+        
+        logger.log_it("Suggested dtype {0}".format(suggested_dtype), "ERROR")
+        
+        profiles = np.array(data, dtype=suggested_dtype)
+
+        #profiles = np.transpose(profiles)
 
         # The following does *not* transpose a matrix defined as n x N=4**k
         # n is the number of independent files/samples, (fasta/fastq=>kdb) being assessed
         # N=4**k is the dimensionality of the vector, sparse or not, that makes up the perceived profile, the descriptors is the column dimension.
         # The names for the columns are taken as the basenamed filepath, with all extensions (substrings beginning with '.') stripped.
 
         if arguments.column_names is None:
             columns = list(map(lambda kdbrdr: os.path.basename(kdbrdr._filepath).split(".")[0], files))
         else:
             with open(arguments.column_names, 'r') as column_names:
                 columns = [line.rstrip() for line in column_names]
         if len(columns) != len(files):
             raise RuntimeError("Number of column names {0} does not match number of input files {1}...".format(len(columns, len(files))))
-        logger.debug("Shape: {0}".format(profiles.shape))
-        logger.info("Converting arrays of k-mer counts into a pandas DataFrame...")
+
+        
+        logger.log_it("Shape: {0}".format(profiles.shape), "DEBUG")
+        logger.log_it("Converting arrays of k-mer counts into a pandas DataFrame...", "INFO")
+        
         #columns = list(df.columns) # I hate this language, it's hateful.
         n = len(columns)
     elif len(arguments.input) == 1 and (arguments.input[0] == "STDIN" or arguments.input[0] == "/dev/stdin"):
-        logger.info("Reading input as tsv/csv from STDIN")
+
+        feature = 2
+        step = 2
+
+
+        
+        logger.log_it("Reading input as tsv/csv from STDIN", "INFO")
         try:
             df = pd.read_csv(sys.stdin, sep=arguments.delimiter)
         except pd.errors.EmptyDataError as e:
-            logger.error(e)
-            logger.error("Pandas error on DataFrame reading. Perhaps a null dataset being read?")
-            sys.exit(1)
-        profiles = np.transpose(np.array(df))
+            logger.log_it(e.__str__(), "ERROR")
+            logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
+            
+            raise e
+        profiles = np.array(df)
+        #profiles = np.transpose(np.array(df))
         columns = list(df.columns)
         assert profiles.shape[0] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
         n = len(columns)
 
     elif len(arguments.input) == 1 and (os.path.splitext(arguments.input[0])[-1] == ".tsv" or os.path.splitext(arguments.input[0])[-1] == ".csv"):
+
+        feature = 2
+        step = 2
+        
         try:
             df = pd.read_csv(arguments.input[0], sep=arguments.delimiter)
         except pd.errors.EmptyDataError as e:
-            logger.error(e)
-            logger.error("Pandas error on DataFrame reading. Perhaps a null dataset being read?")
-            sys.exit(1)
-        profiles = np.transpose(np.array(df))
+            logger.log_it(e, "ERROR")
+            logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
+            raise e
+        #profiles = np.transpose(np.array(df))
+        profiles = np.array(df)
         columns = list(df.columns) # I'm sorry I ever made this line. Please forgive me.
         # This is just gratuitous code and language. I'm really really not sure what I want to express here.
-        assert profiles.shape[0] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
+        #assert profiles.shape[0] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
         n = len(columns)
     elif len(arguments.input) == 1 and os.path.splitext(arguments.input[0])[-1] == ".kdb":
-        logger.error("Not sure why you'd want a singular distance.")
-        logger.error("kdb distance requires more than one .kdb file as positional inputs")
+        logger.log_it("Not sure why you'd want a singular distance.", "ERROR")
+        logger.log_it("kdb distance requires more than one .kdb file as positional inputs", "ERROR")
         sys.exit(1)
     else:
-        logger.error("bin/kdb.distances() received {0} arguments as input, which were not supported.".format(len(arguments.input)))
+        logger.log_it("bin/kdb.distances() received {0} arguments as input, which were not supported.".format(len(arguments.input)), "ERROR")
         sys.exit(1)
 
-    # Masthead stuff
-    sys.stderr.write(config.DEFAULT_MASTHEAD)
-    if logger.level == logging.DEBUG or logger.level == logging.INFO:
-        sys.stderr.write(config.DEBUG_MASTHEAD)
-    sys.stderr.write(config.DISTANCE_MASTHEAD)
 
-    logger.info("Custom calculating a {0}x{0} '{1}' distance matrix...".format(n, arguments.metric))
 
+    feature = 3
+    step = 3
+    logger.log_it("Custom calculating a {0}x{0} '{1}' distance matrix...".format(n, arguments.metric), "INFO")    
+
+    #print(profiles.shape)
+    #raise RuntimeError("phooey")
+    
     if arguments.metric in ["pearson", "spearman"]:
+
+        profiles = np.transpose(np.array(df))
         
         #files = list(map(lambda f: fileutil.open(f, 'r', slurp=True), arguments.input))
         data = [['' for x in range(n)] for y in range(n)]
         for i in range(n):
             for j in range(n):
-                logger.debug("Calculating the {0}x{1} cell".format(i, j))
-                logger.info("Calculating {0} distance between {1}:({2}) and {3}:({4}) columns...".format(arguments.metric, columns[i], i, columns[j], j))
+                logger.log_it("Calculating the {0}x{1} cell".format(i, j), "DEBUG")
+                logger.log_it("Calculating {0} distance between {1}:({2}) and {3}:({4}) columns...".format(arguments.metric, columns[i], i, columns[j], j), "INFO")
 
                 if i == j:
-                    logger.info("Was self, reverting to identity.")
+                    logger.log_it("Was self, reverting to identity.", "INFO")
                     data[i][j] = distance.identity[arguments.metric]
                 elif i > j:
                     data[i][j] = None
-                    logger.info("Refusing to recompute custom distance metric for symmetric matrix")
+                    logger.log_it("Refusing to recompute custom distance metric for symmetric matrix", "INFO")
+
                 elif i < j:
                     #print("Info: ixj {0}x{1}")
-                    logger.debug("Info: ixj {0}x{1}".format(i, j))
+                    logger.log_it("Info: ixj {0}x{1}".format(i, j), "DEBUG")
                     
                     if arguments.metric == "pearson":
-                        logger.info("Computing custom Pearson correlation coefficient...")
+                        logger.log_it("Computing custom Pearson correlation coefficient...", "INFO")
+
+                        
                         #data[i][j] = distance.correlation(profiles[i], profiles[j])
                         if has_cython is True:
                             idstr = "{0}x{1}".format(i, j)
                             r = mp.Value('d', 0.0)
                             p = mp.Process(target=pearson_correlation, args=(profiles[i], profiles[j], profiles[i].size, r))
                             p.start()
                             #data[i][j] = correlation(profiles[i], profiles[j], profiles[i].size)
                             p.join()
                             data[i][j] = r.value
                         else:
                             raise RuntimeError("Cannot calculate pearson correlation without NumPy and Cython")
                     elif arguments.metric == "spearman":
                         cor, pval = distance.spearman(profiles[i], profiles[j])
-                        logger.info("Computing SciPy Spearman distance")
+                        logger.log_it("Computing SciPy Spearman distance", "INFO")
+                        
                         # FIXME! also print pval matrices
                         data[i][j] = cor
                     elif arguments.metric == "EMD":
-                        logger.error("Custom EMD distance is deprecated")
+                        logger.log_it("Custom EMD distance is deprecated", "ERROR")
                         raise RuntimeError("Genuine bug, please report the usage of deprecated custom distance functions")
                         data[i][j] = distance.EMD(profiles[i], profiles[j])
                     elif arguments.metric == "d2s":
-                        logger.error("Custom d2s distance is deprecated")
+                        logger.log_it("Custom d2s distance is deprecated", "ERROR")
                         raise RuntimeError("Genuine bug, please report the usage of deprecated custom distance functions")
                         data[i][j] = distance.d2s(profiles[i], profiles[j])
                     else:
-                        logger.error("Other distances are not implemented yet")
+                        logger.log_it("Other distances are not implemented yet", "ERROR")
                         sys.exit(1)
                 # This double loop quickly identifies empty cells and sets the data correctly from the permutation above
-        logger.info("Joining processes for parallel correlations")
-        logger.info("\n\n")
-        logger.info("Done joining processes")
-        logger.info("\n\n")
+        logger.log_it("Joining processes for parallel correlations", "INFO")
+        logger.log_it("\n\n\nDone joining processes...", "INFO")
+
 
         
 
-        logger.info("Completing matrix from shared process values")
+        logger.log_it("Completing matrix from shared process values", "INFO")
         for i in range(n):
             for j in range(n):
                 if not i < j:
                     data[i][j] = None
-        logger.info("Filling in symmetrical matrix...")
+        logger.log_it("Filling in symmetrical matrix...", "INFO")
         for i in range(n):
             for j in range(n):
                 if data[i][j] is None:
                     data[i][j] = data[j][i]
                     #logger.info("\n\n\nSwerve swerve\n\n\n")
 
                     
         dist = np.array(data)
     else:
+
+        
         dist = pdist(np.transpose(profiles), metric=arguments.metric)
         dist = squareform(dist)
-        # if arguments.metric == "correlation":
-        #     ones = np.ones(dist.shape, dtype="int64")
-        #     dist = np.subtract(ones, dist)
+
+
     if dist.shape == (2,2):
         print(dist[0][1])
     else:
+
         df = pd.DataFrame(dist, columns=columns)
         
         ## FIXME: CUSTOM sorting code, not commiting to git repo
         #suffixes = [(int(x.split("_")[1]), i) for i, x in enumerate(column_names)] # A list of a 2-tuple of the correct sort order and the index
         #suffixes.sort(key=lambda x: x[0])
         #sorted_column_names = [column_names[s[1]] for s in suffixes]
         #df.sort_values(sorted_column_names)
         
 
         df.to_csv(sys.stdout, sep=arguments.output_delimiter, index=False)
 
 def get_matrix(arguments):
-    logging.getLogger('matplotlib.font_manager').disabled = True
-    logging.getLogger('matplotlib').setLevel(logging.WARNING)
+
+
+    
+    import logging as pylog
+    pylog.getLogger('matplotlib.font_manager').disabled = True
+    pylog.getLogger('matplotlib').setLevel(logging.WARNING)
 
     from multiprocessing import Pool
     
     import numpy as np
     import pandas as pd
     import matplotlib.pyplot as plt
     from sklearn.decomposition import PCA
     from sklearn.manifold import TSNE
     
     from kmerdb import fileutil, config
 
 
+
+    global logger
+    global feature
+    global step
+
+
+    step = 0
+    feature = 0
+
     
     if len(arguments.input) > 1:
 
-        file_reader = fileutil.FileReader()
-        files = list(map(lambda f: fileutil.open(f, 'r', slurp=False), arguments.input))
+        
+        files = list(map(lambda f: fileutil.open(f, 'r', slurp=False, logger=logger), arguments.input))
 
         if arguments.k is None:
             arguments.k = files[0].k
         if not all(os.path.splitext(kdb)[-1] == ".kdb" for kdb in arguments.input):
             raise IOError("One or more parseable .kdb filepaths did not end in '.kdb'")
         ks = [kdbrdr.k for kdbrdr in files]
         suggested_k = ks[0]
         if not all(k == suggested_k for k in ks):
-            logger.error("Files: {0}".format(files))
-            logger.error("Choices of k: {0}".format(ks))
-            logger.error("By default the inferred value of k is used when k is not specified at the command line, which was {0}".format(arguments.k))
-            logger.error("Default choice of k, since not specified at the CLI is {0}".format(arguments.k))
-            logger.error("Proceeding with k set to {0}".format(suggested_k))
+            logger.log_it("Files: {0}".format(files), "ERROR")
+            
+            logger.log_it("Choices of k: {0}".format(ks), "ERROR")
+
+            logger.log_it("By default the inferred value of k is used when k is not specified at the command line, which was {0}".format(arguments.k), "ERROR")
+
+            logger.log_it("Default choice of k, since not specified at the CLI is {0}".format(arguments.k), "ERROR")
+
+            logger.log_it("Proceeding with k set to {0}".format(suggested_k), "ERROR")
+
+            
             raise TypeError("One or more files did not have k set to be equal to {0}".format(arguments.k))
         dtypes = [kdbrdr.metadata["count_dtype"] for kdbrdr in files]
         suggested_dtype = dtypes[0]
         if not all(kdbrdr.count_dtype == suggested_dtype for kdbrdr in files):
             raise TypeError("One of more files did not have dtype = {0}".format(suggested_dtype))
+
         if arguments.parallel > 1:
+            infile = fileutil.FileReader(arguments, logger=logger)
+            
             with Pool(processes=arguments.parallel) as pool:
                 try:
-                    files = pool.map(file_reader.load_file, arguments.input)
+
+
+                    
+                    files = pool.map(infile.parsefile, arguments.input)
+                    
                 except StopIteration as e:
-                    logger.error("Files: {)}".format(", ".join(arguments.input)))
-                    logger.error(e)
+                    logger.log_it("Files: {)}".format(", ".join(arguments.input)), "ERROR")
                     raise e
         else:
             files = []
 
             for f in arguments.input:
-                sys.stderr.write("Reading input from '{0}'...Please be patient...".format(f))
-                fh = fileutil.open(f, 'r', slurp=True) # no metadata on matrix command
+                logger.log_it("Reading input from '{0}'...Please be patient...".format(f), "INFO")
+
+                fh = fileutil.open(f, 'r', slurp=True, logger=logger) # no metadata on matrix command
                 files.append(fh)
 
 
         data = [kdbrdr.counts for kdbrdr in files]
-        logger.info(data)
                      
         pure_data = np.array(data, dtype=suggested_dtype)
         profiles = np.transpose(pure_data)
         # The following does *not* transpose a matrix defined as n x N=4**k
         # n is the number of independent files/samples, (fasta/fastq=>kdb) being assessed
         # N=4**k is the dimensionality of the vector, sparse or not, that makes up the perceived profile, the descriptors is the column dimension.
 
         # The names for the columns are taken as the basenamed filepath, with all extensions (substrings beginning with '.') stripped.
-        logger.info("============================================================")
-        logger.info("Converting arrays of k-mer counts into a pandas DataFrame...")
-        logger.info("============================================================")
-
+        logger.log_it("============================================================", "INFO")
+        logger.log_it("Converting arrays of k-mer counts into a pandas DataFrame...", "INFO")
+        logger.log_it("============================================================", "INFO")
+        
 
 
         if arguments.column_names is None:
             columns = list(map(lambda kdbrdr: os.path.basename(kdbrdr._filepath).split(".")[0], files))
         else:
             with open(arguments.column_names, 'r') as column_names:
                 rows = [line.rstrip() for line in column_names]
@@ -475,145 +577,196 @@
                     raise ValueError("Could not properly parse .tsv column_names accessory file")
         if len(columns) != len(files):
             raise RuntimeError("Number of column names {0} does not match number of input files {1}...".format(len(columns), len(files)))
         suggested_metadata = files[0].metadata
         expected, num_columns = 4**suggested_k, len(columns)
         if profiles.shape != (expected, num_columns):
             #logger.info("Time is money.")
-            logger.error("Check shape self...")
-            logger.error("Expected shape: {0} x {1}".format(expected, num_columns))
-            logger.error("Actual shape: {0}".format(profiles.shape))
+            logger.log_it("Check shape self...", "ERROR")
+
+            logger.log_it("Expected shape: {0} x {1}".format(expected, num_columns), "ERROR")
+
+            logger.log_it("Actual shape: {0}".format(profiles.shape), "ERROR")
+
+            
             raise RuntimeError("Raw profile shape (a NumPy array) doesn't match expected dimensions")
         df = pd.DataFrame(profiles, columns=columns)
         is_uint32 = False
         is_uint64 = False
         is_float32 = False
         is_float64 = False
         is_uint32 = all([x.dtype.name == 'uint32' for x in profiles])
         is_uint64 = all([x.dtype.name == 'uint64' for x in profiles])
         is_float32 = all([x.dtype.name == 'float32' for x in profiles])
         is_float64 = all([x.dtype.name == 'float64' for x in profiles])
 
     elif len(arguments.input) == 0 or (len(arguments.input) == 1 and (arguments.input[0] == "STDIN" or arguments.input[0] == "/dev/stdin")):
-        logger.info("Reading input as tsv/csv from STDIN")
+
+        feature = 1
+        step = 1
+        
+        logger.log_it("Reading input as tsv/csv from STDIN", "INFO")
         try:
             df = pd.read_csv(sys.stdin, sep=arguments.delimiter)
         except pd.errors.EmptyDataError as e:
-            logger.error(e)
-            logger.error("Pandas error on DataFrame reading. Perhaps a null dataset being read?")
-            sys.exit(1)
+            logger.log_it(e.__str__(), "INFO")
+
+            logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
+            raise e
         columns = list(df.columns)
     elif len(arguments.input) == 1 and (os.path.splitext(arguments.input[0])[-1] == ".tsv" or os.path.splitext(arguments.input[0])[-1] == ".csv"):
-        logger.info("Reading input file as tsv/csv")
+
+        feature = 1
+        step = 1
+        
+        
+        logger.log_it("Reading input file as tsv/csv...", "INFO")
         try:
             df = pd.read_csv(arguments.input[0], sep=arguments.delimiter)
         except pd.errors.EmptyDataError as e:
-            logger.error(e)
-            logger.error("Pandas error on DataFrame reading. Perhaps a null dataset being read?")
-            sys.exit(1)
+            logger.log_it(e.__str__(), "ERROR")
+
+
+            logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
+
+            
+            raise e
         columns = list(df.columns)
     else:
-        logger.error(arguments)
-        logger.error("bin/kdb.get_matrix() received {0} arguments as input, and this is not supported.".format(len(arguments.input)))
-        logger.error(arguments.input)
-        sys.exit(1)
-    sys.stderr.write(config.DEFAULT_MASTHEAD)
-    if logger.level == logging.DEBUG or logger.level == logging.INFO:
-        sys.stderr.write(config.DEBUG_MASTHEAD)
-    sys.stderr.write(config.MATRIX_MASTHEAD)
+        logger.log_it(arguments, "ERROR")
+
+        logger.log_it(str(arguments.input), "ERROR")
 
 
+        
+        raise ArgumentError("kmerdb matrix received {0} arguments as input, and this is not supported.".format(len(arguments.input)))
+
     final_df = None
     if arguments.method == "DESeq2":
+        
+        feature = 2
+        step = 4
+
+        
         # if arguments.normalize_with == "ecopy":
         #     import ecopy as ep
         #     logger.info("Normalizing the DataFrame for sample size with ecopy...")
         #     normalized = ep.transform(df, method="normalize", axis=0)
         # # Normalizing across the 0th axis will normalize across the row meaning between samples. To arrive at this I checked the column sums of both to be sure I understood what was being normalized.
         # # We don't necessarily need to standardize, and not standardizing will make rationalizations or sensitivity to the real number range more clear.
         # if arguments.normalize_with == "DESeq2":
 
-        logger.info("Normalizing the DataFrame with DESeq2 NB-compatible count normalization via rpy2...")
+        logger.log_it("Normalizing the DataFrame with DESeq2 NB-compatible count normalization via rpy2...", "INFO")
+
         '''
         The following was shown to me by the following medium post.
         https://w1ndy.medium.com/calling-r-libraries-from-python-5ffbf3c3e5a8
         '''
         from rpy2.robjects.packages import importr, PackageNotInstalledError
         from rpy2.robjects import FloatVector, DataFrame, r, pandas2ri, Formula
         pandas2ri.activate()
         try:
             #fitdistrplus = importr('fitdistrplus')
             deseq = importr('DESeq2')
             count_matrix = pandas2ri.py2rpy(df)
             ncol = r['ncol']
             seq = r['seq']
             colData = pd.DataFrame(np.transpose(columns), columns=["Species"])
-            logger.info("colData:\n{0}".format(colData))
+            
+            logger.log_it("colData:\n{0}".format(colData), "INFO")
+
                 
             dds = r['DESeqDataSetFromMatrix'](count_matrix, colData, Formula('~ Species'))
-            logger.info("DESeq dataset:\n{0}".format(str(dds)))
+            logger.log_it("DESeq dataset:\n{0}".format(str(dds)), "INFO")
+            
             dds = r['estimateSizeFactors'](dds)
                 
             normalized = r['counts'](dds, normalized = True)
             if not arguments.no_normalized_ints:
                 normalized = np.array(np.rint(normalized), dtype="int64")
             normalized = pd.DataFrame(normalized, columns=columns)
-            logger.debug(normalized)
-            logger.info("Normalized matrix shape: {0}".format(normalized.shape))
+            
+            logger.log_it("Normalized matrix shape: {0}".format(normalized.shape), "INFO")
+
 
             #     if arguments.method == "Unnormalized":
             #         cf = r['descdist'](r_dataframe, discrete=True)
             #     else:
             #         cf = r['descdist'](r_dataframe, discrete=False)
         except PackageNotInstalledError as e:
-            logger.error(e)
-            logger.error("One or more R packages were not installed. Please see the install documentation about installing the associated R packages")
-            logger.error("Use -vv for suggested installation instructions.")
-            sys.exit(1)
+            logger.log_it(e.__str__(), "ERROR")
+
+            logger.log_it("One or more R packages were not installed. Please see the install documentation about installing the associated R packages", "ERROR")
+
+            logger.log_it("Use -vv for suggested installation instructions.", "ERROR")
+
+            
+            raise e
+
         #normalized.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
 
         # logger.error("False ending of Normalized")
         # logger.debug("final_df should be set as normalized")
         # sys.exit(1)
         final_df = normalized
     elif arguments.method == "pass":
+
+        feature = 2
+        step = 4
+        
         #df.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
         final_df = df
     elif arguments.method == "Frequency":
+
+        feature = 2
+        step = 4
+        
+        
         final_df = df # 4/5/24 - frequencies are given in the standard format
         #k = suggested_metadata['k']
         #total_kmers = suggested_metadata["total_kmers"]
         #final_df = df.div(total_kmers)
     elif arguments.method == "PCA":
+
+
+
+        feature = 2
+        step = 2
+
+
+        
         # This method is actually dimensionality reduction via SVD, and this process is used during principal components analysis.
         # We generate the elbow graph in this step if the required dimensionality parameter '-n' is not supplied.
         # In this case we assume they have not provided the parameter because they'd like to use the so-called 'auto-detection'
         
         # I've specified a feature called 'auto-detect' such that the elbow graph is produced
         # they supply the number of dimensions they'd like after viewing the graph,
         # And in this way by viewing the graph, the 'correct' number of dimensions is attained.
         #
         #################################
         # PCA dimensionality reduction
         #################################
     
-        logger.info("Performing preliminary dimensionality reduction to the MLE")
+        logger.log_it("Performing preliminary dimensionality reduction to the MLE", "INFO")
+
+
+        
         pca = PCA()#n_components="mle", svd_solver='auto')
         pca.fit(np.transpose(df)) # PCA of the normalized matrix or its transpose?
         # We want the number of k-mers, the number of features reduced, so we transpose the original matrix
 
 
         plt.plot(range(1, len(pca.explained_variance_ratio_)+1), pca.explained_variance_ratio_.cumsum(), marker='o', linestyle="--")
         plt.title("Explained variance by components")
         plt.xlabel("Number of components")
         plt.ylabel("Cumulative explained variance")
         plt.savefig(config.pca_variance_fig_filepath)
 
         if arguments.n is not None:
-            logger.info("Using selected PCA dimensionality to reduce the transpose matrix/DataFrame again for use in 'kdb kmeans'")
+            logger.log_it("Using selected PCA dimensionality to reduce the transpose matrix/DataFrame again for use in 'kdb kmeans'", "INFO")
             pca = PCA(n_components=arguments.n)
             pca.fit(np.transpose(df))
             sys.stderr.write("\n\n\n")
             sys.stderr.write("-"*30)
             
             sys.stderr.write("Explained variances: {0}\n".format(pca.explained_variance_ratio_))
             sys.stderr.write("Log-likelihoods: {0}\n".format(pca.score_samples(normalized)))
@@ -622,20 +775,31 @@
 
             score_matrix = pca.transform(np.transpose(df))
             score_df = pd.DataFrame(np.transpose(score_matrix), columns=columns)
 
             #score_df.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
             final_df = score_df
         else:
-            logger.warning("You must look at '{0}' to decide on the choice of '-n' for specify when generating the dimensionally reduced matrix for clustering function".format(config.pca_variance_fig_filepath))
-            sys.exit(1)
+            logger.log_it("You must look at '{0}' to decide on the choice of '-n' for specify when generating the dimensionally reduced matrix for clustering function".format(config.pca_variance_fig_filepath), "WARNING")
+
+
+            
         #logger.debug("Components:\n{0}".format(pca.components_))
         # The shape for my first run was 10x11 and I have 11 samples. So I decided to not transpose this matrix to simply add it to a DataFrame and rename the samples.
         #df = pd.DataFrame(pca.components_, columns=list(map(lambda kdbrdr: os.path.splitext(os.path.basename(kdbrdr._filepath))[0], files)))
     elif arguments.method == "tSNE":
+
+
+        feature = 2
+        step = 3
+
+
+
+
+        
         '''
         In t-SNE, perplexity or k is defined as 2^S, where S is the Shannon entropy of the conditional probability distribution.
         '''
         if arguments.n is None:
             raise TypeError("'kdb matrix tSNE' requires a keyword argument '-n' equal to the number of components of the subspace for tSNE to project the data into. A choice of 2 is recommended")
         tsne = TSNE(n_components=arguments.n, perplexity=arguments.perplexity).fit_transform(np.transpose(df))
         tsne_df = pd.DataFrame(np.transpose(tsne), columns=columns)
@@ -645,24 +809,27 @@
     ## FIXME: CUSTOM SORTING. WILL NOT COMMIT TO GIT REPO
     #suffixes = [(int(x.split("_")[1]), i) for i, x in enumerate(column_names)] # A list of a 2-tuple of the correct sort order and the index
     #suffixes.sort(key=lambda x: x[0])
     #sorted_column_names = [column_names[s[1]] for s in suffixes]
     #final_df.sort_values(sorted_column_names)
 
     final_df.to_csv(sys.stdout, sep=arguments.output_delimiter, index=arguments.with_index)
-    logger.info("Done printing {0} matrix to STDOUT".format(arguments.method))
+
+    
+    logger.log_it("Done printing {0} matrix to STDOUT".format(arguments.method), "INFO")
 
     #logger.info("Beginning distribution analysis in R...")
     #logger.warn("Not implemented in Python...")
     
     sys.stderr.write(config.DONE)
 
 
 
 def kmeans(arguments):
+    import logging
     logging.getLogger('matplotlib.font_manager').disabled = True
     logging.getLogger('matplotlib').setLevel(logging.WARNING)
     from io import TextIOWrapper
     import numpy as np
     import pandas as pd
     import matplotlib.pyplot as plt
     from sklearn import metrics
@@ -680,25 +847,21 @@
         #df.set_index('index')
     elif arguments.input is None or arguments.input == "/dev/stdin" or arguments.input == "STDIN":
         df = pd.read_csv(sys.stdin, sep=arguments.delimiter)
         column_names = df.columns
         df = df.transpose()
         #df.set_index('index')
     else:
-        logger.error("An unknown IO type was detected in bin/kdb.cluster()")
-        sys.exit(1)
-
-    sys.stderr.write(config.DEFAULT_MASTHEAD) # Not working
-    if logger.level == logging.DEBUG or logger.level == logging.INFO: # Not working
-        sys.stderr.write(config.DEBUG_MASTHEAD)
-    sys.stderr.write(config.KMEANS_MASTHEAD) # Not working
+        logger.log_it("An unknown IO type was detected in kmeans", "ERROR")
+        raise IOError("Unable to process input argument")
 
         
     num_samples, num_features = df.shape
-    logger.info("Input DataFrame shape: {0}".format(df.shape))
+    logger.log_it("Input DataFrame shape: {0}".format(df.shape), "INFO")
+    
     t0 = time.time()
 
     
     wcss = []
     for i in range(1, num_samples+1):
         kmeans_pca = KMeans(n_clusters = i, init="k-means++", random_state=42)
         kmeans_pca.fit(df)
@@ -726,29 +889,33 @@
         # }})
         df.to_csv(arguments.output, sep=arguments.output_delimiter)
         colnames = list(df.columns)
         fig, ax = plt.subplots()
         scatter = ax.scatter(df.iloc[:, 1], df.iloc[:, 2], c=df.iloc[:, 0])
         legend = ax.legend(*scatter.legend_elements(), loc="upper right", title="Cluster")
 
+        print("K-means coordinates")
         for x,y,z in zip(np.array(df.iloc[:, 1]), np.array(df.iloc[:, 2]), column_names):
-            sys.stderr.write("{0}\t{1}\t{2}".format(x,y,z))
+            
+            print("{0}\t{1}\t{2}".format(x,y,z))
+            #sys.stderr.write("{0}\t{1}\t{2}\n".format(x,y,z))
             ax.annotate(z, xy=(x, y), xycoords='data', xytext=(0, -45), textcoords='offset points', arrowprops=dict(facecolor='black', shrink=0.05), horizontalalignment='left', verticalalignment='bottom')
         ax.set_xlabel("Dim1")
         ax.set_ylabel("Dim2")
         ax.set_title("K-means clustering")
         ax.add_artist(legend)
         ax.grid(True)
 
 
         plt.savefig(config.kmeans_clustering_fig_filepath)
         
         #centroids = kmeans.cluster_centers_
-        logger.info(list(column_names))
-        logger.info(labels)
+        logger.log_it(str(list(column_names)), "INFO")
+        
+        logger.log_it(", ".join(list(map(str, labels))), "INFO")
     
         '''
         Clustering score quality estimation from 
         https://scikit-learn.org/stable/auto_examples/cluster/plot_kmeans_digits.html#define-our-evaluation-benchmark
     
         '''
         name = "K-means metrics"
@@ -803,31 +970,34 @@
         ax.set_ylabel("Dim2")
         ax.set_title("K-means clustering")
         ax.add_artist(legend)
         ax.grid(True)
         plt.savefig(config.kmeans_clustering_fig_filepath)
         
         #centroids = kmeans.cluster_centers_
-        logger.info(list(column_names))
-        logger.info(labels)
+        logger.log_it(", ".join(list(column_names)), "INFO")
+
+        logger.log_it(", ".join(labels), "INFO")
+
         
     sys.stderr.write("Generated {0} clusters projected onto reduced dimension 1 and 2 of the input dataset\n".format(arguments.k))
     sys.stderr.write("The figure was written to {0}\n\n".format(config.kmeans_clustering_fig_filepath))
 
-    logger.info("The annotated sample matrix can be printed by specifying an output files with [ -o|--output OUTFILE ]")
+    logger.log_it("The annotated sample matrix can be printed by specifying an output files with [ -o|--output OUTFILE ]", "INFO")
     
     sys.stderr.write(config.DONE)
 
 
 
 def hierarchical(arguments):
     """
     Thanks to https://www.analyticsvidhya.com/blog/2019/05/beginners-guide-hierarchical-clustering/
     for the inspiration
     """
+    import logging
     logging.getLogger('matplotlib.font_manager').disabled = True
     logging.getLogger('matplotlib').setLevel(logging.WARNING)
     from io import TextIOWrapper
     import numpy as np
     import pandas as pd
     import matplotlib.pyplot as plt
     import scipy.cluster.hierarchy as shc
@@ -843,24 +1013,21 @@
         column_names = list(df.columns)
         df = df.transpose()
     elif arguments.input is None or arguments.input == "STDIN" or arguments.input == "/dev/stdin":
         df = pd.read_csv(sys.stdin, sep=arguments.delimiter)
         column_names = list(df.columns)
         df = df.transpose()
     else:
-        logger.error("An unknown IO type was detected in bin/kdb.cluster()")
-        sys.exit(1)
+        logger.log_it("An unknown IO type was detected in hierarchical", "INFO")
+        raise IOError("Unable to process input")
+
 
-    sys.stderr.write(config.DEFAULT_MASTHEAD)
-    if logger.level == logging.DEBUG or logger.level == logging.INFO:
-        sys.stderr.write(config.DEBUG_MASTHEAD)
-    sys.stderr.write(config.HIERARCHICAL_MASTHEAD)
     
     num_samples, num_features = df.shape
-    logger.info("Input DataFrame shape: {0}".format(df.shape))
+    logger.log_it("Input DataFrame shape: {0}".format(df.shape), "INFO")
 
     #tree = treecluster(distancematrix=np.array(df)) # Can this be exported to Newick?
     plt.figure(figsize=(16, 9)) # figsize=(10, 7)
     plt.title("Dendrogram")
     dend = shc.dendrogram(shc.linkage(df, method=arguments.method), labels=column_names, leaf_rotation=90)
     #plt.show()
     plt.savefig(config.hierarchical_clustering_dendrogram_fig_filepath)
@@ -910,19 +1077,14 @@
 #         df = pd.read_csv(sys.stdin, sep=arguments.delimiter)
 #         column_names = df.columns
 #         df = df.transpose()
 #     else:
 #         logger.error("An unknown IO type was detected in bin/kdb.cluster()")
 #         sys.exit(1)
 
-#     sys.stderr.write(config.DEFAULT_MASTHEAD)
-#     if logger.level == logging.DEBUG:
-#         sys.stderr.write(config.DEBUG_MASTHEAD)
-#     sys.stderr.write(config.RAREFY_MASTHEAD)
-
 
 #     num_samples, num_features = df.shape
 #     t0 = time.time()
 
 #     logger.warning("Multiple files: Untested behavior with ecopy.diversity.rarefy")
 #     test = rarefy(df, config.ecopy_rarefaction_fig_filepath, 'rarecurve')
 #     #arguments.output.write(test)
@@ -952,23 +1114,25 @@
 
     if sfx == ".kdb":
         kdb = fileutil.open(arguments.kdb, mode='r', sort=arguments.re_sort, slurp=True)
         metadata = kdb.metadata
         kmer_ids_dtype = metadata["kmer_ids_dtype"]
         N = 4**metadata["k"]
         if metadata["version"] != config.VERSION:
-            logger.warning("KDB version is out of date, may be incompatible with current KDBReader class")
+            logger.log_it(".kdb version is out of date, may be incompatible with current KDBReader class", "WARNING")
+
         assert kdb.kmer_ids.size == N, "view | read kmer_ids size did not match N from the header metadata"
         assert kdb.counts.size == N, "view | read counts size did not match N from the header metadata"
         assert kdb.frequencies.size == N, "view | read frequencies size did not match N from the header metadata"
         metadata = kdb.metadata
     elif sfx == ".kdbg":
         kdb = graph.open(arguments.kdb, mode='r')
         if kdb.metadata["version"] != config.VERSION:
-            logger.warning("KDB file version is out of date, may be incompatible with current fileutil.KDBReader class")
+            logger.log_it(".kdb file version is out of date, may be incompatible with current fileutil.KDBReader class", "WARNING")
+
         N = 4**kdb.metadata["k"]
         metadata = kdb.metadata
 
     if arguments.json:
         print(dict(kdb.metadata))
     else:
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
@@ -1005,15 +1169,17 @@
 
         if line.rstrip() != config.end_header_line:
             header += line
             return header
         else:
             header_dict = yaml.safe_load(header)
             if type(header_dict) is not dict:
-                logger.debug("Tried to parse:\n{0}\n".format(header))
+                logger.log_it("Tried to parse:\n{0}\n".format(header), "DEBUG")
+
+                
                 raise ValueError("Could not parse YAML formatted header")
             else:
                 return header_dict
 
     assert type(arguments.kdb_in) is str, "kdb_in must be a str"
     sfx = os.path.splitext(arguments.kdb_in)[-1]
 
@@ -1027,89 +1193,104 @@
         raise IOError("Viewable .kdb(g) filepath '{0}' does not exist on the filesystem".format(arguments.kdb_in))
     if sfx == ".kdb":
         with fileutil.open(arguments.kdb_in, mode='r', sort=arguments.re_sort, slurp=True) as kdb_in:
             metadata = kdb_in.metadata
             kmer_ids_dtype = metadata["kmer_ids_dtype"]
             N = 4**metadata["k"]
             if metadata["version"] != config.VERSION:
-                logger.warning("KDB version is out of date, may be incompatible with current KDBReader class")
+                logger.log_it("KDB version is out of date, may be incompatible with current KDBReader class", "WARNING")
             if arguments.kdb_out is None or (arguments.kdb_out == "/dev/stdout" or arguments.kdb_out == "STDOUT"): # Write to stdout, uncompressed
                 if arguments.header:
                     yaml.add_representer(OrderedDict, util.represent_ordereddict)
                     print(yaml.dump(metadata, sort_keys=False))
                     print(config.header_delimiter)
-            logger.info("Reading from file...")
-            logger.debug("I cut off the json-formatted unstructured column for the main view.")
+            logger.log_it("Reading from file...", "INFO")
+
+            
+            
             try:
                 if not arguments.un_sort and arguments.re_sort and metadata["sorted"] is True:
                     kmer_ids_sorted_by_count = np.lexsort((kdb_in.counts, kdb_in.kmer_ids))
                     reverse_kmer_ids_sorted_by_count = np.flipud(kmer_ids_sorted_by_count)
                     for i, idx in enumerate(kmer_ids_sorted_by_count):
                         kmer_id = kdb_in.kmer_ids[i]
-                        logger.debug("The first is an implicit row-index. The second is a k-mer id, then the counts and frequencies.")
-                        logger.debug("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]))
+                        logger.log_it("The first is an implicit row-index. The second is a k-mer id, then the counts and frequencies.", "DEBUG")
+                        
+                        logger.log_it("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]), "DEBUG")
+
 
                         print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]))
                 else:
                     for i, idx in enumerate(kdb_in.kmer_ids):
                         kmer_id = kdb_in.kmer_ids[idx]
-                        logger.debug("The row in the file should follow this order:")
-                        logger.debug("The first is an implicit row-index. The second is a k-mer id, then the counts and frequencies.")
-                        logger.debug("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]))
+                        logger.log_it("The row in the file should follow this order:", "DEBUG")
+                        
+                        logger.log_it("The first is an implicit row-index. The second is a k-mer id, then the counts and frequencies.", "DEBUG")
+                        
+                        logger.log_it("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]), "DEBUG")
+
+                        
                         try:
                             if arguments.un_sort is True:
                                 assert kmer_id == idx, "view | kmer_id {0} didn't match the expected k-mer id.".format(idx, kmer_id)
                                 assert i == kmer_id, "view | kmer_id {0} didn't match the implicit index {1}".format(idx, i)
                             else:
                                 #logger.debug("Not sorting, so skipping assertion about profile (col1, column 2)")
                                 pass
                         except AssertionError as e:
-                            logger.warning(e)
-                            logger.warning("K-mer id {0} will be printed in the {1} row".format(idx, i))
+                            logger.log_it(e.__str__(), "WARNING")
+                            
+                            logger.log_it("K-mer id {0} will be printed in the {1} row".format(idx, i), "WARNING")
+                            
                         #raise e
-                        logger.debug("{0} line:".format(i))
-                        logger.debug("=== = = = ======= =  =  =  =  =  = |")
+                        logger.log_it("{0} line:".format(i), "DEBUG")
+                        
+                        logger.log_it("=== = = = ======= =  =  =  =  =  = |", "DEBUG")
+
                         if arguments.un_sort is True:
                             print("{0}\t{1}\t{2}\t{3}".format(i, idx, kdb_in.counts[idx], kdb_in.frequencies[idx]))
                         else:
                             print("{0}\t{1}\t{2}\t{3}".format(i, idx, kdb_in.counts[kmer_id], kdb_in.frequencies[kmer_id]))
                 # I don't think anyone cares about the graph representation.
                 # I don't think this actually matters because I can't figure out what the next data structure is.
                 # Is it a Cypher query and creation node set?
                 # I need to demonstrate a capacity for graph based learning.
                 # (:-|X) The dread pirate roberts got me.
                 # :)
             except BrokenPipeError as e:
-                logger.error(e)
+                logger.log_it(e.__str__(), "ERROR")
                 raise e
         if arguments.kdb_out is not None and arguments.compress: # Can't yet write compressed to stdout
-            logger.error("Can't write kdb to stdout! We need to use a Bio.bgzf filehandle.")
-            sys.exit(1)
+            logger.log_it("Can't write .kdb to stdout! We need to use a Bio.bgzf filehandle.", "ERROR")
+            raise IOError("Can't write .kdb to stdout! We need to use a Bio.bgzf filehandle.")
+
         elif arguments.kdb_out is not None and type(arguments.kdb_out) is not str:
             raise ValueError("Cannot write a file to an argument that isn't a string")
-        elif arguments.kdb_out is not None and os.path.exists(arguments.kdb_out):
-            logger.warning("Overwriting '{0}'...".format(arguments.kdb_out))
-        elif arguments.kdb_out is not None and not os.path.exists(arguments.kdb_out):
-            logger.debug("Creating '{0}'...".format(arguments.kdb_out))
+        elif arguments.kdb_out is not None and (os.path.exists(arguments.kdb_out) or not os.path.exists(arguments.kdb_out)):
+            if os.path.exists(arguments.kdb_out):
+                logger.log_it("Overwriting '{0}'...".format(arguments.kdb_out), "WARNING")
+
+            logger.log_it("Creating '{0}'...".format(arguments.kdb_out), "DEBUG")
+            
             if arguments.kdb_out is not None:
                 with fileutil.open(arguments.kdb_in, 'r', dtype=suggested_dtype, sort=arguments.sorted, slurp=True) as kdb_in:
                     assert kdb_in.kmer_ids.size == N, "view | read kmer_ids size did not match N from the header metadata"
                     assert kdb_in.counts.size == N, "view | read counts size did not match N from the header metadata"
                     assert kdb_in.frequencies.size == N, "view | read frequencies size did not match N from the header metadata"
                     with fileutil.open(arguments.kdb_out, metadata=metadata, mode='w') as kdb_out:
                         try:
                             for i, idx in enumerate(kdb_in.kmer_ids):
                                 kmer_id = idx
                                 seq = kmer.id_to_kmer(kmer_id, arguments.k)
                                 kmer_metadata = kmer.neighbors(seq, arguments.k)
-                                logger.debug("The first is the actual row id. This is the recorded row-id in the file. This should always be sequential. Next is the k-mer id. ")
+                                logger.log_it("The first is the actual row id. This is the recorded row-id in the file. This should always be sequential. Next is the k-mer id. ", "DEBUG")
                                 kdb_out.write("{0}\t{1}\t{2}\t{3}\n".format(i, kmer_id, kdb_in.counts[kmer_id],  kdb_in.frequencies[kmer_id], kmer_metadata))
                     
                         except StopIteration as e:
-                            logger.error(e)
+                            logger.log_it(e.__str__(), "ERROR")
                             raise e
                         finally:
                             #kdb_out._write_block(kdb_out._buffer)
                             #kdb_out._handle.flush()
                             #kdb_out._handle.close()
                             sys.stderr.write(config.DONE)
     elif sfx == ".kdbg":
@@ -1118,56 +1299,71 @@
 
         n1_dtype      = metadata["n1_dtype"]
         n2_dtype      = metadata["n2_dtype"]
         weights_dtype = metadata["weights_dtype"]
 
             
         if metadata["version"] != config.VERSION:
-            logger.warning("KDB version is out of date, may be incompatible with current KDBReader class")
+            logger.log_it("KDB version is out of date, may be incompatible with current KDBReader class", "WARNING")
+            
         if arguments.kdb_out is None or (arguments.kdb_out == "/dev/stdout" or arguments.kdb_out == "STDOUT"): # Write to stdout, uncompressed
             if arguments.header:
                 yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
                 print(yaml.dump(metadata, sort_keys=False))
                 print(config.header_delimiter)
-        logger.info("Reading from file...")
-        logger.debug("I cut off the json-formatted unstructured column for the main view.")
+        logger.log_it("Reading from file...", "INFO")
+        
+        logger.log_it("I cut off the json-formatted unstructured column for the main view.", "DEBUG")
+        
 
         for i in range(len(kdbg_in.n1)):
             n1 = kdbg_in.n1[i]
             n2 = kdbg_in.n2[i]
             w  = kdbg_in.weights[i]
-            logger.debug("The row in the file should follow this order:")
-            logger.debug("The first is an implicit row-index. The second and third are k-mer ids, then edge weight")
-            logger.debug("{0}\t{1}\t{2}\t{3}".format(i, n1, n2, w))
-            logger.debug("{0} line:".format(i))
-            logger.debug("=== = = = ======= =  =  =  =  =  = |")
+            logger.log_it("The row in the file should follow this order:", "DEBUG")
+            
+            logger.log_it("The first is an implicit row-index. The second and third are k-mer ids, then edge weight", "DEBUG")
+            
+            logger.log_it("{0}\t{1}\t{2}\t{3}".format(i, n1, n2, w), "DEBUG")
+            
+            logger.log_it("{0} line:".format(i), "DEBUG")
+
+            logger.log_it("=== = = = ======= =  =  =  =  =  = |", "DEBUG")
+
+            
             print("{0}\t{1}\t{2}\t{3}".format(i, n1, n2, w))
                 # I don't think anyone cares about the graph representation.
                 # I don't think this actually matters because I can't figure out what the next data structure is.
                 # Is it a Cypher query and creation node set?
                 # I need to demonstrate a capacity for graph based learning.
                 # (:-|X) The dread pirate roberts got me.
                 # :)
         if arguments.kdb_out is not None and arguments.compress: # Can't yet write compressed to stdout
-            logger.error("Can't write kdb to stdout! We need to use a Bio.bgzf filehandle.")
-            sys.exit(1)
+            logger.log_it("Can't write kdb to stdout! We need to use a Bio.bgzf filehandle.", "ERROR")
+            raise IOError("Can't write kdb to stdout! We need to use a Bio.bgzf filehandle.")
+
         elif arguments.kdb_out is not None and type(arguments.kdb_out) is not str:
             raise ValueError("Cannot write a file to an argument that isn't a string")
         elif arguments.kdb_out is not None and os.path.exists(arguments.kdb_out):
-            logger.warning("Overwriting '{0}'...".format(arguments.kdb_out))
+            
+            logger.log_it("Overwriting '{0}'...".format(arguments.kdb_out), "WARNING")
+
+            
         elif arguments.kdb_out is not None and not os.path.exists(arguments.kdb_out):
-            logger.debug("Creating '{0}'...".format(arguments.kdb_out))
+            
+            logger.log_it("Creating '{0}'...".format(arguments.kdb_out), "DEBUG")
+            
             if arguments.kdb_out is not None:
                 with graph.open(arguments.kdb_out, metadata=metadata, mode='w') as kdb_out:
                     try:
                         for i in range(len(kdbg.n1)):
                             kdb_out.write("{0}\t{1}\t{2}\t{3}\n".format(i, kdbg_in.n1[i], kdbg_in.n2[i],  kdbg_in.w[i]))
                     
                     except StopIteration as e:
-                        logger.error(e)
+                        logger.log_it(e.__str__(), "ERROR")
                         raise e
                     finally:
                         #kdb_out._write_block(kdb_out._buffer)
                         #kdb_out._handle.flush()
                         #kdb_out._handle.close()
                         sys.stderr.write(config.DONE)
 
@@ -1202,39 +1398,42 @@
             n2_dtype      = metadata["n2_dtype"]
             weights_dtype = metadata["weights_dtype"]
 
 
 
             
             if metadata["version"] != config.VERSION:
-                logger.warning("KDB version is out of date, may be incompatible with current KDBReader class")
+                logger.log_it(".kdb version is out of date, may be incompatible with current KDBReader class", "WARNING")
+
+                
             if arguments.kdb_out is None or (arguments.kdb_out == "/dev/stdout" or arguments.kdb_out == "STDOUT"): # Write to stdout, uncompressed
                 if arguments.header:
                     yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
                     print(yaml.dump(metadata, sort_keys=False))
                     print(config.header_delimiter)
-            logger.info("Reading from file...")
-            logger.debug("I cut off the json-formatted unstructured column for the main view.")
+            logger.log_it("Reading from file...", "INFO")
+
+            
             try:
 
 
 
                 nodes = list(set(kdbg_in.n1 + kdbg_in.n2))
                 edges = list(zip(kdbg_in.n1, kdbg_in.n2, list(map(lambda w: {'weight': w} , kdbg_in.weights))))
 
                 graph.create_graph(nodes, edges)
                 
             except BrokenPipeError as e:
-                logger.error(e)
+                logger.log_it(e.__str__(), "ERROR")
                 raise e
 
     
                             
                                               
-def make_kdbg(arguments):
+def make_graph(arguments):
     """
     Another ugly function that takes a argparse Namespace object as its only positional argument
 
     Basically, from a fasta file, I want to generate a file format that consists of unique row ids, k-mer ids, adjacency list, 
 
     and finally an int field (0 represents unused) representing the order of the row-kmer being used in a graph traversal.
 
@@ -1245,38 +1444,56 @@
     from multiprocessing import Pool
 
 
     import jsonschema
     
     import numpy as np
     
-    from kmerdb import graph, kmer, util
+    from kmerdb import kmer, util, graph
     from kmerdb.config import VERSION
 
+    global logger
+    global step
+    global feature
+    
 
     
-    logger.debug("Printing entire CLI argparse option Namespace...")
-    logger.debug(arguments)
+    logger.log_it("Printing entire CLI argparse option Namespace...", "DEBUG")
+
+    logger.log_it(str(arguments), "DEBUG")
     
     # The extension should be .kdb because I said so.
-    logger.info("Checking extension of output file...")
+    logger.log_it("Checking extension of output file...", "INFO")
+
+    
     if os.path.splitext(arguments.kdbg)[-1] != ".kdbg":
         raise IOError("Destination .kdbg filepath does not end in '.kdbg'")
 
     file_metadata = []
     theoretical_kmers_number = 4**arguments.k # Dimensionality of k-mer profile
 
+
+
     
-    logger.info("Parsing {0} sequence files to generate a k-mer adjacency list...".format(len(list(arguments.seqfile))))
-    infile = graph.Parseable(arguments) # NOTE: Uses the kmerdb.graph module
+    logger.log_it("Parsing {0} sequence files to generate a k-mer adjacency list...".format(len(list(arguments.seqfile))), "INFO")
 
     
-    logger.info("Processing {0} fasta/fastq files across {1} processors...".format(len(list(arguments.seqfile)), arguments.parallel))
-    logger.debug("Parallel (if specified) mapping the kmerdb.parse.parsefile() method to the seqfile iterable")
-    logger.debug("In other words, running the kmerdb.parse.parsefile() method on each file specified via the CLI")
+    infile = graph.Parseable(arguments, logger=logger) # NOTE: Uses the kmerdb.graph module
+
+
+    feature = 1
+    step = 1
+
+    
+    logger.log_it("Processing {0} fasta/fastq files across {1} processors...".format(len(list(arguments.seqfile)), arguments.parallel), "INFO")
+    
+    logger.log_it("Parallel (if specified) mapping the kmerdb.parse.parsefile() method to the seqfile iterable", "DEBUG")
+    
+    logger.log_it("In other words, running the kmerdb.parse.parsefile() method on each file specified via the CLI", "DEBUG")
+    
     if arguments.parallel > 1:
         with Pool(processes=arguments.parallel) as pool:
             # data files_metadata
             data = pool.map(infile.parsefile, arguments.seqfile) # Returns a list of k-mer ids
     else:
             # data files_metadata
             data = list(map(infile.parsefile, arguments.seqfile))
@@ -1287,15 +1504,15 @@
     ######################################
     Step 1. Completed
     ######################################
     """
 
 
 
-
+    step = 2
 
 
             
     """
     Summary statistics and metadata structure
     """
 
@@ -1331,45 +1548,62 @@
         "n2_dtype": "uint64",
         "weights_dtype": "uint64",
         "tags": [],
         "files": file_metadata
     })
 
     
-    logger.info("Validating aggregated metadata structure for .kdbg header...")
+    logger.log_it("Validating aggregated metadata structure for .kdbg header...", "INFO")
+
     try:
         np.dtype(metadata["n1_dtype"])
         np.dtype(metadata["n2_dtype"])
         np.dtype(metadata["weights_dtype"])
     except TypeError as e:
-        logger.error(metadata)
-        logger.error(e)
-        logger.error("kmerdb encountered a type error and needs to exit")
+        logger.log_it(metadata, "ERROR")
+        
+        logger.log_it(e.__str__(), "ERROR")
+        
+        logger.log_it("kmerdb encountered a type error and needs to exit", "ERROR")
+        
         raise TypeError("Incorrect dtype detected in metadata structure. Internal error.")
     
     try:
         jsonschema.validate(instance=metadata, schema=config.graph_schema)
     except jsonschema.ValidationError as e:
-        logger.debug(e)
-        logger.error("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML")
-        raise e
+        logger.log_it(e.__str__(), "ERROR")
 
-    logger.debug("Validation complete.")
+        
+        logger.log_it("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML", "ERROR")
+
+        
+        raise e
 
+    logger.log_it("Validation complete.", "DEBUG")
     
-    sys.stderr.write("\n\n\tCompleted summation and metadata aggregation across all inputs...\n\n")
+    logger.log_it("\n\n\tCompleted summation and metadata aggregation across all inputs...\n\n", "INFO")
 
 
 
     """
     ACCUMULATE ALL EDGE WEIGHTS ACROSS ALL FILES
     """
     """
     task 1: initialize the final edge datastructure, a hashmap, keyed on a pair of k-mer ids, and containing only an integer weight
     """
+
+
+
+
+
+    step = 3
+
+
+
+    
     # Initialize empty data structures
     all_edges_in_kspace = {}
     n1 = []
     n2 = []
     weights = []
     # Loop over the input files and initialize the dictionary on the valid pairs, setting them to 0.
     for d in data:
@@ -1384,15 +1618,15 @@
         edges, h, counts, nullomers = d
         pair_ids = edges.keys()
         
         for p in pair_ids:
             try:
                 all_edges_in_kspace[p] += edges[p]
             except KeyError as e:
-                logger.error("Unknown edge detected, evaded prepopulation. Internal error.")
+                logger.log_it("Unknown edge detected, evaded prepopulation. Internal error.", "ERROR")
                 raise e
     """
     task 3: Add edges (2 k-mer ids) and weight to lists for conversion to NumPy array.
     """
     for e in all_edges_in_kspace.keys():
         n1.append(e[0])
         n2.append(e[1])
@@ -1419,41 +1653,48 @@
 
         
     """
     N would be the number of edges, pairs of nodes, and weights.
     """
     N = len(n1)
     
-    logger.debug("Initializing Numpy arrays of {0} uint for the edges and corresponding weight...".format(N))
+    logger.log_it("Initializing Numpy arrays of {0} uint for the edges and corresponding weight...".format(N), "DEBUG")
     n1 = np.array(n1, dtype=metadata["n1_dtype"])
     n2 = np.array(n2, dtype=metadata["n2_dtype"])
     weights = np.array(weights, dtype=metadata["weights_dtype"])
-    logger.info("Initialization of profile completed, using approximately {0} bytes per array".format(n1.nbytes))
+    logger.log_it("Initialization of profile completed, using approximately {0} bytes per array".format(n1.nbytes), "INFO")
 
     """
     Write the YAML metadata header to the .kdbg file
     """
     yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
     sys.stderr.write(yaml.dump(metadata, sort_keys=False))
 
     sys.stderr.write("\n\n\n")
-    logger.info("Wrote metadata header to .kdbg...")
+    
+    logger.log_it("Wrote metadata header to .kdbg...", "INFO")
+    
 
     
     """
     Cause pandas isn't edge-y enough.
     """
     # Convert the list of numpy arrays (the uint64 3-tuple of the edge) to pandas dataframe
     #df = pd.DataFrame(twoD_weighted_edge_list)
     #df.to_csv(sys.stdout, sep=arguments.output_delimiter, index=False)
 
 
     """
     Write the dataset (weighted edge list) to a file with '.kdbg' as its suffix.
     """
+
+
+    feature = 2
+    step = 4
+    
     kdbg_out = graph.open(arguments.kdbg, mode='wb', metadata=metadata)
     
     try:
         sys.stderr.write("\n\n\nWriting edge list to {0}...\n\n\n".format(arguments.kdbg))
         for i, node1 in enumerate(n1):
             
             node2 = n2[i]
@@ -1486,15 +1727,15 @@
         sys.stderr.write("="*30 + "\n")
         sys.stderr.write(".kdbg stats:\n")
         sys.stderr.write("-"*30 + "\n")
         sys.stderr.write("Edges in file:  {0}\n".format(N))
         sys.stderr.write("Non-zero weights: {0}\n".format(int(np.count_nonzero(weights))))
         sys.stderr.write("\nDone\n")
 
-    logger.info("Done printing weighted edge list to .kdbg")
+    logger.log_it("Done printing weighted edge list to .kdbg", "INFO")
 
     sys.stderr.write(config.DONE)
 
     
             
 def profile(arguments):
     """
@@ -1520,63 +1761,94 @@
     from multiprocessing import Pool
     import json
     import time
     import numpy as np
     from kmerdb import parse, fileutil, kmer, util
     from kmerdb.config import VERSION
 
-    logger.debug("Printing entire CLI argparse option Namespace...")
-    logger.debug(arguments)
+    global logger
+    global feature
+    global step
+
+
+    step = 0
+    feature = 0
+    
+    logger.log_it("Printing entire CLI argparse option Namespace...", "DEBUG")
+    logger.log_it(str(arguments), "DEBUG")
 
     # The number of specified processors should be available
-    logger.debug("Validating processor count for parallelization...")
+    logger.log_it("Validating processor count for parallelization...", "DEBUG")
     if arguments.parallel <= 0 or arguments.parallel > cpu_count()+1:
         raise argparse.ArgumentError("-p, --parallel must be a valid processor count.")
 
     # The extension should be .kdb because I said so.
-    logger.info("Checking extension of output file...")
+    logger.log_it("Checking extension of output file...", "INFO")
     if os.path.splitext(arguments.kdb)[-1] != ".kdb":
         raise IOError("Destination .kdb filepath does not end in '.kdb'")
 
 
 
 
     file_metadata = []
     total_kmers = 4**arguments.k # Dimensionality of k-mer profile
     N = total_kmers
     theoretical_kmers_number = N
 
-    logger.info("Parsing {0} sequence files to generate a composite k-mer profile...".format(len(list(arguments.seqfile))))
+    logger.log_it("Parsing {0} sequence files to generate a composite k-mer profile...".format(len(list(arguments.seqfile))), "INFO")
     nullomers = set()
     # Initialize arrays
     
+    # kmerdb.parse.Parseable
+
+    infile = parse.Parseable(arguments, logger=logger) #
+
+    feature += 1
+    step += 1
+
+    
+    logger.log_it("Processing {0} fasta/fastq files across {1} processors...".format(len(list(arguments.seqfile)), arguments.parallel), "INFO")
+    
+    logger.log_it("Parallel (if specified) mapping the kmerdb.parse.parsefile() method to the seqfile iterable", "DEBUG")
+    
+    logger.log_it("In other words, running the kmerdb.parse.parsefile() method on each file specified via the CLI", "DEBUG")
+
+    """
+    This is .fa/.fq parsing. It is delegated to the parse.Parseable class for argument intake, which then refers to the module-level method
+    'parsefile', not to be confused with parse.Parseable.parsefile, which simply executes the parsefile function on behalf of the wrapper class
+    'Parseable' such that the function may be used with 'multiprocessing.Pool'
+    """
 
-    infile = parse.Parseable(arguments) #
 
     
-    logger.info("Processing {0} fasta/fastq files across {1} processors...".format(len(list(arguments.seqfile)), arguments.parallel))
-    logger.debug("Parallel (if specified) mapping the kmerdb.parse.parsefile() method to the seqfile iterable")
-    logger.debug("In other words, running the kmerdb.parse.parsefile() method on each file specified via the CLI")
+    
     if arguments.parallel > 1:
         with Pool(processes=arguments.parallel) as pool:
             data = pool.map(infile.parsefile, arguments.seqfile)
     else:
         data = list(map(infile.parsefile, arguments.seqfile))
 
-    # 'data' is now a list of 4-tuples
+        
+    # the actual 'data' is now a list of 4-tuples
     # Each 4-tuple represents a single file
     # (edges, header_dictionary<dict>, nullomers<list>, all_kmer_metadata<list>)
 
     # Construct a final_counts array for the composite profile across all inputs
 
 
+
+    
+
+    
+    step += 1
     counts = np.zeros(N, dtype="uint64")
     # Complete collating of counts across files
     # This technically uses 1 more arrray than necessary 'final_counts' but its okay
-    logger.info("Summing counts from individual fasta/fastq files into a composite profile...")
+    logger.log_it("Summing counts from individual fasta/fastq files into a composite profile...", "INFO")
+    
     for d in data:
         counts = counts + d[0]
 
     sys.stderr.write("\n\n\tCompleted summation and metadata aggregation across all inputs...\n\n")
     # unique_kmers = int(np.count_nonzero(counts))
     # #total_nullomers = total_kmers - unique_kmers
 
@@ -1590,22 +1862,33 @@
     3/20/24
     *Massive* nullomer and count validation regression.
     """
 
     """
     Summary statistics and metadata structure
     """
-
+    step +=1
+    feature += 1
+    
     nullomer_ids = []
     counts = []
     file_metadata = []
     for d in data:
         nullomer_ids.extend(d[2])
         counts.extend(d[0])
         file_metadata.append(d[1])
+
+        # Extract the *new* logs from parse.parsefile
+        newlogs = d[3]
+        for line in newlogs:
+            try:
+                logger.logs.index(line)
+            except ValueError as e:
+                logger.logs.append(line)
+
     
     all_observed_kmers = int(np.sum(counts))
     unique_nullomers = len(set(nullomer_ids))
     unique_kmers = int(np.count_nonzero(counts))
 
     
     # Key assertion
@@ -1622,16 +1905,18 @@
     # # 
     # unique_kmers = int(np.sum(list(map(lambda h: h["unique_kmers"], file_metadata))))
 
     # assert unique_kmers + unique_nullomers == N, "kmerdb | internal error: unique nullomers ({0}) + unique kmers ({1}) should equal 4^k = {2} (was {3})".format(unique_nullomers, unique_kmers, N, unique_kmers + unique_nullomers)
     
     # all_observed_kmers = int(np.sum(counts))
 
-    logger.info("Initial counting process complete, creating BGZF format file (.kdb)...")
-    logger.info("Formatting master metadata dictionary...")
+    logger.log_it("Initial counting process complete, creating BGZF format file (.kdb)...", "INFO")
+    
+    logger.log_it("Formatting master metadata dictionary...", "INFO")
+    
 
     metadata=OrderedDict({
         "version": VERSION,
         "metadata_blocks": 1,
         "k": arguments.k,
         "total_kmers": all_observed_kmers,
         "unique_kmers": unique_kmers,
@@ -1648,31 +1933,35 @@
         
     try:
         np.dtype(metadata["kmer_ids_dtype"])
         np.dtype(metadata["profile_dtype"])
         np.dtype(metadata["count_dtype"])
         np.dtype(metadata["frequencies_dtype"])
     except TypeError as e:
-        logger.error(e)
-        logger.error("kmerdb encountered a type error and needs to exit")
+        logger.log_it(e.__str__(), "ERROR")
+
         raise TypeError("Incorrect dtype.")
 
-    logger.debug("Initializing Numpy array of {0} uint zeroes for the final composite profile...".format(total_kmers))
+    logger.log_it("Initializing Numpy array of {0} uint zeroes for the final composite profile...".format(total_kmers), "ERROR")
+    
     kmer_ids = np.array(range(N), dtype=metadata["kmer_ids_dtype"])
     profile = np.array(range(N), dtype=metadata["profile_dtype"])
     counts = np.array(counts, dtype=metadata["count_dtype"])
     frequencies = np.divide(counts, metadata["total_kmers"])
-    logger.info("Initialization of profile completed, using approximately {0} bytes per profile".format(counts.nbytes))
+    
+    logger.log_it("Initialization of profile completed, using approximately {0} bytes per profile".format(counts.nbytes), "INFO")
+    
     yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
     sys.stderr.write(yaml.dump(metadata, sort_keys=False))
 
     
+    step += 1
 
-
-    logger.info("Collapsing the k-mer counts across the various input files into the final kdb file '{0}'".format(arguments.kdb)) 
+    logger.log_it("Collapsing the k-mer counts across the various input files into the final kdb file '{0}'".format(arguments.kdb), "INFO")
+    
     kdb_out = fileutil.open(arguments.kdb, 'wb', metadata=metadata)
     try:
         sys.stderr.write("\n\nWriting outputs to {0}...\n\n".format(arguments.kdb))
 
 
         # Numpy indexing is trash
         #kmer_ids = np.zeros(total_kmers, dtype=metadata["kmer_ids_dtype"])
@@ -1680,41 +1969,49 @@
         #counts = np.zeros(total_kmers, dtype=metadata["count_dtype"])
         #frequencies = np.zeros(total_kmers, dtype=metadata["frequencies_dtype"])
         if arguments.sorted:
 
             kmer_ids_sorted_by_count = np.lexsort(duple_of_arrays)
             reverse_kmer_ids_sorted_by_count = list(kmer_ids_sorted_by_count)
             reverse_kmer_ids_sorted_by_count.reverse()
-            logger.debug("K-mer id sort example: {0}".format(reverse_kmer_ids_sorted_by_count[:30]))
+
+            
+            logger.log_it("K-mer id sort example: {0}".format(reverse_kmer_ids_sorted_by_count[:30]), "INFO")
+
+            
             for i, idx in enumerate(reverse_kmer_ids_sorted_by_count):
 
                 kmer_id = int(kmer_ids[idx])
                 seq = kmer.id_to_kmer(kmer_id, arguments.k)
-                logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_ids[idx], counts[idx], frequencies[idx]))
+                
+                logger.log_it("{0}\t{1}\t{2}\t{3}".format(i, kmer_ids[idx], counts[idx], frequencies[idx]), "INFO")
+
+                
                 c[idx] = counts[idx]
                 f[idx] = frequencies[idx]
                 if arguments.quiet is not True:
                     print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
                 kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_id, c, f))
         else:
             for i, idx in enumerate(kmer_ids):
 
 
                 kmer_id = int(kmer_ids[idx])
                 seq = kmer.id_to_kmer(kmer_id, arguments.k)
                 c = counts[idx]
                 f = frequencies[idx]
 
-                logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
+                logger.log_it("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f), "INFO")
+                
                 if arguments.quiet is not True:
                     print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
                 kdb_out.write("{0}\t{1}\t{2}\t{3}\n".format(i, kmer_id, c, f))
-        logger.info("Wrote 4^k = {0} k-mer counts + neighbors to the .kdb file.".format(total_kmers))
+                
+        logger.log_it("Wrote 4^k = {0} k-mer counts + neighbors to the .kdb file.".format(total_kmers), "INFO")
 
-        logger.info("Done")
             
     finally:
         kdb_out._write_block(kdb_out._buffer)
         kdb_out._handle.flush()
         kdb_out._handle.close()
 
         """
@@ -1730,25 +2027,14 @@
         sys.stderr.write("Theoretical {0}-mer number (4^{0}):     {1}\n".format(arguments.k, theoretical_kmers_number))
         sys.stderr.write("="*30 + "\n")
         sys.stderr.write("\nDone\n")
 
 
     
         
-def get_root_logger(level):
-    levels=[logging.WARNING, logging.INFO, logging.DEBUG]
-    if level < 0 or level > 2:
-        raise TypeError("{0}.get_root_logger expects a verbosity between 0-2".format(__file__))
-    logging.basicConfig(level=levels[level], format="%(levelname)s: %(asctime)s %(funcName)s L%(lineno)s| %(message)s", datefmt="%Y/%m/%d %I:%M:%S")
-    root_logger = logging.getLogger()
-    for name in logging.Logger.manager.loggerDict.keys():
-        if ('boto' in name) or ('urllib3' in name) or ('s3' in name) or ('findfont' in name):
-            logging.getLogger(name).setLevel(logging.WARNING)
-
-    return root_logger
 
 
 def citation_info():
     citation = None
 
     MODULE_ROOT = os.path.dirname(__file__)
     citation_file = os.path.join(MODULE_ROOT,  'CITATION.txt')
@@ -1781,14 +2067,15 @@
 
     return kmerdb_appmap
 
 def cli():
 
     import sys
 
+    from kmerdb import config
 
     
     argv = sys.argv
 
     
     sys.stderr.write("Running kdb script from '{0}'\n".format(__file__))
     sys.stderr.write("Checking installed environment...\n")
@@ -1808,95 +2095,116 @@
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(help="Use --help with sub-commands")
 
 
     profile_parser = subparsers.add_parser("profile", help="Parse data into the database from one or more sequence files")
     profile_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+
     profile_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)")
 
     profile_parser.add_argument("-p", "--parallel", type=int, default=1, help="Shred k-mers from reads in parallel")
 
     # profile_parser.add_argument("--batch-size", type=int, default=100000, help="Number of updates to issue per batch to PostgreSQL while counting")
     # profile_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
     #profile_parser.add_argument("-n", type=int, default=1000, help="Number of k-mer metadata records to keep in memory at once before transactions are submitted, this is a space limitation parameter after the initial block of reads is parsed. And during on-disk database generation")
-
+    profile_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
+    profile_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     profile_parser.add_argument("--keep-db", action="store_true", help=argparse.SUPPRESS)
     #profile_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
     
     #profile_parser.add_argument("--all-metadata", action="store_true", default=False, help="Include read-level k-mer metadata in the .kdb")
     profile_parser.add_argument("--sorted", action="store_true", default=False, help="Sort the output kdb file by count")
     profile_parser.add_argument("--quiet", action="store_true", default=False, help="Do not log the entire .kdb file to stdout")
+    profile_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     #profile_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
 
     profile_parser.add_argument("seqfile", nargs="+", type=str, metavar="<.fasta|.fastq>", help="Fasta or fastq files")
     profile_parser.add_argument("kdb", type=str, help="Kdb file")
     profile_parser.set_defaults(func=profile)
 
     graph_parser = subparsers.add_parser("graph", help="Generate an adjacency list from .fa/.fq files")
     graph_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+
     graph_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)", required=True)
 
     graph_parser.add_argument("-p", "--parallel", type=int, default=1, help="Parallel file reading only.")
-
+    graph_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
+    graph_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     #graph_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
     #graph_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
     graph_parser.add_argument("--quiet", action="store_true", default=False, help="Do not list all edges and neighboring relationships to stderr")
     graph_parser.add_argument("--sorted", action="store_true", default=False, help=argparse.SUPPRESS)
+    graph_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     #graph_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
 
     graph_parser.add_argument("seqfile", nargs="+", type=str, metavar="<.fasta|.fastq>", help="Fasta or fastq files")
     graph_parser.add_argument("kdbg", type=str, help=".kdbg file")
-    graph_parser.set_defaults(func=make_kdbg)
+    graph_parser.set_defaults(func=make_graph)
 
     # assembly_parser = subparsers.add_parser("assemble", help="Use NetworkX (and/or cugraph) to perform deBruijn graphs")
     # assembly_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     # assembly_parser.add_argument("-g", "--gpu", action="store_true", default=False, help="Utilize GPU resources (requires CUDA library cugraph)")
     # assembly_parser.add_argument("kdbg", type=str, help=".kdbg file")
     # assembly_parser.set_defaults(func=assembly)
 
 
     usage_parser = subparsers.add_parser("usage", help="provide expanded usage information on parameters and functions provided")
     usage_parser.add_argument("-m", "--method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), required=True, help="Print expanded usage statement")
     usage_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    usage_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    usage_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
+    usage_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help=argparse.SUPPRESS)
     usage_parser.set_defaults(func=expanded_help)
 
     help_parser = subparsers.add_parser("help", help="provide expanded help section on parameters and functions provided")
     help_parser.add_argument("-m", "--method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), required=True, help="Print expanded usage statement")
     help_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    help_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    help_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
+    help_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help=argparse.SUPPRESS)
     help_parser.set_defaults(func=expanded_help)
     
     
     view_parser = subparsers.add_parser("view", help="View the contents of the .kdb file")
     view_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    view_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    view_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     view_parser.add_argument("-H", "--header", action="store_true", help="Include header in the output")
-    view_parser.add_argument("--re-sort", action="store_true", help="Sort the k-mer profile before displaying")
-    view_parser.add_argument("--un-sort", action="store_true", help="Unsort the k-mer profile before displaying")
+    view_parser.add_argument("--re-sort", action="store_true", help="Sort the k-mer profile before displaying") # FIXME
+    view_parser.add_argument("--un-sort", action="store_true", help="Unsort the k-mer profile before displaying") # FIXME 
     view_parser.add_argument("--dtype", type=str, default="uint64", help="Read in the profiles as unsigned integer 64bit NumPy arrays")
     view_parser.add_argument("-d", "--decompress", action="store_true", help="Decompress input? DEFAULT: ")
     view_parser.add_argument("-c", "--compress", action="store_true", help="Print compressed output")
     view_parser.add_argument("kdb_in", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be read (Optional)")
     view_parser.add_argument("kdb_out", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be written to (Optional)")
     view_parser.set_defaults(func=view)
 
     header_parser = subparsers.add_parser("header", help="Print the YAML header of the .kdb file and exit")
     header_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    header_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    header_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     header_parser.add_argument("-j", "--json", help="Print as JSON. DEFAULT: YAML")
     header_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
     header_parser.set_defaults(func=header)
 
 
     matrix_parser = subparsers.add_parser("matrix", help="Generate a reduced-dimensionality matrix of the 4^k * n (k-mers x samples) data matrix.")
     matrix_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    matrix_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    matrix_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+    matrix_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
+
     matrix_parser.add_argument("-p", "--parallel", type=int, default=1, help="Read files in parallel")
     matrix_parser.add_argument("--with-index", default=False, action="store_true", help="Print the row indices as well")
     matrix_parser.add_argument("--column-names", default=None, type=str, help="A filepath to a plaintext flat file of column names.")
     matrix_parser.add_argument("--delimiter", default="\t", type=str, help="The choice of delimiter to parse the input .tsv with. DEFAULT: '\t'")
     matrix_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write. DEFAULT: '\t'")
-        
+
+
     #matrix_parser.add_argument("--normalize-with", type=str, choices=["ecopy", "DESeq2"], default="DESeq2", help="Normalize with which method? DEFAULT: DESeq2")
     matrix_parser.add_argument("--no-normalized-ints", action="store_true", default=False, help="Don't round normalized counts to the nearest integer")
     matrix_parser.add_argument("-k", default=None, type=int, help="The k-dimension that the files have in common")
     matrix_parser.add_argument("-n", default=None, type=int, help="The number of dimensions to reduce with PCA or t-SNE. DEFAULT: an elbow graph will be generated if -n is not provided to help the user choose -n")
 
     matrix_parser.add_argument("--perplexity", default=5, type=int, help="The choice of the perplexity for t-SNE based dimensionality reduction")
     matrix_parser.add_argument("method", choices=["PCA", "tSNE", "DESeq2", "pass", "Frequency"], default=None, help="Choice of distance metric between two profiles")
@@ -1909,34 +2217,43 @@
     # rarefy_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     # rarefy_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input reduced dimension or simply normalized matrix to use with K-means clustering")
     # rarefy_parser.add_argument("-o", "--output", type=argparse.FileType("w"), default=None, help="THe output csv/tsv of rarefied data")
     # rarefy_parser.set_defaults(func=rarefy)
 
     kmeans_parser = subparsers.add_parser("kmeans", help="Cluster the files according to their k-mer profile")
     kmeans_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    kmeans_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    kmeans_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+    kmeans_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
     kmeans_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter of the input csv/tsv to parse, presumably produced by 'kdb matrix'.")
     kmeans_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     kmeans_parser.add_argument("--distance", type=str, default='e', choices=['e', 'b', 'c', 'a', 'u', 'x', 's', 'k'], help="Different distance metrics offered by kcluster. It is highly advised that you check both this source and their documentation to see how this is implemented.")
 
     
     kmeans_parser.add_argument("-k", default=None, type=int, help="The choice of k for clustering", required=True)
     kmeans_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input reduced dimension or mereley normalized matrix to use with K-means clustering")
     kmeans_parser.add_argument("-o", "--output", type=argparse.FileType("w"), default=None, help="The output csv/tsv with added 'label' to use for graphing in R, if the matplotlib graphs are not sufficient.")
     kmeans_parser.add_argument("method", choices=["sklearn", "Biopython"], default="Biopython", help="The Python implementation of k-means to use. The Biopython method is selected for access to alternative distance metrics")
     kmeans_parser.set_defaults(func=kmeans)
 
     hierarchical_parser = subparsers.add_parser("hierarchical", help="Use scipy.cluster.hierarchy to generate a dendrogram from a distance matrix")
     hierarchical_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    hierarchical_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    hierarchical_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+    hierarchical_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
     hierarchical_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter to use when reading the csv.")
     hierarchical_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input distance matrix for hierarchical clustering")
     hierarchical_parser.add_argument("-m", "--method", type=str, choices=["single", "complete", "average", "weighted", "centroid", "median", "ward"], default="ward", help="The method for linkage fitting in R to use")
     hierarchical_parser.set_defaults(func=hierarchical)
     
     dist_parser = subparsers.add_parser("distance", help="Calculate various distance metrics between profiles")
     dist_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    dist_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    dist_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")        
+    dist_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     dist_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     dist_parser.add_argument("-p", "--parallel", type=int, default=1, help="Read files in parallel")
     dist_parser.add_argument("--column-names", type=str, default=None, help="A filepath to a plaintext flat file of column names.")
     dist_parser.add_argument("--delimiter", type=str, default="\t", help="The delimiter to use when printing the csv.")
     dist_parser.add_argument("-k", default=None, type=int, help="The k-dimension that the files have in common")
     
     dist_parser.add_argument("metric", choices=[
@@ -1966,19 +2283,25 @@
         "yule"], default="correlation", help="Choice of distance metric between two profiles")
     dist_parser.add_argument("input", nargs="*", default=[], metavar="<kdbfile1 kdbfile2 ...|input.tsv|STDIN>", help="Two or more .kdb files, or another count matrix in tsv/csv")
     dist_parser.set_defaults(func=distances)
 
 
     index_parser = subparsers.add_parser("index", help="Create a index file that can be held in memory")
     index_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    index_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    index_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+    index_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     index_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
     index_parser.set_defaults(func=index_file)
 
     shuf_parser = subparsers.add_parser("shuf", help="Create a shuffled .kdb file")
     shuf_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    shuf_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    shuf_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+    shuf_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     shuf_parser.add_argument("kdb_in", type=str, help="An indexed k-mer database file (.kdb)")
     shuf_parser.add_argument("kdb_out", type=str, help="The output shuffled k-mer database file (.kdb)")
     shuf_parser.set_defaults(func=shuf)
 
     
     # markov_probability_parser = subparsers.add_parser("probability", help=u"""
 # Calculate the log-odds ratio of the Markov probability of a given sequence from the product (pi) of the transition probabilities(aij) times the frequency of the first k-mer (P(X1)), given the entire k-mer profile of a species.
@@ -1993,31 +2316,114 @@
     # markov_probability_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
     # markov_probability_parser.add_argument("seqfile", type=str, metavar="<.fasta|.fastq>", default=None, help="Sequences to calculate standard Markov-chain probabilities from, either .fasta or .fastq")
     # markov_probability_parser.add_argument("kdb", type=str, help="An indexed k-mer database file (.kdb)")
     # markov_probability_parser.set_defaults(func=markov_probability)
 
     citation_parser = subparsers.add_parser("citation", help="Silence the citation notice on further runs")
     citation_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    citation_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
+    citation_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     citation_parser.set_defaults(func=citation)
     
     args=parser.parse_args()
     global logger
-    logger = get_root_logger(args.verbose)
+    global exit_code
+
+    
+    global step
+    global feature
+
+    
+    global logs
+
+
 
     sys.stderr.write("Constructed a logger for the program...\n")
     #logger.debug(sys.path)
 
     # Print program header
-
-
+    sys.stderr.write("Starting the program run-time timer...\n\n\n")
+    start = time.time()
 
 
     """
     Print detailed debugging information prior to program log.
     """
+
+
+    #signal.signal(signal.SIGINT, graceful_interrupt)
+    #signal.signal(signal.SIGTERM, graceful_termination)
+    subcommand_name = vars(args)['func'].__name__
+
+
+    from kmerdb import config
+    logger = kdbLogger.Loggah(logfile=args.log_file or None, level=args.verbose)
+        
+
     from kmerdb import appmap
-    kmerdb_appmap = appmap.kmerdb_appmap( argv )
+    kmerdb_appmap = appmap.kmerdb_appmap( argv , logger )
     kmerdb_appmap.print_program_header()
 
-    
-    args.func(args)
-    
+    sys.stderr.write("Beginning program...\n")
+
+
+    if args.debug is True:
+        args.func(args)
+    else:
+        try:
+
+            args.func(args)
+            exit_code = 0
+
+        except TypeError as e:
+
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            exit_code = 1
+        
+            raise e
+        except ValueError as e:
+        
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            exit_code = 2
+        
+            raise e
+        except KeyError as e:
+        
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            exit_code = 3
+        
+            raise e
+        except RuntimeError as e:
+        
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = 4
+        
+            raise e
+        except OSError as e:
+
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = 5
+        
+            raise e
+        except ArgumentError as e:
+        
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = 6
+        
+            raise e
+        except AssertionError as e:
+        
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = 7
+        
+            raise e
+        except Exception as e:
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = -1
+        
+            raise e
+        finally:
+
+            sys.stderr.write("Program ran for {0} seconds...\n\n\n".format(time.time() - start))
+            sys.stderr.write(config.thanks)
+            sys.stderr.write(config.DONE)
+            sys.exit(exit_code)
```

### Comparing `kmerdb-0.7.9/kmerdb/__main__.py` & `kmerdb-0.8.0/kmerdb/__main__.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/appmap.py` & `kmerdb-0.8.0/kmerdb/appmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 '''
 import sys
 import os
 
 import yaml
 from collections import OrderedDict
 
-
-
-
+import jsonschema
 
 
 from kmerdb import config, util
 
 
+
 yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
 
+default_logline_choices = (20, 50, 100, 200)
+PINNED_ISSUES = (132, 133, 137)
+
 PROGRAM_BANNER = """
 **** 
  o-O      |||
 o---O     |||             [|[          kmerdb           ]|]
 O---o     |||
  O-o      |||        version :     v{0}
   O       |||
@@ -128,249 +130,265 @@
  O-o
   O
  o-O
 o---O
 """
 
 GITHUB_PROJECT_BANNER = """
-=======================================================
+==============================================================
                   ||      G i t H u b     ||
-=======================================================
+==============================================================
                          Repo: kmerdb
                Feature branch: graph_algo
+
+Issue Tracker: https://github.com/MatthewRalston/kmerdb/issues
 -------------------------------------------------------
 """
 
 
 
 PINNED_ISSUE = """
-                 Pinned issue: #130
-"""
+                 Pinned issue: {0}
+""".format(", ".join(list(map(str, PINNED_ISSUES))))
 
 
 
 class kmerdb_appmap:
 
 
 
         
 
 
     
-    def __init__(self, argv):
+    def __init__(self, argv, logger=None):
 
+
+        if logger is not None:
+            self.logger = logger
+            self.logfile = logger.logfile
+        else:
+            self.logger = None
+            self.logfile = None
+        self._loggable = logger is not None
+        
+        
         self.MODULE_ROOT = os.path.join("..", os.path.dirname(__file__))
         self.COMMAND_FILE = os.path.join(self.MODULE_ROOT, "__init__.py")
         self.PACKAGE_MANAGER = """
                       package manger : pip
-                        version      : v24.0
+                        version      : >= 24.0
         package root : {0}
         exe file     : {1}
 
                       required packages : {2}
                    development packages : {3}
 
            ARGV : {4}
         """.format(self.MODULE_ROOT, self.COMMAND_FILE, config.requirements_count, config.requirements_dev_count, argv)
         self.REQUIRES_PYTHON = config.REQUIRES_PYTHON
-        self.VERSION_HARDCODED = "                                                                          v :         v{0}\n".format(config.REQUIRES_PYTHON)
+        self.VERSION_HARDCODED = "                                                                          v :      >= v{0}\n".format(config.REQUIRES_PYTHON)
+
 
+        
         #
         # loaded_modules
         #
 
         #
         # dependencies
         #
         #      required:
         #      optional:
 
         # usage_notes.txt
-
-
-        self.GRAPH_BANNER = """
-                          name : graph
-                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
+        
+        self.PROFILE_BANNER = """
+                          name : profile
+                   description : create a k-mer count vector. g-zipped and tallied.
         """
 
-        self.GRAPH_PARAMS = OrderedDict({
+        self.PROFILE_PARAMS = OrderedDict({
             "name": "arguments",
-            "values": [
+            "type": "array",
+            "items": [
                 {
                     "name"  : "k",
-                    "type"  : "int",
-                    "value" : "choice of k-mer size"
-                    },
+                    "type"  : "parameter",
+                    "value" : "choice of k-mer size parameter 'k'",
+                },
+                {
+                    "name" : "sorted",
+                    "type" : "flag",
+                    "value": "descending in k-mer count"
+                },
                 {
                     "name"  : "quiet",
                     "type"  : "flag",
                     "value" : "Write additional debug level information to stderr?"
                 }
             ]
         })
-        
-        
 
-        self.GRAPH_INPUTS = OrderedDict({
+        self.PROFILE_INPUTS = OrderedDict({
             "name": "inputs",
-            "values": [
+            "type": "array",
+            "items": [
                 {
                     "name"  : "<.fasta|.fastq>",
                     "type"  : "array",
                     "value" : "gzipped or uncompressed .fasta or .fastq file(s)"
                 },
                 {
-                    "name"  : ".kdbg",
+                    "name"  : ".kdb",
                     "type"  : "file",
-                    "value" : "edge list."
+                    "value" : "4 column table (row number, index number, k-mer id, count)."
                 }
             ]
         })
 
 
-        self.GRAPH_FEATURES = OrderedDict({
+        self.PROFILE_FEATURES = OrderedDict({
             "name": "features",
             "type": "array",
             "items": [
                 OrderedDict({
-                    "title": "k-mer id arrays organized linearly as file is read through sliding window. (Un)compressed support for .fa/.fq.",
+                    "name": "k-mer id arrays organized linearly as file is read through sliding window. (Un)compressed support for .fa/.fq.",
                     "shortname": "parallel OOP sliding window k-mer shredding",
-                    "description": "a Reader class is instantiated, and invoked on every file, supporting message passing and output collation. The data are read sequentially, so the possible edges for consideration are available by the identity of the k-mer and necessarily its 8 nearest neighbors. The appropriate pair observed in the dataset, and this pair is considered an 'edge' in the edge space constrained under k. It is added to the edge list by virtue of proximity in the file's base vector. In the case of secondary, tertiary, etc. sequences in the .fa or under massively parallel sequencing conditions (such as that by virtue of sequencing-by-synthesis) the offending edge is removed for the beginning and end of each sequence, and a warning is given to the user. Summary statistics for the entire file are given for each file read, as well as a cohesive structure, provided to the user before edge generation begins"
+                    "description": "a Reader class is instantiated, and invoked on every file, supporting message passing and output collation. The data are read sequentially, so a length N = 4^k array is populated from the k-mer counts in the file. A k-mer id and count are recorded in the .kdb file."
                 }),
                 OrderedDict({
-                    "title": "k-mer neighbors assessed and tallied, creates a unsorted edge list, weight weights",
-                    "shortname": "weighted undirected graph",
-                    "description": "an edge list is generated from all k-mers in the forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers in the sequence data are added to the tally of the k-mer nodes of the de Bruijn graph and the edges provided by the data."
+                    "name": "k-mers are tallied, and metadata merged from the input files",
+                    "shortname": "merge counts, metadata from across inputs",
+                    "description": "an final metadata structure and output metrics are collected for display to the user."
                 })
+
             ]
         })
 
 
-        self.GRAPH_STEPS = OrderedDict({
+        self.PROFILE_STEPS = OrderedDict({
             "name": "steps",
             "type": "array",
             "items": [
                 OrderedDict({
                     "name": "read input file(s) from filesystem into k-mer arrays",
                     "shortname": "shred inputs into k-mer count arrays",
                     "description": "shred input sequences into k-mer count vector",
                 }),
                 OrderedDict({
+                    "name": "collate the count array",
+                    "shortname": "collate the count array",
+                    "description": "aggregate counts from different input files"
+                }),
+                OrderedDict({
                     "name": "merge k-mer arrays and aggregate metadata",
                     "shortname": "merge k-mer count arrays for aggregate metadata (header)",
                     "description": "merge counts of nullomers, unique kmers, and total kmers."
                 }),
                 OrderedDict({
-                    "name": "collate the weighted edge list from graph.parsefile's Parser object during parallel file reading. This returns a edge_list, header, counts, and a nullomer_array.",
-                    "shortname": "extract undirected weighted graph",
-                    "description": "consists of info from a .kdb file and a .kdbg file. The node IDs, the edges, and the number of times the pair was observed from forward sequences in the provided dataset"
-                }),
-                OrderedDict({
                     "name": "print 'table' Final stats and close output file",
                     "shortname": "metrics and shutdown",
                     "description": "print final statistics, typically metadata values, and ensure file is closed."
                 })
-                
+
             ]
+
         })
-        
 
-        
-        self.PROFILE_BANNER = """
-                          name : profile
-                   description : create a k-mer count vector. g-zipped and tallied.
+
+
+        self.GRAPH_BANNER = """
+                          name : graph
+                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
         """
 
-        self.PROFILE_PARAMS = OrderedDict({
+        self.GRAPH_PARAMS = OrderedDict({
             "name": "arguments",
-            "values": [
+            "type": "array",
+            "items": [
                 {
                     "name"  : "k",
-                    "type"  : "parameter",
-                    "value" : "choice of k-mer size parameter 'k'",
-                },
-                {
-                    "name" : "sorted",
-                    "type" : "flag",
-                    "value": "descending in k-mer count"
-                },
+                    "type"  : "int",
+                    "value" : "choice of k-mer size"
+                    },
                 {
                     "name"  : "quiet",
                     "type"  : "flag",
                     "value" : "Write additional debug level information to stderr?"
                 }
             ]
         })
+        
+        
 
-        self.PROFILE_INPUTS = OrderedDict({
+        self.GRAPH_INPUTS = OrderedDict({
             "name": "inputs",
-            "values": [
+            "type": "array",
+            "items": [
                 {
                     "name"  : "<.fasta|.fastq>",
                     "type"  : "array",
                     "value" : "gzipped or uncompressed .fasta or .fastq file(s)"
                 },
                 {
-                    "name"  : ".kdb",
+                    "name"  : ".kdbg",
                     "type"  : "file",
-                    "value" : "4 column table (row number, index number, k-mer id, count)."
+                    "value" : "edge list."
                 }
             ]
         })
 
 
-        self.PROFILE_FEATURES = OrderedDict({
+        self.GRAPH_FEATURES = OrderedDict({
             "name": "features",
             "type": "array",
             "items": [
                 OrderedDict({
-                    "title": "k-mer id arrays organized linearly as file is read through sliding window. (Un)compressed support for .fa/.fq.",
+                    "name": "k-mer id arrays organized linearly as file is read through sliding window. (Un)compressed support for .fa/.fq.",
                     "shortname": "parallel OOP sliding window k-mer shredding",
-                    "description": "a Reader class is instantiated, and invoked on every file, supporting message passing and output collation. The data are read sequentially, so a length N = 4^k array is populated from the k-mer counts in the file. A k-mer id and count are recorded in the .kdb file."
+                    "description": "a Reader class is instantiated, and invoked on every file, supporting message passing and output collation. The data are read sequentially, so the possible edges for consideration are available by the identity of the k-mer and necessarily its 8 nearest neighbors. The appropriate pair observed in the dataset, and this pair is considered an 'edge' in the edge space constrained under k. It is added to the edge list by virtue of proximity in the file's base vector. In the case of secondary, tertiary, etc. sequences in the .fa or under massively parallel sequencing conditions (such as that by virtue of sequencing-by-synthesis) the offending edge is removed for the beginning and end of each sequence, and a warning is given to the user. Summary statistics for the entire file are given for each file read, as well as a cohesive structure, provided to the user before edge generation begins"
                 }),
                 OrderedDict({
-                    "title": "k-mers are tallied, and metadata merged from the input files",
-                    "shortname": "merge counts, metadata from across inputs",
-                    "description": "an final metadata structure and output metrics are collected for display to the user."
+                    "name": "k-mer neighbors assessed and tallied, creates a unsorted edge list, weight weights",
+                    "shortname": "weighted undirected graph",
+                    "description": "an edge list is generated from all k-mers in the forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers in the sequence data are added to the tally of the k-mer nodes of the de Bruijn graph and the edges provided by the data."
                 })
-
             ]
         })
 
 
-        self.PROFILE_STEPS = OrderedDict({
+        self.GRAPH_STEPS = OrderedDict({
             "name": "steps",
             "type": "array",
             "items": [
                 OrderedDict({
                     "name": "read input file(s) from filesystem into k-mer arrays",
                     "shortname": "shred inputs into k-mer count arrays",
                     "description": "shred input sequences into k-mer count vector",
                 }),
                 OrderedDict({
                     "name": "merge k-mer arrays and aggregate metadata",
                     "shortname": "merge k-mer count arrays for aggregate metadata (header)",
                     "description": "merge counts of nullomers, unique kmers, and total kmers."
                 }),
                 OrderedDict({
-                    "name": "collate the count array",
-                    "shortname": "collate the count array",
-                    "description": "aggregate counts from different input files"
+                    "name": "collate the weighted edge list from graph.parsefile's Parser object during parallel file reading. This returns a edge_list, header, counts, and a nullomer_array.",
+                    "shortname": "extract undirected weighted graph",
+                    "description": "consists of info from a .kdb file and a .kdbg file. The node IDs, the edges, and the number of times the pair was observed from forward sequences in the provided dataset"
                 }),
                 OrderedDict({
                     "name": "print 'table' Final stats and close output file",
                     "shortname": "metrics and shutdown",
                     "description": "print final statistics, typically metadata values, and ensure file is closed."
                 })
-
+                
             ]
-
         })
-
-
+        
         
         self.MATRIX_BANNER = """
                           name : matrix
                    description : create a k-mer array as a matrix/data-frame. tsv to stdout and/or output file.
         """
         
         self.MATRIX_PARAMS = OrderedDict({
@@ -471,14 +489,19 @@
                         "description": "Uses scipy t-SNE to apply dimensionality reduction on input matrix"
                     }),
                     OrderedDict({
                         "name": "Apply DESeq-2 'median-of-ratios' count normalization",
                         "shortname": "DESeq-2 normalize",
                         "description": "Uses rpy2 to call the R server and pass the data matrix for DESeq-2 normalization"
 
+                    }),
+                    OrderedDict({
+                        "name": "pass unnormalized counts",
+                        "shortname": "unnormalized data",
+                        "description": "Passes the unnormalized data in Data Frame tsv format to STDOUT/file"
                     })
 
                 ]
 
         })
 
     
@@ -567,14 +590,47 @@
                         "shortname": "distance matrix generation",
                         "description": "Use input data matrix to create a distance matrix, produced by SciPy and a choice of distance method"
                     })
 
                 ]
 
         })
+
+
+
+        
+        self.ALL_PARAMS = {
+            "profile": self.PROFILE_PARAMS["items"],
+            "make_graph": self.GRAPH_PARAMS["items"],
+            "get_matrix": self.MATRIX_PARAMS["items"],
+            "distance": self.DISTANCE_PARAMS["items"]
+        }
+
+        self.ALL_INPUTS = {
+            "profile": self.PROFILE_INPUTS["items"],
+            "make_graph": self.GRAPH_INPUTS["items"],
+            "get_matrix": self.MATRIX_INPUTS["items"],
+            "distance": self.DISTANCE_INPUTS["items"]
+        }
+
+        self.ALL_FEATURES = {
+            "profile": self.PROFILE_FEATURES["items"],
+            "make_graph": self.GRAPH_FEATURES["items"],
+            "get_matrix": self.MATRIX_FEATURES["items"],
+            "distance": self.DISTANCE_FEATURES["items"]
+        }
+
+
+        self.ALL_STEPS = {
+            "profile": self.PROFILE_STEPS["items"],
+            "make_graph": self.GRAPH_STEPS["items"],
+            "get_matrix": self.MATRIX_STEPS["items"],
+            "distance": self.DISTANCE_STEPS["items"]
+        }
+        
         # KMEANS_BANNER = """
         #                   name : kmeans
         #            description : 
         # """
 
         # HIERARCHICAL_BANNER = """
 
@@ -592,178 +648,299 @@
         sys.stderr.write(INTERPRETER)
         sys.stderr.write(self.VERSION_HARDCODED)
         sys.stderr.write(self.PACKAGE_MANAGER)
 
         # Spacer
         sys.stderr.write(DNA_COLUMN_1)
 
+        sys.stderr.write(THREE_LINES)
+
     def print_graph_header(self):
 
         
         sys.stderr.write(self.GRAPH_BANNER)
+
+        sys.stderr.write(THREE_LINES)
         
         sys.stderr.write(yaml.dump(self.GRAPH_PARAMS))
-
+        
+        sys.stderr.write(THREE_LINES)
+        
         sys.stderr.write(yaml.dump(self.GRAPH_INPUTS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.GRAPH_FEATURES))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.GRAPH_STEPS))
 
+        # Spacer
+        sys.stderr.write(DNA_COLUMN_1)
+
+        sys.stderr.write(THREE_LINES)
+
+
     def print_profile_header(self):
         
         sys.stderr.write(self.PROFILE_BANNER)
+
+        sys.stderr.write(THREE_LINES)
             
         sys.stderr.write(yaml.dump(self.PROFILE_PARAMS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.PROFILE_INPUTS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.PROFILE_FEATURES))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.PROFILE_STEPS))
 
+        # Spacer
+        sys.stderr.write(DNA_COLUMN_1)
+        
+        sys.stderr.write(THREE_LINES)
+
+
     def print_matrix_header(self):
 
         sys.stderr.write(self.MATRIX_BANNER)
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.MATRIX_PARAMS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.MATRIX_INPUTS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.MATRIX_FEATURES))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.MATRIX_STEPS))
 
+        # Spacer
+        sys.stderr.write(DNA_COLUMN_1)
+
+        sys.stderr.write(THREE_LINES)
+
 
     def print_distance_header(self):
 
         sys.stderr.write(self.DISTANCE_BANNER)
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.DISTANCE_PARAMS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.DISTANCE_INPUTS))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.DISTANCE_FEATURES))
 
+        sys.stderr.write(THREE_LINES)
+
         sys.stderr.write(yaml.dump(self.DISTANCE_STEPS))
 
+        # Spacer
+        sys.stderr.write(DNA_COLUMN_1)
 
 
 
 
 
-# #
-# #          logger and selected log lines
-# #
 
 
-# # LOGGER BANNER + SPACER
 
+    def print_github_block(self):
 
 
 
-# #               POST_LOG_HEADER
-# #
+        sys.stderr.write(THREE_LINES)
+        
+        sys.stderr.write(DNA_SPACER_1)
 
-# PROFILE_BANNER = """
-# =======================================================
-#                ||     p r o f i l e     ||
-# =======================================================
-#                     inputs  : 
-#                     outputs :
-#                  output_dir :
-#                     logfile :
-#               relevant_loc  :     # an hash of value: documentation strings and lines-of-code(loc) given a feature or error.
-#            relevant_issues  : 
+        sys.stderr.write(THREE_LINES)
 
+        sys.stderr.write(GITHUB_LOGO)
 
+        sys.stderr.write(THREE_LINES)
 
-#                  parameters : {0}
-# -------------------------------------------------------
+        sys.stderr.write(GITHUB_PROJECT_BANNER)
 
-# PARAMS_YAML:
+        sys.stderr.write(PINNED_ISSUE)
 
+        sys.stderr.write(THREE_LINES)
 
-# parameters : [
-#  - param1 (DEFAULT: SOME_DEFAULT_VALUE, type=) : 
-#  - param2 (some_functionality)  :
+        sys.stderr.write(DNA_SPACER_1)
 
+        sys.stderr.write(THREE_LINES)
 
-# -------------------------------------------------------
+        
+        
 
-# """
-# HEADER_BANNER =
-# VIEW_BANNER =
-# MATRIX_BANNER =
-# DISTANCE_BANNER =
-# GRAPH_BANNER = 
-# KMEANS_BANNER =
-# HIERARCHICAL_BANNER = 
+    def exit_gracefully(self, e:Exception, subcommand:str=None, step:int=None, feature:int=None, logs:list=None, n_logs:int=None):
+        """
+        We need to handle exit gracefully. The 'step' and 'feature' categories/flags/ints are passed from __init__ or down its callstack to 
+        """
+        import traceback
+        
 
+        if e is None:
+            raise ValueError("Need an error to exit")
+        elif not isinstance(e, Exception):
+            raise ValueError("Need an error to exit")
 
-# # From usage-notes (include description
-# #
-# # parameters:
-# #      - (short), (long), type, description, examples, help 
-# #      - ...
-# #      -
-# #
+        
+        if n_logs is None or type(n_logs) is not int:
+            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument n_logs to be a int")
+        elif logs is None or type(logs) is not list:
+            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument logs to be a list")
+        elif feature is not None and type(feature) is not int:
+            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument feature to be a int")
+        elif step is not None and type(step) is not int:
+            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument step to be a int")
+        elif subcommand is not None and type(subcommand) is not str:
+            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument subcommand to be a str")
+
+
+
+        
+        N = len(logs) 
+        loggable_line = N
+        assert subcommand in config.subcommands, "Unknown subcommand"
+
+
+
+
+        
+
+        # This is the "Error blocks" metadata
+        exit_summary = OrderedDict({
+            "subcommand": subcommand,
+            "kmerdb-version": config.VERSION,
+            "python-version": config.REQUIRES_PYTHON,
+            "feature": feature,
+            "feature_name": self.ALL_FEATURES[subcommand][feature]["name"],
+            "feature_shortname": self.ALL_FEATURES[subcommand][feature]["shortname"],
+            "feature_description": self.ALL_FEATURES[subcommand][feature]["description"],
+            "step" : step,
+            "step_name": self.ALL_STEPS[subcommand][step]["name"],
+            "step_shortname": self.ALL_STEPS[subcommand][step]["shortname"],
+            "step_description": self.ALL_STEPS[subcommand][step]["description"],
+            # The *total* number of logged lines produced by the program and returned to the global 'logs' var in __init__.py
+            "log_file": self.logfile,
+            "traceback": str(traceback.extract_tb(e.__traceback__)),
+            "last_logged_line": loggable_line, 
+            "error": e.__str__(),
+        })
 
 
-# # ISO-8601
-# RUNTIME
+        yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
+        
 
+        try:
+            jsonschema.validate(instance=exit_summary, schema=config.exit_summary_schema)
+        except jsonschema.ValidationError as e:
+            sys.stderr.write("Failed to validate the exit summary. Internal Error.\n")
+            raise e
+                
 
-# LOGFILE
 
-# EXIT_CODE
 
-# TRACEBACK
 
-# # caught exception
-# LOGGABLE_LINE
 
 
-# # 20, 50, 100, 200 -n
-# LAST_N_LINES_OF_LOG
 
+        self.print_github_block()
+
+        """
+        Print last n lines of log
+        """
+        for i in range(n_logs):
+
+            try:
+                if self._loggable:
+                    sys.stderr.write("{0} - last line of log\n".format(n_logs - i))
+                    self.logger.log_it(logs[i], "ERROR")
+                else:
+                    sys.stderr.write("{0} - last line of log\n".format(n_logs - i))
+                    sys.stderr.write(logs[i], "ERROR")
+            except Exception as e:
+                raise e
+                
+        sys.stderr.write("-" * 80 + "\n")
+        if self._loggable:
+            
+            self.logger.log_it("...displaying last {0} lines of the log. Please see '{1}' for more details...".format(n_logs, self.logfile), "ERROR")
+            self.logger.log_it(e.__str__())
 
+            sys.stderr.write(THREE_LINES)
 
-# METADATA # [metadata] via YAML representer, key indices, key/values, last program stage
-# METADATA_VALUES_DESCRIPTIONS # Just simple key-value descriptions
+            sys.stderr.write(DNA_SPACER_1)
 
+            sys.stderr.write(THREE_LINES)
 
-# METADATA_SCHEMA_TXT # Use YAML representer...
-# METADATA_SCHEMA_DESCRIPTION # What the loops, maps, conditionals/branches, and data structure validation mean in this data structure, how it changes, where invalid scenarios may be involved, which test datasets to use and test command.
-# SCHEMA_COUNT = "                      schema count: {0}".format(schemas_count)
+            self.logger.log_it("="*40 + "\n", "ERROR")
 
+            self.logger.log_it(" "*20 + "ERROR: Program exit summary:\n", "ERROR")
+            
+            self.logger.log_it("="*40 + "\n", "ERROR")
+            
+            self.logger.log_it("\n" + yaml.dump(exit_summary), "ERROR")
 
-# PROGRAM_STAGE_HEADER = """
-# ========================================================
+            self.logger.log_it("="*40 + "\n")
 
-#            s t a g e : 1,2,3,...
+            sys.stderr.write(THREE_LINES)
+            
+            
+        else:
+            sys.stderr.write("...displaying last {0} lines of the log. Please see '{1}' for more details...\n".format(n_logs, self.logfile))
+            sys.stderr.write(e.__str__())
 
-# ========================================================
+            sys.stderr.write(THREE_LINES)
 
-#              name     :
-#          description  :
+            sys.stderr.write(DNA_SPACER_1)
 
-#                          LOREM IPSUM
-# """
+            sys.stderr.write(THREE_LINES)
 
-# TYPES_OF_ERRORS = """
-#               name: error1
-#       title   : something_descriptive_for_example
-#           description :
+            sys.stderr.write("="*40 + "\n\n")
 
-#                  LOREM IPSUM
+            sys.stderr.write(" "*20 + "ERROR: Program exit summary:\n\n")
+            
+            sys.stderr.write("="*40 + "\n")
+            
+            sys.stderr.write("\n" + yaml.dump(exit_summary) + "\n")
+
+            sys.stderr.write("="*40 + "\n")
+
+            sys.stderr.write(THREE_LINES)
+
+
+
+            
+        return exit_summary
+
+
+# #
+# #          logger and selected log lines
+# #
 
-#           related_issues : (N/A) 133, 132, 101
-#                  exit_codes : 1, 2, 3, ...etc.,
-# """
```

### Comparing `kmerdb-0.7.9/kmerdb/banners.py` & `kmerdb-0.8.0/kmerdb/banners.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/distance.c` & `kmerdb-0.8.0/kmerdb/distance.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include"
+            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "kmerdb.distance",
         "sources": [
             "kmerdb/distance.pyx"
         ]
     },
     "module_name": "kmerdb.distance"
@@ -1674,177 +1674,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1877,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18030,261 +18030,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18293,29 +18293,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18326,15 +18326,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18343,29 +18343,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18376,15 +18376,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18393,29 +18393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18426,15 +18426,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18443,29 +18443,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18476,15 +18476,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18493,29 +18493,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18526,217 +18526,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18752,15 +18752,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18768,68 +18768,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18837,15 +18837,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18860,15 +18860,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18884,15 +18884,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18900,68 +18900,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18969,15 +18969,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18992,15 +18992,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19016,15 +19016,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19032,68 +19032,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19101,15 +19101,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19124,170 +19124,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22077,26 +22077,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `kmerdb-0.7.9/kmerdb/distance.pyx` & `kmerdb-0.8.0/kmerdb/distance.pyx`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/fileutil.py` & `kmerdb-0.8.0/kmerdb/fileutil.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,18 +37,22 @@
 from Bio import SeqIO, bgzf
 
 #sys.path.append('..')
 
 from kmerdb import kmer, util, config
 
 # Logging configuration
-import logging
-logger = logging.getLogger(__file__)
+global logger
+logger = None
+
+
 # S3 configuration
-s3prefix = "s3://"
+#s3prefix = "s3://"
+
+
 
 
 is_integer = re.compile("^[-+]?[0-9]+$")
 findall_float = re.compile(r"[-+]?(?:\d*\.\d+|\d+)")
 
 def is_all_fasta(filenames):
     """Tests if all the strings in a list are fasta format.
@@ -73,68 +77,68 @@
 
     :param num: Check if a string is a float, or could be converted to a float
     :type num: str
     :returns: Whether or not the string can be parsed as a float
     :rtype: bool
     """
     if type(num) is str:
-        logger.debug("Type of number being interpreted through pure Python : {0}".format(type(num)))
+        #logger.debug("Type of number being interpreted through pure Python : {0}".format(type(num)))
         findall_float.match(num)
-        logger.debug(re.match(findall_float, num))
+        #logger.debug(re.match(findall_float, num))
         return re.match(findall_float, num) is not None
     elif type(num) is float:
         return True
     elif type(num) is int:
         return False
     else:
-        logger.error(type(num))
+        #logger.error(type(num))
         #logger.error(num.dtype)
         raise TypeError("kmerdb.fileutil.isfloat expects a single str as a positional argument")
 
 
-def _s3_file_download(self, seqpath, temporary=True):
-    """
-    Note: the file will be downloaded into a temporary file that needs to be deleted afterwards
-    It will create the temporary file with respect to the TMP bash variable 'export TMP=/some/temporary/location'
-    :param seqpath: The s3 identifier of a object. 's3://bucket/example.fasta'
-    :type seqpath: str
-    :returns: The location of a downloaded gennomic Fasta file
-    :rtype: str
-    """
-    import boto3
-    s3 = boto3.resource('s3')
-    s3client = boto3.client('s3')
+# def _s3_file_download(self, seqpath, temporary=True):
+#     """
+#     Note: the file will be downloaded into a temporary file that needs to be deleted afterwards
+#     It will create the temporary file with respect to the TMP bash variable 'export TMP=/some/temporary/location'
+#     :param seqpath: The s3 identifier of a object. 's3://bucket/example.fasta'
+#     :type seqpath: str
+#     :returns: The location of a downloaded gennomic Fasta file
+#     :rtype: str
+#     """
+#     import boto3
+#     s3 = boto3.resource('s3')
+#     s3client = boto3.client('s3')
 
 
 
-    if type(seqpath) is not str:
-        raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects a str 'seqpath' as its first positional argument")
-    elif seqpath[0:5] != s3prefix:
-        raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects a s3 object reference its first positional argument. e.g. 's3://bucket/example.txt'")
-    elif type(temporary) is not bool:
-        raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects the keyword argument temporary to be a bool")
-    seqpath = seqpath.lstrip(s3prefix)
-    pathsegs =seqpath.split('/')
-    bucket = pathsegs.pop(0)
-    fname = os.path.basename(seqpath)
-    key = '/'.join(pathsegs)
-    if seqpath[-3:] == ".gz":
-        suffix = '.' + '.'.join(seqpath.split('.')[-2:])
-    else:
-        suffix = path.splitext(seqpath)[1]
-    if temporary is True:
-        filepath = tempfile.NamedTemporaryFile(mode='w+b', suffix=suffix, delete=False)
-        logger.info("Downloading '{0}' => '{1}'...".format(seqpath, filepath.name))
-    else:
-        filepath = open(fname, 'w+b')
-        logger.info("Downloading '{0}' => '{1}'...".format(seqpath, fname))
-    obj = s3.Object(bucket, key)
-    obj.download_fileobj(filepath)
-    filepath.close()
-    return filepath.name
+#     if type(seqpath) is not str:
+#         raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects a str 'seqpath' as its first positional argument")
+#     elif seqpath[0:5] != s3prefix:
+#         raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects a s3 object reference its first positional argument. e.g. 's3://bucket/example.txt'")
+#     elif type(temporary) is not bool:
+#         raise TypeError("kmerdb.fileutil.SeqReader.__s3_file_download expects the keyword argument temporary to be a bool")
+#     seqpath = seqpath.lstrip(s3prefix)
+#     pathsegs =seqpath.split('/')
+#     bucket = pathsegs.pop(0)
+#     fname = os.path.basename(seqpath)
+#     key = '/'.join(pathsegs)
+#     if seqpath[-3:] == ".gz":
+#         suffix = '.' + '.'.join(seqpath.split('.')[-2:])
+#     else:
+#         suffix = path.splitext(seqpath)[1]
+#     if temporary is True:
+#         filepath = tempfile.NamedTemporaryFile(mode='w+b', suffix=suffix, delete=False)
+#         logger.info("Downloading '{0}' => '{1}'...".format(seqpath, filepath.name))
+#     else:
+#         filepath = open(fname, 'w+b')
+#         logger.info("Downloading '{0}' => '{1}'...".format(seqpath, fname))
+#     obj = s3.Object(bucket, key)
+#     obj.download_fileobj(filepath)
+#     filepath.close()
+#     return filepath.name
 
 def parse_line(line):
     """
     Parses a line according to the expected .kdb syntax, and returns the python data types expected as a tuple.
 
     :param line:
     :type line: str
@@ -145,33 +149,33 @@
     if type(line) is not str:
         raise TypeError("kmerdb.fileutil.parse_line expects to a str as its first positional argument")
     elif type(line) is str and line == "":
         return None
     else:
         linesplit = line.rstrip().split("\t")
         if len(linesplit) != 3:
-            logger.error("Full line:\n{0}".format(line))
+            #logger.error("Full line:\n{0}".format(line))
             raise ValueError("kmerdb.fileutil.parse_line() encountered a .kdb line without 3 columns, a violation of the format")
         else:
             kmer_id, count, kmer_metadata = linesplit
             if isfloat(count):
                 kmer_id, count = int(kmer_id), float(count)
             else:
                 kmer_id, count = int(kmer_id), int(count)
             kmer_metadata = yaml.safe_load(kmer_metadata)
             if type(kmer_metadata) is dict:
                 return kmer_id, count, kmer_metadata
             else:
-                logger.error("Improperly formatted k-mer metadata field")
-                logger.error(line)
+                #logger.error("Improperly formatted k-mer metadata field")
+                #logger.error(line)
                 raise ValueError("kmerdb.fileutil.parse_line(): Improperly formatted k-mer metadata field")
 
 
 
-def open(filepath, mode="r", metadata=None, sort:bool=False, slurp:bool=False):
+def open(filepath, mode="r", metadata=None, sort:bool=False, slurp:bool=False, logger=None):
     """
     Opens a file for reading or writing. Valid modes are 'xrwbt'. 'metadata=' is needed when writing/creating.
     Returns a lazy-loading KDBReader object or a KDBWriter object.
     The data may be force loaded with 'slurp=True'
 
     :param filepath:
     :type filepath: str
@@ -192,14 +196,17 @@
         raise TypeError("kmerdb.fileutil.open expects the keyword argument 'mode' to be a str")
     elif ("w" in mode or "x" in mode) and (metadata is None or not isinstance(metadata, OrderedDict)):
         raise TypeError("kmerdb.fileutil.open expects an additional metadata dictionary")
     elif type(sort) is not bool:
         raise TypeError("kmerdb.fileutil.open expects a boolean for the keyword argument 'sort'")
     elif type(slurp) is not bool:
         raise TypeError("kmerdb.fileutil.open expects a boolean for the keyword argument 'slurp'")
+
+
+    
     modes = set(mode)
     if modes - set("xrwbt") or len(mode) > len(modes):
         raise ValueError("invalid mode: {}".format(mode))
 
 
     
     creating = "x" in modes
@@ -210,17 +217,17 @@
 
     if text and binary:
         raise ValueError("can't have text and binary mode at once")
     elif not (creating or reading or writing):
         raise ValueError("must have exactly one or read/write")
 
     if "r" in mode.lower():
-        return KDBReader(filename=filepath, mode=mode, sort=sort, slurp=slurp)
+        return KDBReader(filename=filepath, mode=mode, sort=sort, slurp=slurp, logger=logger)
     elif "w" in mode.lower() or "x" in mode.lower():
-        return KDBWriter(metadata, filename=filepath, mode=mode)
+        return KDBWriter(metadata, filename=filepath, mode=mode, logger=logger)
     else:
         raise ValueError("Bad mode %r" % mode)
 
 
 
 
 
@@ -235,21 +242,38 @@
     :ivar max_cache: int
     :ivar column_dtype: NumPy uint datatype
     :ivar count_dtypes: Numpy uint datatype
     :ivar frequencies_dtype: NumPy float datatype
     :ivar sort: bool
     :ivar slurp: bool
     """
-    def __init__(self, filename:str=None, fileobj:io.IOBase=None, mode:str="r", max_cache:int=100, column_dtype:str="uint64", count_dtypes:str="uint64", frequencies_dtype:str="float64", sort:bool=False, slurp:bool=False):
+    def __init__(self, filename:str=None, fileobj:io.IOBase=None, mode:str="r", max_cache:int=100, column_dtype:str="uint64", count_dtype:str="uint64", frequencies_dtype:str="float64", sort:bool=False, slurp:bool=False, logger=None):
         if fileobj is not None and not isinstance(fileobj, io.IOBase):
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'fileobj' to be a file object")
         elif filename is not None and type(filename) is not str:
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'filename' to be a str")
-        elif type(sort) is not bool:
+        elif sort is None or type(sort) is not bool:
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'sort' to be a bool")
+        elif max_cache is None or type(max_cache) is not int:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'max_cache' to be a int")
+        elif mode is None or type(mode) is not str:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'mode' to be a str")
+        elif column_dtype is None or type(column_dtype) is not str:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'column_dtype' to be a str")
+        elif count_dtype is None or type(count_dtype) is not str:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'count_dtype' to be a str")
+        elif frequencies_dtype is None or type(frequencies_dtype) is not str:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'frequencies_dtype' to be a str")
+        elif slurp is None or type(slurp) is not bool:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'slurp' to be a bool")
+        elif logger is None:
+            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'logger' to be valid")
+
+        
+        
         
         if fileobj:
             assert filename is None
             handle = fileobj
             assert "b" in handle.mode.lower()
         else:
             if "w" in mode.lower() or "a" in mode.lower():
@@ -269,86 +293,99 @@
         self._block_raw_length = None
         self.kmer_ids     = None
         self.counts       = None
         self.frequencies  = None
         self.count_dtype = None
         self.frequencies_dtype = None
         self.kmer_ids_dtype = None
+
+        self.logger = logger
+
+        self._loggable = logger is not None
+        
         '''
         Here we want to load the metadata blocks. We want to load the first two lines of the file: the first line is the version, followed by the number of metadata blocks
         '''
         # 0th block
-        logger.info("Loading the 0th block from '{0}'...".format(self._filepath))
+        if self._loggable:
+            self.logger.log_it("Loading the 0th block from '{0}'...".format(self._filepath), "INFO")
         self._load_block(self._handle.tell())
 
         self._buffer = self._buffer.rstrip(config.header_delimiter)
         
         initial_header_data = OrderedDict(yaml.safe_load(self._buffer))
         num_header_blocks = None
 
         if type(initial_header_data) is str:
-            logger.info("Inappropriate type for the header data.")
+            if self._loggable:
+                self.logger.log_it("Inappropriate type for the header data.", "INFO")
             #logger.info("Um, what the fuck is this in my metadata block?")
             raise TypeError("kmerdb.fileutil.KDBReader could not parse the YAML formatted metadata in the first blocks of the file")
         elif type(initial_header_data) is OrderedDict:
-            logger.info("Successfully parsed the 0th block of the file, which is expected to be the first block of YAML formatted metadata")
-            logger.info("Assuming YAML blocks until delimiter reached.")
+            if self._loggable:
+                self.logger.log_it("Successfully parsed the 0th block of the file, which is expected to be the first block of YAML formatted metadata", "INFO")
+                self.logger.log_it("Assuming YAML blocks until delimiter reached.", "INFO")
             if "version" not in initial_header_data.keys():
                 raise TypeError("kmerdb.fileutil.KDBReader couldn't validate the header YAML")
             elif "metadata_blocks" not in initial_header_data.keys():
                 raise TypeError("kmerdb.fileutil.KDBReader couldn't validate the header YAML")
             else:
-                logger.debug(initial_header_data)
+                if self._loggable:
+                    self.logger.log_it(str(initial_header_data), "INFO")
                 if initial_header_data["metadata_blocks"] == 1:
-                    logger.info("1 metadata block: Not loading any additional blocks")
+                    if self._loggable:
+                        self.logger.log_it("1 metadata block: Not loading any additional blocks", "INFO")
+                    pass
                 else:
                     for i in range(initial_header_data["metadata_blocks"] - 1):
-                        logger.info("Multiple metadata blocks read...")
                         self._load_block(self._handle.tell())
-                        logger.debug("Secondary blocks read")
+                        if self._loggable:
+                            self.logger.log_it("Multiple metadata blocks read...", "DEBUG")
+                            self.logger.log_it("Secondary blocks read", "DEBUG")
                         addtl_header_data = yaml.safe_load(self._buffer.rstrip(config.header_delimiter))
                         if type(addtl_header_data) is str:
-                            logger.error(addtl_header_data)
-                            logger.error("Couldn't determine this block.::/")
+                            if self._loggable:
+                                self.logger.log_it(addtl_header_data, "ERROR")
+                                self.logger.log_it("Couldn't determine this block.::/", "ERROR")
                             raise TypeError("kmerdb.fileutil.KDBReader determined the data in the {0} block of the header data from '{1}' was not YAML formatted".format(i, self._filepath))
                         elif type(addtl_header_data) is dict:
                             sys.stderr.write("\r")
                             sys.stderr.write("Successfully parsed {0} blocks of YAML formatted metadata".format(i))
                             initial_header_data.update(addtl_header_data)
                             num_header_blocks = i
                         else:
-                            logger.error(addtl_header_data)
+                            if self._loggable:
+                                self.logger.log_it(addtl_header_data, "ERROR")
                             raise RuntimeError("kmerdb.fileutil.KDBReader encountered a addtl_header_data type that wasn't expected when parsing the {0} block from the .kdb file '{1}'.".format(i, self._filepath))
         else:
             raise RuntimeError("kmerdb.fileutil.KDBReader encountered an unexpected type for the header_dict read from the .kdb header blocks")
-        logger.info("Reading additional blocks as YAML...")
-        logger.debug("Reading additional blocks as YAML...")
-        sys.stderr.write("\n")
-        logger.info("Validating the header data against the schema...")
+        if self._loggable:
+            self.logger.log_it("Reading additional blocks as YAML...", "INFO")
+            self.logger.log_it("Validating the header data against the schema...", "INFO")
         try:
             jsonschema.validate(instance=initial_header_data, schema=config.kdb_metadata_schema)
             self.metadata = dict(initial_header_data)
             
             self.k = self.metadata['k']
             self.kmer_ids_dtype = self.metadata["kmer_ids_dtype"]
             self.count_dtype = self.metadata["count_dtype"]
             self.frequencies_dtype = self.metadata["frequencies_dtype"]
             self.sorted = self.metadata["sorted"]
-            logger.info("Self assigning dtype to uint64 probably")
-            logger.debug("Checking for metadata inference...")
+            if self._loggable:
+                self.logger.log_it("Self assigning dtype to uint64 probably", "DEBUG")
+                self.logger.log_it("Checking for metadata inference...", "DEBUG")
             self.kmer_ids = np.zeros(4**self.metadata["k"], dtype=self.metadata["kmer_ids_dtype"])
             self.counts = np.zeros(4**self.metadata["k"], dtype=self.metadata["count_dtype"])
             self.frequencies = np.zeros(4**self.metadata["k"], dtype=self.metadata["frequencies_dtype"])
-            logger.info("Squash target this.")
         except jsonschema.ValidationError as e:
-            logger.debug(e)
             logger.error("kmerdb.fileutil.KDBReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks))
             raise e
         self.metadata["header_offset"] = self._handle.tell()
-        logger.debug("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]))
+        if self._loggable:
+            self.logger.log_it("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]), "DEBUG")
         #self._reader = gzip.open(self._filepath, 'r')
         self._offsets = deque()
         for values in bgzf.BgzfBlocks(self._handle):
             #logger.debug("Raw start %i, raw length %i, data start %i, data length %i" % values)
             self._offsets.appendleft(values) # raw start, raw length, data start, data length
         if len(self._offsets) == 0:
             raise IOError("kmerdb.fileutil.KDBReader opened an empty file")
@@ -362,18 +399,18 @@
 
         if sort is True and self.metadata["sorted"] is True:
             sort is True
         else:
             sort is False
 
         if slurp is True:
-            self.slurp(column_dtypes=column_dtype, count_dtypes=count_dtypes, frequencies_dtype=frequencies_dtype, sort=sort)
+            self.slurp(column_dtypes=column_dtype, count_dtypes=count_dtype, frequencies_dtype=frequencies_dtype, sort=sort)
         self.is_int = True
         self.kmer_ids_dtype = column_dtype
-        self.count_dtypes = count_dtypes
+        self.count_dtypes = count_dtype
         self.frequencies_dtype = frequencies_dtype
         handle.close()
         self._handle.close()
         self._handle = None
         handle = None
         fileobj=None
         return
@@ -408,215 +445,175 @@
         elif type(frequencies_dtype) is not str:
             raise TypeError("kmerdb.fileutil.KDBReader.slurp expects the frequencies_dtype keyword argument to be a str")
         try:
             np.dtype(column_dtypes)
             np.dtype(count_dtypes)
             np.dtype(frequencies_dtype)
         except TypeError as e:
-            logger.error(e)
-            logger.error("kmerdb.fileutil.KDBReader.slurp encountered a TypeError while assessing a numpy dtype")
+            if self._loggable:
+                self.logger.log_it(e.__str__(), "ERROR")
+                self.logger.log_it("kmerdb.fileutil.KDBReader.slurp encountered a TypeError while assessing a numpy dtype", "ERROR")
             raise TypeError("kmerdb.fileutil.KDBReader._slurp expects the dtype keyword argument to be a valid numpy data type")
         if type(sort) is not bool:
             raise TypeError("kmerdb.fileutil.KDBReader._slurp expects the sort keyword argument to be a bool")
         if self._handle is None:
             self._handle = _open(self._filepath, 'rb')
         # First calculate the amount of memory required by the array
         N = 4**self.k # The dimension of the k-space, or the number of elements for the array
         num_bytes = 4 * N
-        logger.info("Approximately {0} bytes".format(num_bytes))
+        #logger.info("Approximately {0} bytes".format(num_bytes))
         vmem = psutil.virtual_memory()
         self.kmer_ids = np.zeros(N, dtype=column_dtypes)
         self.counts = np.zeros(N, dtype=count_dtypes)
         self.frequencies = np.zeros(N, dtype=frequencies_dtype)
         self.all_kmer_metadata = []
         kmer_ids = []
         profile = []
         counts = []
         frequencies = []
         if vmem.available > num_bytes:
             # Do the slurp
-            logger.info("Reading profile into memory")
+            if self._loggable:
+                self.logger.log_it("Reading profile into memory", "INFO")
             if sort is False:
                 i = 0
                 try:
                     for j in range(N):
                         #logger.debug("Reading {0}th line...".format(j))
                         try:
                             line = next(self)
                         except StopIteration as e:
-                            logger.error("Finished loading initial profile through slurp-on-init")
-                            logger.error("Read profile from: {0}".format(self._filepath))
+                            if self._loggable:
+                                self.logger.log_it("Finished loading initial profile through slurp-on-init", "ERROR")
+                                self.logger.log_it("Read profile from: {0}".format(self._filepath), "ERROR")
                             raise e
                         if line is None:
-                            logger.warning("Next was None... profile was sparse, breaking")
-                            sys.exit(1)
-                            break
+                            if self._loggable:
+                                self.logger.log_it("'next' was None... Internal Error", "ERROR")
+                            raise RuntimeError("Could not complete parsing of file. Internal Error")
                         # Don't forget to not parse the metadata column [:-1]
 
                         l = line.rstrip().split("\t")
-                        assert len(l) == 5
-                        x, kmer_id, _count, _frequency, kmer_metadata = l
+                        try:
+                            assert len(l) == config.KDB_COLUMN_NUMBER, "kmerdb.fileutil.KDBReader requires .kdb files to have {0} columns.".format(config.KDB_COLUMN_NUMBER)
+                        except AssertionError as e:
+                            self.logger.log_it("Found .kdb table line with {0} columns. Requires {1} columns.".format(l, config.KDB_COLUMN_NUMBER))
+                            self.logger.log_it(line, "ERROR")
+                            raise e
+                            
+                        x, kmer_id, _count, _frequency = l
                         x = int(x)
                         kmer_id = int(kmer_id)                            
-                        logger.debug(line.rstrip())
-
 
                         assert j == x, "Line number did not match"
 
-                        logger.debug("{0}\t{1}\t{2}\t'{3}'".format(x, kmer_id, _count, _frequency))
+                        #self.logger.log_it("{0}\t{1}\t{2}\t'{3}'".format(x, kmer_id, _count, _frequency), "DEBUG")
                         kmer_ids.append(kmer_id)
 
                         if isfloat(_count):
                             parsed_integer_string = is_integer.match(_count)
                             if parsed_integer_string is not None:
-                                logger.info("Casting count field to integer...")
-                                logger.info("Starting count | castin' as int '{0}'".format(_count))
-
                                 count = int(_count)
-                                #logger.warning("Casting count field to integer.")
-                                #raise TypeError("Shouldn't be normal usage. Unsupported")
                             else:
-                                logger.info("Starting count | cast as float '{0}'".format(_count))
                                 count = float(_count)
-                            logger.info("Determining the type of data in the file1...")
-                            logger.info("File counts at {0}, file frequency = {1}".format(count, _frequency))
                         else:
                             parsed_integer_string = is_integer.match(_count)
                             if parsed_integer_string is not None:
-                                logger.info("Casting count field to integer...")
-                                logger.info("Starting count | castin' as int '{0}'".format(_count))
                                 count = int(_count)
-                                #logger.warning("Casting count field to integer.")
-                                #raise TypeError("Shouldn't be normal usage. Unsupported")
                             else:
-                                logger.info("Starting count | IDGAF castin' as int '{0}'".format(_count))
                                 count = int(_count)
-                            logger.info("Determining the type of data in the file2...")
-                            logger.info("File counts at {0}, file frequency = '{1}'".format(count, _frequency))
                         assert type(count) is int, "_slurp | type of count field is not int"
                         frequency = float(count)/N
                         self.kmer_ids[j] = kmer_id
                         self.counts[kmer_id] = count
                         self.frequencies[kmer_id] = _frequency
-                        self.all_kmer_metadata.append(kmer_metadata)
+
                         #sys.stderr.write("::DEBUG::   |\-)(||||..... KMER_ID: {0} COUNT: {1}".format(kmer_id, count))
                         try:
                             if isfloat(_frequency):
-                                logger.debug("Frequency: '{0}'".format(_frequency))
                                 try:
-                                    logger.debug("type: {0}".format(type(_frequency)))
-                                    logger.debug("Using integer matching regex...")
                                     pis = is_integer.match(_frequency)
                                 except TypeError as e:
-                                    logger.error(e)
                                     raise e
                                 if pis is not None:
-                                    logger.warning("Matched frequency as integer: perhaps an error or a genuine zero...Reseting to zero")
+                                    if self._loggable:
+                                        self.logger.log_it("Matched frequency as integer: perhaps an error or a genuine zero...Reseting to zero", "WARNING")
                                     frequency = float(0)
-                                    logger.error("Starting frequency cast as fresh float 0.0 | '{0}'".format(_frequency))
-                                    #raise TypeError("Matched frequency to integer instead of float. Aborting.")
                                 else:
-                                    logger.info("Starting frequency cast as float | '{0}'")
                                     frequency = float(_frequency)
-                                logger.info("Determining type of data in the file3...")
-                                logger.info("It looks like the frequency data is a double. interpretted frequency as {0}, frequency string: '{1}'".format(frequency, _frequency))
                                 assert frequency == float(_frequency), "kmerdb.fileutil.KDBReader._slurp | Frequency did not match expected value based on the count during recalculation of frequencies..."
 
                             else:
                                 parsed_integer_string = is_integer.match(_frequency)
                                 if parsed_integer_string is not None:
-                                    logger.warning("Casting frequency field to integer.")
                                     raise TypeError("Casting frequency field to integer is unsupported.")
                                 else:
-                                    logger.info("Starting frequency | cast as int '{0}'".format(_frequency))
-                                    logger.info("Castin' frequency field to an integer.")
-                                        
                                     frequency = int(count)
-                                logger.info("Determining type of data in the file4...")
-                                logger.info("It looks like the frequency data is an int. python frequency as {0}, frequency string: '{1}'".format(frequency, _frequency))
-                                    #logger.info("It looks like the frequency data is a double. Caclulated frequency at {0}, frequency read: {1}".format(frequency, _frequency))
                                 assert float(frequency) == float(_frequency), "kmerdb.fileutil.KDBReader._slurp | Frequency did not match expected value based on the count during recalculation of frequencies..."
 
 
                         except AssertionError as e:
-                            logger.error(e)
-                            logger.warning("Interpretting string for NumPy formatting")
+                            self.logger.log_it(e.__str__(), "ERROR")
+                            self.logger.log_it("Interpretting string for NumPy formatting", "WARNING")
                             raise e
                         assert type(frequency) is float, "_slurp | frequency field not cast as float"
                         
-                    logger.debug("The {0}th line was kmer-id: {1} with an abundance of {2}".format(j, kmer_id, count))
+                    #self.logger.log_it("The {0}th line was kmer-id: {1} with an abundance of {2}".format(j, kmer_id, count), "DEBUG")
                     i += 1
 
 
                     self.kmer_ids[j] = kmer_id
                     self.counts[kmer_id] = count
                     self.frequencies[kmer_id] = frequency
-                    #self.all_kmer_metadata[i] = kmer_metadata)
+
                 except StopIteration as e:
                     if i == N:
-                        logger.debug("Read {0} lines from the file...".format(i))
-                        logger.warning("StopIteration was raised!!!")
                         raise e
                     else:
-                        logger.error("Number of lines read: {0}".format(i))
-                        logger.error("Number of k-mers (N) set globally.".format(N))
-                        logger.error("Read only {0} lines from the file...".format(i))
-                        logger.error("Profile must have been read before this point")
-                        logger.error(e)
+                        if self._loggable:
+                            self.logger.log_it("Number of lines read: {0}".format(i), "DEBUG")
+                            self.logger.log_it("Number of k-mers (N) set globally.".format(N), "DEBUG")
+                            self.logger.log_it("Read only {0} lines from the file...".format(i), "DEBUG")
+                            self.logger.log_it("Profile must have been read before this point", "DEBUG")
+                            self.logger.log_it(e.__str__(), "ERROR")
                         raise e
                 except Exception as e:
-                    logger.error(e)
                     raise e
-                logger.debug("Validating shape prior to if unsorted is True")
-                logger.debug("Number of lines read: {0}".format(i))
-                logger.debug("Number of k-mer (N) set globally: {0}".format(N))
-                logger.debug("Kmer_ids shape: {0}".format(self.kmer_ids.size))
-                logger.debug("Counts shape: {0}".format(self.counts.size))
-                logger.debug("Frequencies shape: {0}".format(self.frequencies.size))
                 assert self.counts.size == self.kmer_ids.size, "Counts size has diverged from the kmer_ids shape"
                 assert self.counts.size == self.frequencies.size, "Frequencies size has diverged from counts shape"
             elif sort is True:
                 i = 0
                 try:
                     for j in range(N):
                         #logger.debug("Reading {0}th line...".format(j))
                         try:
                             line = next(self)
                         except StopIteration as e:
-                            logger.error("Finished loading initial profile through slurp-on-init")
+                            self.logger.log_it("Finished loading initial profile through slurp-on-init", "ERROR")
                             raise e
                         if line is None:
-                            logger.warning("Next was None... profile was sparse, breaking")
-                            sys.exit(1)
-                            break
-                        # Don't forget to not parse the metadata column [:-1]
+                            self.logger.log_it("Next was None... profile was sparse, breaking", "WARNING")
+                            raise IOError("next method was None on sorted import. Internal Error.")
 
-                        x, kmer_id, _count, _frequency, metadata = line.rstrip().split("\t")
+                        # Don't forget to not parse the metadata column [:-1]
 
-                        logger.debug(line.rstrip())
+                        x, kmer_id, _count, _frequency = line.rstrip().split("\t")
 
-                        logger.debug("{0}\t{1}\t{2}\t{3}".format(j, kmer_id, _count, _frequency))
 
                         _frequency = float(_frequency)
                         kmer_id = int(kmer_id)
 
                         if isfloat(_count):
                             s = findall_float.match(_count)
                             if s is not None:
                                 count = float(_count)
                             else:
                                 raise TypeError("kmerdb.fileutil.KDBReader._slurp | couldn't properly detect float")
                             count = float(_count)
-                            logger.info("Determining the type of data in the file1...")
-                            logger.info("File counts at {0}, file frequency = {1}".format(count, _frequency))
                         else:
-                            logger.info("Determining the type of data in the file2...")
-                            logger.info("File counts at {0}, file frequency = {1}".format(count, _frequency))
-                            logger.debug("kmer_id: {0}, count: {1}, frequency: {2}".format(kmer_id, count, _frequency))
-
                             s = is_integer.match(_count)
                             if s is not None:
                                 count = int(_count)
                             else:
                                 raise TypeError("kmerdb.fileutil.KDBReader._slurp | couldn't properly detect integer")
 
                         frequency = float(count)/N
@@ -627,86 +624,57 @@
                         self.kmer_ids[j] = kmer_id
                         self.counts[kmer_id] = count
                         self.frequencies[kmer_id] = _frequency
                         i+=1
                         #sys.stderr.write("::DEBUG::   |\-)(||||..... KMER_ID: {0} COUNT: {1}".format(kmer_id, count))
                         try:
                             if isfloat(_frequency):
-                                logger.info("Determining type of data in the file3...")
-                                logger.info("It looks like the frequency data is a double. interpretted frequency as {0}, frequency string: '{1}'".format(frequency, _frequency))
                                 assert float(frequency) == float(_frequency), "Frequency did not match expected value based on the count..."
                             else:
-                                logger.info("Determining type of data in the file4...")
-                                logger.info("It looks like the frequency data is a double. python frequency as {0}, frequency string: '{1}'".format(frequency, _frequency))
-                                #logger.info("It looks like the frequency data is a double. Caclulated frequency at {0}, frequency read: {1}".format(frequency, _frequency))
                                 assert float(frequency) == float(_frequency), "Frequency did not match expected value based on the count..."
 
                         except AssertionError as e:
-                            logger.error(e)
-                            logger.warning("Interpretting string for NumPy formatting")
+                            self.logger.log_it(e.__str__(), "ERROR")
+                            self.logger.log_it("Interpretting string for NumPy formatting", "ERROR")
                             raise e
-                    logger.debug("The {0}th line was kmer-id: {1} with an abundance of {2}".format(j, kmer_id, count))
-                    
-
-                    logger.debug("Validating shape prior to if unsorted is True")
-                    logger.debug("Number of lines read: {0}".format(i))
-                    logger.debug("Number of k-mer (N) set globally: {0}".format(N))
-                    logger.debug("Kmer_ids shape: {0}".format(self.kmer_ids.size))
-                    logger.debug("Counts shape: {0}".format(self.counts.size))
-                    logger.debug("Frequencies shape: {0}".format(self.frequencies.size))
                     assert self.kmer_ids.size == self.counts.size, "Counts size has diverged from kmer_ids size/shape"
                     assert self.counts.size == self.frequencies.size, "Frequencies size has diverged from counts shape"
 
                 except StopIteration as e:
                     if i == N:
-                        logger.debug("Read {0} lines from the file...".format(i))
-                        logger.warning("StopIteration was raised!!!")
                         raise e
                     else:
-                        logger.error("Number of lines read: {0}".format(i))
-                        logger.error("Number of k-mers (N) set globally.".format(N))
-                        logger.error("Read only {0} lines from the file...".format(i))
-                        logger.error("Profile must have been read before this point")
-                        logger.error(e)
                         raise e
                 except Exception as e:
-                    logger.error(e)
                     raise e
-                logger.info("Read {0} lines from the file...".format(i))
-                logger.debug("Rechecking shape... I can't help myself.")
+                if self._loggable:
+                    self.logger.log_it("Read {0} lines from the file...".format(i), "INFO")
                 assert self.kmer_ids.size == self.counts.size, "Counts size is mismatched in with kmer_ids size"
                 assert self.frequencies.size == self.counts.size, "Frequencies size is mismatched in count from counts size"
-                logger.debug("Check completed...")            
+                if self._loggable:
+                    self.logger.log_it("Correct array sizes match...", "DEBUG")
                 self._handle.seek(0)
                 self._load_block()
-
-                logger.debug("Dammit, why can't i reset the Bio.bgzf filehandle...")
+                #logger.debug("Dammit, why can't i reset the Bio.bgzf filehandle...")
                 if sort is True:
                     # If the file is sorted, do not sort
                     kmer_ids_sorted_by_count = np.lexsort((self.kmer_ids, self.counts))
                     reverse_kmer_ids_sorted_by_count = np.flipud(kmer_ids_sorted_by_count)
                     for i, idx in enumerate(kmer_ids_sorted_by_count): # This is right, not fixing this.
                         kmer_id = self.kmer_ids[idx]
                         count = self.counts[idx]
 
-                        logger.debug("{0}\t{1}\t{2}\t{3}".format(i, idx,  kmer_id, count))
-                        # I stand corrected
+                        ## I stand corrected. m
                         #self.kmer_ids[i] = kmer_ids[profile[i]]
                         #self.counts[idx] = counts[idx]
                         ###self.frequencies[idx] = frequencies[idx]
-                        logger.debug("Just in casey eggs and bakey...")
+                        #logger.debug("Just in casey eggs and bakey...")
 
             else:
-                logger.debug("Profile has been intiailized as zeros only, incorrect instantiation.")
-                raise RuntimeError("Whoops, something went wrong there")
-                sys.exit(1)
-                                    
-                logger.info("Data types | kmer_ids: {0}, counts: {1}, frequencies: {2}".format(type(self.kmer_ids[0]), type(self.counts[0]), type(self.frequencies[0])))
-                logger.warning("Profile, dickhead, it's already in memory. Dont rerun.")
-                logger.warning("Profile is already loaded in memory! Did you remember to deallocate it when you were done?")
+                raise RuntimeError("Internal error. Failed to initialize array when determining sort strategy")
         else:
             raise OSError("The dimensionality at k={0} or 4^k = {1} exceeds the available amount of available memory (bytes) {2}".format(self.k, N, vmem.available))
         if self.kmer_ids.dtype != self.kmer_ids_dtype:
             raise TypeError("kmerdb.fileutil.KDBReader._slurp encountered an awful TypeError")
         elif self.counts.dtype != self.count_dtype:
             raise TypeError("kmerdb.fileutil.KDBReader._slurp encountered an awful TypeError")
         elif self.frequencies.dtype != self.frequencies_dtype:
@@ -714,23 +682,15 @@
         #self.kmer_ids = np.array(kmer_ids, dtype=suggested_dtype)
         #self.kmer_ids = np.array(kmer_ids, dtype=column_dtypes)
         #self.counts = np.array(counts, dtype=count_dtypes)
         #self.frequencies = np.array(frequencies, dtype=frequencies_dtype)
         self._handle.seek(0)
         self._load_block()
         #print([x for x in np.ndindex(self.kmer_ids.flat) if x < ])
-        logger.info("Data types read from file")
-        logger.info(type(self.kmer_ids[0]))
-        logger.info(type(self.counts[0]))
-        logger.info(type(self.frequencies[0]))
 
-
-        logger.info("Kmer_ids size: {0}".format(self.kmer_ids.size))
-        logger.info("Counts size: {0}".format(self.counts.size))
-        logger.info("Frequencies size: {0}".format(self.frequencies.size))
         assert self.kmer_ids.size == self.counts.size, "Number of Counts is mismatched in count from row-index 'profile'"
         assert self.frequencies.size == self.counts.size, "Number of Frequencies is mismatched in count from row-index 'profile'"
         
         return self.counts
 
     def slurp(self, column_dtypes:str="uint64", count_dtypes:str="uint64", frequencies_dtype:str="float64", sort:bool=False):
         """
@@ -760,26 +720,32 @@
     :ivar metadata: OrderedDict
     :ivar filename: str
     :ivar mode: str
     :ivar fileobj: io.IOBase
     :ivar compresslevel: int
     """
     
-    def __init__(self, metadata:OrderedDict, filename=None, mode="w", fileobj=None, compresslevel=6):
+    def __init__(self, metadata:OrderedDict, filename=None, mode="w", fileobj=None, compresslevel=6, logger=None):
         """Initilize the class."""
+
+        self.logger = logger
+        self._loggable = logger is not None
+
+        
         if not isinstance(metadata, OrderedDict):
             raise TypeError("kmerdb.fileutil.KDBWriter expects a valid metadata object as its first positional argument")
         try:
-            logger.debug("Validating metadata schema against the config.py header schema")
+            if self._loggable:
+                self.logger.log_it("Validating metadata schema against the config.py header schema", "DEBUG")
             jsonschema.validate(instance=dict(metadata), schema=config.kdb_metadata_schema)
             self.metadata = metadata
             self.k = self.metadata['k']
         except jsonschema.ValidationError as e:
-            logger.debug(e)
-            logger.error("kmerdb.fileutil.KDBReader couldn't validate the header YAML")
+            if self._loggable:
+                self.logger.log_it("kmerdb.fileutil.KDBReader couldn't validate the header YAML", "ERROR")
             raise e
 
         if fileobj:
             assert filename is None
             handle = fileobj
         else:
             if "w" not in mode.lower() and "a" not in mode.lower():
@@ -790,37 +756,41 @@
             else:
                 handle = _open(filename, "wb")
         self._text = "b" not in mode.lower()
         self._handle = handle
         self._buffer = b"" if "b" in mode.lower() else ""
         self.compresslevel = compresslevel
 
+
+        
         """
         Write the header to the file
         """
 
 
 
-        
-        logger.info("Constructing a new .kdb file '{0}'...".format(self._handle.name))
+        if self._loggable:
+            self.logger.log_it("Constructing a new .kdb file '{0}'...".format(self._handle.name), "INFO")
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
         if "b" in mode.lower():
             metadata_bytes = bytes(yaml.dump(self.metadata, sort_keys=False), 'utf-8')
             metadata_plus_delimiter_in_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
             self.metadata["metadata_blocks"] = math.ceil( sys.getsizeof(metadata_plus_delimiter_in_bytes) / ( 2**16 ) ) # First estimate
             metadata_bytes = bytes(yaml.dump(self.metadata, sort_keys=False), 'utf-8')
             metadata_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
             self.metadata["metadata_blocks"] = math.ceil( sys.getsizeof(metadata_bytes) / ( 2**16 ) ) # Second estimate
             metadata_bytes = bytes(yaml.dump(self.metadata, sort_keys=False), 'utf-8')
             metadata_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
-            logger.info("Writing the {0} metadata blocks to the new file".format(self.metadata["metadata_blocks"]))
-            logger.debug(self.metadata)
-            logger.debug("Header is being written as follows:\n{0}".format(yaml.dump(self.metadata, sort_keys=False)))
+            if self._loggable:
+                self.logger.log_it("Writing the {0} metadata blocks to the new file".format(self.metadata["metadata_blocks"]), "INFO")
 
             # 01-01-2022 This is still not a completely functional method to write data to bgzf through the Bio.bgzf.BgzfWriter class included in BioPython
+            # 04-10-2023 This is still disgusting to me. I understand a limited amount of the Bio.bgzf source or the nuances of the format specification
+            # That said, it's producing files, with data in the correct order. The metadata_blocks/offset calculation is still rudimentary
+            # But I'm able to generate my file format reasonably.
             # I've needed to implement a basic block_writer, maintaining compatibility with the Biopython bgzf submodule.
             #self.write(bytes(yaml.dump(metadata, sort_keys=False), 'utf-8'))
         
             for i in range(self.metadata["metadata_blocks"]):
                 metadata_slice = metadata_bytes[:65536]
                 metadata_bytes = metadata_bytes[65536:]
                 self._write_block(metadata_slice)
@@ -829,21 +799,25 @@
                 self._buffer = b""
                 self._handle.flush()
         elif "w" == mode.lower() or "x" == mode.lower():
             self.write(yaml.dump(metadata, sort_keys=False))
             self._buffer = ""
             self._handle.flush()
         else:
-            logger.error("Mode: {}".format(mode.lower()))
             raise RuntimeError("Could not determine proper encoding for write operations to .kdb file")
 
 
-
 class FileReader:
+    def __init__(self, args, logger=None):
+        self.arguments = args
+        self.logger = logger
 
-    def load_file(self, f):
-        self.file = open(f, 'r', slurp=False)
-        return self.file
-
-    def slurp(self):
-        return self.file.slurp()
+        
+    def parsefile(self, filename):
+        """Wrapper function for the KDBReader to keep arguments succinct for deployment through multiprocessing.Pool
+            
+        :param filename: the filepath of the fasta(.gz)/fastq(.gz) to process with parsefile -> parse.SeqParser
+        :type filename: str
+        :returns: (db, m, n)
+        """
+        return open(filename, mode='r', slurp=True, logger=self.logger)
```

### Comparing `kmerdb-0.7.9/kmerdb/graph.py` & `kmerdb-0.8.0/kmerdb/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,20 @@
 
 import numpy as np
 #import networkx as nx
 
 from kmerdb import fileutil, parse, kmer, config, util
 
 # Logging configuration
-import logging
-logger = logging.getLogger(__file__)
+global logger
+logger = None
 
 
 
-
-def open(filepath, mode="r", metadata=None, slurp:bool=False):
+def open(filepath, mode="r", metadata=None, slurp:bool=False, logger=None):
     """
     Opens a file for reading or writing. Valid modes are 'xrwbt'. 
     Returns a lazy-loading KDBGReader object or a KDBGWriter object.
     The data may be force loaded with 'slurp=True'
 
 
     Opens a .kdbg file, still only view goals.
@@ -145,14 +144,18 @@
         return KDBGReader(filename=filepath, mode=mode, slurp=slurp)
     elif "w" in mode.lower() or "x" in mode.lower():
         return KDBGWriter(filename=filepath, mode=mode, metadata=metadata)
     else:
         raise ValueError("Bad mode %r" % mode)
 
 
+    self.logger = logger
+    self._loggable = logger is not None
+
+
 def bytesize_of_metadata(metadata):
     """
     defers to util.get_bytesize_of_metadata
     """
     return util.bytessize_of_metadata
 
     
@@ -187,24 +190,24 @@
         raise StopIteration("empty table line")
     
     if type(sort_arr) is not bool:
         raise TypeError("kmerdb.graph.parse_kdbg_table_line needs 'sort_arr' to be bool")
     try:
         np.dtype(row_dtype)
     except TypeError as e:
-        logger.error("Invalid numpy dtype")
+        sys.stderr.write("Invalid numpy dtype\n")
         raise e
     finally:
 
 
 
         linesplit = kdbg_table_line.rstrip().split("\t")
         
         if len(linesplit) != 4:
-            logger.error("Full line:\n{0}".format(line))
+            sys.stderr.write("Full line:\n{0}".format(line) + "\n")
             raise ValueError("kmerdb.graph.parse_kdbg_table_line encountered a .kdbg line without 4 columns. Invalid format for edge list")
         else:
             i, node1_id, node2_id, weight = linesplit
             i, node1_id, node2_id, weight = int(i), int(node1_id), int(node2_id), int(weight)
         
             e = np.array([node1_id, node2_id, weight], dtype=row_dtype)
             
@@ -222,15 +225,15 @@
             
             # Objective function def
             return [i] + list(e)
     
 
             
 
-def parsefile(filepath:str, k:int, quiet:bool=True, b:int=50000, both_strands:bool=False):
+def parsefile(filepath:str, k:int, quiet:bool=True, b:int=50000, both_strands:bool=False, logger=None):
     """
     Parse a single sequence file.
     
     :param filepath: Path to a fasta or fastq file
     :type filepath: str
     :param k: Choice of k to shred k-mers with
     :type k: int
@@ -262,81 +265,86 @@
     elif type(k) is not int:
         raise TypeError("kmerdb.graph.parsefile expects an int as its second positional argument")
     elif type(b) is not int:
         raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'b' to be an int")
     elif type(both_strands) is not bool:
         raise TypeError("kmerdb.graph.parsefile expects the keyword argument 'both_strands' to be a bool")
 
+    _loggable = logger is not None
+    
+
     N = 4**k
     counts = np.zeros(N, dtype="uint64")
-    
-    logger.debug("Initializing edge list fileparser...")
+
+
+    if _loggable:
+        logger.log_it("Initializing edge list fileparser...", "DEBUG")
     seqprsr = parse.SeqParser(filepath, b, k)
     fasta = not seqprsr.fastq # Look inside the seqprsr object for the type of file
     
     # Initialize the kmer class for sequence shredding activities
     Kmer = kmer.Kmers(k) # A wrapper class to shred k-mers with
     
     # Actually load in records 'recs'
     recs = [r for r in seqprsr]
-        
-    logger.info("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
+
+
+    if _loggable:
+        logger.log_it("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
         
         
     while len(recs):
         num_recs = len(recs)
-        logger.debug("\n\nAcquiring list of all k-mer ids from {0} sequence records...\n\n".format(num_recs))
+        #logger.debug("\n\nAcquiring list of all k-mer ids from {0} sequence records...\n\n".format(num_recs))
 
 
         list_of_dicts = list(map(Kmer._shred_for_graph, recs))
 
-        
-        logger.info("k-mer shredding a block of {0} reads/sequences".format(num_recs))
+        if _loggable:
+            logger.log_it("k-mer shredding a block of {0} reads/sequences".format(num_recs), "INFO")
         kmer_ids = list(chain.from_iterable(list_of_dicts))
 
         
-        logger.debug("Successfully allocated linked-list for all k-mer ids read.")
-
         num_kmers = len(kmer_ids)
 
         if num_kmers == 0:
             raise ValueError("No k-mers to add. Something likely went wrong. Please report to the issue tracker")
         else:
-            sys.stderr.write("\nAccumulating all k-mers from this set of records...")
+            sys.stderr.write("\nAccumulating all k-mers from this set of records...\n")
             for kmer in kmer_ids:
                 counts[kmer] += 1
         
 
         # END WHILE routine
         # load_more_records, according to 'block size'. Legacy syntax
         recs = [r for r in seqprsr] # The next block of exactly 'b' reads
         # This will be logged redundantly with the sys.stderr.write method calls at line 141 and 166 of parse.py (in the _next_fasta() and _next_fastq() methods)
         #sys.stderr("\n")
         # JUST LOGGING
-        logger.info("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
+        if _loggable:
+            logger.log_it("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "DEBUG")
 
 
 
 
-    
-    logger.info("Read {0} k-mers from the input file".format(len(kmer_ids)))
+    if _loggable:
+        logger.log_it("Read {0} k-mers from the input file".format(len(kmer_ids)), "INFO")
 
     sys.stderr.write("\n\n\n")
-    logger.info("K-mer counts read from input(s)")
+    if _loggable:
+        logger.log_it("K-mer counts read from input(s)", "INFO")
     sys.stderr.write("="*40 + "\n")
 
-    logger.info("K-space dimension: {0}".format(4**k))
-    logger.info("Number of k-mers: {0}".format(len(kmer_ids)))
-    sys.stderr.write("\n\n\n")
-
-    
-    logger.info("Constructing weighted edge list...")
-    edge_list = make_graph(kmer_ids, k, quiet=quiet)
-    logger.info("Number of edges: {0}".format(len(edge_list)))
-    sys.stderr.write("\n\nEdge list generation completed...\n")
+    if _loggable:
+        logger.log_it("Constructing weighted edge list...", "INFO")
+    edge_list = make_graph(kmer_ids, k, quiet=quiet, logger=logger)
+
+    if _loggable:
+        logger.log_it("Number of edges: {0}".format(len(edge_list)), "INFO")
+        logger.log_it("Edge list generation completed...", "INFO")
 
     unique_kmers = int(np.count_nonzero(counts))
     # FIXME
     num_nullomers = int(len(list(np.where(counts == 0)[0])))
 
 
     all_kmer_ids = list(range(N))
@@ -352,15 +360,15 @@
     seqprsr.unique_kmers = unique_kmers
     seqprsr.nullomers = num_nullomers
     seqprsr.nullomer_array = nullomer_array
 
     
     return (edge_list, seqprsr.header_dict(), counts, seqprsr.nullomer_array)
 
-def make_graph(kmer_ids:list, k:int=None, quiet:bool=True):
+def make_graph(kmer_ids:list, k:int=None, quiet:bool=True, logger=None):
     """
     Make a neighbor graph from a k-mer id list.
 
     More specifically, this is a edge list
 
     Even more so, an edge list of technically adjacent k-mers in a .fa or .fq file.
 
@@ -409,14 +417,15 @@
     if kmer_ids is None or type(kmer_ids) is not list:
         raise TypeError("kmerdb.graph.make_graph expects a list as its only positional argument")
     elif k is None or type(k) is not int:
         raise TypeError("kmerdb.graph.make_graph expects the keyword argument k to be an int")
     elif quiet is None or type(quiet) is not bool:
         raise TypeError("kmerdb.graph.make_graph expects the keyword argument quiet to be a bool")
 
+    _loggable = logger is not None
     # Initialize total_list of possible k-mer neighbor pairs from the edge list.
     # Step 1. Complete
 
     # # NIICE.
     # neighbors = None
     # #neighbors = 
 
@@ -535,15 +544,16 @@
         #     print("Sequence:")
         #     print(current_kmer)
         #     print(just_eight_edges)
             
         #     print("SUCCESS. This k-mer, current k-mer : {0}|{1} has 8 neighbors. {2} . None should be self".format(k_id, current_kmer, just_eight_edges))
         #     #print(all_edges_in_kspace)
         #     sys.exit(1)
-        logger.info("adjacency space completed...")
+        if _loggable:
+            logger.log_it("adjacency space completed...", "INFO")
         continue
 
         
     """
     At this point, the adjacency structure is a simple list of tuples. Redundant tuples may exist in disparate parts of the graph.
 
     The structure of the neighbor_graph is [(from_node_id, to_node_id), ...]
@@ -580,25 +590,25 @@
 
             current_kmer_id = kmer_ids[i]
             current_kmer = kmer.id_to_kmer(current_kmer_id, k)
             pair = (current_kmer, kmer.id_to_kmer(kmer_ids[i+1], k)) 
             pair_ids = tuple(map(kmer.kmer_to_id, pair))
             
             common_seq = current_kmer[1:]
-            logger.debug("Kmer_id: = kmer_ids[i] = |||                {0}".format(current_kmer_id))
-            logger.debug(" -----pair: = '{0}'  <-> '{1}'".format(pair[0], pair[1]))
+            sys.stderr.write("Kmer_id: = kmer_ids[i]     =        {0}\n".format(current_kmer_id))
+            sys.stderr.write(" -----pair: = '{0}'  <-> '{1}'\n".format(pair[0], pair[1]))
             all_edges_in_kspace[pair_ids] = 0
             # Create the neighbor lists from the list of chars, prepended or appended to the k-mer suffix/prefix
             """
             BOGUS ASSERTIONS AND NONGUARANTEES...
             """
             assert len(current_kmer) == k
             assert len(common_seq) == k-1
             
-            logger.debug("Validations completed for k-mer {0}.".format(current_kmer_id))
+            #logger.debug("Validations completed for k-mer {0}.".format(current_kmer_id))
             k1 = current_kmer[1:] # 11 characters (k - 1) remove the left most char, so new char goes on end to make the neighbor
             # not_the_king_but_the_rook = None
             k2 = current_kmer[:-1] # 11 characters ( k - 1) remove the final character so new char is prepended
             # Do we even assert these?
 
             # Comments:
             # The char_last requires its first char deleted.
@@ -629,70 +639,87 @@
             """
             LOCAL
 
             B A D         P A I R S
             debuging problematic pair of k-mer ids
             """
             if pair_ids == bad_pair:
-                logger.error("Problematic pair of k-mer ids identified...")
-                logger.error("Pair: ({0})".format(", ".join(pair_ids)))
+                sys.stderr.write("Problematic pair of k-mer ids identified...\n")
+                sys.stderr.write("Pair: ({0})\n".format(", ".join(pair_ids)))
                 raise ValueError("DEBUGGING PURPOSES ONLY: Identified a pair of k-mers noted as problematic. If you see this error, file an issue at https://github.com/MatthewRalston/kmerdb")
 
             try:
                 """
                 This is real concise. performance focused, not too much style. 
                 but this is the best way in python to concisely assert that the string slice is equivalent from k-mer to k-mer neighbor. Ensuring this throughout is damn routine.
                 essentially, this code block is added as indication that these assertions hold on a single sequence .fa file
                 by ensuring that sequential k-mer ids retrieved (via sliding window) from a single sequence .fa are, in fact, related by a common sequence.
                 when the assertion error is triggered, it is most likely that this is due to subsequent reads in a .fastq file, resulting in an erroneous 'pair' of k-mers from the algorithm above, targeting the n'th and n+1'th k-mers in the kmer_id array.
                 """
                 assert pair[0][1:] == pair[1][:-1], "kmerdb.graph expects neighboring k-mers to have at least k-1 residues in common. Must be from a fastq file."
                 assert (common_seq in pair[0]) and (common_seq in pair[1]), "kmerdb.graph expects the common_seq be in both sequences of the pair."
             except AssertionError as e:
                 error_count += 1
-                logger.error(pair)
-                logger.warning("This k-mer pair should have this subsequence in common: {0}".format(common_seq))
-                logger.warning("k1: '{0}'           k2: '{1}'".format(k1, k2))
-                logger.warning("It is explicitly assumed this is from .fastq input")
-                #logger.debug("Types: pair[0] : {0} pair[1] : {1}".format(type(pair[0]), type(pair[1])))
-                logger.debug("'{0}' == '{1}'".format(pair[0][1:], pair[1][:-1]))
-                logger.debug("Is pair0[1:] == pair1[:-1]? : {0}".format(pair[0][1:] == pair[1][:-1]))
-                logger.debug(e)
+                # logger.error(pair)
+                # logger.warning("This k-mer pair should have this subsequence in common: {0}".format(common_seq))
+                # logger.warning("k1: '{0}'           k2: '{1}'".format(k1, k2))
+                # logger.warning("It is explicitly assumed this is from .fastq input")
+                # #logger.debug("Types: pair[0] : {0} pair[1] : {1}".format(type(pair[0]), type(pair[1])))
+                # logger.debug("'{0}' == '{1}'".format(pair[0][1:], pair[1][:-1]))
+                # logger.debug("Is pair0[1:] == pair1[:-1]? : {0}".format(pair[0][1:] == pair[1][:-1]))
+                # logger.debug(e)
                 pass
             try:
                 # Accumulate for each edge pair
                 #if (15633431, 12202077) == pair_ids:
                 if bad_pair == pair_ids:
-                    logger.error("\n\nin accumulator... cannot identify the problem for this pairing again. It is in the wrong order in the key submission, and can't be recovered for some reason\n\n")
-                    logger.error("BAD KEY PAIR DETECTED")
-
-                    logger.error(bad_pair)
+                    sys.stderr.write("\n\nin accumulator... cannot identify the problem for this pairing again. It is in the wrong order in the key submission, and can't be recovered for some reason\n\n")
+                    sys.stderr.write(bad_pair)
 
-                    sys.exit(1)
+                    raise ValueError("Internal Error. Related to debugging problematic pairs during .fastq inter-read pair removal from edge list.")
                 """
                 ACCUMULATOR           --------- DONE
                 """
                 all_edges_in_kspace[pair_ids] += 1
+                """
+
+                You might be thinking "HOLY CRAP THATS A LOT OF MESSAGES" without the --quiet flag.
+
+                That's right. Also:
+
+
+                "Well, why can't you just fix the parser so it *only* returns valid edges from the .fq file?"
+
+                i.e. check whether each k-mer... from each read... is at the final index of the read... right?
+
+
+                So instead, I iterate over the k-mer array one time, and remove the edges. The performance difference between the approaches
+                would be negligible. 
+
+                """
+
+                
                 if quiet is False:
-                    logger.debug("Edge: {0} => {1}".format(pair[0], pair[1]))
-                    logger.debug("""
-  ╱|、
-(˚ˎ 。7  
- |、˜〵          
-じしˍ,)ノ
-""")                        
+                    sys.stderr.write("Edge: {0} => {1}".format(pair[0], pair[1]))
+#                     sys.stderr.write("""
+#  ╱|、
+# (˚ˎ 。7  
+#  |、˜〵          
+# じしˍ,)ノ
+# \n""")                        
             except KeyError as e:
-                logger.error("Invalid key(pair) used to access edge list")
+                sys.stderr.write("Invalid key(pair) used to access edge list\n")
                 sys.stderr.write("PAIR: {0} => {1}\n".format(pair[0], pair[1]))
                 sys.stderr.write("pair ids: {0}\n".format(pair_ids))
-                logger.error(30*"=")
-                for i, p in enumerate(all_edges_in_kspace.keys()):
-                    if bad_pair == pair_ids:
-                        logger.error("Debugging the 'bad pair', problematic k-mer id pair...")
-                        logger.error(pair_ids)
+                sys.stderr.write(30*"=" + "\n")
+                # for i, p in enumerate(all_edges_in_kspace.keys()):
+                #     if bad_pair == pair_ids:
+                #         # Double checking
+                #         logger.error("Debugging the 'bad pair', problematic k-mer id pair...")
+                #         logger.error(pair_ids)
                 raise e
             # print("heeeeeey, wow thens doo the prin funshen")
             # print(pair_ids, pair, "wow thans prin funshun ( ---------)_______________________prin fun-shun_______________________________________(    --------------)")
             # print("print funshun you're so smart and tall")
             # print("print funshun why did you sit next to me")
             # print("function")
 
@@ -705,20 +732,18 @@
             
             sys.stderr.write("k-mer 'pair' ({0}, {1}) adjacency from input file(s) verified".format(p1str, p2str))
             sys.stderr.write("\r")
             continue
 
 
     if error_count > 0:
-        logger.warning("\n")
-        logger.warning("\n")
-        logger.warning("\n\n\nNOTE: ADJACENCY ERRORS DETECTED: Found {0} 'improper' k-mer pairs/adjacencies from the input file(s),\n where subsequent k-mers in the k-mer id array (produced from the sliding window method over input seqs/reads) did not share k-1 residues in common.\n These *may* be introduced in the array from the last k-mer of one seq/read (in the .fa/.fq) and the first k-mer of the next seq/read.\n".format(error_count))
+        sys.stderr.write("\n\n\nNOTE: ADJACENCY ERRORS DETECTED: Found {0} 'improper' k-mer pairs/adjacencies from the input file(s),\n where subsequent k-mers in the k-mer id array (produced from the sliding window method over input seqs/reads) did not share k-1 residues in common.\n These *may* be introduced in the array from the last k-mer of one seq/read (in the .fa/.fq) and the first k-mer of the next seq/read.\n".format(error_count))
     sys.stderr.write("\n\n\n")
     sys.stderr.write("All edges populated *and* accumulated across k-mer id arrays from inputs.\n")
-    logger.info("'Graph' generation complete")
+    sys.stderr.write("\n\n\n'Graph' generation complete\n\n")
 
             
     # This variable is unrestricted. A larger k may inflate this var beyond the memory limits of the computer where the observed k-space can be represented with enough resolution through enough profile diversity.
     """
     node_pairs and the k-space diversity 
 
 
@@ -864,15 +889,15 @@
     :ivar n2_dtype: NumPy dtype
     :ivar weights_dtype: NumPy dtype
     :ivar sort: *unimplemented* - uh.. sort the .kdbg edges somehow
     :ivar slurp: Autoload the .kdbg file
 
     
     """
-    def __init__(self, filename:str, fileobj:io.IOBase=None, mode:str="r", n1_dtype:str="uint64", n2_dtype:str="uint64", weights_dtype:str="uint64", sort:bool=False, slurp:bool=False):
+    def __init__(self, filename:str, fileobj:io.IOBase=None, mode:str="r", n1_dtype:str="uint64", n2_dtype:str="uint64", weights_dtype:str="uint64", sort:bool=False, slurp:bool=False, logger=None):
         """
         A wrapper around Bio.bgzf.BgzfReader
 
         :param filename: A valid filepath
         :type filename: str
         :param fileobj: An existing fileobject from io.IOBase
         :type fileobj: io.IOBase
@@ -913,14 +938,17 @@
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'weights_dtype' to be a str")
 
         elif sort is not None and type(sort) is not bool:
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'sort' to be a bool")
         elif slurp is not None and type(slurp) is not bool:
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'slurp' to be a bool")
 
+        if logger is None:
+            raise ValueError("graph.KDBGReader expects the keyword argument 'logger' to be valid")
+        
         """
 
         Handle fileobj or 
         """
         
         if fileobj:
             assert filename is None
@@ -942,15 +970,15 @@
         #       Placeholder
         self.max_cache     = 100
         
         self._buffers      = {}
         self._block_start_offset = None
         self._block_raw_length = None
 
-
+        self.logger = logger
         """
 
         np.array defs
 
         n1
         n2
         weights
@@ -963,15 +991,15 @@
         self.n2_dtype   = None
         self.weights       = None
         self.weights_dtype = None
 
         self.read_and_validate_kdbg_header()
 
         if slurp is True:
-            logger.info("Reading .kdbg contents into memory")
+            self.logger.log_it("Reading .kdbg contents into memory", "INFO")
             self.slurp(n1_dtype=n1_dtype, n2_dtype=n2_dtype, weights_dtype=weights_dtype)
 
         self.is_int = True
         handle.close()
         self._handle.close()
         self._handle = None
         handle = None
@@ -986,92 +1014,86 @@
 
         """
 
         '''
         Here we want to load the metadata blocks. We want to load the first two lines of the file: the first line is the version, followed by the number of metadata blocks
         '''
         # 0th block
-        logger.info("Loading the 0th block from '{0}'...".format(self._filepath))
+        self.logger.log_it("Loading the 0th block from '{0}'...".format(self._filepath), "INFO")
         self._load_block(self._handle.tell())
 
         self._buffer = self._buffer.rstrip(config.header_delimiter)
         
         initial_header_data = OrderedDict(yaml.safe_load(self._buffer))
 
         # Placeholder
         num_header_blocks = None
 
         if type(initial_header_data) is str:
-            logger.info("Inappropriate type for the header data.")
-            #logger.info("Um, what the fuck is this in my metadata block?")
+            self.logger.log_it("Inappropriate type for the header data.", "ERROR")
+            #logger.info("Um, what the heckin' is this in my metadata block?")
             raise TypeError("kmerdb.graph.KDBGReader could not parse the YAML formatted metadata in the first blocks of the file")
         elif type(initial_header_data) is OrderedDict:
-            logger.info("Successfully parsed the 0th block of the file, which is expected to be the first block of YAML formatted metadata")
-            logger.info("Assuming YAML blocks until delimiter reached.")
+            self.logger.log_it("Successfully parsed the 0th block of the file, which is expected to be the first block of YAML formatted metadata", "INFO")
+            self.logger.log_it("Assuming YAML blocks until delimiter reached.", "INFO")
 
         """
 
         KDBGReader
         
         YAML metadata spec validation
         """
             
         if "version" not in initial_header_data.keys():
             raise TypeError("kmerdb.graph.KDBGReader couldn't validate the header YAML")
         elif "metadata_blocks" not in initial_header_data.keys():
             raise TypeError("kmerdb.graph.KDBGReader couldn't validate the header YAML")
             
-        logger.debug(initial_header_data)
+        self.logger.log_it(initial_header_data, "INFO")
         
         if initial_header_data["metadata_blocks"] != 1:
-            logger.error("More than 1 metadata block: uhhhhh are we loading any additional blocks")
+            self.logger.log_it("More than 1 metadata block: uhhhhh are we loading any additional blocks", "ERROR")
             raise IOError("Cannot read more than 1 metadata block yet")
 
         for i in range(initial_header_data["metadata_blocks"] - 1):
-            logger.info("Multiple metadata blocks read...")
+            self.logger.log_it("Multiple metadata blocks read, most likely from a composite edge-graph...", "WARNING")
             self._load_block(self._handle.tell())
-            logger.debug("Secondary blocks read")
             addtl_header_data = yaml.safe_load(self._buffer.rstrip(config.header_delimiter))
             if type(addtl_header_data) is str:
-                logger.error(addtl_header_data)
-                logger.error("Couldn't determine this block.::/")
+                self.logger.log_it(addtl_header_data, "ERROR")
                 raise TypeError("kmerdb.graph.KDBGReader determined the data in the {0} block of the header data from '{1}' was not YAML formatted".format(i, self._filepath))
             elif type(addtl_header_data) is dict:
                 sys.stderr.write("\r")
                 sys.stderr.write("Successfully parsed {0} blocks of YAML formatted metadata".format(i))
                 initial_header_data.update(addtl_header_data)
                 num_header_blocks = i
             else:
-                logger.error(addtl_header_data)
+                self.logger.log_it(addtl_header_data, "ERROR")
                 raise RuntimeError("kmerdb.graph.KDBGReader encountered a addtl_header_data type that wasn't expected when parsing the {0} block from the .kdb file '{1}'.".format(i, self._filepath))
 
         #raise RuntimeError("kmerdb.graph.KDBGReader encountered an unexpected type for the header_dict read from the .kdb header blocks")
 
     
-        logger.info("Reading additional blocks as YAML...")
-        logger.debug("Reading additional blocks as YAML...")
-        sys.stderr.write("\n")
-        logger.info("Validating the header data against the schema...")
+        self.logger.log_it("Validating the header YAML...", "INFO")
+
         try:
             jsonschema.validate(instance=initial_header_data, schema=config.graph_schema)
             self.metadata = dict(initial_header_data)
             
             self.k = self.metadata['k']
             self.n1_dtype = self.metadata["n1_dtype"]
             self.n2_dtype = self.metadata["n2_dtype"]
             self.weights_dtype = self.metadata["weights_dtype"]
             self.sorted = self.metadata["sorted"]
-            logger.info("Self assigning dtype to uint64 probably")
-            logger.debug("Checking for metadata inference...")
+
         except jsonschema.ValidationError as e:
-            logger.debug(e)
-            logger.error("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks))
+            self.logger.log_it("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks), "ERROR")
             raise e
         self.metadata["header_offset"] = self._handle.tell()
-        logger.debug("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]))
+        #logger.debug("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]))
         #self._reader = gzip.open(self._filepath, 'r')
         self._offsets = deque()
         for values in bgzf.BgzfBlocks(self._handle):
             #logger.debug("Raw start %i, raw length %i, data start %i, data length %i" % values)
             self._offsets.appendleft(values) # raw start, raw length, data start, data length
         if len(self._offsets) == 0:
             raise IOError("kmerdb.graph.KDBGReader opened an empty file")
@@ -1124,16 +1146,14 @@
             raise TypeError("kmerdb.graph.KDBGReader.slurp expects weights_dtype to be a str")
 
         try:
             np.dtype(n1_dtype)
             np.dtype(n2_dtype)
             np.dtype(weights_dtype)
         except TypeError as e:
-            logger.error(e)
-            logger.error("kmerdb.graph.KDBGReader.slurp encountered a TypeError while assessing a numpy dtype")
             raise TypeError("kmerdb.graph.KDBGReader.slurp expects each dtype keyword argument to be a valid numpy data type")
 
         vmem = psutil.virtual_memory()
 
         i = 0
 
         idx = []
@@ -1144,19 +1164,19 @@
         reading=True
         while reading is True:
 
             try:
                 line = next(self)
 
             except StopIteration as e:
-                logger.error("Finished loading .kdbg through slurp (on init)")
+                self.logger.log_it("Finished loading .kdbg through slurp (on init)", "ERROR")
                 raise e
             if line is None:
-                logger.warning("Next returned None. Panic")
-                sys.exit(1)
+                self.logger.log_it("'next' returned None. Panic", "WARNING")
+
                 raise RuntimeError("kmerdb.graph.KDBGReader.slurp Panicked on new line")
 
 
                   
             try:
                 
                 arr = self.read_line()
@@ -1190,15 +1210,15 @@
     :ivar mode: read/write mode
     :ivar metadata: header information
     :ivar both_strands: *unimplemented*
     :ivar fileobj: io.IOBase
     :ivar compresslevel: compression parameter
     """
     
-    def __init__(self, filename:str=None, mode:str="w", metadata:OrderedDict=None, both_strands:bool=False, fileobj:io.IOBase=None, compresslevel:int=6):
+    def __init__(self, filename:str=None, mode:str="w", metadata:OrderedDict=None, both_strands:bool=False, fileobj:io.IOBase=None, compresslevel:int=6, logger=None):
         """
         A wrapper around Bio.bgzf.BgzfWriter
 
         :param filename: A valid filepath
         :type filename: str
         :param mode: read/write mode
         :type mode: str
@@ -1225,40 +1245,47 @@
             raise TypeError("kmerdb.graph.KDBGWriter - invalid metadata argument")
         elif both_strands is None or type(both_strands) is not bool:
             raise TypeError("kmerdb.graph.KDBGWriter expects the keyword argument 'both_strands' to be a bool")
         elif fileobj is not None and not isinstance(fileobj, io.IOBase):
             raise TypeError("kmerdb.graph.KDBGWriter expects the keyword argument 'fileobj' to be an instance of io.IOBase")
         elif compresslevel is None or type(compresslevel) is not int:
             raise TypeError("kmerdb.graph.KDBGWriter expects the keyword argument 'compresslevel' to be an int")
+
+        self.logger = logger
+        self._loggable = logger is not None
+
         
         if fileobj:
             assert filename is None, "kmerdb.graph expects filename to be None is fileobj handle is provided"
             handle = fileobj
         else:
             if "w" not in mode.lower() and "a" not in mode.lower():
                 raise ValueError("Must use write or append mode, not %r" % mode)
             elif "wb" == mode:
                 pass
             elif "a" in mode.lower():
                 raise NotImplementedError("Append mode is not implemented yet")
                 # handle = _open(filename, "ab")
             else:
-                logger.error("Mode = {0}".format(mode))
                 raise RuntimeError("Unknown mode for .kdbg file writing class kmerdb.graph.KDBGWriter")
         self._text = "b" not in mode.lower()
         self._handle = _open(filename, "wb")
         self._buffer = b"" if "b" in mode.lower() else ""
         self.compresslevel = compresslevel
 
+
+        self.logger = logger
+        self._loggable = logger is not None
+        
         """
         Write the header to the file
         """
 
-        
-        logger.info("Constructing a new .kdbg file '{0}'...".format(self._handle.name))
+        if self._loggable:
+            self.logger.log_it("Constructing a new .kdbg file '{0}'...".format(self._handle.name), "INFO")
 
 
         # 3-04-2024
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
 
         self.metadata = metadata
 
@@ -1268,17 +1295,17 @@
             metadata_plus_delimiter_in_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
             self.metadata["metadata_blocks"] = math.ceil( sys.getsizeof(metadata_plus_delimiter_in_bytes) / ( 2**16 ) ) # First estimate
             metadata_bytes = bytes(yaml.dump(self.metadata, sort_keys=False), 'utf-8')
             metadata_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
             self.metadata["metadata_blocks"] = math.ceil( sys.getsizeof(metadata_bytes) / ( 2**16 ) ) # Second estimate
             metadata_bytes = bytes(yaml.dump(self.metadata, sort_keys=False), 'utf-8')
             metadata_bytes = metadata_bytes + bytes(config.header_delimiter, 'utf-8')
-            logger.info("Writing the {0} metadata blocks to the new file".format(self.metadata["metadata_blocks"]))
-            logger.debug(self.metadata)
-            logger.debug("Header is being written as follows:\n{0}".format(yaml.dump(self.metadata, sort_keys=False)))
+            if self._loggable:
+                self.logger.log_it("Writing the {0} metadata blocks to the new file".format(self.metadata["metadata_blocks"]), "INFO")
+                self.logger.log_it("Header is being written as follows:\n{0}".format(yaml.dump(self.metadata, sort_keys=False)), "DEBUG")
 
             # 01-01-2022 This is still not a completely functional method to write data to bgzf through the Bio.bgzf.BgzfWriter class included in BioPython
             # I've needed to implement a basic block_writer, maintaining compatibility with the Biopython bgzf submodule.
             #self.write(bytes(yaml.dump(metadata, sort_keys=False), 'utf-8'))
         
             for i in range(self.metadata["metadata_blocks"]):
                 metadata_slice = metadata_bytes[:65536]
@@ -1289,30 +1316,29 @@
                 self._buffer = b""
                 self._handle.flush()
         elif "w" == mode.lower() or "x" == mode.lower():
             self.write(yaml.dump(metadata, sort_keys=False))
             self._buffer = ""
             self._handle.flush()
         else:
-            logger.error("Mode: {}".format(mode.lower()))
             raise RuntimeError("Could not determine proper encoding for write operations to .kdb file")
         
 
     
 
         
 
 class Parseable:
-    def __init__(self, arguments):
+    def __init__(self, arguments, logger):
         self.arguments = arguments
-            
+        self.logger = logger
         
     def parsefile(self, filename):
         """Wrapper function for graph.parsefile to keep arguments succinct for deployment through multiprocessing.Pool
             
         :param filename: the filepath of the fasta(.gz)/fastq(.gz) to process with kmerdb.graph.parsefile
         :type filename: str
         """
-        return parsefile(filename, self.arguments.k, quiet=self.arguments.quiet)
+        return parsefile(filename, self.arguments.k, quiet=self.arguments.quiet, logger=self.logger)
```

### Comparing `kmerdb-0.7.9/kmerdb/index.py` & `kmerdb-0.8.0/kmerdb/index.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/kmer.py` & `kmerdb-0.8.0/kmerdb/kmer.py`

 * *Files 10% similar despite different names*

```diff
@@ -231,18 +231,18 @@
             ######################################################################33
             #       I U P A C        m o d u l e
             ######################################################################33
 
             if len(set(str(s)) - self.__permitted_chars) == 0 and len(iupac_symbols) > 0 and len(non_iupac_symbols) == 0:
                 seqs = None
                 for c in list(set(s) - standard_letters):
-                    logger.debug("character: {0}".format(c))
-                    logger.debug("K-mer: {0}".format(s))
-                    logger.debug("IUPAC symbols in the whole sequence: {0}".format(iupac_symbols))
-                    logger.debug("Non-IUPAC symbols in the whole sequence: {0}".format(non_iupac_symbols))
+                    # logger.debug("character: {0}".format(c))
+                    # logger.debug("K-mer: {0}".format(s))
+                    # logger.debug("IUPAC symbols in the whole sequence: {0}".format(iupac_symbols))
+                    # logger.debug("Non-IUPAC symbols in the whole sequence: {0}".format(non_iupac_symbols))
                     if c in IUPAC_DOUBLET_CHARS:
                         #logger.info("Doublets being replaced")
                         if seqs is None:
                             seqs = list(map(lambda x: replace_char(str(s), c, x), get_doublet_chars(c)))
                         else:
                             seqs = list(chain.from_iterable(map(lambda s: list(map(lambda x: replace_char(s, c, x), get_doublet_chars(c))), seqs)))
                     elif c in IUPAC_TRIPLET_CHARS:
@@ -253,30 +253,30 @@
                             seqs = list(chain.from_iterable(map(lambda s: list(map(lambda x: replace_char(s, c, x), get_triplet_chars(c))), seqs)))
                     elif c in standard_letters:
                         raise RuntimeError("Standard DNA residue detected in IUPAC module")
                     elif c == n:
                         logger.warning("N content detected")
                         continue
                     else:
-                        logger.error(str(seqRecord))
-                        logger.error("Full sequence above")
-                        logger.error("K-mer: {0}".format(s))
-                        logger.error(s)
+                        sys.stderr.write(str(seqRecord) + "\n")
+                        sys.stderr.write("Full sequence above" + "\n")
+                        sys.stderr.write("K-mer: {0}".format(s) + "\n")
+                        sys.stderr.write(s + "\n")
                         raise RuntimeError("kmerdb.kmer.shred: Non-IUPAC character '{0}' made it into sequences generated from IUPAC doublet/triplet counting of the k-mer '{1}'".format(c, s))
                 if seqs is None and "N" not in s:
-                    logger.warning("Permitted IUPAC symbols: {0}".format(iupac_symbols))
-                    logger.warning("Non-IUPAC symbols detected in sequence '{0}': {1}".format(s, non_iupac_symbols))
-                    logger.error("The following k-mer did not have any IUPAC letters: {0}".format(s))
+                    sys.stderr.write("Permitted IUPAC symbols: {0}".format(iupac_symbols))
+                    sys.stderr.write("Non-IUPAC symbols detected in sequence '{0}': {1}".format(s, non_iupac_symbols))
+                    sys.stderr.write("The following k-mer did not have any IUPAC letters: {0}".format(s))
                     raise RuntimeError("kmerdb.kmer.shred: A sequence was rejected from non-IUPAC symbols")
                 elif seqs is None and "N" in s:
                     continue
                 one_word = "".join(seqs)
                 if len(set(one_word) - self.__permitted_chars) > 0:
-                    logger.error(one_word)
-                    logger.error("Doublets/triplets produced from k-mer '{0}': \n{1}".format(s, seqs))
+                    sys.stderr.write(one_word + "\n")
+                    sys.stderr.write("Doublets/triplets produced from k-mer '{0}': \n{1}".format(s, seqs) + "\n")
                     raise ValueError("kmerdb.kmer.shred: at least one non-IUPAC symbol was found during doublets/triplet expansion of the k-mer '{0}'".format(s))
                 else:
                     for x in seqs:
                         logger.debug(x)
                         kmers.append(kmer_to_id(x))
                         if self.all_metadata:
                             reverses.append(False)
@@ -287,45 +287,45 @@
                                 reverses.append(True)
                                 starts.append(i)
 
                     # OKAY you are supposed to remember that
                     # the number of k-mer ids will no-longer match the appended metadata,
                     # So even though the lambda is correct, you have to do separate metadata for each id
             elif len(non_iupac_symbols) > 0:
-                logger.debug("TEST CONDITIONS")
-                logger.debug("Non-permitted characters should be 0: {0}".format(len(set(str(s)) - self.__permitted_chars)))
-                logger.debug("IUPAC symbols should be > 0: {0}".format(len(iupac_symbols)))
-                logger.debug("Non-IUPAC characters should be 0: {0}".format(len(non_iupac_symbols)))
-                logger.debug("Non-IUPAC symbols: {0}".format(non_iupac_symbols))
-                logger.debug("IUPAC symbols: {0}".format(iupac_symbols))
-                logger.debug("K-mer: '{0}'".format(str(s)))
+                sys.stderr.write("TEST CONDITIONS:\n")
+                sys.stderr.write("Non-permitted characters should be 0: {0}".format(len(set(str(s)) - self.__permitted_chars)) + "\n")
+                sys.stderr.write("IUPAC symbols should be > 0: {0}".format(len(iupac_symbols)) + "\n")
+                sys.stderr.write("Non-IUPAC characters should be 0: {0}".format(len(non_iupac_symbols)) + "\n")
+                sys.stderr.write("Non-IUPAC symbols: {0}".format(non_iupac_symbols) + "\n")
+                sys.stderr.write("IUPAC symbols: {0}".format(iupac_symbols) + "\n")
+                sys.stderr.write("K-mer: '{0}'".format(str(s)) + "\n")
                 raise ValueError("kmerdb.kmer.shred: Non-IUPAC symbol(s) detected")
             else:
                 try:
                     kmers.append(kmer_to_id(s))
                     if self.all_metadata:
                         reverses.append(False)
                         starts.append(i)
                     if not self.strand_specific: # Reverse complement by default
                         kmers.append(kmer_to_id(s.reverse_complement()))
                         if self.all_metadata:
                             reverses.append(True)
                             starts.append(i)
                 except KeyError as e:
-                    logger.warning("One or more non-IUPAC letters found their way into a part of the code they're not supposed to go")
-                    logger.warning("We officially support IUPAC but the statement challenging the sequence content failed, causing a genuine runtime error")
-                    logger.warning("This caused the following KeyError")
-                    logger.warning(e)
-                    logger.error("Letters in the sequence: {0}".format(letters))
-                    logger.errror("Permitted letters: {0}".format(self.__permitted_chars))
+                    sys.stderr.write("One or more non-IUPAC letters found their way into a part of the code they're not supposed to go\n")
+                    sys.stderr.write("We officially support IUPAC but the statement challenging the sequence content failed, causing a genuine runtime error\n")
+                    sys.stderr.write("This caused the following KeyError\n")
+                    sys.stderr.write(e.__str__() + "\n")
+                    sys.stderr.write("Letters in the sequence: {0}".format(letters) + "\n")
+                    sys.stderr.write("Permitted letters: {0}".format(self.__permitted_chars) + "\n")
                     raise RuntimeError("IUPAC standard extra base pairs (R, B, etc.) or non-IUPAC characters detected in the sequence")
             del s
         if self.verbose:
             sys.stderr.write("            --- ~~~ --- ~~~  shredded ~~~ --- ~~~ ---\n")
-            sys.stderr.write("a {0}bp long sequence was shredded into L-k+1 {1} total and {2} unique k-mers\n\n{3} were discarded due to sequence content\n\n".format(len(seqRecord.seq), len(str(seqRecord.seq))-self.k+1, len(list(set(kmers))), len([x for x in kmers if x is None])))
+            sys.stderr.write("a {0}bp long sequence was shredded into L-k+1 {1} total and {2} unique k-mers\n\n{3} were discarded due to sequence content\n\n".format(len(seqRecord.seq), len(str(seqRecord.seq))-self.k+1, len(list(set(kmers))), len([x for x in kmers if x is None])) + "\n")
         return {'id': seqRecord.id, 'kmers': kmers, "seqids": repeat(seqRecord.id, len(starts)), "starts": starts, 'reverses': reverses}
 
 
 
 #############################
 #
 # Functions
@@ -365,16 +365,16 @@
         if isinstance(s, Bio.Seq.Seq) or isinstance(s, Bio.SeqRecord.SeqRecord):
             s = str(s)
         for c in bytes(s, "UTF-8"): # Use byteshifting for fast conversion to binary encoding
             idx = idx << 2
             try:
                 idx = idx | letterToBinary[c]
             except KeyError as e:
-                logger.error("Entire sequence: {0}".format(s))
-                logger.error("Problematic character: {0}".format(c))
+                sys.stderr.write("Entire sequence: {0}".format(s) + "\n")
+                sys.stderr.write("Problematic character: {0}".format(c) + "\n")
                 raise e
         return idx
 
 
 def id_to_kmer(id, k):
     """
     Convert an id_to_kmer. I don't understand this docstring's purpose.
@@ -384,19 +384,19 @@
     :param k: The int k is used to byte convert the id to the sequence of characters
     :type k: int
     :raise TypeError: int argument required, non-int type detected
     :returns: The k-mer as string
     :rtype: str
     """
     if type(id) is not int:
-        logger.error("kmer.id_to_kmer was given the following type as an id")
-        logger.error(type(id))
+        sys.stderr.write("kmer.id_to_kmer was given the following type as an id\n")
+        sys.stderr.write(str(type(id)) + "\n")
         raise TypeError("kmerdb.id_to_kmer expects an int as its first positional argument")
     elif type(k) is not int:
-        logger.error(type(k))
+        sys.stderr.write(str(type(k)) + "\n")
         raise TypeError("kmerdb.id_to_kmer expects an int as its second positional argument")
     else:
         kmer = ""
         for i in range(k):
             kmer += binaryToLetter[id & 0x03]
             id = id >> 2
         kmer = list(kmer)
@@ -475,27 +475,33 @@
 # jgs \\|//   \\|///  \\\|//\\\|/// \|///  \\\|//  \\|//  \\\|// 
 # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 # """,
 #               "",
 
 #         )
 
-        logger.debug("kmerdb.kmer.neighbors creating neighbors for k-mer '{0}'...".format(kmer))
-        logger.debug("kmerdb.kmer.neighbors creating the neighbor structure for kmer : '{0}' \n: ==========\n'".format(kmer_id) + ", ".join(list(map(str, new_type1_ids))))
-        logger.debug("kmerdb.kmer.neighbors creating the neighbor structure for kmer : '{0}' \n: ==========\n'".format(kmer_id) + ", ".join(list(map(str, new_type2_ids))))
+        sys.stderr.write("kmerdb.kmer.neighbors creating neighbors for k-mer {0} : '{1}'...".format(kmer_id, kmer) + "\n")
+        sys.stderr.write(" ========================\n\n")
+        sys.stderr.write(", ".join(list(map(str, new_type1_ids))) + "\n")
+        sys.stderr.write(", ".join(list(map(str, new_type2_ids))) + "\n\n")
+        sys.stderr.write(" ------------------------\n\n")
+        
         if quiet is not True:
             sys.stderr.write("""
         k-id : {0}
         kmer : \"    {1}        \"
 
         'neighbors'
 
         {2}
         {3}
 
         'ids':
 
         {4}
         {5}
-""".format(kmer_id, kmer, new_type1, new_type2, new_type1_ids, new_type2_ids))
+\n""".format(kmer_id, kmer, new_type1, new_type2, new_type1_ids, new_type2_ids))
         #return {"appended_first_char_all_ommitted": new_type1_ids, "prepended_last_char_all_omitted": new_type2_ids}
+
+
+        
         return new_type1_ids + new_type2_ids
```

### Comparing `kmerdb-0.7.9/kmerdb/legacy.py` & `kmerdb-0.8.0/kmerdb/legacy.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/parse.py` & `kmerdb-0.8.0/kmerdb/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,22 +39,19 @@
 #from psycopg2 import sql
 import tempfile
 import numpy as np
 
 
 from kmerdb import kmer
 
-import logging
-logger = logging.getLogger(__file__)
 
 
 
 
-
-def parsefile(filepath:str, k:int, ): #rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
+def parsefile(filepath:str, k:int, logger): #rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
     """Parse a single sequence file in blocks/chunks with multiprocessing support
 
     :param filepath: Path to a fasta or fastq file
     :type filepath: str
     :param k: Choice of k to shred k-mers with
     :type k: int
     :param b: Number of reads (per block) to process in parallel
@@ -86,88 +83,90 @@
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'b' to be an int")
     # elif n is None or type(n) is not int:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'n' to be an int")
     # elif both_strands is None or type(both_strands) is not bool:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'both_strands' to be a bool")
     # elif all_metadata is None or type(all_metadata) is not bool:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'all_metadata' to be a bool")
+    if logger is None:
+        raise ValueError("Invalid logger")
     data = {} # This is the dictionary of tuples, keyed on k-mer id, and containing 3-tuples ('kmer_id', 'read/start/reverse')
     keys = set()
     rows = []
     N = 4**k
     nullomers = set()
     # Build fasta/fastq parser object to stream reads into memory
-    logger.debug("Initializing parser...")
-    seqprsr = SeqParser(filepath, k)
+    logger.log_it("Initializing parser...", "INFO")
+    seqprsr = SeqParser(filepath, k, logger)
     fasta = not seqprsr.fastq # Look inside the seqprsr object for the type of file
 
     # Initialize the kmer array
     try:
         counts = np.zeros(N, dtype="uint64")
     except TypeError as e:
-        logger.error("Invalid dtype for numpy array instantiation")
-        logger.error(e)
+        logger.log_it("Invalid dtype for numpy array instantiation", "ERROR")
+        logger.log_it(e.__str__(), "ERROR")
         raise e
 
-    logger.info("Successfully allocated space for {0} unsigned integers: {1} bytes".format(N, counts.nbytes))
+    logger.log_it("Successfully allocated space for {0} unsigned integers: {1} bytes".format(N, counts.nbytes), "INFO")
         # Instantiate the kmer class
     Kmer = kmer.Kmers(k, verbose=fasta) # A wrapper class to shred k-mers with
 
     recs = [r for r in seqprsr] # A block of exactly 'b' reads-per-block to process in parallel
     if not fasta:
-        logger.debug("Read exactly {0} records from the seqparser object".format(len(recs)))
+        logger.log_it("Read exactly {0} records from the seqparser object".format(len(recs)), "DEBUG")
         assert len(recs) <= b, "The seqparser should return exactly {0} records at a time".format(b)
     else:
-        logger.debug("Skipping the block size assertion for fasta files")
-    logger.info("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
+        logger.log_it("Skipping the block size assertion for fasta files", "DEBUG")
+    logger.log_it("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
     all_kmer_metadata = list([] for x in range(N))
     while len(recs): # While the seqprsr continues to produce blocks of reads
 
         num_recs = len(recs)
-        logger.info("Processing a block of {0} reads/sequences".format(num_recs))
+        logger.log_it("Processing a block of {0} reads/sequences".format(num_recs), "INFO")
 
         # Initialize an all_kmer_metadata list
         kmer_metadata = []
         list_of_dicts = list(map(Kmer.shred, recs))
 
         # Flatmap to 'kmers', the dictionary of {'id': read_id, 'kmers': [ ... ]}
-        logger.debug("\n\nAcquiring linked-list of all k-mer ids from {0} sequence records...\n\n".format(num_recs))
+        logger.log_it("\n\nAcquiring linked-list of all k-mer ids from {0} sequence records...\n\n".format(num_recs), "INFO")
         kmer_ids = list(chain.from_iterable(map(lambda x: x['kmers'], list_of_dicts)))
-        logger.debug("Successfully allocated linked-list for all k-mer ids read.")
+
         sus = set()
-        logger.info("Removing any eroneous k-mers without an id, cause by 'N' content, creating new gaps in the k-mer profile...")
-        logger.info("Will substitute IUPAC residues with their respective residues, adding one count for each")
+        logger.log_it("Removing any eroneous k-mers without an id, cause by 'N' content, creating new gaps in the k-mer profile...", "WARNING")
+        logger.log_it("Will substitute IUPAC residues with their respective residues, adding one count for each", "WARNING")
         num_sus = 0
         for i, k in enumerate(kmer_ids):
             if k is None:
                 sus.add(i) # This propagates the N removal, by adding those to the set for removal later.
                 num_sus += 1
 
-        logger.info("Created {0} gaps in the k-mer profile to clean it of N-content".format(num_sus))
+        logger.log_it("Created {0} gaps in the k-mer profile to clean it of N-content".format(num_sus), "INFO")
         if num_sus > 0:
-            logger.warning("{0} uncountable k-mer identified".format(num_sus))
-            logger.warning("Likely caused by the presence of the unspecified nucleotide 'N' in a .fasta file")
-            logger.warning("Will remove from the final committed profile")
+            logger.log_it("{0} uncountable k-mer identified".format(num_sus), "WARNING")
+            logger.log_it("Likely caused by the presence of the unspecified nucleotide 'N' in a .fasta file", "WARNING")
+            logger.log_t("Will remove from the final committed profile", "WARNING")
 
         ########################
         # K-mer cleaning
         #
         # 
         # The following procedure, removes k-mers that don't have a formal k-mer id
         # More specifically, it eliminates entries that were formally loaded into the k-mers array,
         # and thus would be a minor percentage of the total number of k-mers,
         # Specifically, k-mers or subsequences with N can be excluded from the profile
         # To essentially eliminate an area of sequence and create an artificial gap in the "retained" graph.
         # The graph can be explicitly collapsed when you want to, by supplying reads or sequence information, that is contiguous "in your judgement".
         # By introducing these artificial gaps, we expose the errors or unspecified bases through data.
         #
-        logger.info("Found {0} invalid or enumerable k-mers, sequences which have no defined index, i".format(num_sus))
-        logger.debug("In other words, one or more characters in your .fasta or .fastq file were 'N' or otherwise contained IUPAC characters that need to be substituted.")
-        logger.debug("We have chosen to omit k-mer with unspecified nucleotides 'N', and these make gaps in our database explicitly.")
-        logger.info("These can be recovered from the reads if they are needed, and the read ids may be found with the experimental --all-metadata flag")
+        logger.log_it("Found {0} invalid or enumerable k-mers, sequences which have no defined index, i".format(num_sus), "INFO")
+        logger.log_it("In other words, one or more characters in your .fasta or .fastq file were 'N' or otherwise contained IUPAC characters that need to be substituted.", "DEBUG")
+        logger.log_it("We have chosen to omit k-mer with unspecified nucleotides 'N', and these make gaps in our database explicitly.", "DEBUG")
+        logger.log_it("These can be recovered from the reads if they are needed, and the read ids may be found with the experimental --all-metadata flag", "INFO")
         # if all_metadata:
 
         #     logger.warning("\n\n\nGENERATING ALL METADATA\n\n\nThis is extremely expensive and experimental. You have been warned.\n\n\n")
         #     reads = list(chain.from_iterable(map(lambda x: x['seqids'], list_of_dicts)))
         #     starts = list(chain.from_iterable(map(lambda x: x['starts'], list_of_dicts)))
         #     reverses = list(chain.from_iterable(map(lambda x: x['reverses'], list_of_dicts)))
         #     logger.debug("Checking each k-mer for N-content and IUPAC substitution")
@@ -178,32 +177,32 @@
         #             starts[i] = None
         #             reverses[i] = None
         #     kmer_ids = list(filter(lambda k: k is not None, kmer_ids)) 
         #     reads = list(filter(lambda r: r is not None, reads))
         #     starts = list(filter(lambda s: s is not None, starts))
         #     reverses = list(filter(lambda r: r is not None, reverses))
         # else:
-        logger.debug("Checking each k-mer for IUPAC substitution or N content.")
+        logger.log_it("Checking each k-mer for IUPAC substitution or N content.", "DEBUG")
         for i, x in enumerate(kmer_ids): # Here we remove the k-mer ids where N-content is detected, in case they are needed, you can use kmer_ids prior to this point to build functionality.
             if i in sus:
                 kmer_ids[i] = None
-        logger.info("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions")
+        logger.log_it("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions", "INFO")
         kmer_ids = list(filter(lambda k: k is not None, kmer_ids))
         reads = [] # I'm keeping this in, just in case for some reason the variable names are needed in the 
         starts = []
         reverses = []
         if None in kmer_ids:
             # Actually they were just introduced to be filtered out, instead of deleted
             # Because each deletion whould cange the array index
             # So instead we set ghtme to None, and filter out
             raise ValueError("kmerdb.parse.parsefile encountered an invalid kmer_id. Internal error.")
 
 
-        logger.debug("{0} 'clean' kmers were identified successfully from {1} input sequences".format(len(kmer_ids), num_recs))
-        logger.debug("Flatmapped {0} kmers for their metadata aggregation".format(len(kmer_ids), len(starts)))
+        logger.log_it("{0} 'clean' kmers were identified successfully from {1} input sequences".format(len(kmer_ids), num_recs), "DEBUG")
+        logger.log_it("Flatmapped {0} kmers for their metadata aggregation".format(len(kmer_ids), len(starts)), "DEBUG")
         # Assert that all list lengths are equal before adding metadata to k-mers
         # else:
         #     raise RuntimeError("Still have no clue what's going on...")
         # On disk k-mer counting
         # Thank you, this was brilliant
         # https://stackoverflow.com/a/9294062/12855110
         # 01-01-2022 This has been removed in favor of in-memory counting
@@ -217,15 +216,15 @@
                 counts[kmer] += 1
         # all_kmer_metadata
         # if all_metadata:
         #     for single_kmer_id, read, start, reverse in kmer_metadata:
         #         all_kmer_metadata[single_kmer_id].append((read, start, reverse))
 
         recs = [r for r in seqprsr] # The next block of exactly 'b' reads
-        logger.info("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
+        logger.log_it("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
     # Get nullomers
     # only nullomer counts
     unique_kmers = int(np.count_nonzero(counts))
 
 
     all_theoretical_kmer_ids = list(range(N))
 
@@ -238,20 +237,19 @@
 
     assert num_nullomers == len(is_nullomer[0]), "kmerdb.parse module find inconsistencies between two ways of counting nullomers. Internal error."
     
     seqprsr.total_kmers = int(np.sum(counts))
     seqprsr.unique_kmers = unique_kmers
     seqprsr.nullomers = num_nullomers
 
-
     
     seqprsr.nullomer_array = np.array(all_theoretical_kmer_ids, dtype="uint64")[is_nullomer]
-    sys.stderr.write("\n\n\nFinished counting k-mers from '{0}'...\n\n\n".format(filepath))
+    logger.log_it("\n\n\nFinished counting k-mers from '{0}'...\n\n\n".format(filepath), "INFO")
 
-    return counts, seqprsr.header_dict(), seqprsr.nullomer_array
+    return counts, seqprsr.header_dict(), seqprsr.nullomer_array, logger.logs
 
 
 
 
 
 class SeqParser:
     """
@@ -260,27 +258,30 @@
     It allows you to read either fasta or fastq data in blocks, obviously useful for the latter.
 
 
     :ivar filepath: The .fastq, .fastq.gz, .fasta, .fasta.gz, .fna, .fna.gz, .fa, or .fa.gz file.
     :ivar num: The number of records to read in from a .fastq
     :ivar k: The choice of k to initialize the calculation of kmer/nullomer counts.
     """
-    def __init__(self, filepath:str, k:int, num:int=100000, ):
+    def __init__(self, filepath:str, k:int, logger, num:int=100000):
         """
         The SeqParser class wraps up some functionality  
         """
         
         if type(filepath) is not str:
             raise TypeError("kmerdb.parse.SeqParser expects a str as its first positional argument")
         elif not os.access(filepath, os.R_OK):
             raise TypeError("kmerdb.parse.SeqParser expects an existing path on the operating system as its first argument")
         elif type(num) is not int:
             raise TypeError("kmerdb.parse.SeqParser expects an int as its second positional argument")
         elif type(k) is not int:
             raise TypeError("kmerdb.parse.SeqParser expects an int as its third positional argument")
+        elif logger is None:
+            raise ValueError("Invalid logger")
+
         
         self.k = k
         self.num = num
         self.reads = []
         # Header items
         self.filepath = filepath
         self.md5 = None
@@ -317,25 +318,25 @@
             self.__class__.__next__ = self._next_fastq
         else:
             self.__class__.__iter__ = self._iter_fasta
             self.__class__.__next__ = self._next_fasta
                 
         if self.compressed:
             if self.fastq:
-                logger.info("Opening gzipped fastq file '{0}'...".format(filepath))
+                sys.stderr.write("Opening gzipped fastq file '{0}'...\n".format(filepath))
                 self._handle = SeqIO.parse(gzip.open(self.filepath, 'rt'), "fastq")
             else:
-                logger.info("Opening gzipped fasta file '{0}'...".format(filepath))
+                sys.stderr.write("Opening gzipped fasta file '{0}'...\n".format(filepath))
                 self._handle = SeqIO.parse(gzip.open(self.filepath, 'rt'), "fasta")
         else:
             if self.fastq:
-                logger.info("Opening uncompressed fastq file '{0}'...".format(filepath))
+                sys.stderr.write("Opening uncompressed fastq file '{0}'...\n".format(filepath))
                 self._handle = SeqIO.parse(open(self.filepath, 'r'), "fastq")
             else:
-                logger.info("Opening uncompressed fasta file '{0}'...".format(filepath))
+                sys.stderr.write("Opening uncompressed fasta file '{0}'...\n".format(filepath))
                 self._handle = SeqIO.parse(open(self.filepath, 'r'), "fasta")
         # Get checksums
         self.md5, self.sha256 = self.__checksum()
 
 
     def __checksum(self):
         """Generates md5 and sha256 checksums of a file
@@ -381,16 +382,14 @@
         """
         try:
             for i in range(self.num):
                 self.reads.append(next(self._handle))
         except StopIteration as e:
             pass
         except ValueError as e:
-            logger.error(e)
-            logger.error("\n\nFastq format error: '{0}' seems to not be fastq format\n\n")
             raise e
         return self
 
     def _next_fastq(self):
         """
         A custom mononucleotide counter
         
@@ -416,21 +415,23 @@
 
 
 
 
 
 
 class Parseable:
-    def __init__(self, arguments):
+    def __init__(self, arguments, logger=None):
         self.arguments = arguments
+        self.logger = logger
             
+
         
     def parsefile(self, filename):
         """Wrapper function for parse.parsefile to keep arguments succinct for deployment through multiprocessing.Pool
             
         :param filename: the filepath of the fasta(.gz)/fastq(.gz) to process with parsefile -> parse.SeqParser
         :type filename: str
         :returns: (db, m, n)
         """
-        return parsefile(filename, self.arguments.k)
+        return parsefile(filename, self.arguments.k, logger=self.logger)
```

### Comparing `kmerdb-0.7.9/kmerdb/probability.py` & `kmerdb-0.8.0/kmerdb/probability.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb/python_distances.py` & `kmerdb-0.8.0/kmerdb/python_distances.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,21 +78,20 @@
         x = c
         y = counts2[i]
         ssxx += np.square(x - x_bar)
         ssyy += np.square(y - y_bar)
         x_minus_xbar = x - x_bar
         y_minus_ybar = y - y_bar
         ssxy += x_minus_xbar*y_minus_ybar
-        logger.warning("Beware custom correlations")
+        self.logger.log_it("Beware: custom correlation. Check the source for the ssxy/sqrt(ssxx*ssyy) calculation", "WARNING")
     if ssxx*ssyy == 0:
-        logger.error("Incorrect denominator found, skipping...")
+        self.logger.log_it("Incorrect denominator found, skipping...", "ERROR")
         return 0
     else:
-        logger.info("Acquired")
-        #logger.debug("Well done, cap...")
+        #logger.debug("Well done, govna...")
         return ssxy/np.sqrt(ssxx*ssyy)
 
 
 
 def spearman(x, y):
     """
     Thin wrapper for scipy.stats.spearmanr
@@ -106,16 +105,16 @@
     """
     if type(x) is not np.ndarray:
         raise TypeError("kmerdb.distance.spearman expects a Numpy array as its first positional argument")
     elif type(y) is not np.ndarray:
         raise TypeError("kmerdb.distance.spearman expects a Numpy array as its second positional argument")
     from scipy.stats import spearmanr
     cor, pval = spearmanr(x, b=y)
-    logger.debug("Spearman calculation from SciPy")
-    logger.info("Smooth, buttery Spearman correlation coefficients.")
+    self.logger.log_it("Spearman calculation from SciPy", "INFO")
+    self.logger.log_it("\n\n\nSmooth, buttery Spearman correlation coefficients.\n\n\n", "DEBUG")
     return cor, pval
 
 def EMD(x, y):
     """
     Incomplete Earth Mover's Distance
     """
     if type(x) is not np.ndarray:
@@ -132,15 +131,18 @@
     """
     sum = 0
     for i in range(len(x)):
         if x[i] == y[i]:
             sum += 1
     return (1/4**k) * sum
 
-
+"""
+I read a paper a long time ago about using different metrics like EMS when considering non-euclidean distances and their interpretations in
+areas with limited knowledge or agreement. I don't have the paper at my fingertips, it was in EndNote and that didn't play nice with my Arch install
+"""
 
 # def d2s(x, y):
 #     if type(x) is not np.ndarray:
 #         raise TypeError("kmerdb.distance.d2s expects a Numpy array as its first positional argument")
 #     elif type(y) is not np.ndarray:
 #         raise TypeError("kmerdb.distance.d2s expects a Numpy array as its second positional argument")
```

### Comparing `kmerdb-0.7.9/kmerdb/util.py` & `kmerdb-0.8.0/kmerdb/util.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.9/kmerdb.egg-info/PKG-INFO` & `kmerdb-0.8.0/kmerdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.7.9
+Version: 0.8.0
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
 Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
@@ -252,14 +252,15 @@
 Requires-Dist: jsonschema>=4.17.3
 Requires-Dist: psutil>=4.2.0
 Requires-Dist: Cython>=3.0.8
 Requires-Dist: biopython>=1.81
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: pandas>=2.2.2
 Requires-Dist: setuptools>=69.2.0
 Provides-Extra: dev
 Requires-Dist: auditwheel>=5.1.2; extra == "dev"
 Requires-Dist: build>=0.9.0; extra == "dev"
 Requires-Dist: coverage>=4.5.4; extra == "dev"
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
```

### Comparing `kmerdb-0.7.9/kmerdb.egg-info/SOURCES.txt` & `kmerdb-0.8.0/kmerdb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 kmerdb/distance.c
 kmerdb/distance.pyx
 kmerdb/fileutil.py
 kmerdb/graph.py
 kmerdb/index.py
 kmerdb/kmer.py
 kmerdb/legacy.py
+kmerdb/logger.py
 kmerdb/parse.py
 kmerdb/probability.py
 kmerdb/python_distances.py
 kmerdb/util.py
 kmerdb.egg-info/PKG-INFO
 kmerdb.egg-info/SOURCES.txt
 kmerdb.egg-info/dependency_links.txt
```

### Comparing `kmerdb-0.7.9/pyproject.toml` & `kmerdb-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # requires numpy and cython for custom cython correlation function
 
 requires = ["setuptools>=69.2.0", "numpy>=1.21.2", "Cython>=3.0.8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kmerdb"
-version = "0.7.9"
+version = "0.8.0"
 description = "Yet another corretion to the 'yet another correction to just a k-mer counter...'"
 readme = "README.md"
 authors = [{name="Matt Ralston <mralston.development@gmail.com>", email="mralston.development@gmail.com"}]
 license = { file = "LICENSE.txt" }
 classifiers = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
@@ -74,14 +74,15 @@
 	     "jsonschema>=4.17.3", # what was going on here? inflection points. and ms tori
 	     "psutil>=4.2.0", # not important, just as far as i was willing to go
 	     "Cython>=3.0.8",
 	     "biopython>=1.81",
              "scipy>=1.11.4",
              "scikit-learn==1.2.2",
              "matplotlib>=3.5.3",
+	     "pandas>=2.2.2",
              "setuptools>=69.2.0",
 	     ]
 
 requires-python = ">=3.7.4"
 #requires-python = ">=3.12.2"
 
 [project.optional-dependencies]
```

### Comparing `kmerdb-0.7.9/setup.py` & `kmerdb-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 long_description = 'See README.md for details'
 URL = 'https://github.com/MatthewRalston/kmerdb'
 CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz"
 EMAIL = 'mralston.development@gmail.com'
 AUTHOR = 'fross'
 REQUIRES_PYTHON = ">=3.7.4"
 #REQUIRES_PYTHON = '>=3.12.2'
-VERSION = "0.7.9"
+VERSION = "0.8.0"
 KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer"]
 CLASSIFIERS = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
 	    "Development Status :: 7 - Inactive",
 	    "Environment :: Console",
 	    "Intended Audience :: Developers",
```

### Comparing `kmerdb-0.7.9/test/test_kmer.py` & `kmerdb-0.8.0/test/test_kmer.py`

 * *Files identical despite different names*

