# Comparing `tmp/vplanet-2.5.2.tar.gz` & `tmp/vplanet-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vplanet-2.5.2.tar", last modified: Tue Apr  9 17:51:54 2024, max compression
+gzip compressed data, was "vplanet-2.5.3.tar", last modified: Sat Apr 13 04:19:15 2024, max compression
```

## Comparing `vplanet-2.5.2.tar` & `vplanet-2.5.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 17:51:52.000000 vplanet-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-09 17:51:54.348073 vplanet-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-09 17:51:52.000000 vplanet-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:51:54.348073 vplanet-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-09 17:51:52.000000 vplanet-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)   172056 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/atmesc.c
--rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/binary.c
--rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/body.c
--rw-r--r--   0 runner    (1001) docker     (127)    35872 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/control.c
--rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/distorb.c
--rw-r--r--   0 runner    (1001) docker     (127)    84678 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/distrot.c
--rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/eqtide.c
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/evolve.c
--rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/flare.c
--rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/galhabit.c
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/halt.c
--rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/magmoc.c
--rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/options.c
--rw-r--r--   0 runner    (1001) docker     (127)    83300 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/output.c
--rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/poise.c
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/python_interface.c
--rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/radheat.c
--rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/spinbody.c
--rw-r--r--   0 runner    (1001) docker     (127)    77727 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/stellar.c
--rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/system.c
--rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/thermint.c
--rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/update.c
--rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/verify.c
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-09 17:51:52.000000 vplanet-2.5.2/src/vplanet.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/vplanet/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/quantity_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/vplanet_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-09 17:51:52.000000 vplanet-2.5.2/vplanet/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:54.348073 vplanet-2.5.2/vplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 17:51:54.000000 vplanet-2.5.2/vplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 04:19:10.000000 vplanet-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-13 04:19:15.157432 vplanet-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-13 04:19:10.000000 vplanet-2.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:19:15.157432 vplanet-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-13 04:19:11.000000 vplanet-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)   172320 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/atmesc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    90413 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/binary.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45057 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/body.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35872 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/control.c
+-rw-r--r--   0 runner    (1001) docker     (127)   261673 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/distorb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    84678 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/distrot.c
+-rw-r--r--   0 runner    (1001) docker     (127)   173282 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/eqtide.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/evolve.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71119 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/flare.c
+-rw-r--r--   0 runner    (1001) docker     (127)   141475 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/galhabit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/halt.c
+-rw-r--r--   0 runner    (1001) docker     (127)   116650 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/magmoc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    93363 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)   160335 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/options.c
+-rw-r--r--   0 runner    (1001) docker     (127)    83300 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/output.c
+-rw-r--r--   0 runner    (1001) docker     (127)   284882 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/poise.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/python_interface.c
+-rw-r--r--   0 runner    (1001) docker     (127)   245259 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/radheat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48492 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/spinbody.c
+-rw-r--r--   0 runner    (1001) docker     (127)    77727 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/stellar.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33849 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/system.c
+-rw-r--r--   0 runner    (1001) docker     (127)   196096 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/thermint.c
+-rw-r--r--   0 runner    (1001) docker     (127)   159057 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/update.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43834 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/verify.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-13 04:19:11.000000 vplanet-2.5.3/src/vplanet.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/vplanet/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/quantity_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/vplanet_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-13 04:19:11.000000 vplanet-2.5.3/vplanet/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:19:15.157432 vplanet-2.5.3/vplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 04:19:15.000000 vplanet-2.5.3/vplanet.egg-info/top_level.txt
```

### Comparing `vplanet-2.5.2/LICENSE` & `vplanet-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/PKG-INFO` & `vplanet-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.2
+Version: 2.5.3
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -27,14 +27,17 @@
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
+   <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
+     <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
+  </a>
   <br>
   <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.2 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.3 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
-        _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
+    _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
    [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
```

### Comparing `vplanet-2.5.2/README.md` & `vplanet-2.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
+   <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
+     <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
+  </a>
   <br>
   <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
-        _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
+    _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
    [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
```

### Comparing `vplanet-2.5.2/setup.py` & `vplanet-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/atmesc.c` & `vplanet-2.5.3/src/atmesc.c`

 * *Files 1% similar despite different names*

```diff
@@ -4134,26 +4134,33 @@
 
   // 2. Check if planet is beyond RG limit; if user requested water loss to stop
   // (the cold trap prevents water loss) then water does not escape.
   // NOTE: The RG flux limit below is calculated based on body zero's
   // spectrum! The Kopparapu+14 limit is for a single star only. This
   // approximation for a binary is only valid if the two stars have
   // similar spectral types, or if body zero dominates the flux.
-  if (fdInstellation(body, iBody) < fdHZRG14(body, iBody)) {
-    if (body[iBody].dRGDuration == 0.) {
-      body[iBody].dRGDuration = body[iBody].dAge;
-      if (io->iVerbose > VERBPROG && !io->baEnterHZMessage[iBody]) {
-        printf("%s enters the habitable zone at %.2lf Myr.\n",
-               body[iBody].cName, evolve->dTime / (YEARSEC * 1e6));
-        io->baEnterHZMessage[iBody] = 1;
+  double dInstellation = fdInstellation(body, iBody);
+  if (dInstellation == -1 && body[iBody].bCalcFXUV == 0) {
+    // Constant XUV flux, so set water to escape
+    return 1;
+  } else {
+    double dRunawayGreenhouseFlux = fdHZRG14(body, iBody);
+    if (dInstellation < dRunawayGreenhouseFlux) {
+      if (body[iBody].dRGDuration == 0.) {
+        body[iBody].dRGDuration = body[iBody].dAge;
+        if (io->iVerbose > VERBPROG && !io->baEnterHZMessage[iBody]) {
+          printf("%s enters the habitable zone at %.2lf Myr.\n",
+                body[iBody].cName, evolve->dTime / (YEARSEC * 1e6));
+          io->baEnterHZMessage[iBody] = 1;
+        }
+      }
+      // Only stop water loss if user requested, which is default
+      if (body[iBody].bStopWaterLossInHZ) {
+        return 0;
       }
-    }
-    // Only stop water loss if user requested, which is default
-    if (body[iBody].bStopWaterLossInHZ) {
-      return 0;
     }
   }
 
   // 3. Is there still water to be lost?
   if (body[iBody].dSurfaceWaterMass <= 0) {
     return 0;
   }
```

### Comparing `vplanet-2.5.2/src/binary.c` & `vplanet-2.5.3/src/binary.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/body.c` & `vplanet-2.5.3/src/body.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/control.c` & `vplanet-2.5.3/src/control.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/distorb.c` & `vplanet-2.5.3/src/distorb.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/distrot.c` & `vplanet-2.5.3/src/distrot.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/eqtide.c` & `vplanet-2.5.3/src/eqtide.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/evolve.c` & `vplanet-2.5.3/src/evolve.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/flare.c` & `vplanet-2.5.3/src/flare.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/galhabit.c` & `vplanet-2.5.3/src/galhabit.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/halt.c` & `vplanet-2.5.3/src/halt.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/magmoc.c` & `vplanet-2.5.3/src/magmoc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/module.c` & `vplanet-2.5.3/src/module.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/options.c` & `vplanet-2.5.3/src/options.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/output.c` & `vplanet-2.5.3/src/output.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/poise.c` & `vplanet-2.5.3/src/poise.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/python_interface.c` & `vplanet-2.5.3/src/python_interface.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/radheat.c` & `vplanet-2.5.3/src/radheat.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/spinbody.c` & `vplanet-2.5.3/src/spinbody.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/stellar.c` & `vplanet-2.5.3/src/stellar.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/system.c` & `vplanet-2.5.3/src/system.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/thermint.c` & `vplanet-2.5.3/src/thermint.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/update.c` & `vplanet-2.5.3/src/update.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/verify.c` & `vplanet-2.5.3/src/verify.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/src/vplanet.c` & `vplanet-2.5.3/src/vplanet.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/custom_units.py` & `vplanet-2.5.3/vplanet/custom_units.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/log.py` & `vplanet-2.5.3/vplanet/log.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/output.py` & `vplanet-2.5.3/vplanet/output.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/quantity.py` & `vplanet-2.5.3/vplanet/quantity.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/quantity_support.py` & `vplanet-2.5.3/vplanet/quantity_support.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet/wrapper.py` & `vplanet-2.5.3/vplanet/wrapper.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.5.2/vplanet.egg-info/PKG-INFO` & `vplanet-2.5.3/vplanet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.5.2
+Version: 2.5.3
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -27,14 +27,17 @@
   </a>
   <a href="https://VirtualPlanetaryLaboratory.github.io/vplanet/conduct.html">
     <img src="https://img.shields.io/badge/Code%20of-Conduct-7d93c7.svg">
   </a>
   <a href="https://www.youtube.com/@VPLanetCode/playlists">
     <img src="https://img.shields.io/badge/You-Tube-darkred.svg">
   </a>
+   <a href="https://github.com/VirtualPlanetaryLaboratory/vplanet/discussions">
+     <img src="https://img.shields.io/badge/Discussions-darkgreen.svg">
+  </a>
   <br>
   <img src="https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg">
   <img src="https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-linux.yml/badge.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2020-Python%203.6--3.11-7d93c7.svg">
   <img src="https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-7d93c7.svg">
   
   <br>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.5.2 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.5.3 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ************ VVPPLLaanneett:: TThhee VViirrttuuaall PPllaanneett SSiimmuullaattoorr ************
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___d_o_c_s_-_b_l_u_e_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_][https://
    github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/docs.yml/
             badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_a_d_-_t_h_e___p_a_p_e_r_-
    _d_a_r_k_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_-_C_o_n_d_u_c_t_-
-        _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]
+    _7_d_9_3_c_7_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Y_o_u_-_T_u_b_e_-_d_a_r_k_r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/
+                _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_i_s_c_u_s_s_i_o_n_s_-_d_a_r_k_g_r_e_e_n_._s_v_g_]
    [https://img.shields.io/badge/Unit%20Tests-18,062-darkblue.svg][https://
     github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
  linux.yml/badge.svg][https://img.shields.io/badge/Ubuntu%2020-Python%203.6--
  3.11-7d93c7.svg][https://img.shields.io/badge/Ubuntu%2022-Python%203.7--3.11-
                                   7d93c7.svg]
 [https://github.com/VirtualPlanetaryLaboratory/vplanet/actions/workflows/tests-
     macos-intel.yml/badge.svg][https://img.shields.io/badge/MacOS%2011--13-
```

### Comparing `vplanet-2.5.2/vplanet.egg-info/SOURCES.txt` & `vplanet-2.5.3/vplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

