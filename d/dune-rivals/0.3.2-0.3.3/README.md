# Comparing `tmp/dune_rivals-0.3.2.tar.gz` & `tmp/dune_rivals-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.3.2.tar", last modified: Sat Apr 13 18:24:04 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.3.tar", last modified: Sat Apr 13 18:28:19 2024, max compression
```

## Comparing `dune_rivals-0.3.2.tar` & `dune_rivals-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:24:04.238192 dune_rivals-0.3.2/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:24:04.237602 dune_rivals-0.3.2/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.2/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:24:04.237097 dune_rivals-0.3.2/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 18:24:04.000000 dune_rivals-0.3.2/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    16223 2024-04-13 18:23:32.000000 dune_rivals-0.3.2/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 18:23:59.000000 dune_rivals-0.3.2/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 18:24:04.238327 dune_rivals-0.3.2/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:28:19.997154 dune_rivals-0.3.3/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:28:19.996150 dune_rivals-0.3.3/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.3/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 18:28:19.995554 dune_rivals-0.3.3/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 18:28:19.000000 dune_rivals-0.3.3/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    16222 2024-04-13 18:27:49.000000 dune_rivals-0.3.3/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 18:28:15.000000 dune_rivals-0.3.3/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 18:28:19.997351 dune_rivals-0.3.3/setup.cfg
```

### Comparing `dune_rivals-0.3.2/dune_rivals.py` & `dune_rivals-0.3.3/dune_rivals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ray
 import time
 import numpy as np
 
 # TODO: double check that obj. store read is < 0.1 (S3 read time)
 # DEFINITIONS
-SLEEP_SECONDS_PER_TRAVEL_COORD = 0.001
+SLEEP_SECONDS_PER_TRAVEL_COORD = 1e-5
 SLEEP_SECONDS_READ_FROM_S3     = 0.100
 SLEEP_SECONDS_NOT_ON_SPICE     = 1.000
 
 MAP_DIM = int(1e3)
 SPICE_FIELD_PROB = 0.01
 SPICE_FILE_SKEW = 0.7
 S3_FILE = 2
```

