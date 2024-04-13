# Comparing `tmp/jaxonloader-0.3.7.tar.gz` & `tmp/jaxonloader-0.3.8.tar.gz`

## Comparing `jaxonloader-0.3.7.tar` & `jaxonloader-0.3.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/config.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 jaxonloader-0.3.8/PKG-INFO
```

### Comparing `jaxonloader-0.3.7/.github/workflows/nox.yaml` & `jaxonloader-0.3.8/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/docs/getting-started.md` & `jaxonloader-0.3.8/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/docs/index.md` & `jaxonloader-0.3.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/docs/images/performance.png` & `jaxonloader-0.3.8/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/jaxonloader/config.py` & `jaxonloader-0.3.8/jaxonloader/config.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/jaxonloader/dataloader.py` & `jaxonloader-0.3.8/jaxonloader/dataloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
-from numpy import typing as npt
+from beartype.typing import Union
+from jaxtyping import Array
+from numpy import ndarray as NDArray
 
 from jaxonloader import JaxonDataset
 from jaxonloader.utils import get_rng
 
 
 class JaxonDataLoader:
     def __init__(
@@ -31,15 +33,15 @@
         if self.shuffle:
             self.indices = rng.permutation(self.indices)
         self.index = 0
 
     def __iter__(self) -> "JaxonDataLoader":
         return self
 
-    def __next__(self) -> npt.NDArray | tuple[npt.NDArray, ...]:
+    def __next__(self) -> Array | NDArray | tuple[Union[NDArray, Array], ...]:
         if self.index < len(self.indices):
             batch_indices = self.indices[self.index : self.index + self.batch_size]
             self.index += self.batch_size
             return self.dataset[batch_indices]
         else:
             self.index = 0
             raise StopIteration
```

### Comparing `jaxonloader-0.3.7/jaxonloader/dataset.py` & `jaxonloader-0.3.8/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/jaxonloader/utils.py` & `jaxonloader-0.3.8/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.8/jaxonloader/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/jaxonloader/datasets/download.py` & `jaxonloader-0.3.8/jaxonloader/datasets/download.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.8/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/.gitignore` & `jaxonloader-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/LICENSE` & `jaxonloader-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/README.md` & `jaxonloader-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.7/pyproject.toml` & `jaxonloader-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.7"
+version = "0.3.8"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
```

### Comparing `jaxonloader-0.3.7/PKG-INFO` & `jaxonloader-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.7
+Version: 0.3.8
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

