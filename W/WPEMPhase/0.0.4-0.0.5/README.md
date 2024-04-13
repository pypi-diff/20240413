# Comparing `tmp/WPEMPhase-0.0.4.tar.gz` & `tmp/WPEMPhase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPEMPhase-0.0.4.tar", last modified: Sun Feb 18 04:59:58 2024, max compression
+gzip compressed data, was "WPEMPhase-0.0.5.tar", last modified: Sat Apr 13 09:39:08 2024, max compression
```

## Comparing `WPEMPhase-0.0.4.tar` & `WPEMPhase-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-02-18 04:59:58.370789 WPEMPhase-0.0.4/
--rw-r--r--   0 jacob      (501) staff       (20)     1003 2024-02-18 04:59:58.370589 WPEMPhase-0.0.4/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.0.4/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-02-18 04:59:58.368431 WPEMPhase-0.0.4/WPEMPhase/
--rw-r--r--   0 jacob      (501) staff       (20)    10324 2024-02-18 04:59:51.000000 WPEMPhase-0.0.4/WPEMPhase/CPICANN.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.0.4/WPEMPhase/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-02-18 04:59:58.369166 WPEMPhase-0.0.4/WPEMPhase/config/
--rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.0.4/WPEMPhase/config/strucs.csv
--rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.0.4/WPEMPhase/data_format.py
--rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.0.4/WPEMPhase/model.py
--rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.0.4/WPEMPhase/plot.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-02-18 04:59:58.369048 WPEMPhase-0.0.4/WPEMPhase.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1003 2024-02-18 04:59:58.000000 WPEMPhase-0.0.4/WPEMPhase.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      315 2024-02-18 04:59:58.000000 WPEMPhase-0.0.4/WPEMPhase.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2024-02-18 04:59:58.000000 WPEMPhase-0.0.4/WPEMPhase.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       43 2024-02-18 04:59:58.000000 WPEMPhase-0.0.4/WPEMPhase.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       10 2024-02-18 04:59:58.000000 WPEMPhase-0.0.4/WPEMPhase.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2024-02-18 04:59:58.370831 WPEMPhase-0.0.4/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1172 2024-02-18 04:59:04.000000 WPEMPhase-0.0.4/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:39:08.139626 WPEMPhase-0.0.5/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-13 09:39:08.139423 WPEMPhase-0.0.5/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.0.5/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:39:08.137546 WPEMPhase-0.0.5/WPEMPhase/
+-rw-r--r--   0 jacob      (501) staff       (20)    10154 2024-04-13 09:38:35.000000 WPEMPhase-0.0.5/WPEMPhase/CPICANN.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.0.5/WPEMPhase/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:39:08.138294 WPEMPhase-0.0.5/WPEMPhase/config/
+-rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.0.5/WPEMPhase/config/strucs.csv
+-rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.0.5/WPEMPhase/data_format.py
+-rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.0.5/WPEMPhase/model.py
+-rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.0.5/WPEMPhase/plot.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-13 09:39:08.138167 WPEMPhase-0.0.5/WPEMPhase.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-13 09:39:07.000000 WPEMPhase-0.0.5/WPEMPhase.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      315 2024-04-13 09:39:08.000000 WPEMPhase-0.0.5/WPEMPhase.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-13 09:39:07.000000 WPEMPhase-0.0.5/WPEMPhase.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       48 2024-04-13 09:39:07.000000 WPEMPhase-0.0.5/WPEMPhase.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       10 2024-04-13 09:39:07.000000 WPEMPhase-0.0.5/WPEMPhase.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-13 09:39:08.139672 WPEMPhase-0.0.5/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1179 2024-04-13 09:37:16.000000 WPEMPhase-0.0.5/setup.py
```

### Comparing `WPEMPhase-0.0.4/PKG-INFO` & `WPEMPhase-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: torch
 Requires-Dist: plot
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: art
 Requires-Dist: pymatgen
+Requires-Dist: wget
 
 Crystallographic Phase Identifier of Convolutional self-Attention Neural Network (CPICANN)
 
 
 Maintained by Bin Cao. Please feel free to open issues in the Github or contact Bin Cao
 (binjacobcao@gmail.com) in case of any problems/comments/suggestions in using the code.
```

### Comparing `WPEMPhase-0.0.4/WPEMPhase/CPICANN.py` & `WPEMPhase-0.0.5/WPEMPhase/CPICANN.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import csv
 import os
 import datetime
 import pandas as pd
 import torch
 import numpy as np
+import sys
+import wget
 from .plot import _run 
 import zipfile
 import pkg_resources
 from .data_format import convert_file
 from .model import CPICANN_main
 from art import text2art
 
-def PhaseIdentifier(FilePath,Task='single-phase',ElementsSystem='',ElementsContained='',ElementsExclude='',Device='cuda:0',CIFfiles=None,NNparam=None,):
+def PhaseIdentifier(FilePath,Task='single-phase',ElementsSystem='',ElementsContained='',ElementsExclude='',Device='cuda:0',):
     """
     CPICANN : Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 
     Contributors : Shouyang Zhang & Bin Cao
     ================================================================
         Please feel free to open issues in the Github :
         https://github.com/WPEM/CPICANN
@@ -40,44 +42,33 @@
 
     :param ElementsExclude, type=str, default=''
         Specifies the elements to be excluded in the prediction, example: 'Fe_O'
 
     :param Device, type=str, default='cuda:0',
         Which device to run the CPICANN, example: 'cuda:0', 'cpu'.
 
-    :param CIFfiles, type=str, default=None,
-        at the first time execution, user need to assign the location of cifs' database, viz. strucs.zip file we provided, 
-    
-    :param NNparam, type=str, default=None,
-        at the first time execution, user need to assign the location of pretrained NN parameters, viz. pretrained.zip file we provided, 
-
     examples:
     from WPEMPhase import CPICANN
     CPICANN.PhaseIdentifier(FilePath='./single-phase',Device='cpu')
     """
     
     extract_to_folder = pkg_resources.get_distribution('WPEMPhase').location
     loc = os.path.join(extract_to_folder,'WPEMPhase')
     # supply CIF files 
-    if os.path.isdir(os.path.join(loc,'strucs')): pass
+    if os.path.isdir(os.path.join(loc,'strucs')) and os.path.isdir(os.path.join(loc,'pretrained')): pass
     else: 
-        if type(CIFfiles) == str: 
-            zipfile.ZipFile(CIFfiles).extractall(loc)
-        else:
-            print("This is the first time CPICANN is being executed on your computer.")
-            print("Please provide the file location of 'strucs.zip' using the parameter 'CIFfiles'.")
+        print("This is the first time CPICANN is being executed on your computer, configuring...")
+        file_url = "https://figshare.com/ndownloader/files/45638907"
+        _dir = os.path.isdir(os.path.join(loc, 'SystemFiles.zip'))
+        wget.download(file_url, _dir, bar=bar_progress)
+        prefix_dir = os.path.isdir(os.path.join(loc, 'SystemFiles'))
+        zipfile.ZipFile(os.path.isdir(os.path.join(prefix_dir, 'strucs.zip'))).extractall(loc)
+        zipfile.ZipFile(os.path.isdir(os.path.join(prefix_dir, 'pretrained.zip'))).extractall(loc)
+        
 
-    # supply pretrained parameters 
-    if os.path.isdir(os.path.join(loc,'pretrained')): pass
-    else: 
-        if type(NNparam) == str: 
-            zipfile.ZipFile(NNparam).extractall(loc)
-        else:
-            print("This is the first time CPICANN is being executed on your computer.")
-            print("Please provide the file location of 'pretrained.zip' using the parameter 'NNparam'.")
     
     os.makedirs('figs', exist_ok=True)
     now = datetime.datetime.now()
     formatted_date_time = now.strftime('%Y-%m-%d %H:%M:%S')
     print(text2art("CPICANN"))
     print('The phase identification module of WPEM')
     print('URL : https://github.com/WPEM/CPICANN')
@@ -283,7 +274,13 @@
 
 def filter_by_index(logits, index):
     if len(index) == 0:
         return logits
 
     logits[index] = -1e10
     return logits
+
+def bar_progress(current, total, width=80):
+  progress_message = "Downloading: %d%% [%d / %d] bytes" % (current / total * 100, current, total)
+  # Don't use print() as it will print in new line every time.
+  sys.stdout.write("\r" + progress_message)
+  sys.stdout.flush()
```

### Comparing `WPEMPhase-0.0.4/WPEMPhase/config/strucs.csv` & `WPEMPhase-0.0.5/WPEMPhase/config/strucs.csv`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.4/WPEMPhase/data_format.py` & `WPEMPhase-0.0.5/WPEMPhase/data_format.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.4/WPEMPhase/model.py` & `WPEMPhase-0.0.5/WPEMPhase/model.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.4/WPEMPhase/plot.py` & `WPEMPhase-0.0.5/WPEMPhase/plot.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.0.4/WPEMPhase.egg-info/PKG-INFO` & `WPEMPhase-0.0.5/WPEMPhase.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.0.4
+Version: 0.0.5
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: torch
 Requires-Dist: plot
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: art
 Requires-Dist: pymatgen
+Requires-Dist: wget
 
 Crystallographic Phase Identifier of Convolutional self-Attention Neural Network (CPICANN)
 
 
 Maintained by Bin Cao. Please feel free to open issues in the Github or contact Bin Cao
 (binjacobcao@gmail.com) in case of any problems/comments/suggestions in using the code.
```

### Comparing `WPEMPhase-0.0.4/setup.py` & `WPEMPhase-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='WPEMPhase',
-    version='0.0.4',
+    version='0.0.5',
     description="Crystallographic Phase Identifier of Convolutional self-Attention Neural Network",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='CaoBin',
     author_email='bcao@shu.edu.com',
     maintainer='CaoBin',
     maintainer_email='binjacobcao@gmail.com',
@@ -18,14 +18,14 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3.5',
-    install_requires=['torch', 'plot','scipy', 'pandas', 'numpy', 'art','pymatgen'],
+    install_requires=['torch', 'plot','scipy', 'pandas', 'numpy', 'art','pymatgen','wget'],
     entry_points={
         'console_scripts': [
             '',
         ],
     },
 )
```

