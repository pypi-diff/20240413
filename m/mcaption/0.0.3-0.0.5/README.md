# Comparing `tmp/mcaption-0.0.3.tar.gz` & `tmp/mcaption-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcaption-0.0.3.tar", last modified: Fri Apr 12 15:07:05 2024, max compression
+gzip compressed data, was "mcaption-0.0.5.tar", last modified: Sat Apr 13 16:56:50 2024, max compression
```

## Comparing `mcaption-0.0.3.tar` & `mcaption-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:05.618340 mcaption-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 15:06:59.000000 mcaption-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-12 15:07:05.618340 mcaption-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-12 15:06:59.000000 mcaption-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:05.618340 mcaption-0.0.3/mcaption/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 15:06:59.000000 mcaption-0.0.3/mcaption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-12 15:06:59.000000 mcaption-0.0.3/mcaption/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9409 2024-04-12 15:06:59.000000 mcaption-0.0.3/mcaption/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:07:05.618340 mcaption-0.0.3/mcaption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-12 15:07:05.000000 mcaption-0.0.3/mcaption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 15:07:05.000000 mcaption-0.0.3/mcaption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:07:05.000000 mcaption-0.0.3/mcaption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 15:07:05.000000 mcaption-0.0.3/mcaption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:07:05.000000 mcaption-0.0.3/mcaption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:07:05.618340 mcaption-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-12 15:06:59.000000 mcaption-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:56:50.720763 mcaption-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 16:56:43.000000 mcaption-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-13 16:56:50.720763 mcaption-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-13 16:56:43.000000 mcaption-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:56:50.720763 mcaption-0.0.5/mcaption/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-13 16:56:43.000000 mcaption-0.0.5/mcaption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-13 16:56:43.000000 mcaption-0.0.5/mcaption/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-13 16:56:43.000000 mcaption-0.0.5/mcaption/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:56:50.720763 mcaption-0.0.5/mcaption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-13 16:56:50.000000 mcaption-0.0.5/mcaption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 16:56:50.000000 mcaption-0.0.5/mcaption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:56:50.000000 mcaption-0.0.5/mcaption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 16:56:50.000000 mcaption-0.0.5/mcaption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 16:56:50.000000 mcaption-0.0.5/mcaption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:56:50.720763 mcaption-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-13 16:56:43.000000 mcaption-0.0.5/setup.py
```

### Comparing `mcaption-0.0.3/LICENSE` & `mcaption-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcaption-0.0.3/PKG-INFO` & `mcaption-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mcaption
-Version: 0.0.3
+Version: 0.0.5
 Summary: A modern implementation of simple image captioning
-Home-page: https://github.com/manbehindthemadness/modern-craft
+Home-page: https://github.com/manbehindthemadness/modern-caption
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: scikit-image>=0.18.1
 Requires-Dist: transformers>=4.10.2
 Requires-Dist: numpy
 Requires-Dist: ftfy
 Requires-Dist: tqdm
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 <h1>Modern-Caption</h1>
 
 ---
 
 **Description:**
```

### Comparing `mcaption-0.0.3/README.md` & `mcaption-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mcaption-0.0.3/mcaption/main.py` & `mcaption-0.0.5/mcaption/main.py`

 * *Files identical despite different names*

### Comparing `mcaption-0.0.3/mcaption/utils.py` & `mcaption-0.0.5/mcaption/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Utility code.
 """
-import urllib.request
 from pathlib import Path
 from torch import nn
 import torch
 import numpy as np
 import torch.nn.functional as nnf
 from typing import Tuple, Optional
 from transformers import (
@@ -23,33 +22,14 @@
     'coco': {
         'file': 'coco_weights.pth',
         'url': 'https://huggingface.co/Manbehindthemadness/conceptual_coco/resolve/main/coco_weights.pth'
     }
 }
 
 
-def download_if_not_exist(path: Path, url: str):
-    """
-    Checks if a file specified by path exists. If not, downloads it from the given URL.
-
-    Args:
-        path (Path): The path to the file.
-        url (str): The URL from which to download the file.
-    """
-    path.mkdir(parents=True, exist_ok=True)
-    file_name = url.split('/')[-1]
-    file_path = path / file_name
-    if not file_path.exists():
-        print(f"Downloading {path.name} from {url}...")
-        urllib.request.urlretrieve(url, file_path)
-        print("Download complete!")
-    else:
-        print(f"Confirmed {file_path} exists")
-
-
 class MLP(nn.Module):
     def forward(self, x: None) -> None:
         return self.model(x)
 
     def __init__(self, sizes: Tuple[int, ...], bias=True, act=nn.Tanh):
         super(MLP, self).__init__()
         layers = []
```

### Comparing `mcaption-0.0.3/mcaption.egg-info/PKG-INFO` & `mcaption-0.0.5/mcaption.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mcaption
-Version: 0.0.3
+Version: 0.0.5
 Summary: A modern implementation of simple image captioning
-Home-page: https://github.com/manbehindthemadness/modern-craft
+Home-page: https://github.com/manbehindthemadness/modern-caption
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Requires-Dist: scikit-image>=0.18.1
 Requires-Dist: transformers>=4.10.2
 Requires-Dist: numpy
 Requires-Dist: ftfy
 Requires-Dist: tqdm
 Requires-Dist: torch>=2.0.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 <h1>Modern-Caption</h1>
 
 ---
 
 **Description:**
```

### Comparing `mcaption-0.0.3/setup.py` & `mcaption-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     'scikit-image>=0.18.1',
     'transformers>=4.10.2',
     'numpy',
     'ftfy',
     'tqdm',
     'torch>=2.0.0',
     'torchvision>=0.17.0',
+    'quickdl',
 ]
 
 excludes = [
     'torch',
     'torchvision',
 ]
 
@@ -23,27 +24,27 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='mcaption',
-    version='0.0.3',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
     author_email='manbehindthemadness@gmail.com',
     description='A modern implementation of simple image captioning',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/manbehindthemadness/modern-craft',
+    url='https://github.com/manbehindthemadness/modern-caption',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
 )
```

