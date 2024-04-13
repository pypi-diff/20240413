# Comparing `tmp/s2wav-1.0.2.tar.gz` & `tmp/s2wav-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2wav-1.0.2.tar", last modified: Thu Apr 11 16:03:33 2024, max compression
+gzip compressed data, was "s2wav-1.0.3.tar", last modified: Sat Apr 13 08:12:19 2024, max compression
```

## Comparing `s2wav-1.0.2.tar` & `s2wav-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316928 s2wav-1.0.2/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.2/LICENCE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-11 16:03:33.316703 s2wav-1.0.2/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9850 2024-04-09 13:46:46.000000 s2wav-1.0.2/README.md
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.313189 s2wav-1.0.2/s2wav/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      778 2024-04-09 14:10:43.000000 s2wav-1.0.2/s2wav/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24271 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/samples.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.315070 s2wav-1.0.2/s2wav/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/construct.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    14891 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11890 2024-04-11 13:07:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11169 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet_precompute_torch.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316463 s2wav-1.0.2/s2wav.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)      555 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-11 16:03:33.316975 s2wav-1.0.2/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-11 16:02:43.000000 s2wav-1.0.2/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316192 s2wav-1.0.2/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.2/tests/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/conftest.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4813 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_gradients.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10154 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_wavelets.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_wavelets_base.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.048276 s2wav-1.0.3/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.3/LICENCE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-13 08:12:19.048043 s2wav-1.0.3/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9936 2024-04-13 08:09:50.000000 s2wav-1.0.3/README.md
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.045654 s2wav-1.0.3/s2wav/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      778 2024-04-09 14:10:43.000000 s2wav-1.0.3/s2wav/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    21732 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/samples.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.046963 s2wav-1.0.3/s2wav/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/construct.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    14965 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11850 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11129 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet_precompute_torch.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.047786 s2wav-1.0.3/s2wav.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      555 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-13 08:12:19.048315 s2wav-1.0.3/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-13 08:11:03.000000 s2wav-1.0.3/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.047621 s2wav-1.0.3/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.3/tests/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/conftest.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4813 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_gradients.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10154 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_wavelets.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_wavelets_base.py
```

### Comparing `s2wav-1.0.2/LICENCE.txt` & `s2wav-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/PKG-INFO` & `s2wav-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.2
+Version: 1.0.3
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `s2wav-1.0.2/README.md` & `s2wav-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![image](https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml)
 [![image](https://codecov.io/gh/astro-informatics/s2wav/branch/main/graph/badge.svg?token=ZES6J4K3KZ)](https://codecov.io/gh/astro-informatics/s2wav)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![image](https://badge.fury.io/py/s2wav.svg)](https://badge.fury.io/py/s2wav)
 [![image](http://img.shields.io/badge/arXiv-2402.01282-orange.svg?style=flat)](https://arxiv.org/abs/2402.01282) <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-) <!-- ALL-CONTRIBUTORS-BADGE:END --> 
-[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15E64EAQ7TIp2a3cCoXtnNgf7Ud9MYjVq?usp=sharing)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://colab.research.google.com/drive/15E64EAQ7TIp2a3cCoXtnNgf7Ud9MYjVq?usp=sharing](https://colab.research.google.com/github/astro-informatics/s2wav/blob/main/notebooks/jax_transform.ipynb))
 
 <img align="left" height="85" width="98" src="./docs/assets/sax_logo.png">
 
 # Differentiable and accelerated wavelet transform on the sphere
 
 `S2WAV` is a python package for computing wavelet transforms on the sphere
 and rotation group, both in JAX and PyTorch. It leverages autodiff to provide differentiable
```

### Comparing `s2wav-1.0.2/s2wav/__init__.py` & `s2wav-1.0.3/s2wav/__init__.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/s2wav/filters.py` & `s2wav-1.0.3/s2wav/filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/s2wav/samples.py` & `s2wav-1.0.3/s2wav/samples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jax import jit
 import jax.numpy as jnp
 import numpy as np
 import torch
 import math
 from functools import partial
-from typing import Tuple
+from typing import Tuple, List
 from s2fft.sampling import s2_samples, so3_samples
 from scipy.special import loggamma
 from jax.scipy.special import gammaln as jax_gammaln
 
 
 def f_scal(
     L: int,
@@ -228,124 +228,70 @@
                     f_wav_j(L, j, N, lam, sampling, nside, multiresolution),
                     dtype=np.complex128,
                 )
             )
     return f
 
 
-@partial(jit, static_argnums=(0, 1, 2, 3, 4, 5, 6, 7))
+@partial(jit, static_argnums=(0, 1, 2, 3))
 def construct_f_jax(
     L: int,
-    N: int = 1,
     J_min: int = 0,
-    lam: float = 2.0,
-    sampling: str = "mw",
-    nside: int = None,
-    multiresolution: bool = False,
-    scattering: bool = False,
-) -> jnp.ndarray:
-    """Defines a list of arrays corresponding to f_wav.
+    J_max: int = None,
+    lam: float = 2.0
+) -> List:
+    """Defines a list corresponding to f_wav.
 
     Args:
         L (int): Harmonic bandlimit.
 
-        N (int, optional): Upper orientational band-limit. Defaults to 1.
-
         J_min (int, optional): Lowest frequency wavelet scale to be used. Defaults to 0.
 
+        J_max (int, optional): Highest frequency wavelet scale to be used. Defaults to None.
+
         lam (float, optional): Wavelet parameter which determines the scale factor between
             consecutive wavelet scales. Note that :math:`\lambda = 2` indicates dyadic
             wavelets. Defaults to 2.
 
-        sampling (str, optional): Spherical sampling scheme from
-            {"mw", "mwss", "dh", "gl", "healpix"}. Defaults to "mw".
-
-        nside (int, optional): HEALPix Nside resolution parameter.  Only required if
-            sampling="healpix".  Defaults to None.
-
-        multiresolution (bool, optional): Whether to store the scales at :math:`j_{\text{max}}`
-            resolution or its own resolution. Defaults to False.
-
-        scattering (bool, optional): Whether to create minimal arrays for scattering transform to
-            optimise for memory. Defaults to False.
-
     Returns:
-        jnp.ndarray: Empty array (or list of empty arrays) in which to write data.
+        List: Empty list in which to write data.
     """
-    J = j_max(L, lam)
-    if scattering:
-        f = jnp.zeros(
-            f_wav_j(L, J - 1, N, lam, sampling, nside, multiresolution),
-            dtype=jnp.complex128,
-        )
-    else:
-        f = []
-        for j in range(J_min, J + 1):
-            f.append(
-                jnp.zeros(
-                    f_wav_j(L, j, N, lam, sampling, nside, multiresolution),
-                    dtype=jnp.complex128,
-                )
-            )
+    J = J_max if J_max is not None else j_max(L, lam)
+    f = []
+    for _ in range(J_min, J + 1):
+        f.append([])
     return f
 
 
 def construct_f_torch(
     L: int,
-    N: int = 1,
     J_min: int = 0,
-    lam: float = 2.0,
-    sampling: str = "mw",
-    nside: int = None,
-    multiresolution: bool = False,
-    scattering: bool = False,
-) -> torch.tensor:
-    """Defines a list of tensors corresponding to f_wav.
+    J_max: int = None,
+    lam: float = 2.0
+) -> List:
+    """Defines a list corresponding to f_wav.
 
     Args:
         L (int): Harmonic bandlimit.
 
-        N (int, optional): Upper orientational band-limit. Defaults to 1.
-
         J_min (int, optional): Lowest frequency wavelet scale to be used. Defaults to 0.
 
+        J_max (int, optional): Highest frequency wavelet scale to be used. Defaults to None.
+
         lam (float, optional): Wavelet parameter which determines the scale factor between
             consecutive wavelet scales. Note that :math:`\lambda = 2` indicates dyadic
             wavelets. Defaults to 2.
 
-        sampling (str, optional): Spherical sampling scheme from
-            {"mw", "mwss", "dh", "gl", "healpix"}. Defaults to "mw".
-
-        nside (int, optional): HEALPix Nside resolution parameter.  Only required if
-            sampling="healpix".  Defaults to None.
-
-        multiresolution (bool, optional): Whether to store the scales at :math:`j_{\text{max}}`
-            resolution or its own resolution. Defaults to False.
-
-        scattering (bool, optional): Whether to create minimal arrays for scattering transform to
-            optimise for memory. Defaults to False.
-
     Returns:
-        torch.tensor: Empty tensor (or list of empty tensors) in which to write data.
+        List: Empty list in which to write data.
     """
-    J = j_max(L, lam)
-    if scattering:
-        f = torch.zeros(
-            f_wav_j(L, J - 1, N, lam, sampling, nside, multiresolution),
-            dtype=torch.complex128,
-        )
-    else:
-        f = []
-        for j in range(J_min, J + 1):
-            f.append(
-                torch.zeros(
-                    f_wav_j(L, j, N, lam, sampling, nside, multiresolution),
-                    dtype=torch.complex128,
-                )
-            )
+    J = J_max if J_max is not None else j_max(L, lam)
+    f = []
+    for _ in range(J_min, J + 1):
+        f.append([])
     return f
 
 
 def construct_flm(
     L: int, J_min: int = 0, lam: float = 2.0, multiresolution: bool = False
 ) -> Tuple[int, int]:
     r"""Returns the shape of scaling coefficients in harmonic space.
@@ -533,101 +479,89 @@
 
 
 @partial(jit, static_argnums=(0, 1, 2, 3, 4, 5))
 def construct_flmn_jax(
     L: int,
     N: int = 1,
     J_min: int = 0,
+    J_max: int = None,
     lam: float = 2.0,
-    multiresolution: bool = False,
-    scattering: bool = False,
+    multiresolution: bool = False
 ) -> jnp.ndarray:
     """Defines a list of arrays corresponding to flmn.
 
     Args:
         L (int): Harmonic bandlimit.
 
         N (int, optional): Upper orientational band-limit. Defaults to 1.
 
         J_min (int, optional): Lowest frequency wavelet scale to be used. Defaults to 0.
 
+        J_max (int, optional): Highest frequency wavelet scale to be used. Defaults to None.c
+
         lam (float, optional): Wavelet parameter which determines the scale factor between
             consecutive wavelet scales. Note that :math:`\lambda = 2` indicates dyadic
             wavelets. Defaults to 2.
 
         multiresolution (bool, optional): Whether to store the scales at :math:`j_{\text{max}}`
             resolution or its own resolution. Defaults to False.
 
-        scattering (bool, optional): Whether to create minimal arrays for scattering transform to
-            optimise for memory. Defaults to False.
-
     Returns:
         jnp.ndarray: Empty array (or list of empty arrays) in which to write data.
     """
-    J = j_max(L, lam)
-    if scattering:
-        flmn = jnp.zeros(
-            flmn_wav_j(L, J - 1, N, lam, multiresolution), dtype=jnp.complex128
-        )
-    else:
-        flmn = []
-        for j in range(J_min, J + 1):
-            flmn.append(
-                jnp.zeros(
-                    flmn_wav_j(L, j, N, lam, multiresolution),
-                    dtype=jnp.complex128,
-                )
+    J = J_max if J_max is not None else j_max(L, lam)
+    flmn = []
+    for j in range(J_min, J + 1):
+        flmn.append(
+            jnp.zeros(
+                flmn_wav_j(L, j, N, lam, multiresolution),
+                dtype=jnp.complex128,
             )
+        )
     return flmn
 
 
 def construct_flmn_torch(
     L: int,
     N: int = 1,
     J_min: int = 0,
+    J_max: int = None,
     lam: float = 2.0,
-    multiresolution: bool = False,
-    scattering: bool = False,
+    multiresolution: bool = False
 ) -> torch.tensor:
     """Defines a list of tensors corresponding to flmn.
 
     Args:
         L (int): Harmonic bandlimit.
 
         N (int, optional): Upper orientational band-limit. Defaults to 1.
 
         J_min (int, optional): Lowest frequency wavelet scale to be used. Defaults to 0.
 
+        J_max (int, optional): Highest frequency wavelet scale to be used. Defaults to None.c
+
         lam (float, optional): Wavelet parameter which determines the scale factor between
             consecutive wavelet scales. Note that :math:`\lambda = 2` indicates dyadic
             wavelets. Defaults to 2.
 
         multiresolution (bool, optional): Whether to store the scales at :math:`j_{\text{max}}`
             resolution or its own resolution. Defaults to False.
 
-        scattering (bool, optional): Whether to create minimal arrays for scattering transform to
-            optimise for memory. Defaults to False.
-
     Returns:
         torch.tensor: Empty tensor (or list of empty tensors) in which to write data.
     """
-    J = j_max(L, lam)
-    if scattering:
-        flmn = torch.zeros(
-            flmn_wav_j(L, J - 1, N, lam, multiresolution), dtype=torch.complex128
-        )
-    else:
-        flmn = []
-        for j in range(J_min, J + 1):
-            flmn.append(
-                torch.zeros(
-                    flmn_wav_j(L, j, N, lam, multiresolution),
-                    dtype=torch.complex128,
-                )
+    J = J_max if J_max is not None else j_max(L, lam)
+    flmn = []
+    for j in range(J_min, J + 1):
+        flmn.append(
+            torch.zeros(
+                flmn_wav_j(L, j, N, lam, multiresolution),
+                dtype=torch.complex128,
             )
+        )
     return flmn
 
 
 def j_max(L: int, lam: float = 2.0) -> int:
     r"""Computes needlet maximum level required to ensure exact reconstruction.
 
     Args:
```

### Comparing `s2wav-1.0.2/s2wav/transforms/base.py` & `s2wav-1.0.3/s2wav/transforms/base.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/s2wav/transforms/construct.py` & `s2wav-1.0.3/s2wav/transforms/construct.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/s2wav/transforms/wavelet.py` & `s2wav-1.0.3/s2wav/transforms/wavelet.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,16 +223,16 @@
     if precomps == None and not use_c_backend:
         precomps = construct.generate_wigner_precomputes(
             L, N, J_min, lam, sampling, nside, False, reality
         )
     J = samples.j_max(L, lam)
     Ls = samples.scal_bandlimit(L, J_min, lam, True)
 
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_jax(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_jax(L, J_min, J, lam)
 
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters[0]),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
@@ -341,14 +341,16 @@
 
         L (int): Harmonic bandlimit.
 
         N (int, optional): Upper azimuthal band-limit. Defaults to 1.
 
         J_min (int, optional): Lowest frequency wavelet scale to be used. Defaults to 0.
 
+        J_max (int, optional): Highest frequency wavelet scale to be used. Defaults to None.
+
         lam (float, optional): Wavelet parameter which determines the scale factor between consecutive wavelet scales.
             Note that :math:`\lambda = 2` indicates dyadic wavelets. Defaults to 2.
 
         sampling (str, optional): Spherical sampling scheme from {"mw","mwss", "dh", "healpix"}. Defaults to "mw".
 
         nside (int, optional): HEALPix Nside resolution parameter.  Only required if sampling="healpix".  Defaults
             to None.
@@ -375,16 +377,16 @@
     if precomps == None and not use_c_backend:
         precomps = construct.generate_wigner_precomputes(
             L, N, J_min, lam, sampling, nside, False, reality
         )
 
     J = J_max if J_max is not None else samples.j_max(L, lam)
 
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_jax(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_jax(L, J_min, J, lam)
 
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
@@ -402,17 +404,17 @@
                     flm[L0j:Lj, L - Lj : L - 1 + Lj],
                     wav_lm[j, L0j:Lj, L - Nj : L - 1 + Nj : 2],
                     optimize=True,
                 )
             )
         )
 
-        f_wav[j - J_min] = (
+        f_wav[j - J_min] = jnp.array(
             s2fft.wigner.inverse(
-                f_wav_lmn[j - J_min],
+                jnp.array(f_wav_lmn[j - J_min]),
                 Lj,
                 Nj,
                 nside,
                 sampling,
                 "jax_ssht",
                 reality,
                 _ssht_backend=_ssht_backend,
```

### Comparing `s2wav-1.0.2/s2wav/transforms/wavelet_precompute.py` & `s2wav-1.0.3/s2wav/transforms/wavelet_precompute.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,16 +163,16 @@
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = samples.j_max(L, lam)
     Ls = samples.scal_bandlimit(L, J_min, lam, True)
 
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_jax(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_jax(L, J_min, J, lam)
 
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters[0]),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
@@ -275,16 +275,16 @@
             with shape :math:`[n_{\theta}, n_{\phi}]`.
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = J_max if J_max is not None else samples.j_max(L, lam)
 
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_jax(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_jax(L, J_min, J, lam)
 
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
```

### Comparing `s2wav-1.0.2/s2wav/transforms/wavelet_precompute_torch.py` & `s2wav-1.0.3/s2wav/transforms/wavelet_precompute_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,16 @@
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = samples.j_max(L, lam)
     Ls = samples.scal_bandlimit(L, J_min, lam, True)
 
-    f_wav_lmn = samples.construct_flmn_torch(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_torch(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_torch(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_torch(L, J_min, J, lam)
 
     wav_lm = torch.einsum(
         "jln, l->jln",
         torch.conj(filters[0]),
         8 * torch.pi**2 / (2 * torch.arange(L, dtype=torch.float64) + 1),
     )
 
@@ -261,16 +261,16 @@
             with shape :math:`[n_{\theta}, n_{\phi}]`.
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = J_max if J_max is not None else samples.j_max(L, lam)
 
-    f_wav_lmn = samples.construct_flmn_torch(L, N, J_min, lam, True)
-    f_wav = samples.construct_f_torch(L, N, J_min, lam, sampling, nside, True)
+    f_wav_lmn = samples.construct_flmn_torch(L, N, J_min, J, lam, True)
+    f_wav = samples.construct_f_torch(L, J_min, J, lam)
 
     wav_lm = torch.einsum(
         "jln, l->jln",
         torch.conj(filters),
         8 * torch.pi**2 / (2 * torch.arange(L, dtype=torch.float64) + 1),
     )
```

### Comparing `s2wav-1.0.2/s2wav.egg-info/PKG-INFO` & `s2wav-1.0.3/s2wav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.2
+Version: 1.0.3
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `s2wav-1.0.2/s2wav.egg-info/SOURCES.txt` & `s2wav-1.0.3/s2wav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/setup.py` & `s2wav-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="s2wav",
-    version="1.0.2",
+    version="1.0.3",
     url="https://github.com/astro-informatics/s2wav",
     author="Authors & Contributors",
     license="GNU General Public License v3 (GPLv3)",
     python_requires=">=3.8",
     install_requires=requirements,
     description=("Differentiable and accelerated wavelet transforms with JAX"),
     long_description_content_type="text/x-rst",
```

### Comparing `s2wav-1.0.2/tests/conftest.py` & `s2wav-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/tests/test_filters.py` & `s2wav-1.0.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/tests/test_gradients.py` & `s2wav-1.0.3/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/tests/test_wavelets.py` & `s2wav-1.0.3/tests/test_wavelets.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.2/tests/test_wavelets_base.py` & `s2wav-1.0.3/tests/test_wavelets_base.py`

 * *Files identical despite different names*

