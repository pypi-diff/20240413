# Comparing `tmp/braintools-0.0.2-py2.py3-none-any.whl.zip` & `tmp/braintools-0.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 79791 bytes, number of entries: 38
--rw-rw-rw-  2.0 fat      914 b- defN 24-Apr-06 07:27 braintools/__init__.py
+Zip file size: 79983 bytes, number of entries: 38
+-rw-rw-rw-  2.0 fat      912 b- defN 24-Apr-13 06:57 braintools/__init__.py
 -rw-rw-rw-  2.0 fat     1025 b- defN 24-Apr-06 08:01 braintools/functional/__init__.py
 -rw-rw-rw-  2.0 fat    18207 b- defN 24-Apr-11 11:10 braintools/functional/_activations.py
--rw-rw-rw-  2.0 fat     1745 b- defN 24-Apr-11 11:10 braintools/functional/_normalization.py
+-rw-rw-rw-  2.0 fat     2149 b- defN 24-Apr-13 06:57 braintools/functional/_normalization.py
 -rw-rw-rw-  2.0 fat     2581 b- defN 24-Apr-11 11:10 braintools/functional/_spikes.py
 -rw-rw-rw-  2.0 fat     1102 b- defN 24-Apr-06 07:27 braintools/init/__init__.py
 -rw-rw-rw-  2.0 fat     1153 b- defN 24-Apr-06 07:27 braintools/init/_base.py
 -rw-rw-rw-  2.0 fat     6427 b- defN 24-Apr-06 07:27 braintools/init/_generic.py
 -rw-rw-rw-  2.0 fat    15361 b- defN 24-Apr-06 07:27 braintools/init/_random_inits.py
 -rw-rw-rw-  2.0 fat     3071 b- defN 24-Apr-06 07:27 braintools/init/_regular_inits.py
 -rw-rw-rw-  2.0 fat      963 b- defN 24-Apr-06 07:27 braintools/input/__init__.py
@@ -28,13 +28,13 @@
 -rw-rw-rw-  2.0 fat     4945 b- defN 24-Apr-11 11:10 braintools/metric/_regression_test.py
 -rw-rw-rw-  2.0 fat     1583 b- defN 24-Apr-06 07:27 braintools/metric/_smoothing.py
 -rw-rw-rw-  2.0 fat     2012 b- defN 24-Apr-11 11:10 braintools/metric/_smoothing_test.py
 -rw-rw-rw-  2.0 fat     1036 b- defN 24-Apr-06 08:01 braintools/metric/_util.py
 -rw-rw-rw-  2.0 fat      924 b- defN 24-Apr-06 07:27 braintools/optim/__init__.py
 -rw-rw-rw-  2.0 fat    15582 b- defN 24-Apr-06 07:27 braintools/optim/_lr_scheduler.py
 -rw-rw-rw-  2.0 fat    45895 b- defN 24-Apr-06 07:27 braintools/optim/_sgd_optimizer.py
--rw-rw-rw-  2.0 fat    11554 b- defN 24-Apr-11 11:21 braintools-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3970 b- defN 24-Apr-11 11:21 braintools-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-11 11:21 braintools-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-11 11:21 braintools-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3344 b- defN 24-Apr-11 11:21 braintools-0.0.2.dist-info/RECORD
-38 files, 264473 bytes uncompressed, 74423 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    11554 b- defN 24-Apr-13 06:58 braintools-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4019 b- defN 24-Apr-13 06:58 braintools-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 06:58 braintools-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-13 06:58 braintools-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3344 b- defN 24-Apr-13 06:58 braintools-0.0.3.dist-info/RECORD
+38 files, 264924 bytes uncompressed, 74615 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -93,23 +93,23 @@
 
 Filename: braintools/optim/_lr_scheduler.py
 Comment: 
 
 Filename: braintools/optim/_sgd_optimizer.py
 Comment: 
 
-Filename: braintools-0.0.2.dist-info/LICENSE
+Filename: braintools-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: braintools-0.0.2.dist-info/METADATA
+Filename: braintools-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: braintools-0.0.2.dist-info/WHEEL
+Filename: braintools-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: braintools-0.0.2.dist-info/top_level.txt
+Filename: braintools-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: braintools-0.0.2.dist-info/RECORD
+Filename: braintools-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## braintools/__init__.py

```diff
@@ -10,16 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
-
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from . import metric
 from . import input
 from . import init
 from . import optim
 from . import functional
```

## braintools/functional/_normalization.py

```diff
@@ -15,48 +15,57 @@
 
 from __future__ import annotations
 from typing import Sequence, Optional
 
 import jax
 import jax.numpy as jnp
 import numpy as np
+import braincore as bc
 
 
 __all__ = [
   'weight_standardization',
 ]
 
 
 def weight_standardization(
     w: jax.typing.ArrayLike,
-    axes: Sequence[int],
-    eps: float,
-    gain: Optional[jax.Array] = None
+    eps: float = 1e-4,
+    gain: Optional[jax.Array] = None,
+    out_axis: int = -1,
 ):
   """
-  Scaled Weight Standardization.
+  Scaled Weight Standardization,
+  see `Micro-Batch Training with Batch-Channel Normalization and Weight Standardization <https://paperswithcode.com/paper/weight-standardization>`_.
 
   Parameters
   ----------
   w : jax.typing.ArrayLike
       The weight tensor.
-  axes : Sequence[int]
-      The axes to calculate the mean and variance.
   eps : float
       A small value to avoid division by zero.
   gain : Array
       The gain function, by default None.
+  out_axis : int
+      The output axis, by default -1.
 
   Returns
   -------
   jax.typing.ArrayLike
       The scaled weight tensor.
-
   """
-  # Get Scaled WS weight HWIO;
-  fan_in = np.prod(w.shape[:-1])
-  mean = jnp.mean(w, axis=axes[:-1], keepdims=True)
-  var = jnp.var(w, axis=axes[:-1], keepdims=True)
-  weight = (w - mean) / (var * fan_in + eps) ** 0.5
+  if out_axis < 0:
+    out_axis = w.ndim + out_axis
+  fan_in = 1  # get the fan-in of the weight tensor
+  axes = []  # get the axes of the weight tensor
+  for i in range(w.ndim):
+    if i != out_axis:
+      fan_in *= w.shape[i]
+      axes.append(i)
+  # normalize the weight
+  mean = jnp.mean(w, axis=axes, keepdims=True)
+  var = jnp.var(w, axis=axes, keepdims=True)
+  scale = jax.lax.rsqrt(jnp.maximum(var * fan_in, eps))
   if gain is not None:
-    weight = gain * weight
-  return weight
+    scale = gain * scale
+  shift = mean * scale
+  return w * scale - shift
```

## Comparing `braintools-0.0.2.dist-info/LICENSE` & `braintools-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `braintools-0.0.2.dist-info/METADATA` & `braintools-0.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braintools
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Toolbox for Brain Dynamics Programming.
 Home-page: https://github.com/brainpy/braintools
 Author: BrainPy Team
 Author-email: BrainPy Team <chao.brain@qq.com>
 License: Apache-2.0 license
 Project-URL: homepage, http://github.com/brainpy/braintools
 Project-URL: repository, http://github.com/brainpy/braintools
@@ -54,21 +54,23 @@
 </p> 
 
 
 
 <p align="center">
 	<a href="https://pypi.org/project/braintools/"><img alt="Supported Python Version" src="https://img.shields.io/pypi/pyversions/braintools"></a>
 	<a href="https://github.com/brainpy/braintools/blob/main/LICENSE"><img alt="LICENSE" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  	<a href="https://brainpy.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation" src="https://readthedocs.org/projects/brainpy/badge/?version=latest"></a>
-  	<a href="https://badge.fury.io/py/braintools"><img alt="PyPI version" src="https://badge.fury.io/py/braintools.svg"></a>
+    <a href='https://braintools.readthedocs.io/en/latest/?badge=latest'>
+        <img src='https://readthedocs.org/projects/braintools/badge/?version=latest' alt='Documentation Status' />
+    </a>  	
+    <a href="https://badge.fury.io/py/braintools"><img alt="PyPI version" src="https://badge.fury.io/py/braintools.svg"></a>
     <a href="https://github.com/brainpy/braintools/actions/workflows/CI.yml"><img alt="Continuous Integration" src="https://github.com/brainpy/braintools/actions/workflows/CI.yml/badge.svg"></a>
 </p>
 
 
-[``braintools``](https://github.com/brainpy/braintools) provides toolboxes for brain dynamics programming. 
+[``braintools``](https://github.com/brainpy/braintools) provides common toolboxes for brain dynamics programming (BDP). 
 
 
 ## Installation
 
 You can install ``braintools`` via pip:
 
 ```bash
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: braintools Version: 0.0.2 Summary: The Toolbox for
+Metadata-Version: 2.1 Name: braintools Version: 0.0.3 Summary: The Toolbox for
 Brain Dynamics Programming. Home-page: https://github.com/brainpy/braintools
 Author: BrainPy Team Author-email: BrainPy Team
 qq.com> License: Apache-2.0 license Project-URL: homepage, http://github.com/
 brainpy/braintools Project-URL: repository, http://github.com/brainpy/
 braintools Keywords: BrainPy,brain simulation,brain-inspired computing
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 4 - Beta Classifier: Intended
@@ -22,21 +22,21 @@
 Extra: cuda11 Requires-Dist: jaxlib[cuda11_pip] ; extra == 'cuda11' Provides-
 Extra: cuda11_mini Requires-Dist: jaxlib[cuda11_pip] ; extra == 'cuda11_mini'
 Provides-Extra: cuda12 Requires-Dist: jaxlib[cuda12_pip] ; extra == 'cuda12'
 Provides-Extra: cuda12_mini Requires-Dist: jaxlib[cuda12_pip] ; extra ==
 'cuda12_mini' Provides-Extra: testing Requires-Dist: pytest ; extra ==
 'testing' Provides-Extra: tpu Requires-Dist: jaxlib[tpu] ; extra == 'tpu'
                          [Header image of braintools.]
-  _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_I_C_E_N_S_E_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_C_o_n_t_i_n_u_o_u_s
-                                 _I_n_t_e_g_r_a_t_i_o_n_]
-[``braintools``](https://github.com/brainpy/braintools) provides toolboxes for
-brain dynamics programming. ## Installation You can install ``braintools`` via
-pip: ```bash pip install braintools --upgrade ``` ## Documentation The official
-documentation is hosted on Read the Docs: [https://braintools.readthedocs.io]
-(https://braintools.readthedocs.io) ## See also the BDP ecosystem -
-[``brainpy``](https://github.com/brainpy/BrainPy): The solution for the
-general-purpose brain dynamics programming. - [``braincore``](https://
+    _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_I_C_E_N_S_E_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]
+                           _[_C_o_n_t_i_n_u_o_u_s_ _I_n_t_e_g_r_a_t_i_o_n_]
+[``braintools``](https://github.com/brainpy/braintools) provides common
+toolboxes for brain dynamics programming (BDP). ## Installation You can install
+``braintools`` via pip: ```bash pip install braintools --upgrade ``` ##
+Documentation The official documentation is hosted on Read the Docs: [https://
+braintools.readthedocs.io](https://braintools.readthedocs.io) ## See also the
+BDP ecosystem - [``brainpy``](https://github.com/brainpy/BrainPy): The solution
+for the general-purpose brain dynamics programming. - [``braincore``](https://
 github.com/brainpy/braincore): The core system for the next generation of
 BrainPy framework. - [``braintools``](https://github.com/brainpy/braintools):
 The tools for the brain dynamics simulation and analysis. - [``brainscale``]
 (https://github.com/brainpy/brainscale): The scalable online learning for
 biological spiking neural networks.
```

## Comparing `braintools-0.0.2.dist-info/RECORD` & `braintools-0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-braintools/__init__.py,sha256=28iT8j5bpoXJCdZMMKpLTgM2k7aEhTe2RrlZFPCIPLE,914
+braintools/__init__.py,sha256=AQUeRHpFnPSS_nSNRu8Y8_sFgleR4-HgKW4B2g9ffnU,912
 braintools/functional/__init__.py,sha256=Y5DiZqdZJzJCAu821TNaiAyBoZ8RI6jGew0bVQfGX7I,1025
 braintools/functional/_activations.py,sha256=VF_JGa7frjamuf0B2GV_N-QGGsQFKxw0RCHjzboTdSE,18207
-braintools/functional/_normalization.py,sha256=eyotm4XfzsQlm-5Vi5befjfupg54KFW4IhYRITWrrHQ,1745
+braintools/functional/_normalization.py,sha256=rLO69zQ90JrnL3Vm-24sFRc7u5j31vntxB5Cuwsdg4Y,2149
 braintools/functional/_spikes.py,sha256=rNlABZIIZXvc6_tT8koPDZrECr_O6rGM8YKSytgU8E0,2581
 braintools/init/__init__.py,sha256=p0QKaKZQ29IsrY8R3-4t_teGlCgQKEJYYdBizpiKkkc,1102
 braintools/init/_base.py,sha256=OcetgiXdDHvzoaTzaKh_XAKEscX7e9iHZkP4oZBg2Do,1153
 braintools/init/_generic.py,sha256=j9VMOle_D44lT0IfUf6wqrJRi0ztq3JEcmqqViljE7w,6427
 braintools/init/_random_inits.py,sha256=6jCIdtZ-SkSbLaGPe722NhrZPDoSk7OHYeK-TauLpIQ,15361
 braintools/init/_regular_inits.py,sha256=bA5frDYeeDXtqnaUws1-JsCkt-PVKCn9HOT3SmQdl1E,3071
 braintools/input/__init__.py,sha256=Z3jEuruG5iLKSsqznq9GW-gaJq6tg9nKhSTx6c7Pep0,963
@@ -27,12 +27,12 @@
 braintools/metric/_regression_test.py,sha256=CrVCvpQF4LB_ikiyzpjHC_CRBrQGFF_iIExnbcqCXSM,4945
 braintools/metric/_smoothing.py,sha256=GJ5HaOw-Ec6sledF_T289Ow7A6mQgNXMnSRw3188VME,1583
 braintools/metric/_smoothing_test.py,sha256=isVXdZs6nT8bnZzBabIdF2xh11LLq2rxbp0K8UZHAcc,2012
 braintools/metric/_util.py,sha256=l1oOKSWEIaWQSgoHpRF6hzpJhZ3Yf5Pq278M8uY7D2U,1036
 braintools/optim/__init__.py,sha256=ceb586IP74ya8vsWyQMCvf_xUX5Nbf3ECN2SIfXEADQ,924
 braintools/optim/_lr_scheduler.py,sha256=1ZB-5vkMBSXeIYPEInOi5RNDzt3FuGcKAZNklZ-vlGY,15582
 braintools/optim/_sgd_optimizer.py,sha256=ylz8QsP3nbG5TkgQgA2GYGiTppBrN1vfS7oTkoupkeg,45895
-braintools-0.0.2.dist-info/LICENSE,sha256=6fh5QkGp7UhVlXVDg46cZBy4gXG2927_iGk1KL0nGy4,11554
-braintools-0.0.2.dist-info/METADATA,sha256=Soky18WHe8VxKj2rVSmD_0TD8ULigp7aH7mJGCoG3MM,3970
-braintools-0.0.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-braintools-0.0.2.dist-info/top_level.txt,sha256=kpCUCOcIqo3D72vd6PIcAG-VeUzsgDFUneOQwywwmyc,11
-braintools-0.0.2.dist-info/RECORD,,
+braintools-0.0.3.dist-info/LICENSE,sha256=6fh5QkGp7UhVlXVDg46cZBy4gXG2927_iGk1KL0nGy4,11554
+braintools-0.0.3.dist-info/METADATA,sha256=cnJehafyubL-8XOFiCEuDf3bMe6xAbzuqOG_aOztxkM,4019
+braintools-0.0.3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+braintools-0.0.3.dist-info/top_level.txt,sha256=kpCUCOcIqo3D72vd6PIcAG-VeUzsgDFUneOQwywwmyc,11
+braintools-0.0.3.dist-info/RECORD,,
```

