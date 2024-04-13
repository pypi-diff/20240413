# Comparing `tmp/xian_contracting-0.1.2.tar.gz` & `tmp/xian_contracting-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xian_contracting-0.1.2.tar", max compression
+gzip compressed data, was "xian_contracting-0.1.3.tar", max compression
```

## Comparing `xian_contracting-0.1.2.tar` & `xian_contracting-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35149 2024-02-28 22:50:02.409938 xian_contracting-0.1.2/LICENSE
--rw-r--r--   0        0        0     1389 2024-03-25 17:29:18.195376 xian_contracting-0.1.2/README.md
--rw-r--r--   0        0        0      365 2024-04-12 23:59:51.452324 xian_contracting-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       85 2024-04-12 23:41:42.187329 xian_contracting-0.1.2/xian_contracting/.gitignore
--rw-r--r--   0        0        0        7 2024-04-12 23:41:42.187399 xian_contracting-0.1.2/xian_contracting/.version
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187438 xian_contracting-0.1.2/xian_contracting/__init__.py
--rw-r--r--   0        0        0    11775 2024-04-12 23:59:29.649917 xian_contracting-0.1.2/xian_contracting/client.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187883 xian_contracting-0.1.2/xian_contracting/compilation/__init__.py
--rw-r--r--   0        0        0     3993 2024-04-12 23:59:29.657942 xian_contracting-0.1.2/xian_contracting/compilation/compiler.py
--rw-r--r--   0        0        0    11682 2024-04-12 23:59:29.642039 xian_contracting-0.1.2/xian_contracting/compilation/linter.py
--rw-r--r--   0        0        0     1431 2024-04-12 23:41:42.188181 xian_contracting-0.1.2/xian_contracting/compilation/parser.py
--rw-r--r--   0        0        0     2733 2024-04-12 23:59:29.659873 xian_contracting-0.1.2/xian_contracting/compilation/whitelists.py
--rw-r--r--   0        0        0      670 2024-04-12 23:41:42.188466 xian_contracting-0.1.2/xian_contracting/config.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188542 xian_contracting-0.1.2/xian_contracting/contracts/__init__.py
--rw-r--r--   0        0        0      931 2024-04-12 23:41:42.188620 xian_contracting-0.1.2/xian_contracting/contracts/submission.s.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188683 xian_contracting-0.1.2/xian_contracting/db/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-12 23:59:29.631958 xian_contracting-0.1.2/xian_contracting/db/contract.py
--rw-r--r--   0        0        0    17845 2024-04-12 23:59:29.634728 xian_contracting-0.1.2/xian_contracting/db/driver.py
--rw-r--r--   0        0        0     5541 2024-04-12 23:59:29.646654 xian_contracting-0.1.2/xian_contracting/db/encoder.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.189379 xian_contracting-0.1.2/xian_contracting/db/hdf5/__init__.py
--rw-r--r--   0        0        0     7083 2024-04-12 23:41:42.189581 xian_contracting-0.1.2/xian_contracting/db/hdf5/h5c.c
--rw-r--r--   0        0        0     1836 2024-04-12 23:59:29.622042 xian_contracting-0.1.2/xian_contracting/db/hdf5/hdf5.py
--rw-r--r--   0        0        0     4679 2024-04-12 23:59:29.661491 xian_contracting-0.1.2/xian_contracting/db/orm.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190019 xian_contracting-0.1.2/xian_contracting/execution/__init__.py
--rw-r--r--   0        0        0     6224 2024-04-12 23:59:29.627638 xian_contracting-0.1.2/xian_contracting/execution/executor.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190327 xian_contracting-0.1.2/xian_contracting/execution/metering/__init__.py
--rw-r--r--   0        0        0      887 2024-04-12 23:41:42.190405 xian_contracting-0.1.2/xian_contracting/execution/metering/cu_costs.const
--rw-r--r--   0        0        0     1540 2024-04-12 23:41:42.190472 xian_contracting-0.1.2/xian_contracting/execution/metering/datastack.h
--rw-r--r--   0        0        0      685 2024-04-12 23:41:42.190540 xian_contracting-0.1.2/xian_contracting/execution/metering/filedisp.h
--rw-r--r--   0        0        0      709 2024-04-12 23:41:42.190607 xian_contracting-0.1.2/xian_contracting/execution/metering/stats.h
--rw-r--r--   0        0        0    13222 2024-04-12 23:41:42.190849 xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.c
--rw-r--r--   0        0        0     1985 2024-04-12 23:41:42.190914 xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.h
--rw-r--r--   0        0        0     2994 2024-04-12 23:41:42.190981 xian_contracting-0.1.2/xian_contracting/execution/metering/util.h
--rw-r--r--   0        0        0     4125 2024-04-12 23:59:29.651520 xian_contracting-0.1.2/xian_contracting/execution/module.py
--rw-r--r--   0        0        0     3080 2024-04-12 23:59:29.638246 xian_contracting-0.1.2/xian_contracting/execution/runtime.py
--rw-r--r--   0        0        0     5027 2024-04-12 23:41:42.191312 xian_contracting-0.1.2/xian_contracting/hlcpy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191372 xian_contracting-0.1.2/xian_contracting/stdlib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191439 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/__init__.py
--rw-r--r--   0        0        0     1184 2024-04-12 23:59:29.648140 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/access.py
--rw-r--r--   0        0        0     4726 2024-04-12 23:59:29.636816 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/decimal.py
--rw-r--r--   0        0        0      809 2024-04-12 23:41:42.191676 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/hashing.py
--rw-r--r--   0        0        0     2667 2024-04-12 23:59:29.655655 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/imports.py
--rw-r--r--   0        0        0     1407 2024-04-12 23:59:29.652728 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/orm.py
--rw-r--r--   0        0        0     2984 2024-04-12 23:59:29.639637 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/random.py
--rw-r--r--   0        0        0     7298 2024-04-12 23:59:29.644900 xian_contracting-0.1.2/xian_contracting/stdlib/bridge/time.py
--rw-r--r--   0        0        0      936 2024-04-12 23:59:29.630041 xian_contracting-0.1.2/xian_contracting/stdlib/env.py
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 xian_contracting-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-28 22:50:02.409938 xian_contracting-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1389 2024-03-25 17:29:18.195376 xian_contracting-0.1.3/README.md
+-rw-r--r--   0        0        0      365 2024-04-13 00:21:15.718066 xian_contracting-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-12 23:41:42.187329 xian_contracting-0.1.3/xian_contracting/.gitignore
+-rw-r--r--   0        0        0        7 2024-04-12 23:41:42.187399 xian_contracting-0.1.3/xian_contracting/.version
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187438 xian_contracting-0.1.3/xian_contracting/__init__.py
+-rw-r--r--   0        0        0    11775 2024-04-12 23:59:29.649917 xian_contracting-0.1.3/xian_contracting/client.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.187883 xian_contracting-0.1.3/xian_contracting/compilation/__init__.py
+-rw-r--r--   0        0        0     3993 2024-04-12 23:59:29.657942 xian_contracting-0.1.3/xian_contracting/compilation/compiler.py
+-rw-r--r--   0        0        0    11682 2024-04-12 23:59:29.642039 xian_contracting-0.1.3/xian_contracting/compilation/linter.py
+-rw-r--r--   0        0        0     1431 2024-04-12 23:41:42.188181 xian_contracting-0.1.3/xian_contracting/compilation/parser.py
+-rw-r--r--   0        0        0     2733 2024-04-12 23:59:29.659873 xian_contracting-0.1.3/xian_contracting/compilation/whitelists.py
+-rw-r--r--   0        0        0      670 2024-04-12 23:41:42.188466 xian_contracting-0.1.3/xian_contracting/config.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188542 xian_contracting-0.1.3/xian_contracting/contracts/__init__.py
+-rw-r--r--   0        0        0      931 2024-04-12 23:41:42.188620 xian_contracting-0.1.3/xian_contracting/contracts/submission.s.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.188683 xian_contracting-0.1.3/xian_contracting/db/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-12 23:59:29.631958 xian_contracting-0.1.3/xian_contracting/db/contract.py
+-rw-r--r--   0        0        0    17845 2024-04-12 23:59:29.634728 xian_contracting-0.1.3/xian_contracting/db/driver.py
+-rw-r--r--   0        0        0     5541 2024-04-12 23:59:29.646654 xian_contracting-0.1.3/xian_contracting/db/encoder.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.189379 xian_contracting-0.1.3/xian_contracting/db/hdf5/__init__.py
+-rw-r--r--   0        0        0     7083 2024-04-12 23:41:42.189581 xian_contracting-0.1.3/xian_contracting/db/hdf5/h5c.c
+-rw-r--r--   0        0        0     1836 2024-04-12 23:59:29.622042 xian_contracting-0.1.3/xian_contracting/db/hdf5/hdf5.py
+-rw-r--r--   0        0        0     4679 2024-04-12 23:59:29.661491 xian_contracting-0.1.3/xian_contracting/db/orm.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190019 xian_contracting-0.1.3/xian_contracting/execution/__init__.py
+-rw-r--r--   0        0        0     6224 2024-04-12 23:59:29.627638 xian_contracting-0.1.3/xian_contracting/execution/executor.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.190327 xian_contracting-0.1.3/xian_contracting/execution/metering/__init__.py
+-rw-r--r--   0        0        0      887 2024-04-12 23:41:42.190405 xian_contracting-0.1.3/xian_contracting/execution/metering/cu_costs.const
+-rw-r--r--   0        0        0     1540 2024-04-12 23:41:42.190472 xian_contracting-0.1.3/xian_contracting/execution/metering/datastack.h
+-rw-r--r--   0        0        0      685 2024-04-12 23:41:42.190540 xian_contracting-0.1.3/xian_contracting/execution/metering/filedisp.h
+-rw-r--r--   0        0        0      709 2024-04-12 23:41:42.190607 xian_contracting-0.1.3/xian_contracting/execution/metering/stats.h
+-rw-r--r--   0        0        0    13222 2024-04-12 23:41:42.190849 xian_contracting-0.1.3/xian_contracting/execution/metering/tracer.c
+-rw-r--r--   0        0        0     1985 2024-04-12 23:41:42.190914 xian_contracting-0.1.3/xian_contracting/execution/metering/tracer.h
+-rw-r--r--   0        0        0     2994 2024-04-12 23:41:42.190981 xian_contracting-0.1.3/xian_contracting/execution/metering/util.h
+-rw-r--r--   0        0        0     4125 2024-04-12 23:59:29.651520 xian_contracting-0.1.3/xian_contracting/execution/module.py
+-rw-r--r--   0        0        0     3080 2024-04-12 23:59:29.638246 xian_contracting-0.1.3/xian_contracting/execution/runtime.py
+-rw-r--r--   0        0        0     5027 2024-04-12 23:41:42.191312 xian_contracting-0.1.3/xian_contracting/hlcpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191372 xian_contracting-0.1.3/xian_contracting/stdlib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 23:41:42.191439 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-12 23:59:29.648140 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/access.py
+-rw-r--r--   0        0        0     4726 2024-04-12 23:59:29.636816 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/decimal.py
+-rw-r--r--   0        0        0      809 2024-04-12 23:41:42.191676 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/hashing.py
+-rw-r--r--   0        0        0     2667 2024-04-12 23:59:29.655655 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/imports.py
+-rw-r--r--   0        0        0     1407 2024-04-12 23:59:29.652728 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/orm.py
+-rw-r--r--   0        0        0     2984 2024-04-12 23:59:29.639637 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/random.py
+-rw-r--r--   0        0        0     7298 2024-04-12 23:59:29.644900 xian_contracting-0.1.3/xian_contracting/stdlib/bridge/time.py
+-rw-r--r--   0        0        0      936 2024-04-12 23:59:29.630041 xian_contracting-0.1.3/xian_contracting/stdlib/env.py
+-rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 xian_contracting-0.1.3/PKG-INFO
```

### Comparing `xian_contracting-0.1.2/LICENSE` & `xian_contracting-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/README.md` & `xian_contracting-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/client.py` & `xian_contracting-0.1.3/xian_contracting/client.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/compilation/compiler.py` & `xian_contracting-0.1.3/xian_contracting/compilation/compiler.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/compilation/linter.py` & `xian_contracting-0.1.3/xian_contracting/compilation/linter.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/compilation/parser.py` & `xian_contracting-0.1.3/xian_contracting/compilation/parser.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/compilation/whitelists.py` & `xian_contracting-0.1.3/xian_contracting/compilation/whitelists.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/config.py` & `xian_contracting-0.1.3/xian_contracting/config.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/contracts/submission.s.py` & `xian_contracting-0.1.3/xian_contracting/contracts/submission.s.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/contract.py` & `xian_contracting-0.1.3/xian_contracting/db/contract.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/driver.py` & `xian_contracting-0.1.3/xian_contracting/db/driver.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/encoder.py` & `xian_contracting-0.1.3/xian_contracting/db/encoder.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/hdf5/h5c.c` & `xian_contracting-0.1.3/xian_contracting/db/hdf5/h5c.c`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/hdf5/hdf5.py` & `xian_contracting-0.1.3/xian_contracting/db/hdf5/hdf5.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/db/orm.py` & `xian_contracting-0.1.3/xian_contracting/db/orm.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/executor.py` & `xian_contracting-0.1.3/xian_contracting/execution/executor.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/cu_costs.const` & `xian_contracting-0.1.3/xian_contracting/execution/metering/cu_costs.const`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/datastack.h` & `xian_contracting-0.1.3/xian_contracting/execution/metering/datastack.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/filedisp.h` & `xian_contracting-0.1.3/xian_contracting/execution/metering/filedisp.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/stats.h` & `xian_contracting-0.1.3/xian_contracting/execution/metering/stats.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.c` & `xian_contracting-0.1.3/xian_contracting/execution/metering/tracer.c`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/tracer.h` & `xian_contracting-0.1.3/xian_contracting/execution/metering/tracer.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/metering/util.h` & `xian_contracting-0.1.3/xian_contracting/execution/metering/util.h`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/module.py` & `xian_contracting-0.1.3/xian_contracting/execution/module.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/execution/runtime.py` & `xian_contracting-0.1.3/xian_contracting/execution/runtime.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/hlcpy/__init__.py` & `xian_contracting-0.1.3/xian_contracting/hlcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/access.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/access.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/decimal.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/decimal.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/hashing.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/hashing.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/imports.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/imports.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/orm.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/orm.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/random.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/random.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/bridge/time.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/bridge/time.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/xian_contracting/stdlib/env.py` & `xian_contracting-0.1.3/xian_contracting/stdlib/env.py`

 * *Files identical despite different names*

### Comparing `xian_contracting-0.1.2/PKG-INFO` & `xian_contracting-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xian-contracting
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: endogen
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astor (>=0.8.1,<0.9.0)
```

