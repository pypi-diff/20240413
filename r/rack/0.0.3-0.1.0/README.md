# Comparing `tmp/rack-0.0.3.tar.gz` & `tmp/rack-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rack-0.0.3.tar", last modified: Sat Apr 13 05:36:24 2024, max compression
+gzip compressed data, was "rack-0.1.0.tar", last modified: Sat Apr 13 13:13:53 2024, max compression
```

## Comparing `rack-0.0.3.tar` & `rack-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.637436 rack-0.0.3/
-drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.636436 rack-0.0.3/LICENSES/
--rw-rw-r--   0 cJ        (1000) cJ        (1000)     1078 2024-04-13 05:32:55.000000 rack-0.0.3/LICENSES/MIT.txt
--rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 05:36:24.637436 rack-0.0.3/PKG-INFO
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      260 2024-04-13 05:29:52.000000 rack-0.0.3/README.rst
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      227 2024-04-13 05:35:08.000000 rack-0.0.3/__init__.py
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      593 2024-04-13 05:33:17.000000 rack-0.0.3/pyproject.toml
-drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:36:24.637436 rack-0.0.3/rack.egg-info/
--rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/PKG-INFO
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      177 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/SOURCES.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)        1 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/dependency_links.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)        5 2024-04-13 05:36:24.000000 rack-0.0.3/rack.egg-info/top_level.txt
--rw-rw-r--   0 cJ        (1000) cJ        (1000)       38 2024-04-13 05:36:24.637436 rack-0.0.3/setup.cfg
--rw-rw-r--   0 cJ        (1000) cJ        (1000)      425 2024-04-13 05:25:37.000000 rack-0.0.3/setup.py
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 13:13:53.720533 rack-0.1.0/
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 13:13:53.719533 rack-0.1.0/LICENSES/
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)     1078 2024-04-13 05:32:55.000000 rack-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 13:13:53.720533 rack-0.1.0/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      260 2024-04-13 05:29:52.000000 rack-0.1.0/README.rst
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      227 2024-04-13 13:13:12.000000 rack-0.1.0/__init__.py
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      593 2024-04-13 05:33:17.000000 rack-0.1.0/pyproject.toml
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 13:13:53.719533 rack-0.1.0/rack.egg-info/
+-rw-r--r--   0 cJ        (1000) cJ        (1000)     1892 2024-04-13 13:13:53.000000 rack-0.1.0/rack.egg-info/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      177 2024-04-13 13:13:53.000000 rack-0.1.0/rack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        1 2024-04-13 13:13:53.000000 rack-0.1.0/rack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        5 2024-04-13 13:13:53.000000 rack-0.1.0/rack.egg-info/top_level.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)       38 2024-04-13 13:13:53.720533 rack-0.1.0/setup.cfg
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      425 2024-04-13 05:25:37.000000 rack-0.1.0/setup.py
```

### Comparing `rack-0.0.3/LICENSES/MIT.txt` & `rack-0.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `rack-0.0.3/PKG-INFO` & `rack-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rack
-Version: 0.0.3
+Version: 0.1.0
 Summary: Persistent (LMDB-backed) data structures mimicking as Python native containers
 Author: Jérôme Carretero
 License: MIT License
         
         Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `rack-0.0.3/pyproject.toml` & `rack-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rack-0.0.3/rack.egg-info/PKG-INFO` & `rack-0.1.0/rack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rack
-Version: 0.0.3
+Version: 0.1.0
 Summary: Persistent (LMDB-backed) data structures mimicking as Python native containers
 Author: Jérôme Carretero
 License: MIT License
         
         Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

