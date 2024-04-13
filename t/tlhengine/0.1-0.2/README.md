# Comparing `tmp/tlhengine-0.1-py2.py3-none-any.whl.zip` & `tmp/tlhengine-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,33 @@
-Zip file size: 28454 bytes, number of entries: 18
--rw-r--r--  2.0 unx       41 b- defN 23-Oct-12 08:41 tlhengine/__init__.py
+Zip file size: 66109 bytes, number of entries: 31
+-rw-r--r--  2.0 unx      465 b- defN 23-Dec-25 09:19 tlhengine/__init__.py
 -rw-r--r--  2.0 unx     5377 b- defN 23-Dec-22 02:14 tlhengine/dataset.py
--rw-r--r--  2.0 unx     8734 b- defN 23-Dec-22 02:14 tlhengine/engine.py
+-rw-r--r--  2.0 unx     8735 b- defN 23-Dec-25 16:20 tlhengine/engine.py
 -rw-r--r--  2.0 unx    12254 b- defN 23-Oct-12 08:41 tlhengine/loss.py
 -rw-r--r--  2.0 unx    10203 b- defN 23-Dec-22 02:14 tlhengine/models.py
+-rw-r--r--  2.0 unx    10203 b- defN 23-Dec-22 02:14 tlhengine/models1.py
 -rw-r--r--  2.0 unx    13498 b- defN 23-Oct-12 08:41 tlhengine/resnetv1_b.py
 -rw-r--r--  2.0 unx     7105 b- defN 23-Oct-12 08:41 tlhengine/scores.py
 -rw-r--r--  2.0 unx     2076 b- defN 23-Oct-12 08:41 tlhengine/segbase.py
 -rw-r--r--  2.0 unx     3180 b- defN 23-Oct-12 08:41 tlhengine/tfmodels.py
--rw-r--r--  2.0 unx    18882 b- defN 23-Dec-22 02:14 tlhengine/utils.py
+-rw-r--r--  2.0 unx    24373 b- defN 24-Apr-13 07:53 tlhengine/utils.py
 -rw-r--r--  2.0 unx     5536 b- defN 23-Oct-12 08:41 tlhengine/zhihu_deeplab.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-12 08:41 tlhengine/datasets/__init__.py
 -rw-r--r--  2.0 unx     3570 b- defN 23-Oct-12 08:41 tlhengine/datasets/segbase.py
 -rw-r--r--  2.0 unx    13010 b- defN 23-Oct-12 08:41 tlhengine/datasets/voc.py
--rw-r--r--  2.0 unx      585 b- defN 23-Dec-22 02:15 tlhengine-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Dec-22 02:15 tlhengine-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Dec-22 02:15 tlhengine-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1403 b- defN 23-Dec-22 02:15 tlhengine-0.1.dist-info/RECORD
-18 files, 105574 bytes uncompressed, 26194 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx     7415 b- defN 23-Dec-25 16:20 tlhengine/models/__init__.py
+-rw-r--r--  2.0 unx    25343 b- defN 23-Dec-25 16:20 tlhengine/models/beit.py
+-rw-r--r--  2.0 unx    14406 b- defN 23-Dec-25 16:20 tlhengine/models/deploy.py
+-rw-r--r--  2.0 unx     1713 b- defN 23-Dec-25 16:20 tlhengine/models/protonet.py
+-rw-r--r--  2.0 unx     6351 b- defN 23-Dec-25 16:20 tlhengine/models/resnet_v2.py
+-rw-r--r--  2.0 unx     8327 b- defN 23-Dec-25 16:20 tlhengine/models/utils.py
+-rw-r--r--  2.0 unx     9292 b- defN 23-Dec-25 16:20 tlhengine/models/vision_transformer.py
+-rw-r--r--  2.0 unx    15509 b- defN 23-Dec-25 16:20 tlhengine/models/vit_google.py
+-rw-r--r--  2.0 unx       20 b- defN 23-Dec-25 16:20 tlhengine/models/clip/__init__.py
+-rw-r--r--  2.0 unx     8589 b- defN 23-Dec-25 16:20 tlhengine/models/clip/clip.py
+-rw-r--r--  2.0 unx    23365 b- defN 23-Dec-25 16:20 tlhengine/models/clip/model.py
+-rw-r--r--  2.0 unx     4632 b- defN 23-Dec-25 16:20 tlhengine/models/clip/simple_tokenizer.py
+-rw-r--r--  2.0 unx      585 b- defN 24-Apr-13 08:06 tlhengine-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 08:06 tlhengine-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-13 08:06 tlhengine-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2528 b- defN 24-Apr-13 08:06 tlhengine-0.2.dist-info/RECORD
+31 files, 247762 bytes uncompressed, 62099 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: tlhengine/loss.py
 Comment: 
 
 Filename: tlhengine/models.py
 Comment: 
 
+Filename: tlhengine/models1.py
+Comment: 
+
 Filename: tlhengine/resnetv1_b.py
 Comment: 
 
 Filename: tlhengine/scores.py
 Comment: 
 
 Filename: tlhengine/segbase.py
@@ -36,20 +39,56 @@
 
 Filename: tlhengine/datasets/segbase.py
 Comment: 
 
 Filename: tlhengine/datasets/voc.py
 Comment: 
 
-Filename: tlhengine-0.1.dist-info/METADATA
+Filename: tlhengine/models/__init__.py
+Comment: 
+
+Filename: tlhengine/models/beit.py
+Comment: 
+
+Filename: tlhengine/models/deploy.py
+Comment: 
+
+Filename: tlhengine/models/protonet.py
+Comment: 
+
+Filename: tlhengine/models/resnet_v2.py
+Comment: 
+
+Filename: tlhengine/models/utils.py
+Comment: 
+
+Filename: tlhengine/models/vision_transformer.py
+Comment: 
+
+Filename: tlhengine/models/vit_google.py
+Comment: 
+
+Filename: tlhengine/models/clip/__init__.py
+Comment: 
+
+Filename: tlhengine/models/clip/clip.py
+Comment: 
+
+Filename: tlhengine/models/clip/model.py
+Comment: 
+
+Filename: tlhengine/models/clip/simple_tokenizer.py
+Comment: 
+
+Filename: tlhengine-0.2.dist-info/METADATA
 Comment: 
 
-Filename: tlhengine-0.1.dist-info/WHEEL
+Filename: tlhengine-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: tlhengine-0.1.dist-info/top_level.txt
+Filename: tlhengine-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tlhengine-0.1.dist-info/RECORD
+Filename: tlhengine-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tlhengine/__init__.py

```diff
@@ -1,2 +1,17 @@
 from . import dataset
-from . import utils
+from . import utils
+import logging
+
+_logger = logging.getLogger(__name__)
+_logger.setLevel(logging.INFO)
+
+_console = logging.StreamHandler()
+_console.setLevel(logging.INFO)
+
+formatter = logging.Formatter("%(filename)s says %(levelname)s: %(message)s")
+_console.setFormatter(formatter)
+_logger.addHandler(_console)
+
+_logger.info("Initializing engine")
+for handler in _logger.handlers:
+    print(handler.__class__.__name__, ': from ', __file__ )
```

## tlhengine/engine.py

```diff
@@ -17,15 +17,15 @@
 
 from tqdm import tqdm
 import time
 import datetime
 
 from PIL import Image
 from tlhengine.scores import SegmentationMetric, MeanMetric, Acc
-from tlhengine.models import SegBaseModel
+from tlhengine.models1 import SegBaseModel
 from torch.nn.parallel import DistributedDataParallel as DDP
 
 
 class Trainer:
     def __init__(
         self,
         model,
```

## tlhengine/utils.py

```diff
@@ -1,20 +1,233 @@
+import math
 import time
         
 import copy
 import datetime
 import errno
 import hashlib
 import os
 from collections import defaultdict, deque, OrderedDict
 from typing import List, Optional, Tuple
+import warnings
 
 import torch
 import torch.distributed as dist
-from torch import nn
+from torch import default_generator, nn
+from torch.utils.data import Subset
+from torch import optim
+from torch._utils import _accumulate
+from torch.optim.lr_scheduler import _LRScheduler
+import numpy as np
+import pickle
+import logging
+
+logger = logging.getLogger(__name__)
+
+def set_debug_mode():
+    # make torch show shape by changing its __repr__ method
+    normal_repr = torch.Tensor.__repr__
+    torch.Tensor.__repr__ = lambda self: f"{self.shape}_{normal_repr(self)}"
+        
+
+class Hparams(dict):
+    def __getattr__(self, attr):
+        return self[attr]
+
+    def __setattr__(self, attr, value):
+        self[attr] = value
+
+def test_logger ():
+    logger.info("hello logger")
+    logger.warn('hello warn')
+    for handler in logger.handlers:
+        print(handler.__class__.__name__, ' from ', handler.__class__.__name__)
+
+
+def get_pickle(load_fun, pkl_file, *args, **kwargs):
+    """
+    This is used for those time consuming data loading operations
+    e.g. in few shot learning, generating the meta dataset is time consuming
+    using this saved a lot of time, helped me for fast development.
+    """
+    if not os.path.exists(pkl_file):
+        with open(pkl_file, 'wb') as f:
+            data = load_fun(*args, **kwargs)
+            pickle.dump(data, f)
+    else:
+        with open(pkl_file, 'rb') as f:
+            data = pickle.load(f)
+    return data
+
+def set_weight_decay(
+    model: torch.nn.Module,
+    weight_decay: float,
+    norm_weight_decay: Optional[float] = None,
+    norm_classes: Optional[List[type]] = None,
+    custom_keys_weight_decay: Optional[List[Tuple[str, float]]] = None,
+):
+    if not norm_classes:
+        norm_classes = [
+            torch.nn.modules.batchnorm._BatchNorm,
+            torch.nn.LayerNorm,
+            torch.nn.GroupNorm,
+            torch.nn.modules.instancenorm._InstanceNorm,
+            torch.nn.LocalResponseNorm,
+        ]
+    norm_classes = tuple(norm_classes)
+
+    params = {
+        "other": [],
+        "norm": [],
+    }
+    params_weight_decay = {
+        "other": weight_decay,
+        "norm": norm_weight_decay,
+    }
+    custom_keys = []
+    if custom_keys_weight_decay is not None:
+        for key, weight_decay in custom_keys_weight_decay:
+            params[key] = []
+            params_weight_decay[key] = weight_decay
+            custom_keys.append(key)
+
+    def _add_params(module, prefix=""):
+        for name, p in module.named_parameters(recurse=False):
+            if not p.requires_grad:
+                continue
+            is_custom_key = False
+            for key in custom_keys:
+                target_name = f"{prefix}.{name}" if prefix != "" and "." in key else name
+                if key == target_name:
+                    params[key].append(p)
+                    is_custom_key = True
+                    break
+            if not is_custom_key:
+                if norm_weight_decay is not None and isinstance(module, norm_classes):
+                    print("adding norm layer set weight decay to 0")
+                    params["norm"].append(p)
+                else:
+                    params["other"].append(p)
+
+        for child_name, child_module in module.named_children():
+            child_prefix = f"{prefix}.{child_name}" if prefix != "" else child_name
+            _add_params(child_module, prefix=child_prefix)
+
+    _add_params(model)
+
+    param_groups = []
+    for key in params:
+        if len(params[key]) > 0:
+            param_groups.append({"params": params[key], "weight_decay": params_weight_decay[key]})
+    return param_groups
+
+class LinearWarmupCosineAnnealingLR(_LRScheduler):
+    def __init__(
+        self, optimizer, warmup_epochs, max_epochs, warmup_start_factor, eta_min=0
+    ):
+        self.warmup_epochs = warmup_epochs
+        self.max_epochs = max_epochs
+        self.warmup_start_lr = warmup_start_factor * \
+                                optimizer.param_groups[0]['lr']
+        self.eta_min = eta_min
+        self.cycle_epochs = max_epochs - warmup_epochs
+        super(LinearWarmupCosineAnnealingLR, self).__init__(optimizer)
+
+    def get_lr(self):
+        if self.last_epoch < self.warmup_epochs:
+            # Linear warmup phase
+            alpha = self.last_epoch / self.warmup_epochs
+            return [
+                self.warmup_start_lr + alpha * (base_lr - self.warmup_start_lr)
+                for base_lr in self.base_lrs
+            ]
+        else:
+            # Cosine annealing phase
+            progress = (self.last_epoch - self.warmup_epochs) / self.cycle_epochs
+            return [
+                self.eta_min
+                + 0.5 * (base_lr - self.eta_min) * (1 + np.cos(np.pi * progress))
+                for base_lr in self.base_lrs
+            ]
+
+class AvgMeter(object):
+    def __init__(self, name=None, fmt=':f'):
+        self.name = name
+        self.fmt = fmt
+        self.reset()
+
+    def reset(self):
+        self.val = 0
+        self.avg = 0
+        self.sum = 0
+        self.count = 0
+
+    def update(self, val, n=1):
+        self.val = val
+        self.sum += val * n
+        self.count += n
+        self.avg = self.sum / self.count
+
+
+def random_split(dataset, lengths, generator=default_generator):
+    r"""
+    Randomly split a dataset into non-overlapping new datasets of given lengths.
+
+    If a list of fractions that sum up to 1 is given,
+    the lengths will be computed automatically as
+    floor(frac * len(dataset)) for each fraction provided.
+
+    After computing the lengths, if there are any remainders, 1 count will be
+    distributed in round-robin fashion to the lengths
+    until there are no remainders left.
+
+    Optionally fix the generator for reproducible results, e.g.:
+
+    >>> random_split(range(10), [3, 7], generator=torch.Generator().manual_seed(42))
+    >>> random_split(range(30), [0.3, 0.3, 0.4], generator=torch.Generator(
+    ...   ).manual_seed(42))
+
+    Args:
+        dataset (Dataset): Dataset to be split
+        lengths (sequence): lengths or fractions of splits to be produced
+        generator (Generator): Generator used for the random permutation.
+    """
+    if math.isclose(sum(lengths), 1) and sum(lengths) <= 1:
+        subset_lengths: List[int] = []
+        for i, frac in enumerate(lengths):
+            if frac < 0 or frac > 1:
+                raise ValueError(f"Fraction at index {i} is not between 0 and 1")
+            n_items_in_split = int(
+                math.floor(len(dataset) * frac)  # type: ignore[arg-type]
+            )
+            subset_lengths.append(n_items_in_split)
+        remainder = len(dataset) - sum(subset_lengths)  # type: ignore[arg-type]
+        # add 1 to all the lengths in round-robin fashion until the remainder is 0
+        for i in range(remainder):
+            idx_to_add_at = i % len(subset_lengths)
+            subset_lengths[idx_to_add_at] += 1
+        lengths = subset_lengths
+        for i, length in enumerate(lengths):
+            if length == 0:
+                warnings.warn(
+                    f"Length of split at index {i} is 0. "
+                    f"This might result in an empty dataset."
+                )
+
+    # Cannot verify that dataset is Sized
+    if sum(lengths) != len(dataset):  # type: ignore[arg-type]
+        raise ValueError(
+            "Sum of input lengths does not equal the length of the input dataset!"
+        )
+
+    indices = randperm(sum(lengths), generator=generator).tolist()  # type: ignore[call-overload]
+    return [
+        Subset(dataset, indices[offset - length : offset])
+        for offset, length in zip(_accumulate(lengths), lengths)
+    ]
 
 
 def copy_parameters(source_dict, target_dict):
     for (source_name, source_param), (target_name, target_param) in zip(source_dict, target_dict):
         if source_param.data.size() == target_param.data.size():
             target_param.data.copy_(source_param.data)
         else:
@@ -476,67 +689,10 @@
 
     t = torch.tensor(val, device="cuda")
     dist.barrier()
     dist.all_reduce(t)
     return t
 
 
-def set_weight_decay(
-    model: torch.nn.Module,
-    weight_decay: float,
-    norm_weight_decay: Optional[float] = None,
-    norm_classes: Optional[List[type]] = None,
-    custom_keys_weight_decay: Optional[List[Tuple[str, float]]] = None,
-):
-    if not norm_classes:
-        norm_classes = [
-            torch.nn.modules.batchnorm._BatchNorm,
-            torch.nn.LayerNorm,
-            torch.nn.GroupNorm,
-            torch.nn.modules.instancenorm._InstanceNorm,
-            torch.nn.LocalResponseNorm,
-        ]
-    norm_classes = tuple(norm_classes)
 
-    params = {
-        "other": [],
-        "norm": [],
-    }
-    params_weight_decay = {
-        "other": weight_decay,
-        "norm": norm_weight_decay,
-    }
-    custom_keys = []
-    if custom_keys_weight_decay is not None:
-        for key, weight_decay in custom_keys_weight_decay:
-            params[key] = []
-            params_weight_decay[key] = weight_decay
-            custom_keys.append(key)
-
-    def _add_params(module, prefix=""):
-        for name, p in module.named_parameters(recurse=False):
-            if not p.requires_grad:
-                continue
-            is_custom_key = False
-            for key in custom_keys:
-                target_name = f"{prefix}.{name}" if prefix != "" and "." in key else name
-                if key == target_name:
-                    params[key].append(p)
-                    is_custom_key = True
-                    break
-            if not is_custom_key:
-                if norm_weight_decay is not None and isinstance(module, norm_classes):
-                    params["norm"].append(p)
-                else:
-                    params["other"].append(p)
-
-        for child_name, child_module in module.named_children():
-            child_prefix = f"{prefix}.{child_name}" if prefix != "" else child_name
-            _add_params(child_module, prefix=child_prefix)
-
-    _add_params(model)
-
-    param_groups = []
-    for key in params:
-        if len(params[key]) > 0:
-            param_groups.append({"params": params[key], "weight_decay": params_weight_decay[key]})
-    return param_groups
+if __name__ == '__main__':
+    print('done')
```

## Comparing `tlhengine-0.1.dist-info/METADATA` & `tlhengine-0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlhengine
-Version: 0.1
+Version: 0.2
 Summary: my package
 Home-page: https://github.com/your-username/your-package-repo
 Author: tian lh
 Author-email: tianlhcs@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `tlhengine-0.1.dist-info/RECORD` & `tlhengine-0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,31 @@
-tlhengine/__init__.py,sha256=0EpzPK5cLl6j_2tzsOdCJGsflnC3kYIDZ6j5wyYzroA,41
+tlhengine/__init__.py,sha256=uY4bPHBnzqdse3DW9B8gGVzR7p97Ycf16C_prAheC-A,465
 tlhengine/dataset.py,sha256=Vt-XtNyqDdaGzrEcauPjbedt2y4n7PhQ_RfGhR10LLE,5377
-tlhengine/engine.py,sha256=kxa8YDfKti5sfY0DW4oT7SoZpJQdnZDq7EG6BcCHYHg,8734
+tlhengine/engine.py,sha256=7Dpgteafi-WS2pl42zLXOuC8gieFJBxXfXBLGTowkKw,8735
 tlhengine/loss.py,sha256=5nBbuYWljPScxZNUdWnA_7A73kEGSLn4tk6oH19_LGU,12254
 tlhengine/models.py,sha256=u9NQZftv3bNo9-OBRox8_91YPDLHogmUvTj7p5k1-i4,10203
+tlhengine/models1.py,sha256=u9NQZftv3bNo9-OBRox8_91YPDLHogmUvTj7p5k1-i4,10203
 tlhengine/resnetv1_b.py,sha256=lsJrrGSboBGQR3ojLJB8_pF9XLYNu10j0uf0Xw0qpcg,13498
 tlhengine/scores.py,sha256=Ez-Hbt-xp0uY0WBe9GY4iEcC9easCsJCRGT1SJDkaU0,7105
 tlhengine/segbase.py,sha256=vr-MIvPqivs5J8W6v5W4-VTNGTZqyZcdwCq1lsaUtp0,2076
 tlhengine/tfmodels.py,sha256=IW9UsXneU1UvFNQ_wt7GRxYVeQrWhfMw3AYCQqNH_aE,3180
-tlhengine/utils.py,sha256=yfQJFN6CskiEwk0Pcht8mWg1_Nh1zkLBWcEZ9SMKxQg,18882
+tlhengine/utils.py,sha256=s1XE767-azhVAa7HKrNpHjByXs9aaN6cMp1SVA0Mprw,24373
 tlhengine/zhihu_deeplab.py,sha256=0FPhs4OpKz6mfn5OTB0D_jgoi2ZAfILvgeIVsrcJdyQ,5536
 tlhengine/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tlhengine/datasets/segbase.py,sha256=jSGJGubgqhuUzPqwRAGoGZLznMmeqJ0xL7hkSt3fXxA,3570
 tlhengine/datasets/voc.py,sha256=FxeOQSfDDdg5D5BL4NpEl_LsrxQKT190qKkTOG4zMkE,13010
-tlhengine-0.1.dist-info/METADATA,sha256=sQjaNaf0PqdC5v2-b3JHX50xz_2KPTAyyZNQ748g4Mg,585
-tlhengine-0.1.dist-info/WHEEL,sha256=P2T-6epvtXQ2cBOE_U1K4_noqlJFN3tj15djMgEu4NM,110
-tlhengine-0.1.dist-info/top_level.txt,sha256=lx8s3cg1-c3YB-TFGmkE1z2WOOYfy9gM83uH8zklVGQ,10
-tlhengine-0.1.dist-info/RECORD,,
+tlhengine/models/__init__.py,sha256=wIeHtO1jX1-Hznb22HUppEjrZyXSyXFSFfKY075-_Q0,7415
+tlhengine/models/beit.py,sha256=_n9jJ5j3PE505juO_6wdlCFJPbtCw8wdkaW4u0hadIY,25343
+tlhengine/models/deploy.py,sha256=iihAW-vnHJpM0ITzV85TdCTx3akS_OHPpFSryy9gox8,14406
+tlhengine/models/protonet.py,sha256=PrZIEuQ9x_4oQTpvYUYKzID0aCAdzVcoWaIZW6pPNow,1713
+tlhengine/models/resnet_v2.py,sha256=gcHu1E47Mgq_htZbze2Tnb0t41Ya3OZ_cf5_7A6j4As,6351
+tlhengine/models/utils.py,sha256=XyHlTtwphitQ1W7snOZKEdKvbWbd3kAUbsRZfJQEgcM,8327
+tlhengine/models/vision_transformer.py,sha256=O1fXfM4ZXkDcF7KVnMOVgj0meK-GY49S6XVgNAhCoDc,9292
+tlhengine/models/vit_google.py,sha256=mEtPWZ9e18TMviC4E0ZaOh25jQIDYhwzkL_ZiWX051s,15509
+tlhengine/models/clip/__init__.py,sha256=15MOspDr7UMhFnlckUcyANCYRRqUwK7dSuD5NPl5Veg,20
+tlhengine/models/clip/clip.py,sha256=qtgW_aRQu1XLy1T23mWQb5Ei0rIN8ovUd-FnoXznY8s,8589
+tlhengine/models/clip/model.py,sha256=bPN1QuKVpjTAqExhPubY3qUPOBcKK31-BCvyRdfuDLQ,23365
+tlhengine/models/clip/simple_tokenizer.py,sha256=0bCfEO09Hiw0NhnLmMv6y5I2PdhgdSakOqf-LWDRW60,4632
+tlhengine-0.2.dist-info/METADATA,sha256=dCQ3vgoDvwK9hVbJawM8b3jlqa_LRGOuEcA4wywmDQ0,585
+tlhengine-0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tlhengine-0.2.dist-info/top_level.txt,sha256=lx8s3cg1-c3YB-TFGmkE1z2WOOYfy9gM83uH8zklVGQ,10
+tlhengine-0.2.dist-info/RECORD,,
```

