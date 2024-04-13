# Comparing `tmp/unite_toolbox-0.1.5.tar.gz` & `tmp/unite_toolbox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unite_toolbox-0.1.5.tar", last modified: Mon Feb 26 18:15:49 2024, max compression
+gzip compressed data, was "unite_toolbox-0.1.6.tar", last modified: Sat Apr 13 13:42:02 2024, max compression
```

## Comparing `unite_toolbox-0.1.5.tar` & `unite_toolbox-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:15:49.810651 unite_toolbox-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-26 18:15:49.810651 unite_toolbox-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 18:15:49.810651 unite_toolbox-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:15:49.810651 unite_toolbox-0.1.5/unite_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/unite_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/unite_toolbox/bin_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/unite_toolbox/kde_estimators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-02-26 18:15:36.000000 unite_toolbox-0.1.5/unite_toolbox/knn_estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:15:49.810651 unite_toolbox-0.1.5/unite_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-26 18:15:49.000000 unite_toolbox-0.1.5/unite_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-26 18:15:49.000000 unite_toolbox-0.1.5/unite_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 18:15:49.000000 unite_toolbox-0.1.5/unite_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-26 18:15:49.000000 unite_toolbox-0.1.5/unite_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-26 18:15:49.000000 unite_toolbox-0.1.5/unite_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/bin_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/kde_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/knn_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/data_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/marginal_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-13 13:41:56.000000 unite_toolbox-0.1.6/unite_toolbox/utils/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:42:02.049980 unite_toolbox-0.1.6/unite_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 13:42:02.000000 unite_toolbox-0.1.6/unite_toolbox.egg-info/top_level.txt
```

### Comparing `unite_toolbox-0.1.5/PKG-INFO` & `unite_toolbox-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 Metadata-Version: 2.1
 Name: unite_toolbox
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolbox for practical applications of information theory.
 Author-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>, Anneli Guthke <anneli.guthke@simtech.uni-stuttgart.de>, Uwe Ehret <uwe.ehret@kit.edu>, Hoshin Gupta <hoshin@arizona.edu>
 Maintainer-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>
 License: MIT License
 Project-URL: Documentation, https://unite-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/manuel-alvarez-chaves/unite_toolbox
 Project-URL: Team, https://www.simtech.uni-stuttgart.de/exc/research/junior-research-groups/statistical-model-data-integration/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Provides-Extra: dev
 Requires-Dist: jupyterlab>=4.1.2; extra == "dev"
 Requires-Dist: matplotlib>=3.8.3; extra == "dev"
 Requires-Dist: numpy>=1.26.4; extra == "dev"
 Requires-Dist: pandas>=2.2.1; extra == "dev"
 Requires-Dist: pyarrow>=15.0.0; extra == "dev"
 Requires-Dist: scipy>=1.12.0; extra == "dev"
 Requires-Dist: tqdm>=4.66.2; extra == "dev"
 Requires-Dist: xarray>=2024.2.0; extra == "dev"
 
 # UNITE Toolbox
-###  Unified diagnostic evaluation of physics-based, data-driven and hybrid hydrological models based on information theory
 
-This repository contains code for the UNITE set of tools based on information theory for the diagnostic evaluation of hydrological models. In the UNITE tools we have functions to calculate different quantities used in information theory: entropy $H(X)$, Kullback-Leibler divergence $D_{KL}(p||q)$, mutual information $I(X; Y)$, using different methods. More specifically, the methods implemented are:
+### Unified diagnostic evaluation of scientific models based on information theory
 
- - Kernel density based estimation (KDE)
- - Binning using histograms
- - *k*-nearest neighbor based estimation (*k*NN)
+The **UNITE Toolbox** is a Python library for incorporating _Information Theory_
+into data analysis and modeling workflows.
+The toolbox collects different methods of estimating information-theoretic quantities
+in one easy-to-use Python package.
+Currently, UNITE includes functions to calculate entropy $H(X)$,
+Kullback-Leibler divergence $D_{KL}(p||q)$, and mutual information $I(X; Y)$,
+using three methods:
+
+- Kernel density-based estimation (KDE)
+- Binning using histograms
+- _k_-nearest neighbor-based estimation (_k_-NN)
 
 ## Installation
-Although the code is still highly experimental and in very active development, a release version is hosted in PyPI and can be installed using `pip`. Check the `pyproject.toml` for requirements. The current state of the toolbox can be installed directly from this repository using `git`.
+
+Although the code is still highly experimental and in very active development,
+a release version is available on PyPI and can be installed using `pip`.
 
 ```
 pip install unite_toolbox
 ```
 
-## How-to
+Alternatively, the latest updates can be installed directly from this repository
 
-In the folder `examples\` please find a tutorial on the general usage of the toolbox.
+```
+pip install git+https://github.com/manuel-alvarez-chaves/unite_toolbox
+```
+
+Check the `pyproject.toml` for requirements.
+
+## How-to
 
+In the [documentation](https://unite-toolbox.readthedocs.io/) please find
+[tutorials](https://unite-toolbox.readthedocs.io/en/latest/tutorials.html) on
+the general usage of the toolbox and some applications.
```

### Comparing `unite_toolbox-0.1.5/unite_toolbox/knn_estimators.py` & `unite_toolbox-0.1.6/unite_toolbox/knn_estimators.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     p_norm : int
         p (Minkowski) distance. p = 1 is the Manhattan distance,
         p = 2 is the Euclidian distance, etc.
 
     Returns
     -------
     vol : float
-        Volume of the L^p ball"""
+        Volume of the L^p ball
+    """
 
     if p_norm == np.inf:  # faster
         vol = (2**d) * (r**d)
         return vol
 
     a = (2 * gamma(1 / p_norm + 1)) ** d
     b = gamma(d / p_norm + 1)
@@ -112,29 +113,25 @@
         Array of shape (n_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
 
     Returns
     -------
     h : float
-        Entropy of the data set [in nats]"""
+        Entropy of the data set [in nats]
+    """
 
     if len(data.shape) == 1:
         data = data.reshape(-1, 1)
 
     n, d = data.shape
 
     knn_tree = KDTree(data)
     radius = knn_tree.query(data, k + 1, p=p_norm)[0][:, k]
-    h = (
-        digamma(n)
-        - digamma(k)
-        + np.log(vol_lp_ball(1.0, d, p_norm))
-        + d * np.mean(np.log(radius))
-    )
+    h = digamma(n) - digamma(k) + np.log(vol_lp_ball(1.0, d, p_norm)) + d * np.mean(np.log(radius))
     return h
 
 
 def calc_knn_kld(p, q, k=1, p_norm=2):
     r"""Calculates the the Kullback-Leibler divergence (relative entropy) between
     two n-d arrays of data.
 
@@ -142,15 +139,17 @@
     two data sets (p and q) [in nats] using the estimation method proposed
     by Wang et al. (2009). Both p and q are n-d arrays where d >= 1 which means
     they can have multiple features. Typically p represents the true distribution
     while q is the approximate distribution. Different number of total
     samples in p and q is acceptable, 10.1109/TIT.2009.2016060
 
     .. math::
-        \hat{D}_{KL\,n,m}(p||q) = \frac{d}{n} \sum_{i=1}^{n} \log \left ( \frac{\nu_k(i)}{\rho_k(i)} \right ) + \log\left (\frac{m}{n-1}\right )
+        \hat{D}_{KL\,n,m}(p||q)
+        = \frac{d}{n} \sum_{i=1}^{n} \log \left ( \frac{\nu_k(i)}{\rho_k(i)} \right )
+        + \log\left (\frac{m}{n-1}\right )
 
     Where:
         * :math:`d` is the number of dimensions of the data.
         * :math:`n` is the number of samples in *p*.
         * :math:`\rho_k(i)` is the distance between :math:`x_i` and its *k*-NN in :math:`{x_j}_(j \neq i)`.
         * :math:`\nu_k(i)` is the distance between :math:`x_i` and its *k*-NN in :math:`y_j`.
         * :math:`m` is the number of points in *q*.
@@ -166,15 +165,16 @@
     p_norm : int, optional
         p (Minkowski) distance. p = 1 is the Manhattan distance,
         p = 2 is the Euclidian distance, etc.
 
     Returns
     -------
     kld : float
-        Kullback-Leibler divergence between p and q [in nats]"""
+        Kullback-Leibler divergence between p and q [in nats]
+    """
 
     n, m = len(p), len(q)
     d = len(p[0])
 
     rho, _ = KDTree(p).query(p, k + 1, p=p_norm)
     nu, _ = KDTree(q).query(p, k, p=p_norm)
     rho = rho.reshape(-1, k + 1)[:, -1]
@@ -182,43 +182,49 @@
 
     kld = (d / n) * np.sum(np.log(nu / rho)) + np.log(m / (n - 1))
 
     return max(0.0, kld)
 
 
 def calc_knn_mutual_information(x, y, k=15):
-    r"""Calculates the mutual information between two n-d arrays of data.
+    r"""Calculates mutual information between X and Y using $k$-NN.
 
-    Estimates the mutual information between two data sets (x and y) [in nats] using
-    the method of estimation proposed Kraskov et al. (2004). Both x and y
-    can have d >= 1 which means they can have multiple features. By default, the maximum
-    norm (p-norm = ∞) and three neighbors (k = 3) are used. 10.1103/PhysRevE.69.066138
+    Estimates the mutual information between X and Y [in nats] using
+    the method of estimation proposed Kraskov et al. (2004). Both X and Y
+    can have d >= 1 which means they can have multiple features. By default,
+    the maximum norm (p-norm = ∞) and fifteen neighbors (k = 15) are used.
+    10.1103/PhysRevE.69.066138
 
     .. math::
-        \hat{I}(X;Y) = \psi(k) - \frac{1}{N} \sum_{i=1}^{N} \mathbb{E} \left[\psi(n_{i,x} + 1) + \psi(n_{i,y} + 1) \right] + \psi(N)
+        \hat{I}(X;Y)
+        = \psi(k) - \frac{1}{N} \sum_{i=1}^{N} \mathbb{E} \left[\psi(n_{i,x} + 1) + \psi(n_{i,y} + 1) \right]
+        + \psi(N)
 
     Where:
         * :math:`\psi` is the digamma function.
         * :math:`N` is the number of samples.
         * :math:`\mathbb{E}` is the expectation operation.
-        * :math:`n_{i,x}` and :math:`n_{i,y}` are the number of neighbors of every point within a given radius calculated as the distance to the *k*-th nearest neighbor in the joint X-Y space.
+        * :math:`n_{i,x}` and :math:`n_{i,y}` are the number of neighbors
+        of every point within a given radius calculated as the distance to
+        the *k*-th nearest neighbor in the joint X-Y space.
 
     Parameters
     ----------
     x : numpy.ndarray
         Array of shape (n_samples, d_features)
     y : numpy.ndarray
         Array of shape (n_samples, d_features)
     k : int, optional
         no. of nearest neighbors to use
 
     Returns
     -------
     mi : float
-        Mutual information between x and y [in nats]"""
+        Mutual information between x and y [in nats]
+    """
 
     assert len(x) == len(y), "x and y must have the same number of samples."
 
     n_samples = len(x)
     xy = np.hstack((x, y))
 
     xy_tree = KDTree(xy)
```

### Comparing `unite_toolbox-0.1.5/unite_toolbox.egg-info/PKG-INFO` & `unite_toolbox-0.1.6/unite_toolbox.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 Metadata-Version: 2.1
 Name: unite_toolbox
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolbox for practical applications of information theory.
 Author-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>, Anneli Guthke <anneli.guthke@simtech.uni-stuttgart.de>, Uwe Ehret <uwe.ehret@kit.edu>, Hoshin Gupta <hoshin@arizona.edu>
 Maintainer-email: Manuel Álvarez Chaves <manuel.alvarezchaves@simtech.uni-stuttgart.de>
 License: MIT License
 Project-URL: Documentation, https://unite-toolbox.readthedocs.io/
 Project-URL: Repository, https://github.com/manuel-alvarez-chaves/unite_toolbox
 Project-URL: Team, https://www.simtech.uni-stuttgart.de/exc/research/junior-research-groups/statistical-model-data-integration/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: tqdm>=4.66.2
 Provides-Extra: dev
 Requires-Dist: jupyterlab>=4.1.2; extra == "dev"
 Requires-Dist: matplotlib>=3.8.3; extra == "dev"
 Requires-Dist: numpy>=1.26.4; extra == "dev"
 Requires-Dist: pandas>=2.2.1; extra == "dev"
 Requires-Dist: pyarrow>=15.0.0; extra == "dev"
 Requires-Dist: scipy>=1.12.0; extra == "dev"
 Requires-Dist: tqdm>=4.66.2; extra == "dev"
 Requires-Dist: xarray>=2024.2.0; extra == "dev"
 
 # UNITE Toolbox
-###  Unified diagnostic evaluation of physics-based, data-driven and hybrid hydrological models based on information theory
 
-This repository contains code for the UNITE set of tools based on information theory for the diagnostic evaluation of hydrological models. In the UNITE tools we have functions to calculate different quantities used in information theory: entropy $H(X)$, Kullback-Leibler divergence $D_{KL}(p||q)$, mutual information $I(X; Y)$, using different methods. More specifically, the methods implemented are:
+### Unified diagnostic evaluation of scientific models based on information theory
 
- - Kernel density based estimation (KDE)
- - Binning using histograms
- - *k*-nearest neighbor based estimation (*k*NN)
+The **UNITE Toolbox** is a Python library for incorporating _Information Theory_
+into data analysis and modeling workflows.
+The toolbox collects different methods of estimating information-theoretic quantities
+in one easy-to-use Python package.
+Currently, UNITE includes functions to calculate entropy $H(X)$,
+Kullback-Leibler divergence $D_{KL}(p||q)$, and mutual information $I(X; Y)$,
+using three methods:
+
+- Kernel density-based estimation (KDE)
+- Binning using histograms
+- _k_-nearest neighbor-based estimation (_k_-NN)
 
 ## Installation
-Although the code is still highly experimental and in very active development, a release version is hosted in PyPI and can be installed using `pip`. Check the `pyproject.toml` for requirements. The current state of the toolbox can be installed directly from this repository using `git`.
+
+Although the code is still highly experimental and in very active development,
+a release version is available on PyPI and can be installed using `pip`.
 
 ```
 pip install unite_toolbox
 ```
 
-## How-to
+Alternatively, the latest updates can be installed directly from this repository
 
-In the folder `examples\` please find a tutorial on the general usage of the toolbox.
+```
+pip install git+https://github.com/manuel-alvarez-chaves/unite_toolbox
+```
+
+Check the `pyproject.toml` for requirements.
+
+## How-to
 
+In the [documentation](https://unite-toolbox.readthedocs.io/) please find
+[tutorials](https://unite-toolbox.readthedocs.io/en/latest/tutorials.html) on
+the general usage of the toolbox and some applications.
```

