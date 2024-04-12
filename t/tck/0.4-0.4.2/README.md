# Comparing `tmp/tck-0.4.tar.gz` & `tmp/tck-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tck-0.4.tar", last modified: Sat Mar 23 18:08:50 2024, max compression
+gzip compressed data, was "tck-0.4.2.tar", last modified: Sat Apr 13 00:44:39 2024, max compression
```

## Comparing `tck-0.4.tar` & `tck-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-03-23 18:08:50.769651 tck-0.4/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-03-21 23:02:41.000000 tck-0.4/LICENSE
--rw-r--r--   0 filippo   (1001) filippo   (1001)     6100 2024-03-23 18:08:50.765651 tck-0.4/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     5449 2024-03-22 11:29:11.000000 tck-0.4/README.md
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-03-23 18:08:50.769651 tck-0.4/setup.cfg
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      818 2024-03-23 18:08:45.000000 tck-0.4/setup.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-03-23 18:08:50.765651 tck-0.4/tck/
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     6429 2024-03-21 23:18:31.000000 tck-0.4/tck/GMM_MAP_EM.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     2138 2024-03-21 23:23:22.000000 tck-0.4/tck/GMMposterior.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     4725 2024-03-21 23:22:31.000000 tck-0.4/tck/TCK.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-03-21 23:08:34.000000 tck-0.4/tck/__init__.py
--rw-rw-r--   0 filippo   (1001) filippo   (1001)     5496 2024-03-23 18:07:58.000000 tck-0.4/tck/datasets.py
-drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-03-23 18:08:50.765651 tck-0.4/tck.egg-info/
--rw-r--r--   0 filippo   (1001) filippo   (1001)     6100 2024-03-23 18:08:50.000000 tck-0.4/tck.egg-info/PKG-INFO
--rw-rw-r--   0 filippo   (1001) filippo   (1001)      241 2024-03-23 18:08:50.000000 tck-0.4/tck.egg-info/SOURCES.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-03-23 18:08:50.000000 tck-0.4/tck.egg-info/dependency_links.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)       51 2024-03-23 18:08:50.000000 tck-0.4/tck.egg-info/requires.txt
--rw-rw-r--   0 filippo   (1001) filippo   (1001)        4 2024-03-23 18:08:50.000000 tck-0.4/tck.egg-info/top_level.txt
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     1078 2024-03-21 23:02:41.000000 tck-0.4.2/LICENSE
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:44:39.748548 tck-0.4.2/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     5740 2024-03-25 11:34:48.000000 tck-0.4.2/README.md
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       38 2024-04-13 00:44:39.748548 tck-0.4.2/setup.cfg
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      820 2024-04-13 00:43:31.000000 tck-0.4.2/setup.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/tck/
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     6429 2024-03-21 23:18:31.000000 tck-0.4.2/tck/GMM_MAP_EM.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     2138 2024-03-21 23:23:22.000000 tck-0.4.2/tck/GMMposterior.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     4748 2024-04-13 00:42:59.000000 tck-0.4.2/tck/TCK.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        0 2024-03-21 23:08:34.000000 tck-0.4.2/tck/__init__.py
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)     5498 2024-03-23 19:06:23.000000 tck-0.4.2/tck/datasets.py
+drwxrwxr-x   0 filippo   (1001) filippo   (1001)        0 2024-04-13 00:44:39.748548 tck-0.4.2/tck.egg-info/
+-rw-r--r--   0 filippo   (1001) filippo   (1001)     6393 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/PKG-INFO
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)      241 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/SOURCES.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        1 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/dependency_links.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)       51 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/requires.txt
+-rw-rw-r--   0 filippo   (1001) filippo   (1001)        4 2024-04-13 00:44:39.000000 tck-0.4.2/tck.egg-info/top_level.txt
```

### Comparing `tck-0.4/LICENSE` & `tck-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tck-0.4/PKG-INFO` & `tck-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tck
-Version: 0.4
+Version: 0.4.2
 Summary: Kernel similarity for classification and clustering of multi-variate time series with missing values.
 Home-page: https://github.com/FilippoMB/Time-Series-Cluster-Kernel
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,25 @@
 Requires-Dist: numpy>1.19.5
 Requires-Dist: scikit_learn>=1.4
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 [![arXiv](https://img.shields.io/badge/arXiv-1803.07870-b31b1b.svg)](https://arxiv.org/abs/1704.00794)
+[![slides](https://custom-icon-badges.demolab.com/badge/slides-pdf-blue.svg?logo=note&logoSource=feather&logoColor=white)](docs/TCK.pdf)
+[![Downloads](https://static.pepy.tech/badge/tck)](https://pepy.tech/project/tck)
 
-The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. The kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
+The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. Once computed, the kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/FilippoMB/Time-Series-Cluster-Kernel/master/docs/tck_scheme.png" style="width: 18cm">
 <br>
 
-TCK is based on an ensemble of Gaussian Mixture Models for time series that use informative Bayesian priors robust to missing values. The similarity between two time series is proportional to the number of times the two time series are assigned to the same mixtures.
+TCK is based on an ensemble of Gaussian Mixture Models (GMMs) for time series. The GMMs use time-varying means to handle time dependencies and informative Bayesian priors to handle missing values. The similarity between two time series is proportional to the number of times they are assigned to the same mixtures.
 
 
 # Installation
 
 The recommended installation is with pip:
 
 ````bash
@@ -67,17 +69,17 @@
 python examples/clustering.py
 ````
 
 The following notebooks illustrate more advanced use-cases.
 
 - Perform time series dimensionality reduction, cluster analysis, and visualize the results: [view](https://nbviewer.org/github/FilippoMB/Time-Series-Cluster-Kernel/blob/main/notebooks/clustering.ipynb) or [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hLF0SfiZZ13zhik0vAjWfvs__GJvV9c4?usp=sharing)
 
-## Running on Windows
+## &#x26A0; Running on Windows
 
-TCK uses multiprocessing. While using multiprocessing in Python on windows, it is necessary to protect the entry point of the program by using 
+TCK uses multiprocessing. While using multiprocessing in Python on Windows, it is necessary to protect the entry point of the program by using 
 
 ```python
 if __name__ == '__main__':
 ```
 
 Please, refer to the following examples.
```

### Comparing `tck-0.4/README.md` & `tck-0.4.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [![arXiv](https://img.shields.io/badge/arXiv-1803.07870-b31b1b.svg)](https://arxiv.org/abs/1704.00794)
+[![slides](https://custom-icon-badges.demolab.com/badge/slides-pdf-blue.svg?logo=note&logoSource=feather&logoColor=white)](docs/TCK.pdf)
+[![Downloads](https://static.pepy.tech/badge/tck)](https://pepy.tech/project/tck)
 
-The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. The kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
+The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. Once computed, the kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/FilippoMB/Time-Series-Cluster-Kernel/master/docs/tck_scheme.png" style="width: 18cm">
 <br>
 
-TCK is based on an ensemble of Gaussian Mixture Models for time series that use informative Bayesian priors robust to missing values. The similarity between two time series is proportional to the number of times the two time series are assigned to the same mixtures.
+TCK is based on an ensemble of Gaussian Mixture Models (GMMs) for time series. The GMMs use time-varying means to handle time dependencies and informative Bayesian priors to handle missing values. The similarity between two time series is proportional to the number of times they are assigned to the same mixtures.
 
 
 # Installation
 
 The recommended installation is with pip:
 
 ````bash
@@ -48,17 +50,17 @@
 python examples/clustering.py
 ````
 
 The following notebooks illustrate more advanced use-cases.
 
 - Perform time series dimensionality reduction, cluster analysis, and visualize the results: [view](https://nbviewer.org/github/FilippoMB/Time-Series-Cluster-Kernel/blob/main/notebooks/clustering.ipynb) or [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hLF0SfiZZ13zhik0vAjWfvs__GJvV9c4?usp=sharing)
 
-## Running on Windows
+## &#x26A0; Running on Windows
 
-TCK uses multiprocessing. While using multiprocessing in Python on windows, it is necessary to protect the entry point of the program by using 
+TCK uses multiprocessing. While using multiprocessing in Python on Windows, it is necessary to protect the entry point of the program by using 
 
 ```python
 if __name__ == '__main__':
 ```
 
 Please, refer to the following examples.
```

### Comparing `tck-0.4/setup.py` & `tck-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tck",
-    version="0.4",
+    version="0.4.2",
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'numpy>1.19.5',
         'scikit_learn>=1.4',
         'scipy',
         'requests',
```

### Comparing `tck-0.4/tck/GMM_MAP_EM.py` & `tck-0.4.2/tck/GMM_MAP_EM.py`

 * *Files identical despite different names*

### Comparing `tck-0.4/tck/GMMposterior.py` & `tck-0.4.2/tck/GMMposterior.py`

 * *Files identical despite different names*

### Comparing `tck-0.4/tck/TCK.py` & `tck-0.4.2/tck/TCK.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from concurrent.futures import ProcessPoolExecutor
 import numpy as np
-import tqdm
+from tqdm.autonotebook import tqdm
 from sklearn.preprocessing import normalize
 from .GMM_MAP_EM import GMM_MAP_EM
 from .GMMposterior import GMMposterior
 
 class TCK:
     def __init__(self, G=30, C=None):
         self.G = G
```

### Comparing `tck-0.4/tck/datasets.py` & `tck-0.4.2/tck/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             if len(Xte.shape) < 3:
                 Xte = np.atleast_3d(Xte)
             Yte = data['Yte']
             n_classes_tr = len(np.unique(Ytr))
             n_classes_te = len(np.unique(Yte))
             if n_classes_tr != n_classes_te:
                 warnings.warn(f"Number of classes in training and test sets do not match for {alias} dataset.")
-            print(f"Loaded {alias} dataset.\nData shapes:\n Xtr: {Xtr.shape}\n Ytr: {Ytr.shape}\n Xte: {Xte.shape}\n Yte: {Yte.shape}\n Number of classes: {n_classes_tr} ")
+            print(f"Loaded {alias} dataset.\nNumber of classes: {n_classes_tr}\nData shapes:\n  Xtr: {Xtr.shape}\n  Ytr: {Ytr.shape}\n  Xte: {Xte.shape}\n  Yte: {Yte.shape}")
 
             return (Xtr, Ytr, Xte, Yte)
         else:
             print(f"Failed to download {alias} dataset.")
             return None
 
 if __name__ == '__main__':
```

### Comparing `tck-0.4/tck.egg-info/PKG-INFO` & `tck-0.4.2/tck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tck
-Version: 0.4
+Version: 0.4.2
 Summary: Kernel similarity for classification and clustering of multi-variate time series with missing values.
 Home-page: https://github.com/FilippoMB/Time-Series-Cluster-Kernel
 Author: Filippo Maria Bianchi
 Author-email: filippombianchi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,23 +14,25 @@
 Requires-Dist: numpy>1.19.5
 Requires-Dist: scikit_learn>=1.4
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 [![arXiv](https://img.shields.io/badge/arXiv-1803.07870-b31b1b.svg)](https://arxiv.org/abs/1704.00794)
+[![slides](https://custom-icon-badges.demolab.com/badge/slides-pdf-blue.svg?logo=note&logoSource=feather&logoColor=white)](docs/TCK.pdf)
+[![Downloads](https://static.pepy.tech/badge/tck)](https://pepy.tech/project/tck)
 
-The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. The kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
+The Time Series Cluster Kernel (TCK) is a kernel similarity for multivariate time series with missing values. Once computed, the kernel can be used to perform tasks such as classification, clustering, and dimensionality reduction.
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/FilippoMB/Time-Series-Cluster-Kernel/master/docs/tck_scheme.png" style="width: 18cm">
 <br>
 
-TCK is based on an ensemble of Gaussian Mixture Models for time series that use informative Bayesian priors robust to missing values. The similarity between two time series is proportional to the number of times the two time series are assigned to the same mixtures.
+TCK is based on an ensemble of Gaussian Mixture Models (GMMs) for time series. The GMMs use time-varying means to handle time dependencies and informative Bayesian priors to handle missing values. The similarity between two time series is proportional to the number of times they are assigned to the same mixtures.
 
 
 # Installation
 
 The recommended installation is with pip:
 
 ````bash
@@ -67,17 +69,17 @@
 python examples/clustering.py
 ````
 
 The following notebooks illustrate more advanced use-cases.
 
 - Perform time series dimensionality reduction, cluster analysis, and visualize the results: [view](https://nbviewer.org/github/FilippoMB/Time-Series-Cluster-Kernel/blob/main/notebooks/clustering.ipynb) or [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hLF0SfiZZ13zhik0vAjWfvs__GJvV9c4?usp=sharing)
 
-## Running on Windows
+## &#x26A0; Running on Windows
 
-TCK uses multiprocessing. While using multiprocessing in Python on windows, it is necessary to protect the entry point of the program by using 
+TCK uses multiprocessing. While using multiprocessing in Python on Windows, it is necessary to protect the entry point of the program by using 
 
 ```python
 if __name__ == '__main__':
 ```
 
 Please, refer to the following examples.
```

