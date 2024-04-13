# Comparing `tmp/descarteslabs_dynamic_compute-1.1.0.tar.gz` & `tmp/descarteslabs_dynamic_compute-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs_dynamic_compute-1.1.0.tar", max compression
+gzip compressed data, was "descarteslabs_dynamic_compute-1.1.2.tar", max compression
```

## Comparing `descarteslabs_dynamic_compute-1.1.0.tar` & `descarteslabs_dynamic_compute-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      561 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/LICENSE
--rw-r--r--   0        0        0     1786 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/README.md
--rw-r--r--   0        0        0      820 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/__init__.py
--rw-r--r--   0        0        0      308 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/catalog/__init__.py
--rw-r--r--   0        0        0     9728 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/catalog/blob.py
--rw-r--r--   0        0        0    21050 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/compute_map.py
--rw-r--r--   0        0        0     1467 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/datetime_utils.py
--rw-r--r--   0        0        0      648 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dl_utils.py
--rw-r--r--   0        0        0     3890 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dot.py
--rw-r--r--   0        0        0     1007 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dynamic_compute.py
--rw-r--r--   0        0        0        0 2024-03-20 17:39:51.440986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/__init__.py
--rw-r--r--   0        0        0      541 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/client/__init__.py
--rw-r--r--   0        0        0    27598 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/client/client.py
--rw-r--r--   0        0        0      160 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
--rw-r--r--   0        0        0      223 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
--rw-r--r--   0        0        0     5705 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
--rw-r--r--   0        0        0      848 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
--rw-r--r--   0        0        0     5217 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/spec.md
--rw-r--r--   0        0        0      465 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/syntax/__init__.py
--rw-r--r--   0        0        0     3620 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/syntax/syntax.py
--rw-r--r--   0        0        0    11234 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/groupby.py
--rw-r--r--   0        0        0    19407 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/image_stack.py
--rw-r--r--   0        0        0       41 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/__init__.py
--rw-r--r--   0        0        0     1573 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/clearable.py
--rw-r--r--   0        0        0     1179 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/colormaps.py
--rw-r--r--   0        0        0    13247 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/inspector.py
--rw-r--r--   0        0        0    22779 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer.py
--rw-r--r--   0        0        0     3752 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer_controller.py
--rw-r--r--   0        0        0    17054 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
--rw-r--r--   0        0        0     1333 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/lonlat.py
--rw-r--r--   0        0        0    18499 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/map_.py
--rw-r--r--   0        0        0    23843 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/parameters.py
--rw-r--r--   0        0        0     3572 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/tile_url.py
--rw-r--r--   0        0        0     1543 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/utils.py
--rw-r--r--   0        0        0    16050 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/mosaic.py
--rw-r--r--   0        0        0    38941 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/operations.py
--rw-r--r--   0        0        0     3133 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/pyversions.py
--rw-r--r--   0        0        0     1453 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/reductions.py
--rw-r--r--   0        0        0      801 2024-03-20 17:39:51.444986 descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/serialization.py
--rw-r--r--   0        0        0      537 2024-03-20 17:39:51.448986 descarteslabs_dynamic_compute-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2620 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      561 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1786 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/README.md
+-rw-r--r--   0        0        0      945 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/__init__.py
+-rw-r--r--   0        0        0     9728 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/blob.py
+-rw-r--r--   0        0        0    21555 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/compute_map.py
+-rw-r--r--   0        0        0     1467 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/datetime_utils.py
+-rw-r--r--   0        0        0      648 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dl_utils.py
+-rw-r--r--   0        0        0     3890 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dot.py
+-rw-r--r--   0        0        0     1007 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dynamic_compute.py
+-rw-r--r--   0        0        0        0 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/__init__.py
+-rw-r--r--   0        0        0      541 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/__init__.py
+-rw-r--r--   0        0        0    27769 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/client.py
+-rw-r--r--   0        0        0      160 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/exceptions.py
+-rw-r--r--   0        0        0     5705 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py
+-rw-r--r--   0        0        0      848 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py
+-rw-r--r--   0        0        0     5217 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/spec.md
+-rw-r--r--   0        0        0      465 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/__init__.py
+-rw-r--r--   0        0        0     3620 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py
+-rw-r--r--   0        0        0    11234 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/groupby.py
+-rw-r--r--   0        0        0    19407 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/image_stack.py
+-rw-r--r--   0        0        0       41 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/__init__.py
+-rw-r--r--   0        0        0     1573 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/clearable.py
+-rw-r--r--   0        0        0     1179 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/colormaps.py
+-rw-r--r--   0        0        0    13247 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/inspector.py
+-rw-r--r--   0        0        0    22779 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer.py
+-rw-r--r--   0        0        0     3752 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller.py
+-rw-r--r--   0        0        0    17054 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py
+-rw-r--r--   0        0        0     1333 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/lonlat.py
+-rw-r--r--   0        0        0    18499 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/map_.py
+-rw-r--r--   0        0        0    23843 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/parameters.py
+-rw-r--r--   0        0        0     3572 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/tile_url.py
+-rw-r--r--   0        0        0     1543 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/utils.py
+-rw-r--r--   0        0        0    17999 2024-04-13 00:40:32.897564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/mosaic.py
+-rw-r--r--   0        0        0    39359 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/operations.py
+-rw-r--r--   0        0        0     3133 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/pyversions.py
+-rw-r--r--   0        0        0     1453 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/reductions.py
+-rw-r--r--   0        0        0      801 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/serialization.py
+-rw-r--r--   0        0        0      625 2024-04-13 00:40:32.901564 descarteslabs_dynamic_compute-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 descarteslabs_dynamic_compute-1.1.2/PKG-INFO
```

### Comparing `descarteslabs_dynamic_compute-1.1.0/LICENSE` & `descarteslabs_dynamic_compute-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/README.md` & `descarteslabs_dynamic_compute-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/catalog/blob.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/catalog/blob.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/compute_map.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/compute_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 
 import descarteslabs as dl
 import numpy as np
 
 from .graft.client import client as graft_client
 from .graft.interpreter.interpreter import interpret
 from .graft.syntax import syntax as graft_syntax
-from .operations import _func_op, _math_op, _resolution_graft, compute_aoi
+from .operations import (
+    _func_op,
+    _math_op,
+    _resolution_graft_x,
+    _resolution_graft_y,
+    compute_aoi,
+)
 
 
 class DotDict(dict):
     """
     dot-notation access to top-level dictionary attributes
 
     From https://stackoverflow.com/a/23689767
@@ -98,15 +104,19 @@
     return None
 
 
 def clip_data(*args, **kwargs):
     return None
 
 
-def graft_resolution(*args, **kwargs):
+def graft_resolution_x(*args, **kwargs):
+    return None
+
+
+def graft_resolution_y(*args, **kwargs):
     return None
 
 
 def band_op(*args, **kwargs):
     return None
 
 
@@ -192,15 +202,16 @@
                     ("array", array),
                     ("groupby", groupby),
                     ("filter_data", filter_data),
                     ("groupby_data", groupby_data),
                     ("math", math_op),
                     ("reduction", reduction_op),
                     ("clip", clip_data),
-                    ("resolution", graft_resolution),
+                    ("resolution_y", graft_resolution_y),
+                    ("resolution_x", graft_resolution_x),
                     ("band_op", band_op),
                     ("index", index),
                     ("length", length),
                     ("mask", mask),
                     ("functional", functional),
                     ("dot", dot),
                 ],
@@ -335,24 +346,36 @@
         # `a` is a Dict, but not a ComputeMap. If `a` it isn't a graft,
         # the ComputeMap constructor will throw the necessary exception.
         return ComputeMap(a)
 
     return a
 
 
-def resolution():
+def resolution_x():
+    """
+    Generate ComputeMap representation of resolution_x.
+
+    Returns
+    -------
+    Resolution: ComputeMap
+        A dynamic-compute object representation of resolution east-west
+    """
+    return as_compute_map(_resolution_graft_x())
+
+
+def resolution_y():
     """
-    Generate ComputeMap representation of resolution.
+    Generate ComputeMap representation of resolution_y.
 
     Returns
     -------
     Resolution: ComputeMap
-        A dynamic-compute object representation of resolution.
+        A dynamic-compute object representation of resolution n-s.
     """
-    return as_compute_map(_resolution_graft())
+    return as_compute_map(_resolution_graft_y())
 
 
 def type_max(
     t1: Union[np.ndarray, ComputeMap], t2: Union[np.ndarray, ComputeMap]
 ) -> Union[np.ndarray, ComputeMap]:
     """
     Return the more general of two types. If either t1 or t2 is a number or array
@@ -710,14 +733,17 @@
 
     return op
 
 
 #
 # functional operations
 #
+def arctan2(x, y):
+    return _math_op(x, "arctan2", y)
+
 
 sqrt = _functional_op("sqrt")
 
 cos = _functional_op("cos")
 sin = _functional_op("sin")
 tan = _functional_op("tan")
```

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/datetime_utils.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dl_utils.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dl_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dot.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dot.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/dynamic_compute.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/dynamic_compute.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/client/__init__.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/client/client.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 import base64
 import contextlib
 import copy
 import itertools
 import json
 from io import BytesIO
-from typing import Dict, Hashable, List
+from typing import Any, Dict, List
 
 import numpy as np
 import six
 
 from .. import syntax
 
 NO_INITIAL = "_no_initial_"
@@ -258,15 +258,15 @@
     for key in replacements:
         _ = new_graft.pop(key)
 
     # We've modified the graft, perform another pass to see if more compression is possible.
     return compress_graft(new_graft)
 
 
-def splice(graft1: dict, splice_value: Hashable, graft2: dict) -> dict:
+def splice(graft1: dict, splice_value: Any, graft2: dict) -> dict:
     """
     Splice two grafts together by replacing a particular value in graft1 with
     the returned content of graft2.
 
     For example
     >>> splice(
     >>>     {
@@ -336,17 +336,22 @@
                 if isinstance(object, dict):
                     object_as_dict = object
                     for subkey in object_as_dict:
                         object_as_dict[subkey] = key_remap.get(
                             object_as_dict[subkey], object_as_dict[subkey]
                         )
 
+        if key == "returns":
+            spliced_graft["returns"] = key_remap.get(
+                spliced_graft["returns"], spliced_graft["returns"]
+            )
+
     spliced_graft.update(graft2)
 
-    return spliced_graft
+    return compress_graft(spliced_graft)
 
 
 def op_args(op_list: List) -> List:
     """
     Given a list that encodes an operation and its arguments return the arguments
 
     Parameters
```

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/interpreter/scopedchainmap.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/spec.md` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/spec.md`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/graft/syntax/syntax.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/graft/syntax/syntax.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/groupby.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/groupby.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/image_stack.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/image_stack.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/clearable.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/clearable.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/colormaps.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/colormaps.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/inspector.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/inspector.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer_controller.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/layer_controller_row.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/layer_controller_row.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/lonlat.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/lonlat.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/map_.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/map_.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/parameters.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/parameters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/tile_url.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/tile_url.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/interactive/utils.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/mosaic.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/mosaic.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,32 @@
     FloorDivMixin,
     LogicalMixin,
     MulMixin,
     NumpyReductionMixin,
     SignedMixin,
     SubMixin,
     TrueDivMixin,
+    arctan,
+    arctan2,
+    pi,
+    sqrt,
 )
 from .datetime_utils import normalize_datetime_or_none
 from .dl_utils import get_product_or_fail
 from .interactive.tile_url import validate_scales
 from .operations import (
     _band_op,
     _clip_data,
     _mask_op,
+    _resolution_graft_x,
+    _resolution_graft_y,
     create_mosaic,
     format_bands,
+    gradient_x,
+    gradient_y,
     is_op,
     op_args,
     op_type,
     reset_graft,
     set_cache_id,
 )
 from .reductions import reduction
@@ -463,14 +471,83 @@
             graft=dict(self),
             product_id=self.product_id,
             bands=self.bands,
             start_datetime=self.start_datetime,
             end_datetime=self.end_datetime,
         ).json()
 
+    def gradient_x(self, resolution: Optional[float] = None) -> Mosaic:
+        """
+        Compute the gradient in the x (E-W) direction
+
+        Returns
+        -------
+        Mosaic
+            Mosaic object with the E-W gradient
+        """
+
+        if resolution is None:
+            resolution = ComputeMap(_resolution_graft_x())
+
+        return Mosaic(gradient_x(dict(self))) / resolution
+
+    def gradient_y(self, resolution: Optional[float] = None) -> Mosaic:
+        """
+        Compute the gradient in the y (N-S) direction
+
+        Returns
+        -------
+        Mosaic
+            Mosaic object with the N-S gradient
+        """
+        if resolution is None:
+            resolution = ComputeMap(_resolution_graft_y())
+
+        return Mosaic(gradient_y(dict(self))) / resolution
+
+    def slope(
+        self, resolution_x: Optional[float] = None, resolution_y: Optional[float] = None
+    ) -> Mosaic:
+        """
+        Compute the slope of the mosaic
+
+        Returns
+        -------
+        Mosaic
+            Mosaic object with the slope
+        """
+
+        grad_y = self.gradient_y(resolution=resolution_y)
+        grad_x = self.gradient_x(resolution=resolution_x)
+        slope = sqrt(grad_x**2 + grad_y**2)
+
+        # convert to degrees from horizontal
+        slope = arctan(slope) * (180 / pi)
+
+        return slope
+
+    def aspect(
+        self, resolution_x: Optional[float] = None, resolution_y: Optional[float] = None
+    ) -> Mosaic:
+        """
+        Compute the aspect of the mosaic
+
+        Returns
+        -------
+        Mosaic
+            Mosaic object with the aspect
+        """
+
+        grad_y = self.gradient_y(resolution=resolution_y)
+        grad_x = self.gradient_x(resolution=resolution_x)
+
+        aspect = Mosaic(arctan2(grad_x, -grad_y)) * (180 / pi)
+
+        return aspect
+
     @classmethod
     def deserialize(cls, data: str) -> Mosaic:
         """Deserializes into this object from json
 
         Parameters
         ----------
         data : str
```

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/operations.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,22 +377,32 @@
         if isinstance(i, list):
             if i[0] in ["select_scenes", "mosaic"]:
                 pad_key = i[-1]["pad"]
 
     return graft[pad_key]
 
 
-def _resolution_graft() -> dict:
+def _resolution_graft_x() -> dict:
     """
     Returns
     -------
-    resolution_graft: dict
-        Graft that evaluates to resolution.
+    resolution_graft_x: dict
+        Graft that evaluates to resolution_x.
     """
-    return graft_client.apply_graft("resolution")
+    return graft_client.apply_graft("resolution_x")
+
+
+def _resolution_graft_y() -> dict:
+    """
+    Returns
+    -------
+    resolution_graft_y: dict
+        Graft that evaluates to resolution_y.
+    """
+    return graft_client.apply_graft("resolution_y")
 
 
 def _math_op(main_obj, operation, other_obj=None, **kwargs):
     """Apply a math operation between a graft and optionally another graft
 
     Params
     main_obj : graft
@@ -643,14 +653,24 @@
     filtered_graft: Dict
         Graft, which when evaluated results in an ImageCollection object containing images
         for which the filter function evaluates to true.
     """
     return graft_client.apply_graft("filter_data", stack_graft, encoded_filter_func)
 
 
+def gradient_x(graft: Dict):
+
+    return graft_client.apply_graft("math", "gradient_x", graft, None)
+
+
+def gradient_y(graft: Dict):
+
+    return graft_client.apply_graft("math", "gradient_y", graft, None)
+
+
 def groupby(scenes_graft: Dict, encoded_key_func: str):
     return graft_client.apply_graft("groupby_data", scenes_graft, encoded_key_func)
 
 
 def compute_aoi(
     graft: Dict, aoi: dl.geo.AOI, layer_id: str = None
 ) -> np.ma.MaskedArray:
```

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/pyversions.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/pyversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/reductions.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/reductions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/descarteslabs/dynamic_compute/serialization.py` & `descarteslabs_dynamic_compute-1.1.2/descarteslabs/dynamic_compute/serialization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs_dynamic_compute-1.1.0/PKG-INFO` & `descarteslabs_dynamic_compute-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: descarteslabs-dynamic-compute
-Version: 1.1.0
+Version: 1.1.2
 Summary: 
 License: Apache-2.0
 Author: Descartes Labs
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2023.7.22)
-Requires-Dist: cloudpickle (==1.6.0)
+Requires-Dist: cloudpickle (==1.6.0) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: cloudpickle (==3.0.0) ; python_version >= "3.11"
 Requires-Dist: descarteslabs (>=2.0.3,<4)
 Requires-Dist: geojson (>=2.5.0)
 Requires-Dist: ipyleaflet (>=0.15.0)
 Requires-Dist: numpy (<=1.24.2)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0)
 Requires-Dist: shapely (>2,<3)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
```

