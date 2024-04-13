# Comparing `tmp/xdas-0.1b2.tar.gz` & `tmp/xdas-0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdas-0.1b2.tar", last modified: Sun Jul 16 15:01:44 2023, max compression
+gzip compressed data, was "xdas-0.1rc0.tar", last modified: Sat Apr 13 08:26:34 2024, max compression
```

## Comparing `xdas-0.1b2.tar` & `xdas-0.1rc0.tar`

### file list

```diff
@@ -1,31 +1,54 @@
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.556594 xdas-0.1b2/
--rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1b2/LICENSE.md
--rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-07-16 15:01:44.556439 xdas-0.1b2/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      664 2023-06-13 10:17:32.000000 xdas-0.1b2/README.md
--rw-r--r--   0 trabatto   (502) staff       (20)      602 2023-07-16 14:29:25.000000 xdas-0.1b2/pyproject.toml
--rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-07-16 15:01:44.556633 xdas-0.1b2/setup.cfg
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.553653 xdas-0.1b2/tests/
--rw-r--r--   0 trabatto   (502) staff       (20)    10709 2023-06-13 09:50:51.000000 xdas-0.1b2/tests/test_coordinates.py
--rw-r--r--   0 trabatto   (502) staff       (20)     1345 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_core.py
--rw-r--r--   0 trabatto   (502) staff       (20)     1754 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_database.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3017 2023-07-16 14:29:25.000000 xdas-0.1b2/tests/test_processing.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2289 2023-06-28 14:18:52.000000 xdas-0.1b2/tests/test_signal.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2069 2023-06-28 14:18:52.000000 xdas-0.1b2/tests/test_virtual.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.554833 xdas-0.1b2/xdas/
--rw-r--r--   0 trabatto   (502) staff       (20)      216 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)    12128 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/coordinates.py
--rw-r--r--   0 trabatto   (502) staff       (20)     5177 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/core.py
--rw-r--r--   0 trabatto   (502) staff       (20)    12502 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/database.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.556130 xdas-0.1b2/xdas/io/
--rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1b2/xdas/io/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)      677 2023-06-28 14:18:52.000000 xdas-0.1b2/xdas/io/asn.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-06-13 09:50:51.000000 xdas-0.1b2/xdas/io/febus.py
--rw-r--r--   0 trabatto   (502) staff       (20)     9506 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/processing.py
--rw-r--r--   0 trabatto   (502) staff       (20)     6127 2023-07-16 14:29:25.000000 xdas-0.1b2/xdas/signal.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3666 2023-06-28 14:18:52.000000 xdas-0.1b2/xdas/virtual.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-07-16 15:01:44.555705 xdas-0.1b2/xdas.egg-info/
--rw-r--r--   0 trabatto   (502) staff       (20)      200 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      479 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/SOURCES.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/dependency_links.txt
--rw-r--r--   0 trabatto   (502) staff       (20)      170 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/requires.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-07-16 15:01:44.000000 xdas-0.1b2/xdas.egg-info/top_level.txt
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.439315 xdas-0.1rc0/
+-rw-r--r--   0 trabatto   (502) staff       (20)    35149 2024-04-13 06:11:46.000000 xdas-0.1rc0/LICENSE.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      968 2024-04-13 08:26:34.439053 xdas-0.1rc0/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)     2638 2024-04-13 08:24:22.000000 xdas-0.1rc0/README.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      793 2024-04-13 08:24:22.000000 xdas-0.1rc0/pyproject.toml
+-rw-r--r--   0 trabatto   (502) staff       (20)       38 2024-04-13 08:26:34.439368 xdas-0.1rc0/setup.cfg
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.432686 xdas-0.1rc0/tests/
+-rw-r--r--   0 trabatto   (502) staff       (20)     7063 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_atoms.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    20821 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     6922 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    14018 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_dataarray.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     4410 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_datacollection.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2936 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_numpy.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3149 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_parallel.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1156 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_processing.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     4591 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    13715 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_virtual.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1341 2024-04-13 08:24:22.000000 xdas-0.1rc0/tests/test_xarray.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.433824 xdas-0.1rc0/xdas/
+-rw-r--r--   0 trabatto   (502) staff       (20)      718 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/__init__.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.435207 xdas-0.1rc0/xdas/atoms/
+-rw-r--r--   0 trabatto   (502) staff       (20)      138 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/atoms/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    13538 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/atoms/core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    17845 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/atoms/signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      169 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/config.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.436390 xdas-0.1rc0/xdas/core/
+-rw-r--r--   0 trabatto   (502) staff       (20)        0 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    27945 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    35176 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/dataarray.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    17102 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/datacollection.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    21459 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/methods.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3349 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/numpy.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    24856 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/core/routines.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     4521 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/fft.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.437344 xdas-0.1rc0/xdas/io/
+-rw-r--r--   0 trabatto   (502) staff       (20)       45 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/io/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      692 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/io/asn.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1296 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/io/febus.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      726 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/io/optasense.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      762 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/io/sintela.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     6310 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/parallel.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.437841 xdas-0.1rc0/xdas/processing/
+-rw-r--r--   0 trabatto   (502) staff       (20)       98 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/processing/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     5571 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/processing/core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1767 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/processing/monitor.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    31728 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3191 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/synthetics.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    17447 2024-04-13 08:24:22.000000 xdas-0.1rc0/xdas/virtual.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2024-04-13 08:26:34.438069 xdas-0.1rc0/xdas.egg-info/
+-rw-r--r--   0 trabatto   (502) staff       (20)      968 2024-04-13 08:26:34.000000 xdas-0.1rc0/xdas.egg-info/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      929 2024-04-13 08:26:34.000000 xdas-0.1rc0/xdas.egg-info/SOURCES.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        1 2024-04-13 08:26:34.000000 xdas-0.1rc0/xdas.egg-info/dependency_links.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)      220 2024-04-13 08:26:34.000000 xdas-0.1rc0/xdas.egg-info/requires.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        5 2024-04-13 08:26:34.000000 xdas-0.1rc0/xdas.egg-info/top_level.txt
```

### Comparing `xdas-0.1b2/LICENSE.md` & `xdas-0.1rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1b2/xdas/io/asn.py` & `xdas-0.1rc0/xdas/io/asn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import h5py
 import numpy as np
 
-from ..coordinates import Coordinate
-from ..database import Database
-from ..virtual import DataSource
+from ..core.dataarray import DataArray
+from ..virtual import VirtualSource
 
 
 def read(fname):
     with h5py.File(fname, "r") as file:
         header = file["header"]
-        t0 = np.datetime64(round(header["time"][()] * 1e6), "us")
-        dt = np.timedelta64(round(1e6 * header["dt"][()]), "us")
+        t0 = np.datetime64(round(header["time"][()] * 1e9), "ns")
+        dt = np.timedelta64(round(1e9 * header["dt"][()]), "ns")
         dx = header["dx"][()] * np.median(np.diff(header["channels"]))
-        data = DataSource(file["data"])
-    nt, nd = data.shape
-    time = Coordinate([0, nt - 1], [t0, t0 + (nt - 1) * dt])
-    distance = Coordinate([0, nd - 1], [0.0, (nd - 1) * dx])
-    return Database(data, {"time": time, "distance": distance})
+        data = VirtualSource(file["data"])
+    nt, nx = data.shape
+    time = {"tie_indices": [0, nt - 1], "tie_values": [t0, t0 + (nt - 1) * dt]}
+    distance = {"tie_indices": [0, nx - 1], "tie_values": [0.0, (nx - 1) * dx]}
+    return DataArray(data, {"time": time, "distance": distance})
```

