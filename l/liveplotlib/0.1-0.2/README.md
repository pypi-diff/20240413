# Comparing `tmp/liveplotlib-0.1.tar.gz` & `tmp/liveplotlib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveplotlib-0.1.tar", last modified: Fri Apr 12 23:35:51 2024, max compression
+gzip compressed data, was "liveplotlib-0.2.tar", last modified: Sat Apr 13 00:29:58 2024, max compression
```

## Comparing `liveplotlib-0.1.tar` & `liveplotlib-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 23:35:51.007201 liveplotlib-0.1/
--rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.1/LICENSE
--rw-rw-rw-   0        0        0     6069 2024-04-12 23:35:51.007201 liveplotlib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5490 2024-04-12 22:29:00.000000 liveplotlib-0.1/README.md
--rw-rw-rw-   0        0        0      108 2024-04-09 16:47:58.000000 liveplotlib-0.1/pyproject.toml
--rw-rw-rw-   0        0        0      716 2024-04-12 23:35:51.012203 liveplotlib-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 23:35:50.981878 liveplotlib-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 23:35:50.991201 liveplotlib-0.1/src/liveplotlib/
--rw-rw-rw-   0        0        0      280 2024-04-12 21:59:30.000000 liveplotlib-0.1/src/liveplotlib/__init__.py
--rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.1/src/liveplotlib/get_file_format.py
--rw-rw-rw-   0        0        0     1226 2024-04-12 21:49:28.000000 liveplotlib-0.1/src/liveplotlib/if_ipynb.py
--rw-rw-rw-   0        0        0     2863 2024-04-12 23:21:47.000000 liveplotlib-0.1/src/liveplotlib/live_plot_only_train.py
--rw-rw-rw-   0        0        0     4732 2024-04-12 23:25:03.000000 liveplotlib-0.1/src/liveplotlib/live_plot_train_and_val.py
-drwxrwxrwx   0        0        0        0 2024-04-12 23:35:51.006202 liveplotlib-0.1/src/liveplotlib.egg-info/
--rw-rw-rw-   0        0        0     6069 2024-04-12 23:35:50.000000 liveplotlib-0.1/src/liveplotlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-12 23:35:50.000000 liveplotlib-0.1/src/liveplotlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 23:35:50.000000 liveplotlib-0.1/src/liveplotlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-12 23:35:50.000000 liveplotlib-0.1/src/liveplotlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.515065 liveplotlib-0.2/
+-rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.2/LICENSE
+-rw-rw-rw-   0        0        0     6118 2024-04-13 00:29:58.515065 liveplotlib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5490 2024-04-12 22:29:00.000000 liveplotlib-0.2/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-13 00:24:49.000000 liveplotlib-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      758 2024-04-13 00:29:58.517066 liveplotlib-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.491026 liveplotlib-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.500229 liveplotlib-0.2/src/liveplotlib/
+-rw-rw-rw-   0        0        0      280 2024-04-12 21:59:30.000000 liveplotlib-0.2/src/liveplotlib/__init__.py
+-rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.2/src/liveplotlib/get_file_format.py
+-rw-rw-rw-   0        0        0     1226 2024-04-12 21:49:28.000000 liveplotlib-0.2/src/liveplotlib/if_ipynb.py
+-rw-rw-rw-   0        0        0     2863 2024-04-12 23:21:47.000000 liveplotlib-0.2/src/liveplotlib/live_plot_only_train.py
+-rw-rw-rw-   0        0        0     4732 2024-04-12 23:25:03.000000 liveplotlib-0.2/src/liveplotlib/live_plot_train_and_val.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.514066 liveplotlib-0.2/src/liveplotlib.egg-info/
+-rw-rw-rw-   0        0        0     6118 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/top_level.txt
```

### Comparing `liveplotlib-0.1/LICENSE` & `liveplotlib-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/PKG-INFO` & `liveplotlib-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.1
+Version: 0.2
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt6
+Requires-Dist: matplotlib
 
 # LIVE PLOT LIBrary (liveplotlib)
 - Library for plotting (visualizing) cost function changes during model training (in real time)
 
 
 # Notations
 ### Specific
```

### Comparing `liveplotlib-0.1/README.md` & `liveplotlib-0.2/README.md`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/setup.cfg` & `liveplotlib-0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6976 6570 6c6f 746c 6962 0d0a   = liveplotlib..
-00000020: 7665 7273 696f 6e20 3d20 302e 310d 0a61  version = 0.1..a
+00000020: 7665 7273 696f 6e20 3d20 302e 320d 0a61  version = 0.2..a
 00000030: 7574 686f 7220 3d20 706f 7a68 6172 736b  uthor = pozharsk
 00000040: 7945 0d0a 6175 7468 6f72 5f65 6d61 696c  yE..author_email
 00000050: 203d 2065 7667 656e 792e 706f 7a68 6172   = evgeny.pozhar
 00000060: 736b 7940 676d 6169 6c2e 636f 6d0d 0a64  sky@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 204c 6962  escription = Lib
 00000080: 7261 7279 2066 6f72 2070 6c6f 7474 696e  rary for plottin
 00000090: 6720 2876 6973 7561 6c69 7a69 6e67 2920  g (visualizing) 
@@ -33,13 +33,16 @@
 00000200: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 00000210: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
 00000220: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
 00000230: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
 00000240: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
 00000250: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
 00000260: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000270: 203e 3d33 2e37 0d0a 0d0a 5b6f 7074 696f   >=3.7....[optio
-00000280: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000290: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-000002a0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002b0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002c0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000270: 203e 3d33 2e37 0d0a 696e 7374 616c 6c5f   >=3.7..install_
+00000280: 7265 7175 6972 6573 203d 200d 0a09 5079  requires = ...Py
+00000290: 5174 360d 0a09 6d61 7470 6c6f 746c 6962  Qt6...matplotlib
+000002a0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000002b0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+000002c0: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
+000002d0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000002e0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000002f0: 2030 0d0a 0d0a                            0....
```

### Comparing `liveplotlib-0.1/src/liveplotlib/get_file_format.py` & `liveplotlib-0.2/src/liveplotlib/get_file_format.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/src/liveplotlib/if_ipynb.py` & `liveplotlib-0.2/src/liveplotlib/if_ipynb.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/src/liveplotlib/live_plot_only_train.py` & `liveplotlib-0.2/src/liveplotlib/live_plot_only_train.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/src/liveplotlib/live_plot_train_and_val.py` & `liveplotlib-0.2/src/liveplotlib/live_plot_train_and_val.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.1/src/liveplotlib.egg-info/PKG-INFO` & `liveplotlib-0.2/src/liveplotlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.1
+Version: 0.2
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyQt6
+Requires-Dist: matplotlib
 
 # LIVE PLOT LIBrary (liveplotlib)
 - Library for plotting (visualizing) cost function changes during model training (in real time)
 
 
 # Notations
 ### Specific
```

