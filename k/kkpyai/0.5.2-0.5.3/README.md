# Comparing `tmp/kkpyai-0.5.2.tar.gz` & `tmp/kkpyai-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.5.2.tar", max compression
+gzip compressed data, was "kkpyai-0.5.3.tar", max compression
```

## Comparing `kkpyai-0.5.2.tar` & `kkpyai-0.5.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.5.2/LICENSE
--rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.5.2/README.md
--rw-r--r--   0        0        0     9738 2024-04-11 22:08:07.632143 kkpyai-0.5.2/kkpyai/kktorch.py
--rw-r--r--   0        0        0      439 2024-04-11 22:10:51.586778 kkpyai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 kkpyai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.5.3/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.5.3/README.md
+-rw-r--r--   0        0        0     9296 2024-04-13 01:07:44.652328 kkpyai-0.5.3/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      439 2024-04-13 01:08:34.782037 kkpyai-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 kkpyai-0.5.3/PKG-INFO
```

### Comparing `kkpyai-0.5.2/LICENSE` & `kkpyai-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.5.2/kkpyai/kktorch.py` & `kkpyai-0.5.3/kkpyai/kktorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os.path as osp
 import typing
 # 3rd party
 import kkpyutil as util
 import torch as tc
 import matplotlib.pyplot as plt
 import numpy as np
+from sklearn.model_selection import train_test_split
 
 
 # region globals
 
 def find_fast_device():
     """
     - Apple Silicon uses Apple's own Metal Performance Shaders (MPS) instead of CUDA
@@ -65,32 +66,22 @@
 
 
 # endregion
 
 
 # region dataset
 
-def split_dataset(data, labels, train_ratio=0.8, validation_ratio=0):
+def split_dataset(data, labels, train_ratio=0.8, random_seed=42,):
     """
     - split dataset into training and testing sets
     """
-    split_train = int(train_ratio * len(data))
-    split_val = int(validation_ratio * len(data))
-    X_train, y_train = data[:split_train], labels[:split_train]
-    X_test, y_test = data[split_train:], labels[split_train:]
-    if validation_ratio:
-        X_val, y_val = X_test[:split_val], y_test[:split_val]
-        X_test, y_test = X_test[split_val:], y_test[split_val:]
-        train_set = {'data': X_train, 'labels': y_train}
-        test_set = {'data': X_test, 'labels': y_test}
-        validation_set = {'data': X_val, 'labels': y_val}
-        return train_set, test_set, validation_set
+    X_train, X_test, y_train, y_test = train_test_split(data, labels, train_size=train_ratio, random_state=random_seed)
     train_set = {'data': X_train, 'labels': y_train}
     test_set = {'data': X_test, 'labels': y_test}
-    return train_set, test_set, validation_ratio
+    return train_set, test_set
 
 # endregion
 
 # region model
 
 
 class Model(Loggable):
```

