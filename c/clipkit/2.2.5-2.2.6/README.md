# Comparing `tmp/clipkit-2.2.5.tar.gz` & `tmp/clipkit-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipkit-2.2.5.tar", last modified: Thu Apr  4 03:23:04 2024, max compression
+gzip compressed data, was "clipkit-2.2.6.tar", last modified: Fri Apr 12 23:23:04 2024, max compression
```

## Comparing `clipkit-2.2.5.tar` & `clipkit-2.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.954371 clipkit-2.2.5/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.2.5/LICENSE.md
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-04 03:23:04.954180 clipkit-2.2.5/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.2.5/README.md
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.953203 clipkit-2.2.5/clipkit/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/__init__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.2.5/clipkit/__main__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2129 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/api.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1849 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/args_processing.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5499 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/clipkit.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/exceptions.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2198 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/files.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.2.5/clipkit/helpers.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/logger.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      563 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/modes.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10486 2024-04-04 03:22:22.000000 clipkit-2.2.5/clipkit/msa.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9703 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/parser.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-18 22:22:33.000000 clipkit-2.2.5/clipkit/settings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/site_classification.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.2.5/clipkit/smart_gap_helper.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/stats.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-04-04 03:22:40.000000 clipkit-2.2.5/clipkit/version.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/warnings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.2.5/clipkit/write.py
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.953891 clipkit-2.2.5/clipkit.egg-info/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/SOURCES.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/dependency_links.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/entry_points.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/requires.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/top_level.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-04-04 03:23:04.954420 clipkit-2.2.5/setup.cfg
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1211 2024-02-18 20:19:59.000000 clipkit-2.2.5/setup.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.708958 clipkit-2.2.6/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.2.6/LICENSE.md
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-12 23:23:04.708525 clipkit-2.2.6/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.2.6/README.md
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.703202 clipkit-2.2.6/clipkit/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/__init__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.2.6/clipkit/__main__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2129 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/api.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1849 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/args_processing.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5517 2024-04-12 23:22:01.000000 clipkit-2.2.6/clipkit/clipkit.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/exceptions.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2198 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/files.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.2.6/clipkit/helpers.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/logger.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      563 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/modes.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10486 2024-04-04 03:22:22.000000 clipkit-2.2.6/clipkit/msa.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9703 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/parser.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-18 22:22:33.000000 clipkit-2.2.6/clipkit/settings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/site_classification.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.2.6/clipkit/smart_gap_helper.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/stats.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-04-12 23:22:08.000000 clipkit-2.2.6/clipkit/version.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/warnings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.2.6/clipkit/write.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.707066 clipkit-2.2.6/clipkit.egg-info/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/entry_points.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/requires.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/top_level.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-04-12 23:23:04.709199 clipkit-2.2.6/setup.cfg
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1211 2024-02-18 20:19:59.000000 clipkit-2.2.6/setup.py
```

### Comparing `clipkit-2.2.5/LICENSE.md` & `clipkit-2.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/PKG-INFO` & `clipkit-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.5 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.2.6 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
```

### Comparing `clipkit-2.2.5/README.md` & `clipkit-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/api.py` & `clipkit-2.2.6/clipkit/api.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/args_processing.py` & `clipkit-2.2.6/clipkit/args_processing.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/clipkit.py` & `clipkit-2.2.6/clipkit/clipkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         TrimmingMode.kpi_smart_gap,
         TrimmingMode.kpic_smart_gap,
     }:
         gaps = smart_gap_threshold_determination(alignment, gap_characters)
 
     site_positions_to_trim = None
     if mode == TrimmingMode.cst:
-        aln_length = len(alignment)
+        aln_length = alignment.get_alignment_length()
         site_positions_to_trim = (
             get_custom_sites_to_trim(auxiliary_file, aln_length) or []
         )
 
     msa = create_msa(alignment, gap_characters)
     msa.trim(
         mode,
```

### Comparing `clipkit-2.2.5/clipkit/files.py` & `clipkit-2.2.6/clipkit/files.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/helpers.py` & `clipkit-2.2.6/clipkit/helpers.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/modes.py` & `clipkit-2.2.6/clipkit/modes.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/msa.py` & `clipkit-2.2.6/clipkit/msa.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/parser.py` & `clipkit-2.2.6/clipkit/parser.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/site_classification.py` & `clipkit-2.2.6/clipkit/site_classification.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/smart_gap_helper.py` & `clipkit-2.2.6/clipkit/smart_gap_helper.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/stats.py` & `clipkit-2.2.6/clipkit/stats.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/warnings.py` & `clipkit-2.2.6/clipkit/warnings.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit/write.py` & `clipkit-2.2.6/clipkit/write.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/clipkit.egg-info/PKG-INFO` & `clipkit-2.2.6/clipkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.5 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.2.6 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
```

### Comparing `clipkit-2.2.5/clipkit.egg-info/SOURCES.txt` & `clipkit-2.2.6/clipkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.5/setup.py` & `clipkit-2.2.6/setup.py`

 * *Files identical despite different names*

