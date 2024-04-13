# Comparing `tmp/Cp2kData-0.6.7.tar.gz` & `tmp/Cp2kData-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cp2kData-0.6.7.tar", last modified: Fri Apr 12 10:50:58 2024, max compression
+gzip compressed data, was "Cp2kData-0.6.8.tar", last modified: Sat Apr 13 13:01:21 2024, max compression
```

## Comparing `Cp2kData-0.6.7.tar` & `Cp2kData-0.6.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/Cp2kData.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 10:50:58.000000 Cp2kData-0.6.7/Cp2kData.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.603613 Cp2kData-0.6.7/cp2kdata/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/block_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/atomic_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/converge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/dft_plus_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/dipole.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/energies.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/errors_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/fep.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/geo_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/header_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/hirshfeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/md_xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/mulliken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/block_parser/stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cli/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/cube/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/cube/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/dpdata_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/matplotlibstyle/jcp.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.607613 Cp2kData-0.6.7/cp2kdata/pdos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/pdos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/pdos/pdos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/cp2kdata/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/fep_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/geo_opt_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/plots/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/cp2kdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:50:58.611613 Cp2kData-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 10:50:54.000000 Cp2kData-0.6.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/Cp2kData.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:01:21.000000 Cp2kData-0.6.8/Cp2kData.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.756707 Cp2kData-0.6.8/cp2kdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.760707 Cp2kData-0.6.8/cp2kdata/block_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/atomic_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/converge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/dft_plus_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/energies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/errors_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/fep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/geo_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/header_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/hirshfeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/md_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/mulliken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/block_parser/stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.760707 Cp2kData-0.6.8/cp2kdata/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cli/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cli/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.760707 Cp2kData-0.6.8/cp2kdata/cube/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/cube/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/dpdata_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.760707 Cp2kData-0.6.8/cp2kdata/matplotlibstyle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/matplotlibstyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/matplotlibstyle/jcp.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/cp2kdata/pdos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/pdos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/pdos/pdos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/cp2kdata/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/plots/fep_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/plots/geo_opt_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/plots/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/cp2kdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:01:21.764707 Cp2kData-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-13 13:01:17.000000 Cp2kData-0.6.8/tests/test.py
```

### Comparing `Cp2kData-0.6.7/Cp2kData.egg-info/PKG-INFO` & `Cp2kData-0.6.8/Cp2kData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cp2kData
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Small Package to Postprocess Cp2k Output
 Author-email: Yongbin Zhuang <robinzhuang@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Cp2kData-0.6.7/Cp2kData.egg-info/SOURCES.txt` & `Cp2kData-0.6.8/Cp2kData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/LICENSE` & `Cp2kData-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/PKG-INFO` & `Cp2kData-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Cp2kData
-Version: 0.6.7
+Version: 0.6.8
 Summary: A Small Package to Postprocess Cp2k Output
 Author-email: Yongbin Zhuang <robinzhuang@outlook.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Cp2kData-0.6.7/README.md` & `Cp2kData-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/atomic_kind.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/atomic_kind.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/cells.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/cells.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/converge.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/converge.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/coordinates.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/coordinates.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/dft_plus_u.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/dft_plus_u.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/dipole.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/dipole.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/forces.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/forces.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/geo_opt.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/geo_opt.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/header_info.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/header_info.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/hirshfeld.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/hirshfeld.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/md_xyz.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/md_xyz.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/mulliken.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/mulliken.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/block_parser/stress.py` & `Cp2kData-0.6.8/cp2kdata/block_parser/stress.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/cell.py` & `Cp2kData-0.6.8/cp2kdata/cell.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/cli/cmd.py` & `Cp2kData-0.6.8/cp2kdata/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/cube/cube.py` & `Cp2kData-0.6.8/cp2kdata/cube/cube.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/dpdata_plugin.py` & `Cp2kData-0.6.8/cp2kdata/dpdata_plugin.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/matplotlibstyle/jcp.mplstyle` & `Cp2kData-0.6.8/cp2kdata/matplotlibstyle/jcp.mplstyle`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/output.py` & `Cp2kData-0.6.8/cp2kdata/output.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/pdos/pdos.py` & `Cp2kData-0.6.8/cp2kdata/pdos/pdos.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/plots/fep_plot.py` & `Cp2kData-0.6.8/cp2kdata/plots/fep_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/plots/geo_opt_plot.py` & `Cp2kData-0.6.8/cp2kdata/plots/geo_opt_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/plots/test_plot.py` & `Cp2kData-0.6.8/cp2kdata/plots/test_plot.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/test_input.py` & `Cp2kData-0.6.8/cp2kdata/test_input.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/units.py` & `Cp2kData-0.6.8/cp2kdata/units.py`

 * *Files identical despite different names*

### Comparing `Cp2kData-0.6.7/cp2kdata/utils.py` & `Cp2kData-0.6.8/cp2kdata/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 this script put misc function here.
 """
-from turtle import pos
 from ase.geometry.analysis import Analysis
 from ase.io import read, write
 #from cp2kdata import Cp2kOutput
 import numpy as np
 import os
 import shutil
```

### Comparing `Cp2kData-0.6.7/pyproject.toml` & `Cp2kData-0.6.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Cp2kData"
-version = "0.6.7"
+version = "0.6.8"
 description = "A Small Package to Postprocess Cp2k Output"
 authors = [
     {name = "Yongbin Zhuang", email = "robinzhuang@outlook.com"}
     ]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
```

### Comparing `Cp2kData-0.6.7/tests/test.py` & `Cp2kData-0.6.8/tests/test.py`

 * *Files identical despite different names*

