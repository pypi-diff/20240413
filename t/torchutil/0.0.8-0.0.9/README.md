# Comparing `tmp/torchutil-0.0.8.tar.gz` & `tmp/torchutil-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchutil-0.0.8.tar", last modified: Wed Nov 29 15:59:45 2023, max compression
+gzip compressed data, was "torchutil-0.0.9.tar", last modified: Tue Dec  5 23:58:12 2023, max compression
```

## Comparing `torchutil-0.0.8.tar` & `torchutil-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.512061 torchutil-0.0.8/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1069 2023-10-10 14:46:18.000000 torchutil-0.0.8/LICENSE
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    20306 2023-11-29 15:59:45.512061 torchutil-0.0.8/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    19816 2023-11-16 16:54:39.000000 torchutil-0.0.8/README.md
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-11-29 15:59:45.512061 torchutil-0.0.8/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      745 2023-11-29 15:58:35.000000 torchutil-0.0.8/setup.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.504061 torchutil-0.0.8/torchutil/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      193 2023-11-16 16:50:56.000000 torchutil-0.0.8/torchutil/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5036 2023-11-24 06:37:27.000000 torchutil-0.0.8/torchutil/checkpoint.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1904 2023-11-19 17:41:47.000000 torchutil-0.0.8/torchutil/download.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      860 2023-11-05 20:11:09.000000 torchutil-0.0.8/torchutil/iterator.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9268 2023-11-10 21:14:15.000000 torchutil-0.0.8/torchutil/metrics.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2562 2023-11-16 16:51:20.000000 torchutil-0.0.8/torchutil/notify.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.508061 torchutil-0.0.8/torchutil/paths/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      101 2023-11-16 16:28:48.000000 torchutil-0.0.8/torchutil/paths/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      601 2023-11-16 16:34:53.000000 torchutil-0.0.8/torchutil/paths/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.508061 torchutil-0.0.8/torchutil/paths/gather/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-11-10 15:05:23.000000 torchutil-0.0.8/torchutil/paths/gather/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4476 2023-11-10 16:06:39.000000 torchutil-0.0.8/torchutil/paths/gather/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.508061 torchutil-0.0.8/torchutil/paths/measure/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-11-10 15:05:23.000000 torchutil-0.0.8/torchutil/paths/measure/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1574 2023-11-29 15:57:46.000000 torchutil-0.0.8/torchutil/paths/measure/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1889 2023-11-29 15:57:30.000000 torchutil-0.0.8/torchutil/paths/measure/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.508061 torchutil-0.0.8/torchutil/paths/purge/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-11-04 18:36:55.000000 torchutil-0.0.8/torchutil/paths/purge/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1093 2023-11-10 16:38:26.000000 torchutil-0.0.8/torchutil/paths/purge/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1933 2023-11-29 15:56:57.000000 torchutil-0.0.8/torchutil/paths/purge/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3171 2023-10-11 01:28:39.000000 torchutil-0.0.8/torchutil/tensorboard.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1879 2023-11-20 00:18:32.000000 torchutil-0.0.8/torchutil/time.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-11-29 15:59:45.512061 torchutil-0.0.8/torchutil.egg-info/
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    20306 2023-11-29 15:59:45.000000 torchutil-0.0.8/torchutil.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      684 2023-11-29 15:59:45.000000 torchutil-0.0.8/torchutil.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-11-29 15:59:45.000000 torchutil-0.0.8/torchutil.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       37 2023-11-29 15:59:45.000000 torchutil-0.0.8/torchutil.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       10 2023-11-29 15:59:45.000000 torchutil-0.0.8/torchutil.egg-info/top_level.txt
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.701948 torchutil-0.0.9/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1069 2023-10-10 14:46:18.000000 torchutil-0.0.9/LICENSE
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    22026 2023-12-05 23:58:12.701948 torchutil-0.0.9/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    21536 2023-12-05 23:55:44.000000 torchutil-0.0.9/README.md
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-12-05 23:58:12.701948 torchutil-0.0.9/setup.cfg
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      745 2023-12-05 23:55:44.000000 torchutil-0.0.9/setup.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      216 2023-12-05 23:55:44.000000 torchutil-0.0.9/torchutil/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5036 2023-11-24 06:37:27.000000 torchutil-0.0.9/torchutil/checkpoint.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1904 2023-11-19 17:41:47.000000 torchutil-0.0.9/torchutil/download.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2661 2023-12-05 23:55:44.000000 torchutil-0.0.9/torchutil/iterator.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9268 2023-11-10 21:14:15.000000 torchutil-0.0.9/torchutil/metrics.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2562 2023-11-16 16:51:20.000000 torchutil-0.0.9/torchutil/notify.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil/paths/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      101 2023-11-16 16:28:48.000000 torchutil-0.0.9/torchutil/paths/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      601 2023-11-16 16:34:53.000000 torchutil-0.0.9/torchutil/paths/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil/paths/gather/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-11-10 15:05:23.000000 torchutil-0.0.9/torchutil/paths/gather/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4476 2023-11-10 16:06:39.000000 torchutil-0.0.9/torchutil/paths/gather/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil/paths/measure/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-11-10 15:05:23.000000 torchutil-0.0.9/torchutil/paths/measure/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1551 2023-11-29 19:11:02.000000 torchutil-0.0.9/torchutil/paths/measure/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1979 2023-11-29 19:10:53.000000 torchutil-0.0.9/torchutil/paths/measure/core.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil/paths/purge/
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-11-04 18:36:55.000000 torchutil-0.0.9/torchutil/paths/purge/__init__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1070 2023-11-29 19:09:33.000000 torchutil-0.0.9/torchutil/paths/purge/__main__.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2023 2023-11-29 19:10:28.000000 torchutil-0.0.9/torchutil/paths/purge/core.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3171 2023-10-11 01:28:39.000000 torchutil-0.0.9/torchutil/tensorboard.py
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1879 2023-11-20 00:18:32.000000 torchutil-0.0.9/torchutil/time.py
+drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-05 23:58:12.697948 torchutil-0.0.9/torchutil.egg-info/
+-rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    22026 2023-12-05 23:58:12.000000 torchutil-0.0.9/torchutil.egg-info/PKG-INFO
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      684 2023-12-05 23:58:12.000000 torchutil-0.0.9/torchutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-12-05 23:58:12.000000 torchutil-0.0.9/torchutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       37 2023-12-05 23:58:12.000000 torchutil-0.0.9/torchutil.egg-info/requires.txt
+-rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       10 2023-12-05 23:58:12.000000 torchutil-0.0.9/torchutil.egg-info/top_level.txt
```

### Comparing `torchutil-0.0.8/LICENSE` & `torchutil-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/PKG-INFO` & `torchutil-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: torchutil
-Version: 0.0.8
-Summary: PyTorch utilities for developing deep learning frameworks
-Home-page: https://github.com/maxrmorrison/torchutil
-Author: Max Morrison
-Author-email: maxrmorrison@gmail.com
-License: MIT
-Keywords: pytorch,utility,training
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: accelerate
-Requires-Dist: apprise
-Requires-Dist: tensorboard
-Requires-Dist: torch
-
 <h1 align="center">torchutil</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/torchutil.svg)](https://pypi.python.org/pypi/torchutil)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/torchutil)](https://pepy.tech/project/torchutil)
 
@@ -38,14 +21,15 @@
 - [Download](#download)
     * [`torchutil.download.file`](#torchutildownloadfile)
     * [`torchutil.download.tarbz2`](#torchutildownloadtarbz2)
     * [`torchutil.download.targz`](#torchutildownloadtargz)
     * [`torchutil.download.zip`](#torchutildownloadzip)
 - [Iterator](#iterator)
     * [`torchutil.iterator`](#torchutiliterator)
+    * [`torchutil.multiprocess_iterator`](#torchutil.multiprocess_iterator)
 - [Metrics](#metrics)
     * [`torchutil.metrics.Accuracy`](#torchutilmetricsaccuracy)
     * [`torchutil.metrics.Average`](#torchutilmetricsaverage)
     * [`torchutil.metrics.F1`](#torchutilmetricsf1)
     * [`torchutil.metrics.L1`](#torchutilmetricsl1)
     * [`torchutil.metrics.MeanStd`](#torchutilmetricsmeanstd)
     * [`torchutil.metrics.Precision`](#torchutilmetricsprecision)
@@ -238,17 +222,38 @@
     """
 ```
 
 
 ## Iterator
 
 ```python
+import time
+import torchutil
+
+def wait(seconds):
+    time.sleep(seconds)
+
+n = 8
+iterable = range(n)
+
+# Monitor single-process job
+for i in torchutil.iterator(iterable, message='single-process'):
+    wait(i)
+
+# Monitor multi-process job
+torchutil.multiprocess_iterator(wait, iterable, message='multi-process')
+```
+
+
+### `torchutil.iterator`
+
+```python
 def iterator(
     iterable: Iterable,
-    message: Optional[str],
+    message: Optional[str] = None,
     initial: int = 0,
     total: Optional[int] = None
 ) -> Iterable:
     """Create a tqdm iterator
 
     Arguments
         iterable
@@ -259,14 +264,50 @@
             Position to display corresponding to index zero of iterable
         total
             Length of the iterable; defaults to len(iterable)
     """
 ```
 
 
+### `torchutil.multiprocess_iterator`
+
+```python
+def multiprocess_iterator(
+    process: Callable,
+    iterable: Iterable,
+    message: Optional[str] = None,
+    initial: int = 0,
+    total: Optional[int] = None,
+    num_workers: int = os.cpu_count(),
+    worker_chunk_size: Optional[int] = None
+) -> List:
+    """Create a multiprocess tqdm iterator
+
+    Arguments
+        process
+            The single-argument function called by each multiprocess worker
+        iterable
+            Items to iterate over
+        message
+            Static message to display
+        initial
+            Position to display corresponding to index zero of iterable
+        total
+            Length of the iterable; defaults to len(iterable)
+        num_workers
+            Multiprocessing pool size; defaults to number of logical CPU cores
+        worker_chunk_size
+            Number of items sent to each multiprocessing worker
+
+    Returns
+        Return values of calling process on each item, in original order
+    """
+```
+
+
 ## Metrics
 
 ```python
 import torch
 import torchutil
 
 # Define a custom, batch-updating loss metric
@@ -657,20 +698,23 @@
 ```
 
 
 ### `torchutil.paths.measure`
 
 ```python
 def measure(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
     recursive: bool = False,
     unit='B'
 ) -> Union[int, float]:
     """Measure data usage of files and directories
 
     Arguments
         globs
@@ -712,31 +756,37 @@
 ```
 
 
 ### `torchutil.paths.purge`
 
 ```python
 def purge(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
-    recursive: bool = False
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
+    recursive: bool = False,
+    force: bool = False
 ) -> None:
     """Remove all files and directories within directory matching glob
 
     Arguments
         globs
-            Globs matching files to delete
+            Globs matching paths to delete
         roots
             Directories to apply glob searches; current directory by default
         recursive
             Apply globs to all subdirectories of root directories
+        force
+            Skip user confirmation of deletion
     """
 ```
 
 This function also has a command-line interface.
 
 ```
 python -m torchutil.paths.purge \
@@ -755,14 +805,16 @@
 optional arguments:
   -h, --help
     show this help message and exit
   --roots ROOTS
     Directories to apply glob searches; current directory by default
   --recursive
     Apply globs to all subdirectories of root directories
+  --force
+    Skip user confirmation of deletion
 ```
 
 
 ## Tensorboard
 
 ```python
 import matplotlib.pyplot as plt
```

### Comparing `torchutil-0.0.8/README.md` & `torchutil-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: torchutil
+Version: 0.0.9
+Summary: PyTorch utilities for developing deep learning frameworks
+Home-page: https://github.com/maxrmorrison/torchutil
+Author: Max Morrison
+Author-email: maxrmorrison@gmail.com
+License: MIT
+Keywords: pytorch,utility,training
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: accelerate
+Requires-Dist: apprise
+Requires-Dist: tensorboard
+Requires-Dist: torch
+
 <h1 align="center">torchutil</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/torchutil.svg)](https://pypi.python.org/pypi/torchutil)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/torchutil)](https://pepy.tech/project/torchutil)
 
@@ -21,14 +38,15 @@
 - [Download](#download)
     * [`torchutil.download.file`](#torchutildownloadfile)
     * [`torchutil.download.tarbz2`](#torchutildownloadtarbz2)
     * [`torchutil.download.targz`](#torchutildownloadtargz)
     * [`torchutil.download.zip`](#torchutildownloadzip)
 - [Iterator](#iterator)
     * [`torchutil.iterator`](#torchutiliterator)
+    * [`torchutil.multiprocess_iterator`](#torchutil.multiprocess_iterator)
 - [Metrics](#metrics)
     * [`torchutil.metrics.Accuracy`](#torchutilmetricsaccuracy)
     * [`torchutil.metrics.Average`](#torchutilmetricsaverage)
     * [`torchutil.metrics.F1`](#torchutilmetricsf1)
     * [`torchutil.metrics.L1`](#torchutilmetricsl1)
     * [`torchutil.metrics.MeanStd`](#torchutilmetricsmeanstd)
     * [`torchutil.metrics.Precision`](#torchutilmetricsprecision)
@@ -221,17 +239,38 @@
     """
 ```
 
 
 ## Iterator
 
 ```python
+import time
+import torchutil
+
+def wait(seconds):
+    time.sleep(seconds)
+
+n = 8
+iterable = range(n)
+
+# Monitor single-process job
+for i in torchutil.iterator(iterable, message='single-process'):
+    wait(i)
+
+# Monitor multi-process job
+torchutil.multiprocess_iterator(wait, iterable, message='multi-process')
+```
+
+
+### `torchutil.iterator`
+
+```python
 def iterator(
     iterable: Iterable,
-    message: Optional[str],
+    message: Optional[str] = None,
     initial: int = 0,
     total: Optional[int] = None
 ) -> Iterable:
     """Create a tqdm iterator
 
     Arguments
         iterable
@@ -242,14 +281,50 @@
             Position to display corresponding to index zero of iterable
         total
             Length of the iterable; defaults to len(iterable)
     """
 ```
 
 
+### `torchutil.multiprocess_iterator`
+
+```python
+def multiprocess_iterator(
+    process: Callable,
+    iterable: Iterable,
+    message: Optional[str] = None,
+    initial: int = 0,
+    total: Optional[int] = None,
+    num_workers: int = os.cpu_count(),
+    worker_chunk_size: Optional[int] = None
+) -> List:
+    """Create a multiprocess tqdm iterator
+
+    Arguments
+        process
+            The single-argument function called by each multiprocess worker
+        iterable
+            Items to iterate over
+        message
+            Static message to display
+        initial
+            Position to display corresponding to index zero of iterable
+        total
+            Length of the iterable; defaults to len(iterable)
+        num_workers
+            Multiprocessing pool size; defaults to number of logical CPU cores
+        worker_chunk_size
+            Number of items sent to each multiprocessing worker
+
+    Returns
+        Return values of calling process on each item, in original order
+    """
+```
+
+
 ## Metrics
 
 ```python
 import torch
 import torchutil
 
 # Define a custom, batch-updating loss metric
@@ -640,20 +715,23 @@
 ```
 
 
 ### `torchutil.paths.measure`
 
 ```python
 def measure(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
     recursive: bool = False,
     unit='B'
 ) -> Union[int, float]:
     """Measure data usage of files and directories
 
     Arguments
         globs
@@ -695,31 +773,37 @@
 ```
 
 
 ### `torchutil.paths.purge`
 
 ```python
 def purge(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
-    recursive: bool = False
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
+    recursive: bool = False,
+    force: bool = False
 ) -> None:
     """Remove all files and directories within directory matching glob
 
     Arguments
         globs
-            Globs matching files to delete
+            Globs matching paths to delete
         roots
             Directories to apply glob searches; current directory by default
         recursive
             Apply globs to all subdirectories of root directories
+        force
+            Skip user confirmation of deletion
     """
 ```
 
 This function also has a command-line interface.
 
 ```
 python -m torchutil.paths.purge \
@@ -738,14 +822,16 @@
 optional arguments:
   -h, --help
     show this help message and exit
   --roots ROOTS
     Directories to apply glob searches; current directory by default
   --recursive
     Apply globs to all subdirectories of root directories
+  --force
+    Skip user confirmation of deletion
 ```
 
 
 ## Tensorboard
 
 ```python
 import matplotlib.pyplot as plt
```

### Comparing `torchutil-0.0.8/setup.py` & `torchutil-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md') as file:
     long_description = file.read()
 
 
 setup(
     name='torchutil',
     description='PyTorch utilities for developing deep learning frameworks',
-    version='0.0.8',
+    version='0.0.9',
     author='Max Morrison',
     author_email='maxrmorrison@gmail.com',
     url='https://github.com/maxrmorrison/torchutil',
     install_requires=['accelerate', 'apprise', 'tensorboard', 'torch'],
     packages=find_packages(),
     package_data={'torchutil': ['assets/*', 'assets/*/*']},
     long_description=long_description,
```

### Comparing `torchutil-0.0.8/torchutil/checkpoint.py` & `torchutil-0.0.9/torchutil/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/download.py` & `torchutil-0.0.9/torchutil/download.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/metrics.py` & `torchutil-0.0.9/torchutil/metrics.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/notify.py` & `torchutil-0.0.9/torchutil/notify.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/paths/core.py` & `torchutil-0.0.9/torchutil/paths/core.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/paths/gather/core.py` & `torchutil-0.0.9/torchutil/paths/gather/core.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/paths/measure/__main__.py` & `torchutil-0.0.9/torchutil/paths/measure/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 def parse_args():
     """Parse command-line arguments"""
     parser = argparse.ArgumentParser(
         description='Measure data usage of files and directories')
     parser.add_argument(
         '--globs',
-        required=True,
         nargs='+',
         help='Globs matching paths to measure')
     parser.add_argument(
         '--roots',
         type=Path,
         nargs='+',
         help='Directories to apply glob searches; '
```

### Comparing `torchutil-0.0.8/torchutil/paths/measure/core.py` & `torchutil-0.0.9/torchutil/paths/measure/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ###############################################################################
 # Measure dataset sizes
 ###############################################################################
 
 
 def measure(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
         List[
             Union[
                 Union[str, bytes, os.PathLike],
                 List[Union[str, bytes, os.PathLike]]
             ]
         ]
@@ -41,18 +41,19 @@
             Directories to apply glob searches; current directory by default
         recursive
             Apply globs to all subdirectories of root directories
         unit
             Unit of memory utilization (bytes to terabytes); default bytes
     """
     # Argument handling
-    if isinstance(globs, str):
+    if not isinstance(globs, list):
         globs = [globs]
     if not isinstance(roots, list):
         roots = [roots]
+    globs = ['*' if glob is None else glob for glob in globs]
     roots = [Path() if root is None else Path(root) for root in roots]
 
     # Get paths to delete
     paths = []
     for root in roots:
         root = Path(root)
         for glob in globs:
```

### Comparing `torchutil-0.0.8/torchutil/paths/purge/__main__.py` & `torchutil-0.0.9/torchutil/paths/purge/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 def parse_args():
     """Parse command-line arguments"""
     parser = argparse.ArgumentParser(
         description='Remove files and directories')
     parser.add_argument(
         '--globs',
-        required=True,
         nargs='+',
         help='Globs matching paths to delete')
     parser.add_argument(
         '--roots',
         type=Path,
         nargs='+',
         help='Directories to apply glob searches; '
```

### Comparing `torchutil-0.0.8/torchutil/paths/purge/core.py` & `torchutil-0.0.9/torchutil/paths/purge/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ###############################################################################
 # Purge
 ###############################################################################
 
 
 def purge(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
         List[
             Union[
                 Union[str, bytes, os.PathLike],
                 List[Union[str, bytes, os.PathLike]]
             ]
         ]
@@ -33,18 +33,19 @@
             Directories to apply glob searches; current directory by default
         recursive
             Apply globs to all subdirectories of root directories
         force
             Skip user confirmation of deletion
     """
     # Argument handling
-    if isinstance(globs, str):
+    if not isinstance(globs, list):
         globs = [globs]
     if not isinstance(roots, list):
         roots = [roots]
+    globs = ['*' if glob is None else glob for glob in globs]
     roots = [Path() if root is None else Path(root) for root in roots]
 
     # Get paths to delete
     paths = []
     for root in roots:
         root = Path(root)
         for glob in globs:
```

### Comparing `torchutil-0.0.8/torchutil/tensorboard.py` & `torchutil-0.0.9/torchutil/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil/time.py` & `torchutil-0.0.9/torchutil/time.py`

 * *Files identical despite different names*

### Comparing `torchutil-0.0.8/torchutil.egg-info/PKG-INFO` & `torchutil-0.0.9/torchutil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchutil
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyTorch utilities for developing deep learning frameworks
 Home-page: https://github.com/maxrmorrison/torchutil
 Author: Max Morrison
 Author-email: maxrmorrison@gmail.com
 License: MIT
 Keywords: pytorch,utility,training
 Classifier: License :: OSI Approved :: MIT License
@@ -38,14 +38,15 @@
 - [Download](#download)
     * [`torchutil.download.file`](#torchutildownloadfile)
     * [`torchutil.download.tarbz2`](#torchutildownloadtarbz2)
     * [`torchutil.download.targz`](#torchutildownloadtargz)
     * [`torchutil.download.zip`](#torchutildownloadzip)
 - [Iterator](#iterator)
     * [`torchutil.iterator`](#torchutiliterator)
+    * [`torchutil.multiprocess_iterator`](#torchutil.multiprocess_iterator)
 - [Metrics](#metrics)
     * [`torchutil.metrics.Accuracy`](#torchutilmetricsaccuracy)
     * [`torchutil.metrics.Average`](#torchutilmetricsaverage)
     * [`torchutil.metrics.F1`](#torchutilmetricsf1)
     * [`torchutil.metrics.L1`](#torchutilmetricsl1)
     * [`torchutil.metrics.MeanStd`](#torchutilmetricsmeanstd)
     * [`torchutil.metrics.Precision`](#torchutilmetricsprecision)
@@ -238,17 +239,38 @@
     """
 ```
 
 
 ## Iterator
 
 ```python
+import time
+import torchutil
+
+def wait(seconds):
+    time.sleep(seconds)
+
+n = 8
+iterable = range(n)
+
+# Monitor single-process job
+for i in torchutil.iterator(iterable, message='single-process'):
+    wait(i)
+
+# Monitor multi-process job
+torchutil.multiprocess_iterator(wait, iterable, message='multi-process')
+```
+
+
+### `torchutil.iterator`
+
+```python
 def iterator(
     iterable: Iterable,
-    message: Optional[str],
+    message: Optional[str] = None,
     initial: int = 0,
     total: Optional[int] = None
 ) -> Iterable:
     """Create a tqdm iterator
 
     Arguments
         iterable
@@ -259,14 +281,50 @@
             Position to display corresponding to index zero of iterable
         total
             Length of the iterable; defaults to len(iterable)
     """
 ```
 
 
+### `torchutil.multiprocess_iterator`
+
+```python
+def multiprocess_iterator(
+    process: Callable,
+    iterable: Iterable,
+    message: Optional[str] = None,
+    initial: int = 0,
+    total: Optional[int] = None,
+    num_workers: int = os.cpu_count(),
+    worker_chunk_size: Optional[int] = None
+) -> List:
+    """Create a multiprocess tqdm iterator
+
+    Arguments
+        process
+            The single-argument function called by each multiprocess worker
+        iterable
+            Items to iterate over
+        message
+            Static message to display
+        initial
+            Position to display corresponding to index zero of iterable
+        total
+            Length of the iterable; defaults to len(iterable)
+        num_workers
+            Multiprocessing pool size; defaults to number of logical CPU cores
+        worker_chunk_size
+            Number of items sent to each multiprocessing worker
+
+    Returns
+        Return values of calling process on each item, in original order
+    """
+```
+
+
 ## Metrics
 
 ```python
 import torch
 import torchutil
 
 # Define a custom, batch-updating loss metric
@@ -657,20 +715,23 @@
 ```
 
 
 ### `torchutil.paths.measure`
 
 ```python
 def measure(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
     recursive: bool = False,
     unit='B'
 ) -> Union[int, float]:
     """Measure data usage of files and directories
 
     Arguments
         globs
@@ -712,31 +773,37 @@
 ```
 
 
 ### `torchutil.paths.purge`
 
 ```python
 def purge(
-    globs: Union[str, List[str]],
+    globs: Optional[List[Union[str, List[str]]]] = None,
     roots: Optional[
-        Union[
-            Union[str, bytes, os.PathLike],
-            List[Union[str, bytes, os.PathLike]]
-        ]] = None,
-    recursive: bool = False
+        List[
+            Union[
+                Union[str, bytes, os.PathLike],
+                List[Union[str, bytes, os.PathLike]]
+            ]
+        ]
+    ] = None,
+    recursive: bool = False,
+    force: bool = False
 ) -> None:
     """Remove all files and directories within directory matching glob
 
     Arguments
         globs
-            Globs matching files to delete
+            Globs matching paths to delete
         roots
             Directories to apply glob searches; current directory by default
         recursive
             Apply globs to all subdirectories of root directories
+        force
+            Skip user confirmation of deletion
     """
 ```
 
 This function also has a command-line interface.
 
 ```
 python -m torchutil.paths.purge \
@@ -755,14 +822,16 @@
 optional arguments:
   -h, --help
     show this help message and exit
   --roots ROOTS
     Directories to apply glob searches; current directory by default
   --recursive
     Apply globs to all subdirectories of root directories
+  --force
+    Skip user confirmation of deletion
 ```
 
 
 ## Tensorboard
 
 ```python
 import matplotlib.pyplot as plt
```

### Comparing `torchutil-0.0.8/torchutil.egg-info/SOURCES.txt` & `torchutil-0.0.9/torchutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

