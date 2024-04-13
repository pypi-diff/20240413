# Comparing `tmp/liveplotlib-0.2.tar.gz` & `tmp/liveplotlib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveplotlib-0.2.tar", last modified: Sat Apr 13 00:29:58 2024, max compression
+gzip compressed data, was "liveplotlib-0.3.tar", last modified: Sat Apr 13 01:19:37 2024, max compression
```

## Comparing `liveplotlib-0.2.tar` & `liveplotlib-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.515065 liveplotlib-0.2/
--rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.2/LICENSE
--rw-rw-rw-   0        0        0     6118 2024-04-13 00:29:58.515065 liveplotlib-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5490 2024-04-12 22:29:00.000000 liveplotlib-0.2/README.md
--rw-rw-rw-   0        0        0      108 2024-04-13 00:24:49.000000 liveplotlib-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      758 2024-04-13 00:29:58.517066 liveplotlib-0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.491026 liveplotlib-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.500229 liveplotlib-0.2/src/liveplotlib/
--rw-rw-rw-   0        0        0      280 2024-04-12 21:59:30.000000 liveplotlib-0.2/src/liveplotlib/__init__.py
--rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.2/src/liveplotlib/get_file_format.py
--rw-rw-rw-   0        0        0     1226 2024-04-12 21:49:28.000000 liveplotlib-0.2/src/liveplotlib/if_ipynb.py
--rw-rw-rw-   0        0        0     2863 2024-04-12 23:21:47.000000 liveplotlib-0.2/src/liveplotlib/live_plot_only_train.py
--rw-rw-rw-   0        0        0     4732 2024-04-12 23:25:03.000000 liveplotlib-0.2/src/liveplotlib/live_plot_train_and_val.py
-drwxrwxrwx   0        0        0        0 2024-04-13 00:29:58.514066 liveplotlib-0.2/src/liveplotlib.egg-info/
--rw-rw-rw-   0        0        0     6118 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 00:29:58.000000 liveplotlib-0.2/src/liveplotlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 01:19:37.975247 liveplotlib-0.3/
+-rw-rw-rw-   0        0        0     1073 2024-04-09 17:06:29.000000 liveplotlib-0.3/LICENSE
+-rw-rw-rw-   0        0        0     6072 2024-04-13 01:19:37.975247 liveplotlib-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5444 2024-04-13 01:05:28.000000 liveplotlib-0.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-13 00:24:49.000000 liveplotlib-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      758 2024-04-13 01:19:37.976247 liveplotlib-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 01:19:37.943246 liveplotlib-0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 01:19:37.956247 liveplotlib-0.3/src/liveplotlib/
+-rw-rw-rw-   0        0        0      351 2024-04-13 01:15:51.000000 liveplotlib-0.3/src/liveplotlib/__init__.py
+-rw-rw-rw-   0        0        0      789 2024-04-12 21:53:13.000000 liveplotlib-0.3/src/liveplotlib/get_file_format.py
+-rw-rw-rw-   0        0        0     1226 2024-04-12 21:49:28.000000 liveplotlib-0.3/src/liveplotlib/if_ipynb.py
+-rw-rw-rw-   0        0        0     2863 2024-04-12 23:21:47.000000 liveplotlib-0.3/src/liveplotlib/live_plot_only_train.py
+-rw-rw-rw-   0        0        0     4732 2024-04-12 23:25:03.000000 liveplotlib-0.3/src/liveplotlib/live_plot_train_and_val.py
+drwxrwxrwx   0        0        0        0 2024-04-13 01:19:37.974249 liveplotlib-0.3/src/liveplotlib.egg-info/
+-rw-rw-rw-   0        0        0     6072 2024-04-13 01:19:37.000000 liveplotlib-0.3/src/liveplotlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-04-13 01:19:37.000000 liveplotlib-0.3/src/liveplotlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 01:19:37.000000 liveplotlib-0.3/src/liveplotlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-13 01:19:37.000000 liveplotlib-0.3/src/liveplotlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 01:19:37.000000 liveplotlib-0.3/src/liveplotlib.egg-info/top_level.txt
```

### Comparing `liveplotlib-0.2/LICENSE` & `liveplotlib-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.2/PKG-INFO` & `liveplotlib-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.2
+Version: 0.3
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,32 +45,33 @@
 - `test` - test subset, used for testing how your model performs on new data
 
 - `epoch` - 1 iteration through the whole dataset (or subset). <br>
 
 
 # Installation
 ```shell
-# install its only dependency - matplotlib (+ matplotlib's own dependencies, of corse (don't worry, they will be installed automatically))
->> pip install matplotlib
-
 >> pip install liveplotlib
+# all dependencies will be installed automatically
 ```
 
 # Usage
 - Only 5 steps!
 - "foo" in names means "this is just for example, it means nothing"
 
 - Basic functionality:
     ```python
     from liveplotlib import LivePlotOnlyTrain
 
+    J_train_history = []
+
     # begin session
     live_plot = LivePlotOnlyTrain()
 
     # update during training
+    # J_train_history.append(new_J_train)
     live_plot.update(J_train_history)
 
     # end session
     live_plot.close()
 
     # (See explanations below)
     ```
```

### Comparing `liveplotlib-0.2/README.md` & `liveplotlib-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,33 @@
 - `test` - test subset, used for testing how your model performs on new data
 
 - `epoch` - 1 iteration through the whole dataset (or subset). <br>
 
 
 # Installation
 ```shell
-# install its only dependency - matplotlib (+ matplotlib's own dependencies, of corse (don't worry, they will be installed automatically))
->> pip install matplotlib
-
 >> pip install liveplotlib
+# all dependencies will be installed automatically
 ```
 
 # Usage
 - Only 5 steps!
 - "foo" in names means "this is just for example, it means nothing"
 
 - Basic functionality:
     ```python
     from liveplotlib import LivePlotOnlyTrain
 
+    J_train_history = []
+
     # begin session
     live_plot = LivePlotOnlyTrain()
 
     # update during training
+    # J_train_history.append(new_J_train)
     live_plot.update(J_train_history)
 
     # end session
     live_plot.close()
 
     # (See explanations below)
     ```
```

### Comparing `liveplotlib-0.2/setup.cfg` & `liveplotlib-0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6976 6570 6c6f 746c 6962 0d0a   = liveplotlib..
-00000020: 7665 7273 696f 6e20 3d20 302e 320d 0a61  version = 0.2..a
+00000020: 7665 7273 696f 6e20 3d20 302e 330d 0a61  version = 0.3..a
 00000030: 7574 686f 7220 3d20 706f 7a68 6172 736b  uthor = pozharsk
 00000040: 7945 0d0a 6175 7468 6f72 5f65 6d61 696c  yE..author_email
 00000050: 203d 2065 7667 656e 792e 706f 7a68 6172   = evgeny.pozhar
 00000060: 736b 7940 676d 6169 6c2e 636f 6d0d 0a64  sky@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 204c 6962  escription = Lib
 00000080: 7261 7279 2066 6f72 2070 6c6f 7474 696e  rary for plottin
 00000090: 6720 2876 6973 7561 6c69 7a69 6e67 2920  g (visualizing)
```

### Comparing `liveplotlib-0.2/src/liveplotlib/get_file_format.py` & `liveplotlib-0.3/src/liveplotlib/get_file_format.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.2/src/liveplotlib/if_ipynb.py` & `liveplotlib-0.3/src/liveplotlib/if_ipynb.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.2/src/liveplotlib/live_plot_only_train.py` & `liveplotlib-0.3/src/liveplotlib/live_plot_only_train.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.2/src/liveplotlib/live_plot_train_and_val.py` & `liveplotlib-0.3/src/liveplotlib/live_plot_train_and_val.py`

 * *Files identical despite different names*

### Comparing `liveplotlib-0.2/src/liveplotlib.egg-info/PKG-INFO` & `liveplotlib-0.3/src/liveplotlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveplotlib
-Version: 0.2
+Version: 0.3
 Summary: Library for plotting (visualizing) cost function changes during model training (in real time)
 Home-page: https://github.com/pozharskyE/liveplotlib
 Author: pozharskyE
 Author-email: evgeny.pozharsky@gmail.com
 Project-URL: Docs, https://github.com/pozharskyE/liveplotlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,32 +45,33 @@
 - `test` - test subset, used for testing how your model performs on new data
 
 - `epoch` - 1 iteration through the whole dataset (or subset). <br>
 
 
 # Installation
 ```shell
-# install its only dependency - matplotlib (+ matplotlib's own dependencies, of corse (don't worry, they will be installed automatically))
->> pip install matplotlib
-
 >> pip install liveplotlib
+# all dependencies will be installed automatically
 ```
 
 # Usage
 - Only 5 steps!
 - "foo" in names means "this is just for example, it means nothing"
 
 - Basic functionality:
     ```python
     from liveplotlib import LivePlotOnlyTrain
 
+    J_train_history = []
+
     # begin session
     live_plot = LivePlotOnlyTrain()
 
     # update during training
+    # J_train_history.append(new_J_train)
     live_plot.update(J_train_history)
 
     # end session
     live_plot.close()
 
     # (See explanations below)
     ```
```

