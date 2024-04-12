# Comparing `tmp/mtpy-v2-2.0.6.tar.gz` & `tmp/mtpy-v2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtpy-v2-2.0.6.tar", last modified: Wed Feb 28 00:52:59 2024, max compression
+gzip compressed data, was "mtpy-v2-2.0.7.tar", last modified: Fri Apr 12 22:53:56 2024, max compression
```

## Comparing `mtpy-v2-2.0.6.tar` & `mtpy-v2-2.0.7.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.516056 mtpy-v2-2.0.6/
--rw-rw-rw-   0        0        0      675 2023-11-13 20:23:07.000000 mtpy-v2-2.0.6/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-10-11 22:30:51.000000 mtpy-v2-2.0.6/LICENSE
--rw-rw-rw-   0        0        0      222 2023-10-27 22:33:39.000000 mtpy-v2-2.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7019 2024-02-28 00:52:59.515058 mtpy-v2-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5464 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.005073 mtpy-v2-2.0.6/docs/
--rw-rw-rw-   0        0        0      632 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:55.893315 mtpy-v2-2.0.6/docs/_build/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:55.893315 mtpy-v2-2.0.6/docs/_build/doctrees/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.290188 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    21794 2023-10-19 19:14:14.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_15_1.png
--rw-rw-rw-   0        0        0    83818 2023-10-19 19:14:14.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_17_1.png
--rw-rw-rw-   0        0        0    13270 2023-10-19 19:14:14.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_20_1.png
--rw-rw-rw-   0        0        0   556473 2023-10-19 19:14:14.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_24_1.png
--rw-rw-rw-   0        0        0    86441 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_16_0.png
--rw-rw-rw-   0        0        0    39672 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_18_0.png
--rw-rw-rw-   0        0        0    96197 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_21_1.png
--rw-rw-rw-   0        0        0   180921 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_23_3.png
--rw-rw-rw-   0        0        0   180550 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_27_1.png
--rw-rw-rw-   0        0        0    80615 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_34_0.png
--rw-rw-rw-   0        0        0    75375 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_35_0.png
--rw-rw-rw-   0        0        0    39992 2023-10-19 19:14:15.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_41_0.png
--rw-rw-rw-   0        0        0   532287 2023-10-19 19:14:16.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_11_1.png
--rw-rw-rw-   0        0        0   536562 2023-10-19 19:14:16.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_12_1.png
--rw-rw-rw-   0        0        0   523509 2023-10-19 19:14:16.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_6_1.png
--rw-rw-rw-   0        0        0   530346 2023-10-19 19:14:16.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_9_1.png
--rw-rw-rw-   0        0        0    45091 2023-10-19 19:14:18.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_19_1.png
--rw-rw-rw-   0        0        0    91249 2023-10-19 19:14:18.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_23_0.png
--rw-rw-rw-   0        0        0    85368 2023-10-19 19:14:19.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_35_0.png
--rw-rw-rw-   0        0        0    90587 2023-10-19 19:14:19.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_37_0.png
--rw-rw-rw-   0        0        0    73035 2023-10-19 19:14:19.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_39_0.png
--rw-rw-rw-   0        0        0    69700 2023-10-19 19:14:19.000000 mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_41_0.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:55.893315 mtpy-v2-2.0.6/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.559279 mtpy-v2-2.0.6/docs/_build/html/_images/
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.675202 mtpy-v2-2.0.6/docs/_build/html/_images/math/
--rw-rw-rw-   0        0        0      315 2023-10-19 18:28:42.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/042a6bff837cb0149f5a431572c06143bb2af48f.png
--rw-rw-rw-   0        0        0      820 2023-10-19 18:28:45.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/0e9c9f04b94469e81f5a8237d85e2d8ab567d772.png
--rw-rw-rw-   0        0        0      818 2023-10-19 18:28:41.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/130d0ff1c73599cfc5f5c9033c00bca4888f4f63.png
--rw-rw-rw-   0        0        0      300 2023-10-19 18:28:38.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/2f8284280aa5d505194fe17f815afc3ce1ac605c.png
--rw-rw-rw-   0        0        0      670 2023-10-19 18:28:44.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/38dd339f9a64ef6e087afeb98ccda3440f647ee8.png
--rw-rw-rw-   0        0        0      656 2023-10-19 18:28:39.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/6746e878cbb5de33d48e59a37cbc01d79f35841c.png
--rw-rw-rw-   0        0        0      323 2023-10-19 18:28:40.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/7b0261b200458096f1fa331b506033face2a24b7.png
--rw-rw-rw-   0        0        0      618 2023-10-19 18:28:39.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/e39affb4d959c71686d408b25e9195f1d9e4049c.png
--rw-rw-rw-   0        0        0      273 2023-10-19 18:28:43.000000 mtpy-v2-2.0.6/docs/_build/html/_images/math/e41e78a2c1d7baf6872761fe4f6252919b99220d.png
--rw-rw-rw-   0        0        0    21794 2023-10-19 18:28:25.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_15_1.png
--rw-rw-rw-   0        0        0    83818 2023-10-19 18:28:25.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_17_1.png
--rw-rw-rw-   0        0        0    13270 2023-10-19 18:28:25.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_20_1.png
--rw-rw-rw-   0        0        0   556473 2023-10-19 18:28:25.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_24_1.png
--rw-rw-rw-   0        0        0    86441 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_16_0.png
--rw-rw-rw-   0        0        0    39672 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_18_0.png
--rw-rw-rw-   0        0        0    96197 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_21_1.png
--rw-rw-rw-   0        0        0   180921 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_23_3.png
--rw-rw-rw-   0        0        0   180550 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_27_1.png
--rw-rw-rw-   0        0        0    80615 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_34_0.png
--rw-rw-rw-   0        0        0    75375 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_35_0.png
--rw-rw-rw-   0        0        0    39992 2023-10-19 18:28:26.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_41_0.png
--rw-rw-rw-   0        0        0   532287 2023-10-19 18:28:27.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_11_1.png
--rw-rw-rw-   0        0        0   536562 2023-10-19 18:28:27.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_12_1.png
--rw-rw-rw-   0        0        0   523509 2023-10-19 18:28:27.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_6_1.png
--rw-rw-rw-   0        0        0   530346 2023-10-19 18:28:27.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_9_1.png
--rw-rw-rw-   0        0        0    85368 2023-10-19 18:28:31.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_35_0.png
--rw-rw-rw-   0        0        0    90587 2023-10-19 18:28:31.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_37_0.png
--rw-rw-rw-   0        0        0    73035 2023-10-19 18:28:31.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_39_0.png
--rw-rw-rw-   0        0        0    69700 2023-10-19 18:28:31.000000 mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_41_0.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.728577 mtpy-v2-2.0.6/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-07-26 21:54:07.000000 mtpy-v2-2.0.6/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mtpy-v2-2.0.6/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0   631086 2023-10-19 17:15:16.000000 mtpy-v2-2.0.6/docs/_build/html/_static/mtpy_logo_01.png
--rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mtpy-v2-2.0.6/docs/_build/html/_static/plus.png
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:56.728577 mtpy-v2-2.0.6/docs/images/
--rw-rw-rw-   0        0        0   631086 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/images/mtpy_logo_01.png
--rwxrwxrwx   0        0        0      810 2023-10-20 14:58:41.000000 mtpy-v2-2.0.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.044859 mtpy-v2-2.0.6/docs/source/
--rw-rw-rw-   0        0        0      175 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/authors.rst
--rw-rw-rw-   0        0        0     5497 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/docs/source/conf.py
--rw-rw-rw-   0        0        0     3607 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/contributing.rst
--rw-rw-rw-   0        0        0      716 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/conventions.rst
--rw-rw-rw-   0        0        0       94 2023-10-19 19:13:30.000000 mtpy-v2-2.0.6/docs/source/history.rst
--rw-rw-rw-   0        0        0     1789 2023-10-19 21:59:08.000000 mtpy-v2-2.0.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     1741 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0       56 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/modules.rst
--rw-rw-rw-   0        0        0      404 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.analysis.rst
--rw-rw-rw-   0        0        0     1221 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.core.rst
--rw-rw-rw-   0        0        0     1119 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.core.transfer_function.rst
--rw-rw-rw-   0        0        0     1036 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.core.transfer_function.z_analysis.rst
--rw-rw-rw-   0        0        0     1682 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.imaging.mtplot_tools.rst
--rw-rw-rw-   0        0        0     3190 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.imaging.rst
--rw-rw-rw-   0        0        0     3079 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.modeling.modem.rst
--rw-rw-rw-   0        0        0     1510 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.modeling.occam2d.rst
--rw-rw-rw-   0        0        0      605 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.modeling.plots.rst
--rw-rw-rw-   0        0        0     3011 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.modeling.rst
--rw-rw-rw-   0        0        0      678 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.processing.rst
--rw-rw-rw-   0        0        0      486 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.rst
--rw-rw-rw-   0        0        0     3016 2023-10-19 18:51:22.000000 mtpy-v2-2.0.6/docs/source/mtpy.utils.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.060484 mtpy-v2-2.0.6/docs/source/scripts/
--rw-rw-rw-   0        0        0     1453 2023-10-21 00:42:28.000000 mtpy-v2-2.0.6/docs/source/scripts/example_occam2d.py
--rw-rw-rw-   0        0        0      350 2023-10-20 14:58:41.000000 mtpy-v2-2.0.6/docs/source/usage.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.091723 mtpy-v2-2.0.6/mtpy/
--rw-rw-rw-   0        0        0     1262 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/mtpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.129483 mtpy-v2-2.0.6/mtpy/analysis/
--rw-rw-rw-   0        0        0      351 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/analysis/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/analysis/residual_phase_tensor.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.214101 mtpy-v2-2.0.6/mtpy/core/
--rw-rw-rw-   0        0        0      351 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/core/__init__.py
--rw-rw-rw-   0        0        0    35378 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/mtpy/core/mt.py
--rw-rw-rw-   0        0        0    29310 2024-02-09 20:59:06.000000 mtpy-v2-2.0.6/mtpy/core/mt_collection.py
--rw-rw-rw-   0        0        0    39910 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/mtpy/core/mt_data.py
--rw-rw-rw-   0        0        0    26814 2024-01-23 23:00:30.000000 mtpy-v2-2.0.6/mtpy/core/mt_dataframe.py
--rw-rw-rw-   0        0        0    15426 2023-10-11 22:08:56.000000 mtpy-v2-2.0.6/mtpy/core/mt_location.py
--rw-rw-rw-   0        0        0    29967 2024-02-15 22:34:32.000000 mtpy-v2-2.0.6/mtpy/core/mt_stations.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.292218 mtpy-v2-2.0.6/mtpy/core/transfer_function/
--rw-rw-rw-   0        0        0      119 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/__init__.py
--rw-rw-rw-   0        0        0    28154 2024-02-06 23:41:21.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/base.py
--rw-rw-rw-   0        0        0    28705 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/pt.py
--rw-rw-rw-   0        0        0    13933 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/tipper.py
--rw-rw-rw-   0        0        0    27587 2024-01-19 20:02:42.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/z.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.367720 mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/
--rw-rw-rw-   0        0        0      317 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/__init__.py
--rw-rw-rw-   0        0        0    17548 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/distortion.py
--rw-rw-rw-   0        0        0     7953 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/niblettbostick.py
--rw-rw-rw-   0        0        0     7269 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/zinvariants.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.392109 mtpy-v2-2.0.6/mtpy/gis/
--rw-rw-rw-   0        0        0       27 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/gis/__init__.py
--rw-rw-rw-   0        0        0     1940 2024-01-24 23:03:19.000000 mtpy-v2-2.0.6/mtpy/gis/raster_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.646069 mtpy-v2-2.0.6/mtpy/imaging/
--rw-rw-rw-   0        0        0     1105 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/__init__.py
--rw-rw-rw-   0        0        0    12399 2024-01-22 23:38:15.000000 mtpy-v2-2.0.6/mtpy/imaging/mtcolors.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:57.779748 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/
--rw-rw-rw-   0        0        0      937 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/arrows.py
--rw-rw-rw-   0        0        0    26901 2023-10-11 22:08:56.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/base.py
--rw-rw-rw-   0        0        0     5730 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/ellipses.py
--rw-rw-rw-   0        0        0    10008 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/map_interpolation_tools.py
--rw-rw-rw-   0        0        0    14197 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/plot_settings.py
--rw-rw-rw-   0        0        0    13920 2024-01-04 19:33:55.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/plotters.py
--rw-rw-rw-   0        0        0     3961 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/utils.py
--rw-rw-rw-   0        0        0    18292 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_mt_response.py
--rw-rw-rw-   0        0        0    27009 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_mt_responses.py
--rw-rw-rw-   0        0        0     3366 2023-09-18 21:32:06.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_penetration_depth_1d.py
--rw-rw-rw-   0        0        0     9786 2023-10-11 22:08:56.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_penetration_depth_map.py
--rw-rw-rw-   0        0        0    28171 2024-01-12 19:24:35.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_phase_tensor_maps.py
--rw-rw-rw-   0        0        0    15425 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_phase_tensor_pseudosection.py
--rw-rw-rw-   0        0        0    14860 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_pseudosection.py
--rw-rw-rw-   0        0        0    12988 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_pt.py
--rw-rw-rw-   0        0        0    22297 2024-01-12 19:26:05.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_residual_pt_maps.py
--rw-rw-rw-   0        0        0    21716 2024-01-12 19:24:16.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_residual_pt_ps.py
--rw-rw-rw-   0        0        0    14152 2023-10-19 23:38:51.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_resphase_maps.py
--rw-rw-rw-   0        0        0    23496 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_spectrogram.py
--rw-rw-rw-   0        0        0     5701 2023-10-22 22:45:55.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_stations.py
--rw-rw-rw-   0        0        0    34312 2023-10-20 00:39:49.000000 mtpy-v2-2.0.6/mtpy/imaging/plot_strike.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.009004 mtpy-v2-2.0.6/mtpy/modeling/
--rw-rw-rw-   0        0        0       84 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/__init__.py
--rw-rw-rw-   0        0        0    14014 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/errors.py
--rw-rw-rw-   0        0        0     6090 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/gocad.py
--rw-rw-rw-   0        0        0    20311 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/mare2dem.py
--rw-rw-rw-   0        0        0    14579 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/mesh_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.208998 mtpy-v2-2.0.6/mtpy/modeling/modem/
--rw-rw-rw-   0        0        0      493 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/__init__.py
--rw-rw-rw-   0        0        0     2219 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/config.py
--rw-rw-rw-   0        0        0     5803 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/control_fwd.py
--rw-rw-rw-   0        0        0     6310 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/control_inv.py
--rw-rw-rw-   0        0        0    11249 2023-11-28 20:12:38.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/convariance.py
--rw-rw-rw-   0        0        0    46171 2024-01-30 18:22:08.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/data.py
--rw-rw-rw-   0        0        0      587 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/exception.py
--rw-rw-rw-   0        0        0    76978 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/model.py
--rw-rw-rw-   0        0        0     8204 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/residual.py
--rw-rw-rw-   0        0        0    18161 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/modem/station.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.378250 mtpy-v2-2.0.6/mtpy/modeling/occam1d/
--rw-rw-rw-   0        0        0      706 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/__init__.py
--rw-rw-rw-   0        0        0    26647 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/data.py
--rw-rw-rw-   0        0        0    15101 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/model.py
--rw-rw-rw-   0        0        0    10105 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/plot_l2.py
--rw-rw-rw-   0        0        0    30284 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/plot_response.py
--rw-rw-rw-   0        0        0     1314 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/run.py
--rw-rw-rw-   0        0        0    10150 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/startup.py
--rw-rw-rw-   0        0        0    16464 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/occam1d/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.516015 mtpy-v2-2.0.6/mtpy/modeling/occam2d/
--rw-rw-rw-   0        0        0      273 2023-10-22 23:13:02.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/__init__.py
--rw-rw-rw-   0        0        0    21958 2023-10-23 16:36:59.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/data.py
--rw-rw-rw-   0        0        0    35233 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/mesh.py
--rw-rw-rw-   0        0        0    10038 2023-10-22 22:12:08.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/model.py
--rw-rw-rw-   0        0        0    20249 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/regularization.py
--rw-rw-rw-   0        0        0     9246 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/occam2d/startup.py
--rw-rw-rw-   0        0        0    16176 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/pek1d.py
--rw-rw-rw-   0        0        0    31877 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/pek1dclasses.py
--rw-rw-rw-   0        0        0    21537 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/pek2d.py
--rw-rw-rw-   0        0        0    22561 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/pek2dforward.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.578507 mtpy-v2-2.0.6/mtpy/modeling/plots/
--rw-rw-rw-   0        0        0      107 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/plots/__init__.py
--rw-rw-rw-   0        0        0    10418 2023-10-20 18:32:35.000000 mtpy-v2-2.0.6/mtpy/modeling/plots/plot_mesh.py
--rw-rw-rw-   0        0        0    13993 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/modeling/plots/plot_modem_rms.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.616262 mtpy-v2-2.0.6/mtpy/modeling/simpeg/
--rw-rw-rw-   0        0        0      349 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/simpeg/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-11-28 20:12:38.000000 mtpy-v2-2.0.6/mtpy/modeling/simpeg/make_2d_mesh.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.663136 mtpy-v2-2.0.6/mtpy/modeling/simpeg/recipes/
--rw-rw-rw-   0        0        0      349 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/simpeg/recipes/__init__.py
--rw-rw-rw-   0        0        0    16948 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/simpeg/recipes/inversion_1d.py
--rw-rw-rw-   0        0        0   103781 2024-02-28 00:46:05.000000 mtpy-v2-2.0.6/mtpy/modeling/structured_mesh_3d.py
--rw-rw-rw-   0        0        0   100437 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/winglink.py
--rw-rw-rw-   0        0        0    19148 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/modeling/winglinktools.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.732141 mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/
--rw-rw-rw-   0        0        0      544 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/__init__.py
--rw-rw-rw-   0        0        0    20158 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/data.py
--rw-rw-rw-   0        0        0     7163 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/startup.py
--rw-rw-rw-   0        0        0     7887 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/stations.py
--rw-rw-rw-   0        0        0     1805 2022-08-07 21:11:24.000000 mtpy-v2-2.0.6/mtpy/mtpy_globals.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:58.816762 mtpy-v2-2.0.6/mtpy/processing/
--rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.6/mtpy/processing/__init__.py
--rw-rw-rw-   0        0        0    48130 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/processing/birrp.py
--rw-rw-rw-   0        0        0    15175 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/processing/filter.py
--rw-rw-rw-   0        0        0    68488 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/processing/tf.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.164054 mtpy-v2-2.0.6/mtpy/utils/
--rw-rw-rw-   0        0        0      674 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/__init__.py
--rw-rw-rw-   0        0        0    16956 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/mtpy/utils/array2raster.py
--rw-rw-rw-   0        0        0     5672 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/basemap_tools.py
--rw-rw-rw-   0        0        0    23141 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/utils/calculator.py
--rw-rw-rw-   0        0        0     8741 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/concatenate_input.py
--rw-rw-rw-   0        0        0    30898 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/configfile.py
--rw-rw-rw-   0        0        0    18864 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/convert_modem_data_to_geogrid.py
--rw-rw-rw-   0        0        0     3926 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/edi_folders.py
--rw-rw-rw-   0        0        0      989 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/exceptions.py
--rw-rw-rw-   0        0        0    57258 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/filehandling.py
--rw-rw-rw-   0        0        0    15867 2023-12-07 21:54:52.000000 mtpy-v2-2.0.6/mtpy/utils/gis_tools.py
--rw-rw-rw-   0        0        0      494 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/matplotlib_utils.py
--rw-rw-rw-   0        0        0     1975 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/mtpy/utils/mtpy_decorator.py
--rw-rw-rw-   0        0        0     4215 2022-07-06 23:26:18.000000 mtpy-v2-2.0.6/mtpy/utils/plot_rms_iterations.py
--rw-rw-rw-   0        0        0     4490 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/sensor_orientation_correction.py
--rw-rw-rw-   0        0        0    56504 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/shapefiles.py
--rw-rw-rw-   0        0        0    38353 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/mtpy/utils/shapefiles_creator.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.233057 mtpy-v2-2.0.6/mtpy_v2.egg-info/
--rw-rw-rw-   0        0        0     7019 2024-02-28 00:52:55.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8709 2024-02-28 00:52:55.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 00:52:55.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-10 00:27:03.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      112 2024-02-28 00:52:55.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-02-28 00:52:55.000000 mtpy-v2-2.0.6/mtpy_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-28 00:52:59.517056 mtpy-v2-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1857 2024-02-28 00:52:24.000000 mtpy-v2-2.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.248675 mtpy-v2-2.0.6/tests/
--rw-rw-rw-   0        0        0     1128 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.248675 mtpy-v2-2.0.6/tests/analysis/
--rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.6/tests/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.359579 mtpy-v2-2.0.6/tests/core/
--rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.6/tests/core/__init__.py
--rw-rw-rw-   0        0        0    10359 2024-01-22 23:39:53.000000 mtpy-v2-2.0.6/tests/core/test_mt.py
--rw-rw-rw-   0        0        0    21672 2024-02-09 21:02:43.000000 mtpy-v2-2.0.6/tests/core/test_mt_collection.py
--rw-rw-rw-   0        0        0     3372 2023-10-11 22:08:56.000000 mtpy-v2-2.0.6/tests/core/test_mt_dataframe.py
--rw-rw-rw-   0        0        0     6792 2023-11-10 00:26:27.000000 mtpy-v2-2.0.6/tests/core/test_mt_location.py
--rw-rw-rw-   0        0        0    31716 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/tests/core/test_mt_stations.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.417928 mtpy-v2-2.0.6/tests/core/transfer_function/
--rw-rw-rw-   0        0        0     4819 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/tests/core/transfer_function/test_pt.py
--rw-rw-rw-   0        0        0    18390 2024-01-31 22:06:45.000000 mtpy-v2-2.0.6/tests/core/transfer_function/test_tf_base.py
--rw-rw-rw-   0        0        0     6888 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/tests/core/transfer_function/test_tipper.py
--rw-rw-rw-   0        0        0    13799 2024-01-19 19:58:09.000000 mtpy-v2-2.0.6/tests/core/transfer_function/test_z.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.433559 mtpy-v2-2.0.6/tests/imaging/
--rw-rw-rw-   0        0        0        0 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/tests/imaging/__init__.py
--rw-rw-rw-   0        0        0     6882 2023-10-20 14:58:41.000000 mtpy-v2-2.0.6/tests/imaging/test_plot_mt_response.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.464800 mtpy-v2-2.0.6/tests/modeling/
--rw-rw-rw-   0        0        0     2893 2022-08-07 21:11:24.000000 mtpy-v2-2.0.6/tests/modeling/__init__.py
--rw-rw-rw-   0        0        0    11392 2023-09-18 21:32:07.000000 mtpy-v2-2.0.6/tests/modeling/test_errors.py
-drwxrwxrwx   0        0        0        0 2024-02-28 00:52:59.512064 mtpy-v2-2.0.6/tests/utils/
--rw-rw-rw-   0        0        0        0 2022-07-05 20:40:17.000000 mtpy-v2-2.0.6/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/tests/utils/test_calculator.py
--rw-rw-rw-   0        0        0    10764 2023-10-18 23:28:13.000000 mtpy-v2-2.0.6/tests/utils/test_gis_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.311214 mtpy-v2-2.0.7/
+-rw-rw-rw-   0        0        0      675 2023-11-13 20:23:07.000000 mtpy-v2-2.0.7/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-10-11 22:30:51.000000 mtpy-v2-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0      222 2023-10-27 22:33:39.000000 mtpy-v2-2.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7019 2024-04-12 22:53:56.311214 mtpy-v2-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5464 2024-04-12 22:31:20.000000 mtpy-v2-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:52.693224 mtpy-v2-2.0.7/docs/
+-rw-rw-rw-   0        0        0      632 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:52.610581 mtpy-v2-2.0.7/docs/_build/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:52.610581 mtpy-v2-2.0.7/docs/_build/doctrees/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:52.942638 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    21794 2023-10-19 19:14:14.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_15_1.png
+-rw-rw-rw-   0        0        0    83818 2023-10-19 19:14:14.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_17_1.png
+-rw-rw-rw-   0        0        0    13270 2023-10-19 19:14:14.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_20_1.png
+-rw-rw-rw-   0        0        0   556473 2023-10-19 19:14:14.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_24_1.png
+-rw-rw-rw-   0        0        0    86441 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_16_0.png
+-rw-rw-rw-   0        0        0    39672 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_18_0.png
+-rw-rw-rw-   0        0        0    96197 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_21_1.png
+-rw-rw-rw-   0        0        0   180921 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_23_3.png
+-rw-rw-rw-   0        0        0   180550 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_27_1.png
+-rw-rw-rw-   0        0        0    80615 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_34_0.png
+-rw-rw-rw-   0        0        0    75375 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_35_0.png
+-rw-rw-rw-   0        0        0    39992 2023-10-19 19:14:15.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_41_0.png
+-rw-rw-rw-   0        0        0   532287 2023-10-19 19:14:16.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_11_1.png
+-rw-rw-rw-   0        0        0   536562 2023-10-19 19:14:16.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_12_1.png
+-rw-rw-rw-   0        0        0   523509 2023-10-19 19:14:16.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_6_1.png
+-rw-rw-rw-   0        0        0   530346 2023-10-19 19:14:16.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_9_1.png
+-rw-rw-rw-   0        0        0    45091 2023-10-19 19:14:18.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_19_1.png
+-rw-rw-rw-   0        0        0    91249 2023-10-19 19:14:18.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_23_0.png
+-rw-rw-rw-   0        0        0    85368 2023-10-19 19:14:19.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_35_0.png
+-rw-rw-rw-   0        0        0    90587 2023-10-19 19:14:19.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_37_0.png
+-rw-rw-rw-   0        0        0    73035 2023-10-19 19:14:19.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_39_0.png
+-rw-rw-rw-   0        0        0    69700 2023-10-19 19:14:19.000000 mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_41_0.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:52.612603 mtpy-v2-2.0.7/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.174400 mtpy-v2-2.0.7/docs/_build/html/_images/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.290264 mtpy-v2-2.0.7/docs/_build/html/_images/math/
+-rw-rw-rw-   0        0        0      315 2023-10-19 18:28:42.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/042a6bff837cb0149f5a431572c06143bb2af48f.png
+-rw-rw-rw-   0        0        0      820 2023-10-19 18:28:45.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/0e9c9f04b94469e81f5a8237d85e2d8ab567d772.png
+-rw-rw-rw-   0        0        0      818 2023-10-19 18:28:41.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/130d0ff1c73599cfc5f5c9033c00bca4888f4f63.png
+-rw-rw-rw-   0        0        0      300 2023-10-19 18:28:38.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/2f8284280aa5d505194fe17f815afc3ce1ac605c.png
+-rw-rw-rw-   0        0        0      670 2023-10-19 18:28:44.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/38dd339f9a64ef6e087afeb98ccda3440f647ee8.png
+-rw-rw-rw-   0        0        0      656 2023-10-19 18:28:39.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/6746e878cbb5de33d48e59a37cbc01d79f35841c.png
+-rw-rw-rw-   0        0        0      323 2023-10-19 18:28:40.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/7b0261b200458096f1fa331b506033face2a24b7.png
+-rw-rw-rw-   0        0        0      618 2023-10-19 18:28:39.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/e39affb4d959c71686d408b25e9195f1d9e4049c.png
+-rw-rw-rw-   0        0        0      273 2023-10-19 18:28:43.000000 mtpy-v2-2.0.7/docs/_build/html/_images/math/e41e78a2c1d7baf6872761fe4f6252919b99220d.png
+-rw-rw-rw-   0        0        0    21794 2023-10-19 18:28:25.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_15_1.png
+-rw-rw-rw-   0        0        0    83818 2023-10-19 18:28:25.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_17_1.png
+-rw-rw-rw-   0        0        0    13270 2023-10-19 18:28:25.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_20_1.png
+-rw-rw-rw-   0        0        0   556473 2023-10-19 18:28:25.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_24_1.png
+-rw-rw-rw-   0        0        0    86441 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_16_0.png
+-rw-rw-rw-   0        0        0    39672 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_18_0.png
+-rw-rw-rw-   0        0        0    96197 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_21_1.png
+-rw-rw-rw-   0        0        0   180921 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_23_3.png
+-rw-rw-rw-   0        0        0   180550 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_27_1.png
+-rw-rw-rw-   0        0        0    80615 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_34_0.png
+-rw-rw-rw-   0        0        0    75375 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_35_0.png
+-rw-rw-rw-   0        0        0    39992 2023-10-19 18:28:26.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_41_0.png
+-rw-rw-rw-   0        0        0   532287 2023-10-19 18:28:27.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_11_1.png
+-rw-rw-rw-   0        0        0   536562 2023-10-19 18:28:27.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_12_1.png
+-rw-rw-rw-   0        0        0   523509 2023-10-19 18:28:27.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_6_1.png
+-rw-rw-rw-   0        0        0   530346 2023-10-19 18:28:27.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_9_1.png
+-rw-rw-rw-   0        0        0    85368 2023-10-19 18:28:31.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_35_0.png
+-rw-rw-rw-   0        0        0    90587 2023-10-19 18:28:31.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_37_0.png
+-rw-rw-rw-   0        0        0    73035 2023-10-19 18:28:31.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_39_0.png
+-rw-rw-rw-   0        0        0    69700 2023-10-19 18:28:31.000000 mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_41_0.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.344576 mtpy-v2-2.0.7/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-07-26 21:54:07.000000 mtpy-v2-2.0.7/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mtpy-v2-2.0.7/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0   631086 2023-10-19 17:15:16.000000 mtpy-v2-2.0.7/docs/_build/html/_static/mtpy_logo_01.png
+-rw-rw-rw-   0        0        0       90 2022-07-26 21:54:07.000000 mtpy-v2-2.0.7/docs/_build/html/_static/plus.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.359172 mtpy-v2-2.0.7/docs/images/
+-rw-rw-rw-   0        0        0   631086 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/images/mtpy_logo_01.png
+-rwxrwxrwx   0        0        0      810 2023-10-20 14:58:41.000000 mtpy-v2-2.0.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.621859 mtpy-v2-2.0.7/docs/source/
+-rw-rw-rw-   0        0        0      175 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     5497 2024-04-12 22:31:20.000000 mtpy-v2-2.0.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3607 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/contributing.rst
+-rw-rw-rw-   0        0        0      716 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/conventions.rst
+-rw-rw-rw-   0        0        0       94 2023-10-19 19:13:30.000000 mtpy-v2-2.0.7/docs/source/history.rst
+-rw-rw-rw-   0        0        0     1789 2023-10-19 21:59:08.000000 mtpy-v2-2.0.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1741 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       56 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      404 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.analysis.rst
+-rw-rw-rw-   0        0        0     1221 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.core.rst
+-rw-rw-rw-   0        0        0     1119 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.core.transfer_function.rst
+-rw-rw-rw-   0        0        0     1036 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.core.transfer_function.z_analysis.rst
+-rw-rw-rw-   0        0        0     1682 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.imaging.mtplot_tools.rst
+-rw-rw-rw-   0        0        0     3190 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.imaging.rst
+-rw-rw-rw-   0        0        0     3079 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.modeling.modem.rst
+-rw-rw-rw-   0        0        0     1510 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.modeling.occam2d.rst
+-rw-rw-rw-   0        0        0      605 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.modeling.plots.rst
+-rw-rw-rw-   0        0        0     3011 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.modeling.rst
+-rw-rw-rw-   0        0        0      678 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.processing.rst
+-rw-rw-rw-   0        0        0      486 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.rst
+-rw-rw-rw-   0        0        0     3016 2023-10-19 18:51:22.000000 mtpy-v2-2.0.7/docs/source/mtpy.utils.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.643990 mtpy-v2-2.0.7/docs/source/scripts/
+-rw-rw-rw-   0        0        0     1453 2023-10-21 00:42:28.000000 mtpy-v2-2.0.7/docs/source/scripts/example_occam2d.py
+-rw-rw-rw-   0        0        0      350 2023-10-20 14:58:41.000000 mtpy-v2-2.0.7/docs/source/usage.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.690863 mtpy-v2-2.0.7/mtpy/
+-rw-rw-rw-   0        0        0     1262 2024-04-12 22:31:20.000000 mtpy-v2-2.0.7/mtpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.722104 mtpy-v2-2.0.7/mtpy/analysis/
+-rw-rw-rw-   0        0        0      351 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/analysis/residual_phase_tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.860104 mtpy-v2-2.0.7/mtpy/core/
+-rw-rw-rw-   0        0        0      351 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/core/__init__.py
+-rw-rw-rw-   0        0        0    35378 2024-02-28 00:52:24.000000 mtpy-v2-2.0.7/mtpy/core/mt.py
+-rw-rw-rw-   0        0        0    29310 2024-02-09 20:59:06.000000 mtpy-v2-2.0.7/mtpy/core/mt_collection.py
+-rw-rw-rw-   0        0        0    39957 2024-04-12 20:54:21.000000 mtpy-v2-2.0.7/mtpy/core/mt_data.py
+-rw-rw-rw-   0        0        0    26814 2024-01-23 23:00:30.000000 mtpy-v2-2.0.7/mtpy/core/mt_dataframe.py
+-rw-rw-rw-   0        0        0    16829 2024-03-06 23:40:21.000000 mtpy-v2-2.0.7/mtpy/core/mt_location.py
+-rw-rw-rw-   0        0        0    29967 2024-02-15 22:34:32.000000 mtpy-v2-2.0.7/mtpy/core/mt_stations.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:53.967559 mtpy-v2-2.0.7/mtpy/core/transfer_function/
+-rw-rw-rw-   0        0        0      119 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/__init__.py
+-rw-rw-rw-   0        0        0    28154 2024-02-06 23:41:21.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/base.py
+-rw-rw-rw-   0        0        0    28705 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/pt.py
+-rw-rw-rw-   0        0        0    13933 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/tipper.py
+-rw-rw-rw-   0        0        0    27587 2024-01-19 20:02:42.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/z.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.020492 mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/
+-rw-rw-rw-   0        0        0      317 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/__init__.py
+-rw-rw-rw-   0        0        0    17548 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/distortion.py
+-rw-rw-rw-   0        0        0     7953 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/niblettbostick.py
+-rw-rw-rw-   0        0        0     7269 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/zinvariants.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.060253 mtpy-v2-2.0.7/mtpy/gis/
+-rw-rw-rw-   0        0        0       27 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/gis/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-01-24 23:03:19.000000 mtpy-v2-2.0.7/mtpy/gis/raster_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.360988 mtpy-v2-2.0.7/mtpy/imaging/
+-rw-rw-rw-   0        0        0     1105 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/__init__.py
+-rw-rw-rw-   0        0        0    12399 2024-01-22 23:38:15.000000 mtpy-v2-2.0.7/mtpy/imaging/mtcolors.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.506804 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/
+-rw-rw-rw-   0        0        0      937 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/__init__.py
+-rw-rw-rw-   0        0        0     1960 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/arrows.py
+-rw-rw-rw-   0        0        0    26901 2023-10-11 22:08:56.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/base.py
+-rw-rw-rw-   0        0        0     5730 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/ellipses.py
+-rw-rw-rw-   0        0        0    10008 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/map_interpolation_tools.py
+-rw-rw-rw-   0        0        0    14205 2024-04-12 21:34:37.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/plot_settings.py
+-rw-rw-rw-   0        0        0    13920 2024-01-04 19:33:55.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/plotters.py
+-rw-rw-rw-   0        0        0     3961 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/utils.py
+-rw-rw-rw-   0        0        0    18437 2024-04-12 22:28:32.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_mt_response.py
+-rw-rw-rw-   0        0        0    27009 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_mt_responses.py
+-rw-rw-rw-   0        0        0     3366 2023-09-18 21:32:06.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_penetration_depth_1d.py
+-rw-rw-rw-   0        0        0     9786 2023-10-11 22:08:56.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_penetration_depth_map.py
+-rw-rw-rw-   0        0        0    28171 2024-01-12 19:24:35.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_phase_tensor_maps.py
+-rw-rw-rw-   0        0        0    15425 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_phase_tensor_pseudosection.py
+-rw-rw-rw-   0        0        0    14860 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_pseudosection.py
+-rw-rw-rw-   0        0        0    12988 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_pt.py
+-rw-rw-rw-   0        0        0    22297 2024-01-12 19:26:05.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_residual_pt_maps.py
+-rw-rw-rw-   0        0        0    21716 2024-01-12 19:24:16.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_residual_pt_ps.py
+-rw-rw-rw-   0        0        0    14152 2023-10-19 23:38:51.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_resphase_maps.py
+-rw-rw-rw-   0        0        0    23496 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_spectrogram.py
+-rw-rw-rw-   0        0        0     5701 2023-10-22 22:45:55.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_stations.py
+-rw-rw-rw-   0        0        0    34312 2023-10-20 00:39:49.000000 mtpy-v2-2.0.7/mtpy/imaging/plot_strike.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.777317 mtpy-v2-2.0.7/mtpy/modeling/
+-rw-rw-rw-   0        0        0       84 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/__init__.py
+-rw-rw-rw-   0        0        0    14014 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/errors.py
+-rw-rw-rw-   0        0        0     6090 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/gocad.py
+-rw-rw-rw-   0        0        0    20311 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/mare2dem.py
+-rw-rw-rw-   0        0        0    14579 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/mesh_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:54.977794 mtpy-v2-2.0.7/mtpy/modeling/modem/
+-rw-rw-rw-   0        0        0      493 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/__init__.py
+-rw-rw-rw-   0        0        0     2219 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/config.py
+-rw-rw-rw-   0        0        0     5803 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/control_fwd.py
+-rw-rw-rw-   0        0        0     6310 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/control_inv.py
+-rw-rw-rw-   0        0        0    11249 2023-11-28 20:12:38.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/convariance.py
+-rw-rw-rw-   0        0        0    46171 2024-01-30 18:22:08.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/data.py
+-rw-rw-rw-   0        0        0      587 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/exception.py
+-rw-rw-rw-   0        0        0    76978 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/model.py
+-rw-rw-rw-   0        0        0     8204 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/residual.py
+-rw-rw-rw-   0        0        0    18161 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/modem/station.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.124610 mtpy-v2-2.0.7/mtpy/modeling/occam1d/
+-rw-rw-rw-   0        0        0      706 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/__init__.py
+-rw-rw-rw-   0        0        0    26647 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/data.py
+-rw-rw-rw-   0        0        0    15101 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/model.py
+-rw-rw-rw-   0        0        0    10105 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/plot_l2.py
+-rw-rw-rw-   0        0        0    30284 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/plot_response.py
+-rw-rw-rw-   0        0        0     1314 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/run.py
+-rw-rw-rw-   0        0        0    10150 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/startup.py
+-rw-rw-rw-   0        0        0    16464 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/occam1d/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.262476 mtpy-v2-2.0.7/mtpy/modeling/occam2d/
+-rw-rw-rw-   0        0        0      273 2023-10-22 23:13:02.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/__init__.py
+-rw-rw-rw-   0        0        0    21958 2023-10-23 16:36:59.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/data.py
+-rw-rw-rw-   0        0        0    35233 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/mesh.py
+-rw-rw-rw-   0        0        0    10038 2023-10-22 22:12:08.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/model.py
+-rw-rw-rw-   0        0        0    20249 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/regularization.py
+-rw-rw-rw-   0        0        0     9246 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/occam2d/startup.py
+-rw-rw-rw-   0        0        0    16176 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/pek1d.py
+-rw-rw-rw-   0        0        0    31877 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/pek1dclasses.py
+-rw-rw-rw-   0        0        0    21537 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/pek2d.py
+-rw-rw-rw-   0        0        0    22561 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/pek2dforward.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.309342 mtpy-v2-2.0.7/mtpy/modeling/plots/
+-rw-rw-rw-   0        0        0      107 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/plots/__init__.py
+-rw-rw-rw-   0        0        0    10418 2023-10-20 18:32:35.000000 mtpy-v2-2.0.7/mtpy/modeling/plots/plot_mesh.py
+-rw-rw-rw-   0        0        0    13993 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/modeling/plots/plot_modem_rms.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.362602 mtpy-v2-2.0.7/mtpy/modeling/simpeg/
+-rw-rw-rw-   0        0        0      349 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/simpeg/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-11-28 20:12:38.000000 mtpy-v2-2.0.7/mtpy/modeling/simpeg/make_2d_mesh.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.410881 mtpy-v2-2.0.7/mtpy/modeling/simpeg/recipes/
+-rw-rw-rw-   0        0        0      349 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/simpeg/recipes/__init__.py
+-rw-rw-rw-   0        0        0    16948 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/simpeg/recipes/inversion_1d.py
+-rw-rw-rw-   0        0        0   103668 2024-03-06 20:21:02.000000 mtpy-v2-2.0.7/mtpy/modeling/structured_mesh_3d.py
+-rw-rw-rw-   0        0        0   100437 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/winglink.py
+-rw-rw-rw-   0        0        0    19148 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/modeling/winglinktools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.515309 mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/
+-rw-rw-rw-   0        0        0      544 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/__init__.py
+-rw-rw-rw-   0        0        0    20158 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/data.py
+-rw-rw-rw-   0        0        0     7163 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/startup.py
+-rw-rw-rw-   0        0        0     7887 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/stations.py
+-rw-rw-rw-   0        0        0     1805 2022-08-07 21:11:24.000000 mtpy-v2-2.0.7/mtpy/mtpy_globals.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.594223 mtpy-v2-2.0.7/mtpy/processing/
+-rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.7/mtpy/processing/__init__.py
+-rw-rw-rw-   0        0        0    48130 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/processing/birrp.py
+-rw-rw-rw-   0        0        0    15175 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/processing/filter.py
+-rw-rw-rw-   0        0        0    68488 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/processing/tf.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.926215 mtpy-v2-2.0.7/mtpy/utils/
+-rw-rw-rw-   0        0        0      674 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    16956 2023-11-10 00:26:27.000000 mtpy-v2-2.0.7/mtpy/utils/array2raster.py
+-rw-rw-rw-   0        0        0     5672 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/basemap_tools.py
+-rw-rw-rw-   0        0        0    23141 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/utils/calculator.py
+-rw-rw-rw-   0        0        0     8741 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/concatenate_input.py
+-rw-rw-rw-   0        0        0    30898 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/configfile.py
+-rw-rw-rw-   0        0        0    18864 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/convert_modem_data_to_geogrid.py
+-rw-rw-rw-   0        0        0     3926 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/edi_folders.py
+-rw-rw-rw-   0        0        0      989 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/exceptions.py
+-rw-rw-rw-   0        0        0    57258 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/filehandling.py
+-rw-rw-rw-   0        0        0    15867 2023-12-07 21:54:52.000000 mtpy-v2-2.0.7/mtpy/utils/gis_tools.py
+-rw-rw-rw-   0        0        0      494 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/matplotlib_utils.py
+-rw-rw-rw-   0        0        0     1975 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/mtpy/utils/mtpy_decorator.py
+-rw-rw-rw-   0        0        0     4215 2022-07-06 23:26:18.000000 mtpy-v2-2.0.7/mtpy/utils/plot_rms_iterations.py
+-rw-rw-rw-   0        0        0     4490 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/sensor_orientation_correction.py
+-rw-rw-rw-   0        0        0    56504 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/shapefiles.py
+-rw-rw-rw-   0        0        0    38353 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/mtpy/utils/shapefiles_creator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:55.995222 mtpy-v2-2.0.7/mtpy_v2.egg-info/
+-rw-rw-rw-   0        0        0     7019 2024-04-12 22:53:51.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8709 2024-04-12 22:53:52.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 22:53:51.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 22:53:51.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      112 2024-04-12 22:53:51.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-12 22:53:51.000000 mtpy-v2-2.0.7/mtpy_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 22:53:56.311214 mtpy-v2-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1857 2024-04-12 22:31:20.000000 mtpy-v2-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.010843 mtpy-v2-2.0.7/tests/
+-rw-rw-rw-   0        0        0     1128 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.010843 mtpy-v2-2.0.7/tests/analysis/
+-rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.7/tests/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.105229 mtpy-v2-2.0.7/tests/core/
+-rw-rw-rw-   0        0        0        0 2022-07-05 20:40:16.000000 mtpy-v2-2.0.7/tests/core/__init__.py
+-rw-rw-rw-   0        0        0    10359 2024-01-22 23:39:53.000000 mtpy-v2-2.0.7/tests/core/test_mt.py
+-rw-rw-rw-   0        0        0    21672 2024-02-09 21:02:43.000000 mtpy-v2-2.0.7/tests/core/test_mt_collection.py
+-rw-rw-rw-   0        0        0     3372 2023-10-11 22:08:56.000000 mtpy-v2-2.0.7/tests/core/test_mt_dataframe.py
+-rw-rw-rw-   0        0        0     7219 2024-04-12 22:41:54.000000 mtpy-v2-2.0.7/tests/core/test_mt_location.py
+-rw-rw-rw-   0        0        0    31716 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/tests/core/test_mt_stations.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.179727 mtpy-v2-2.0.7/tests/core/transfer_function/
+-rw-rw-rw-   0        0        0     4819 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/tests/core/transfer_function/test_pt.py
+-rw-rw-rw-   0        0        0    18390 2024-01-31 22:06:45.000000 mtpy-v2-2.0.7/tests/core/transfer_function/test_tf_base.py
+-rw-rw-rw-   0        0        0     6888 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/tests/core/transfer_function/test_tipper.py
+-rw-rw-rw-   0        0        0    13799 2024-01-19 19:58:09.000000 mtpy-v2-2.0.7/tests/core/transfer_function/test_z.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.210969 mtpy-v2-2.0.7/tests/imaging/
+-rw-rw-rw-   0        0        0        0 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/tests/imaging/__init__.py
+-rw-rw-rw-   0        0        0     6882 2023-10-20 14:58:41.000000 mtpy-v2-2.0.7/tests/imaging/test_plot_mt_response.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.248720 mtpy-v2-2.0.7/tests/modeling/
+-rw-rw-rw-   0        0        0     2893 2022-08-07 21:11:24.000000 mtpy-v2-2.0.7/tests/modeling/__init__.py
+-rw-rw-rw-   0        0        0    11392 2023-09-18 21:32:07.000000 mtpy-v2-2.0.7/tests/modeling/test_errors.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:53:56.295592 mtpy-v2-2.0.7/tests/utils/
+-rw-rw-rw-   0        0        0        0 2022-07-05 20:40:17.000000 mtpy-v2-2.0.7/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/tests/utils/test_calculator.py
+-rw-rw-rw-   0        0        0    10764 2023-10-18 23:28:13.000000 mtpy-v2-2.0.7/tests/utils/test_gis_tools.py
```

### Comparing `mtpy-v2-2.0.6/HISTORY.rst` & `mtpy-v2-2.0.7/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/LICENSE` & `mtpy-v2-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/PKG-INFO` & `mtpy-v2-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtpy-v2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python toolkit for standard magnetotelluric data processing.
 Home-page: https://github.com/MTgeophysics/mtpy-v2
 Author: Jared Peacock, Alison Kirkby, Fei Zhang, Rakib Hassan, Lars Krieger, Stephan Thiel
 Author-email: jpeacock@usgs.gov
 License: MIT
 Keywords: magnetotellurics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,15 +25,15 @@
 [![PyPi version](https://img.shields.io/pypi/v/mtpy-v2.svg)](https://pypi.python.org/pypi/mtpy-v2)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mtpy-v2.svg)](https://anaconda.org/conda-forge/mtpy-v2)
 [![codecov](https://codecov.io/gh/MTgeophysics/mtpy-v2/graph/badge.svg?token=TQPFBFMYDQ)](https://codecov.io/gh/MTgeophysics/mtpy-v2)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/mtpy-v2/badge/?version=latest)](https://mtpy-v2.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MTgeophysics/mtpy-v2/main)
 
-## Version 2.0.6
+## Version 2.0.7
 
 # Description
  
 `mtpy` provides tools for working with magnetotelluric (MT) data.  MTpy-v2 is an updated version of [mtpy](https://github.com/MTgeophysics/mtpy). Many things have changed under the hood and usage is different from mtpy v1. The main difference is that there is a central data type that can hold transfer functions and then read/write to your modeling program, plot, and analyze your data.  No longer will you need a directory of EDI files and then read them in everytime you want to do something.  You only need to build a project once and save it to an MTH5 file and you are ready to go. All metadata uses [mt-metadata](https://github.com/kujaku11/mt-metadata).
 
 # Installation
```

### Comparing `mtpy-v2-2.0.6/README.md` & `mtpy-v2-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPi version](https://img.shields.io/pypi/v/mtpy-v2.svg)](https://pypi.python.org/pypi/mtpy-v2)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mtpy-v2.svg)](https://anaconda.org/conda-forge/mtpy-v2)
 [![codecov](https://codecov.io/gh/MTgeophysics/mtpy-v2/graph/badge.svg?token=TQPFBFMYDQ)](https://codecov.io/gh/MTgeophysics/mtpy-v2)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/mtpy-v2/badge/?version=latest)](https://mtpy-v2.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MTgeophysics/mtpy-v2/main)
 
-## Version 2.0.6
+## Version 2.0.7
 
 # Description
  
 `mtpy` provides tools for working with magnetotelluric (MT) data.  MTpy-v2 is an updated version of [mtpy](https://github.com/MTgeophysics/mtpy). Many things have changed under the hood and usage is different from mtpy v1. The main difference is that there is a central data type that can hold transfer functions and then read/write to your modeling program, plot, and analyze your data.  No longer will you need a directory of EDI files and then read them in everytime you want to do something.  You only need to build a project once and save it to an MTH5 file and you are ready to go. All metadata uses [mt-metadata](https://github.com/kujaku11/mt-metadata).
 
 # Installation
```

### Comparing `mtpy-v2-2.0.6/docs/Makefile` & `mtpy-v2-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_15_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_15_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_17_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_17_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_20_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_20_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_24_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_1_making_MTCollection_24_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_16_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_16_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_18_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_18_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_21_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_21_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_23_3.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_23_3.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_27_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_27_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_34_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_34_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_35_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_35_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_41_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_2_MTData_profile_41_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_11_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_11_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_12_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_12_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_6_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_6_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_9_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_3_MTData_grid_9_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_19_1.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_19_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_23_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_5_make_model_files_23_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_35_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_35_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_37_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_37_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_39_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_39_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/doctrees/nbsphinx/notebooks_mt_object_41_0.png` & `mtpy-v2-2.0.7/docs/_build/doctrees/nbsphinx/notebooks_mt_object_41_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/math/0e9c9f04b94469e81f5a8237d85e2d8ab567d772.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/math/0e9c9f04b94469e81f5a8237d85e2d8ab567d772.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/math/130d0ff1c73599cfc5f5c9033c00bca4888f4f63.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/math/130d0ff1c73599cfc5f5c9033c00bca4888f4f63.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/math/38dd339f9a64ef6e087afeb98ccda3440f647ee8.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/math/38dd339f9a64ef6e087afeb98ccda3440f647ee8.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/math/6746e878cbb5de33d48e59a37cbc01d79f35841c.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/math/6746e878cbb5de33d48e59a37cbc01d79f35841c.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/math/e39affb4d959c71686d408b25e9195f1d9e4049c.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/math/e39affb4d959c71686d408b25e9195f1d9e4049c.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_15_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_15_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_17_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_17_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_20_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_20_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_1_making_MTCollection_24_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_1_making_MTCollection_24_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_16_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_16_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_18_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_18_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_21_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_21_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_23_3.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_23_3.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_27_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_27_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_34_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_34_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_35_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_35_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_2_MTData_profile_41_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_2_MTData_profile_41_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_11_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_11_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_12_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_12_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_6_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_6_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_3_MTData_grid_9_1.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_3_MTData_grid_9_1.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_35_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_35_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_37_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_37_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_39_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_39_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_images/notebooks_mt_object_41_0.png` & `mtpy-v2-2.0.7/docs/_build/html/_images/notebooks_mt_object_41_0.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/_build/html/_static/mtpy_logo_01.png` & `mtpy-v2-2.0.7/docs/_build/html/_static/mtpy_logo_01.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/images/mtpy_logo_01.png` & `mtpy-v2-2.0.7/docs/images/mtpy_logo_01.png`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/make.bat` & `mtpy-v2-2.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/conf.py` & `mtpy-v2-2.0.7/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "2.0.6"
+version = "2.0.7"
 # The full version, including alpha/beta/rc tags.
-release = "2.0.6"
+release = "2.0.7"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `mtpy-v2-2.0.6/docs/source/contributing.rst` & `mtpy-v2-2.0.7/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/conventions.rst` & `mtpy-v2-2.0.7/docs/source/conventions.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/index.rst` & `mtpy-v2-2.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/installation.rst` & `mtpy-v2-2.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.core.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.core.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.core.transfer_function.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.core.transfer_function.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.core.transfer_function.z_analysis.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.core.transfer_function.z_analysis.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.imaging.mtplot_tools.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.imaging.mtplot_tools.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.imaging.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.imaging.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.modeling.modem.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.modeling.modem.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.modeling.occam2d.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.modeling.occam2d.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.modeling.plots.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.modeling.plots.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.modeling.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.modeling.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.processing.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.processing.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/mtpy.utils.rst` & `mtpy-v2-2.0.7/docs/source/mtpy.utils.rst`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/docs/source/scripts/example_occam2d.py` & `mtpy-v2-2.0.7/docs/source/scripts/example_occam2d.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/__init__.py` & `mtpy-v2-2.0.7/mtpy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # common objects
 from mtpy.core.mt import MT
 from mtpy.core.mt_data import MTData
 from mtpy.core.mt_collection import MTCollection
 from mtpy.imaging.mtcolors import MT_CMAP_DICT, register_cmaps
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 __all__ = ["MT", "MTData", "MTCollection"]
 
 # =============================================================================
 # Initiate loggers
 # =============================================================================
 config = {
     "handlers": [
```

### Comparing `mtpy-v2-2.0.6/mtpy/analysis/residual_phase_tensor.py` & `mtpy-v2-2.0.7/mtpy/analysis/residual_phase_tensor.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt.py` & `mtpy-v2-2.0.7/mtpy/core/mt.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt_collection.py` & `mtpy-v2-2.0.7/mtpy/core/mt_collection.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt_data.py` & `mtpy-v2-2.0.7/mtpy/core/mt_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,17 @@
                 self.update(
                     {
                         f"{new_mt_obj.survey_metadata.id}.{new_mt_obj.station}": new_mt_obj
                     }
                 )
 
             else:
-                mt_data.add_station(new_mt_obj, compute_relative_location=False)
+                mt_data.add_station(
+                    new_mt_obj, compute_relative_location=False
+                )
 
         if not inplace:
             return mt_data
 
     def rotate(self, rotation_angle, inplace=True):
         """
         rotate the data by the given angle assuming positive clockwise with
@@ -566,15 +568,17 @@
 
         if not inplace:
             mt_data = self.clone_empty
         for mt_obj in self.values():
             if not inplace:
                 rot_mt_obj = mt_obj.copy()
                 rot_mt_obj.rotation_angle = rotation_angle
-                mt_data.add_station(rot_mt_obj, compute_relative_location=False)
+                mt_data.add_station(
+                    rot_mt_obj, compute_relative_location=False
+                )
             else:
                 mt_obj.rotation_angle = rotation_angle
 
         if not inplace:
             return mt_data
 
     def get_profile(self, x1, y1, x2, y2, radius):
@@ -664,16 +668,20 @@
             self.t_model_error.error_value = t_error_value
         if t_error_type is not None:
             self.t_model_error.error_type = t_error_type
         if t_floor is not None:
             self.t_model_error.floor = t_floor
 
         for mt_obj in self.values():
-            mt_obj.compute_model_z_errors(**self.z_model_error.error_parameters)
-            mt_obj.compute_model_t_errors(**self.t_model_error.error_parameters)
+            mt_obj.compute_model_z_errors(
+                **self.z_model_error.error_parameters
+            )
+            mt_obj.compute_model_t_errors(
+                **self.t_model_error.error_parameters
+            )
 
     def get_nearby_stations(self, station_key, radius, radius_units="m"):
         """
         get stations close to a given station
 
         :param station_key: DESCRIPTION
         :type station_key: TYPE
@@ -877,15 +885,15 @@
         modem_data.z_model_error = self.z_model_error
         modem_data.t_model_error = self.t_model_error
         if data_filename is not None:
             modem_data.write_data_file(file_name=data_filename)
 
         return modem_data
 
-    def from_modem_data(self, data_filename, file_type="data", **kwargs):
+    def from_modem_data(self, data_filename, survey="data", **kwargs):
         """
 
         :param data_filename: DESCRIPTION
         :type data_filename: TYPE
         :param file_type: DESCRIPTION, defaults to "data"
         :type file_type: TYPE, optional
         :param **kwargs: DESCRIPTION
@@ -895,34 +903,34 @@
 
         """
 
         self.logger.warning(
             "'from_modem_data' will be deprecated in future versions, use 'from_modem'"
         )
 
-        self.from_modem(data_filename, file_type=file_type, **kwargs)
+        self.from_modem(data_filename, survey=survey, **kwargs)
 
-    def from_modem(self, data_filename, file_type="data", **kwargs):
+    def from_modem(self, data_filename, survey="data", **kwargs):
         """
         read in a modem data file
 
         :param data_filename: DESCRIPTION
         :type data_filename: TYPE
         :param **kwargs: DESCRIPTION
         :type **kwargs: TYPE
         :return: DESCRIPTION
         :rtype: TYPE
 
         """
         modem_data = Data(**kwargs)
         mdf = modem_data.read_data_file(data_filename)
-        if file_type in ["data"]:
-            mdf.dataframe["survey"] = "data"
-        elif file_type in ["response", "model"]:
-            mdf.dataframe["survey"] = "model"
+
+        # set survey name to something useful
+        mdf.dataframe["survey"] = survey
+
         self.from_dataframe(mdf.dataframe)
         self.z_model_error = ModelErrors(
             mode="impedance", **modem_data.z_model_error.error_parameters
         )
         self.t_model_error = ModelErrors(
             mode="tipper", **modem_data.t_model_error.error_parameters
         )
```

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt_dataframe.py` & `mtpy-v2-2.0.7/mtpy/core/mt_dataframe.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt_location.py` & `mtpy-v2-2.0.7/mtpy/core/mt_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # =============================================================================
 # Imports
 # =============================================================================
 from copy import deepcopy
 from pyproj import CRS
 import numpy as np
 from loguru import logger
+import json
 
 from mtpy.utils.gis_tools import project_point
 
 from mt_metadata.transfer_functions.tf import Station, Survey, Run
 from mt_metadata.transfer_functions.io.tools import get_nm_elev
 
 # =============================================================================
@@ -26,15 +27,14 @@
 class MTLocation:
     """
     Location for a MT site or point measurement
 
     """
 
     def __init__(self, survey_metadata=None, **kwargs):
-
         self.logger = logger
         if survey_metadata is None:
             self._survey_metadata = self._initiate_metadata()
         else:
             self._survey_metadata = self._validate_metadata(survey_metadata)
 
         self._east = 0
@@ -252,19 +252,15 @@
     def utm_crs(self, value):
         if value in [None, "None", "none", "null", ""]:
             return
 
         new_crs = CRS.from_user_input(value)
         if value != self._utm_crs:
             # reproject easting, northing to new zone
-            if (
-                self._utm_crs is not None
-                and self.east != 0
-                and self.north != 0
-            ):
+            if self._utm_crs is not None and self.east != 0 and self.north != 0:
                 self._east, self._north = project_point(
                     self.east, self.north, self._utm_crs, new_crs
                 )
 
             if (
                 self.datum_crs is not None
                 and self.east != 0
@@ -479,7 +475,56 @@
         elev = get_nm_elev(self.latitude, self.longitude)
         if elev != 0:
             self.elevation = elev
         else:
             self.logger.warning(
                 "Could not get elevation data, not setting elevation"
             )
+
+    def to_json(self, filename):
+        """
+        write out information to a json file
+
+        :param filename: DESCRIPTION
+        :type filename: TYPE
+        :return: DESCRIPTION
+        :rtype: TYPE
+
+        """
+
+        js_dict = {
+            "latitude": self.latitude,
+            "longitude": self.longitude,
+            "elevation": self.elevation,
+            "north": self.north,
+            "east": self.east,
+            "model_east": self.model_east,
+            "model_north": self.model_north,
+            "model_elevation": self.model_elevation,
+            "datum_crs": self.datum_crs.to_json_dict(),
+            "utm_crs": self.utm_crs.to_json_dict(),
+        }
+        with open(filename, "w") as fid:
+            json.dump(js_dict, fid)
+
+    def from_json(self, filename):
+        """
+        read in json formatted location
+
+        :param filename: DESCRIPTION
+        :type filename: TYPE
+        :return: DESCRIPTION
+        :rtype: TYPE
+
+        """
+
+        with open(filename, "r") as fid:
+            js_dict = json.load(fid)
+
+        for key, value in js_dict.items():
+            if key in ["datum_crs", "utm_crs"]:
+                if isinstance(value, dict):
+                    setattr(self, key, CRS.from_json_dict(value))
+                else:
+                    setattr(self, key, CRS.from_user_input(value))
+            else:
+                setattr(self, key, value)
```

### Comparing `mtpy-v2-2.0.6/mtpy/core/mt_stations.py` & `mtpy-v2-2.0.7/mtpy/core/mt_stations.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/base.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/base.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/pt.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/pt.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/tipper.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/tipper.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/z.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/z.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/distortion.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/distortion.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/niblettbostick.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/niblettbostick.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/core/transfer_function/z_analysis/zinvariants.py` & `mtpy-v2-2.0.7/mtpy/core/transfer_function/z_analysis/zinvariants.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/gis/raster_tools.py` & `mtpy-v2-2.0.7/mtpy/gis/raster_tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/__init__.py` & `mtpy-v2-2.0.7/mtpy/imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtcolors.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtcolors.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/__init__.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/arrows.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/arrows.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/base.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/base.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/ellipses.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/ellipses.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/map_interpolation_tools.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/map_interpolation_tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/plot_settings.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/plot_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import matplotlib.colors as colors
 import matplotlib.colorbar as mcb
 
 from . import MTEllipse, MTArrows
 
 import mtpy.imaging.mtcolors as mtcl
 
+
 # =============================================================================
 # ==============================================================================
 # Plot settings
 # ==============================================================================
 class PlotSettings(MTArrows, MTEllipse):
     """
     Hold all the plot settings that one might need
@@ -269,16 +270,16 @@
                 )
                 if ph_min > 0:
                     ph_min = 0
                 else:
                     ph_min = round(ph_min / 5) * 5
                 ph_max = max(
                     [
-                        np.nanmax(phase[:, 0, 1]),
-                        np.nanmax(phase[:, 1, 0] + 180),
+                        np.nanmax(phase[nz_xy, 0, 1]),
+                        np.nanmax(phase[nz_yx, 1, 0] + 180),
                     ]
                 )
                 if ph_max < 91:
                     ph_max = 89.9
                 else:
                     ph_max = round(ph_max / 5) * 5
                 return (ph_min, ph_max)
@@ -369,15 +370,14 @@
         }
 
     @property
     def font_dict(self):
         return {"size": self.font_size + 2, "weight": self.font_weight}
 
     def make_pt_cb(self, ax):
-
         cmap = mtcl.cmapdict[self.ellipse_cmap]
         if "seg" in self.ellipse_cmap:
             # normalize the colors
             norms = colors.BoundaryNorm(self.ellipse_cmap_bounds, cmap.N)
 
             # make the colorbar
             cb = mcb.Colorbar(
```

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/plotters.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/plotters.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/mtplot_tools/utils.py` & `mtpy-v2-2.0.7/mtpy/imaging/mtplot_tools/utils.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_mt_response.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_mt_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 
     @rotation_angle.setter
     def rotation_angle(self, theta_r):
         """
         only a single value is allowed
         """
         if not theta_r == 0:
-
             self.Z.rotate(theta_r)
             self.Tipper.rotate(theta_r)
             self.pt.rotate(theta_r)
 
             self._rotation_angle += theta_r
         else:
             self._rotation_angle = theta_r
@@ -245,29 +244,26 @@
             # Removed aspect = "equal" for now, it flows better, if you want
             # a detailed analysis look at plot pt
             self.axpt = self.fig.add_subplot(gs_aux[pdict["pt"], :])
             self.axpt.yaxis.set_label_coords(label_coords[0], label_coords[1])
         return label_coords
 
     def _plot_resistivity(self, axr, period, z_obj, mode="od"):
-
         if mode == "od":
             comps = ["xy", "yx"]
             props = [
                 self.xy_error_bar_properties,
                 self.yx_error_bar_properties,
             ]
         elif mode == "d":
             comps = ["xx", "yy"]
             props = [
                 self.xy_error_bar_properties,
                 self.yx_error_bar_properties,
             ]
-        res_limits = self.set_resistivity_limits(z_obj.resistivity, mode=mode)
-        x_limits = self.set_period_limits(period)
 
         eb_list = []
         label_list = []
         for comp, prop in zip(comps, props):
             ebax = plot_resistivity(
                 axr,
                 period,
@@ -278,16 +274,16 @@
             eb_list.append(ebax)
             label_list.append(f"$Z_{'{'}{comp}{'}'}$")
         # --> set axes properties
         plt.setp(axr.get_xticklabels(), visible=False)
 
         axr.set_yscale("log", nonpositive="clip")
         axr.set_xscale("log", nonpositive="clip")
-        axr.set_xlim(x_limits)
-        axr.set_ylim(res_limits)
+        axr.set_xlim(self.x_limits)
+        axr.set_ylim(self.res_limits)
         axr.grid(
             True, alpha=0.25, which="both", color=(0.25, 0.25, 0.25), lw=0.25
         )
 
         if mode == "od":
             axr.set_ylabel(
                 r"App. Res. ($\mathbf{\Omega \cdot m}$)",
@@ -314,16 +310,16 @@
             ]
         elif mode == "d":
             comps = ["xx", "yy"]
             props = [
                 self.xy_error_bar_properties,
                 self.yx_error_bar_properties,
             ]
-        phase_limits = self.set_phase_limits(z_obj.phase, mode=mode)
 
+        phase_limits = self.set_phase_limits(z_obj.phase, mode=mode)
         for comp, prop in zip(comps, props):
             if comp == "yx":
                 plot_phase(
                     axp,
                     period,
                     getattr(z_obj, f"phase_{comp}"),
                     getattr(z_obj, f"phase_{self._error_str}_{comp}"),
@@ -381,17 +377,20 @@
             markerscale=1,
             borderaxespad=0.01,
             labelspacing=0.07,
             handletextpad=0.2,
             borderpad=0.02,
         )
 
-        self.axr.set_ylim(
-            self.set_resistivity_limits(self.Z.resistivity, mode="det")
-        )
+        if self.res_limits is None:
+            self.axr.set_ylim(
+                self.set_resistivity_limits(self.Z.resistivity, mode="det")
+            )
+        else:
+            self.axr.set_ylim(self.res_limits)
 
     def _plot_tipper(self):
         if self.Tipper is not None:
             self.axt, _, _ = plot_tipper_lateral(
                 self.axt,
                 self.Tipper,
                 self.plot_tipper,
@@ -402,33 +401,36 @@
             if self.plot_tipper.find("y") >= 0:
                 self.axt.set_xlabel("Period (s)", fontdict=self.font_dict)
                 # need to reset the x_limits caouse they get reset when calling
                 # set_ticks for some reason
                 self.axt.set_xlim(
                     np.log10(self.x_limits[0]), np.log10(self.x_limits[1])
                 )
-
+                if self.tipper_limits is not None:
+                    self.axt.set_ylim(self.tipper_limits)
                 self.axt.yaxis.set_major_locator(MultipleLocator(0.2))
                 self.axt.yaxis.set_minor_locator(MultipleLocator(0.1))
                 self.axt.set_xlabel("Period (s)", fontdict=self.font_dict)
                 self.axt.set_ylabel("Tipper", fontdict=self.font_dict)
 
                 # set th xaxis tick labels to invisible
                 if self.plot_pt:
                     plt.setp(self.axt.xaxis.get_ticklabels(), visible=False)
                     self.axt.set_xlabel("")
 
     def _plot_pt(self):
         # ----plot phase tensor ellipse---------------------------------------
         if self.plot_pt:
-
             color_array = self.get_pt_color_array(self.pt)
 
             # -------------plot ellipses-----------------------------------
-            self.cbax, self.cbpt, = plot_pt_lateral(
+            (
+                self.cbax,
+                self.cbpt,
+            ) = plot_pt_lateral(
                 self.axpt,
                 self.pt,
                 color_array,
                 self.ellipse_properties,
                 fig=self.fig,
             )
```

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_mt_responses.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_mt_responses.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_penetration_depth_1d.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_penetration_depth_1d.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_penetration_depth_map.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_penetration_depth_map.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_phase_tensor_maps.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_phase_tensor_maps.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_phase_tensor_pseudosection.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_phase_tensor_pseudosection.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_pseudosection.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_pseudosection.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_pt.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_pt.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_residual_pt_maps.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_residual_pt_maps.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_residual_pt_ps.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_residual_pt_ps.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_resphase_maps.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_resphase_maps.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_spectrogram.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_spectrogram.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_stations.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_stations.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/imaging/plot_strike.py` & `mtpy-v2-2.0.7/mtpy/imaging/plot_strike.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/errors.py` & `mtpy-v2-2.0.7/mtpy/modeling/errors.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/gocad.py` & `mtpy-v2-2.0.7/mtpy/modeling/gocad.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/mare2dem.py` & `mtpy-v2-2.0.7/mtpy/modeling/mare2dem.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/mesh_tools.py` & `mtpy-v2-2.0.7/mtpy/modeling/mesh_tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/config.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/config.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/control_fwd.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/control_fwd.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/control_inv.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/control_inv.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/convariance.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/convariance.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/data.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/data.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/exception.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/exception.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/model.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/model.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/residual.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/residual.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/modem/station.py` & `mtpy-v2-2.0.7/mtpy/modeling/modem/station.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/__init__.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/data.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/data.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/model.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/model.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/plot_l2.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/plot_l2.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/plot_response.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/plot_response.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/run.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/run.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/startup.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/startup.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam1d/tools.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam1d/tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam2d/data.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam2d/data.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam2d/mesh.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam2d/mesh.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam2d/model.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam2d/model.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam2d/regularization.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam2d/regularization.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/occam2d/startup.py` & `mtpy-v2-2.0.7/mtpy/modeling/occam2d/startup.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/pek1d.py` & `mtpy-v2-2.0.7/mtpy/modeling/pek1d.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/pek1dclasses.py` & `mtpy-v2-2.0.7/mtpy/modeling/pek1dclasses.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/pek2d.py` & `mtpy-v2-2.0.7/mtpy/modeling/pek2d.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/pek2dforward.py` & `mtpy-v2-2.0.7/mtpy/modeling/pek2dforward.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/plots/plot_mesh.py` & `mtpy-v2-2.0.7/mtpy/modeling/plots/plot_mesh.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/plots/plot_modem_rms.py` & `mtpy-v2-2.0.7/mtpy/modeling/plots/plot_modem_rms.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/simpeg/make_2d_mesh.py` & `mtpy-v2-2.0.7/mtpy/modeling/simpeg/make_2d_mesh.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/simpeg/recipes/inversion_1d.py` & `mtpy-v2-2.0.7/mtpy/modeling/simpeg/recipes/inversion_1d.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/structured_mesh_3d.py` & `mtpy-v2-2.0.7/mtpy/modeling/structured_mesh_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,28 +568,27 @@
             except IndexError:
                 continue
 
         # --> need to make sure none of the stations lie on the nodes
         for s_north in sorted(self.station_locations.model_north):
             try:
                 node_index = np.where(
-                    abs(s_north - self.grid_north)
-                    < 0.02 * self.cell_size_north
+                    abs(s_north - self.grid_north) < 0.02 * self.cell_size_north
                 )[0][0]
                 if s_north - self.grid_north[node_index] > 0:
                     self.grid_north[node_index] -= 0.02 * self.cell_size_north
                 elif s_north - self.grid_north[node_index] < 0:
                     self.grid_north[node_index] += 0.02 * self.cell_size_north
             except IndexError:
                 continue
 
         if self.z_mesh_method == "custom":
             if self.grid_z is None:
                 self.z_mesh_method = "default"
-                self._logger.warn(
+                self._logger.warning(
                     "No grid_z provided, creating new z mesh using default method"
                 )
 
         if self.z_mesh_method == "custom":
             self.nodes_z, z_grid = (
                 self.grid_z[1:] - self.grid_z[:-1],
                 self.grid_z,
@@ -598,17 +597,15 @@
             self.nodes_z, z_grid = self.make_z_mesh()
         else:
             raise NameError(
                 f'Z mesh method "{self.z_mesh_method}" is not supported'
             )
 
         # compute grid center
-        center_east = np.round(
-            self.grid_east.min() - self.grid_east.mean(), -1
-        )
+        center_east = np.round(self.grid_east.min() - self.grid_east.mean(), -1)
         center_north = np.round(
             self.grid_north.min() - self.grid_north.mean(), -1
         )
         center_z = 0
 
         # this is the value to the lower left corner from the center.
         self.grid_center = np.array([center_north, center_east, center_z])
@@ -688,15 +685,15 @@
         if layer_thickness is None:
             layer_thickness = self.z1_layer
         if np.iterable(layer_thickness):
             add_layers = np.insert(np.cumsum(layer_thickness), 0, 0)[:-1]
             layer_thickness = layer_thickness[-1]
 
             if n_add_layers != len(add_layers):
-                self._logger.warn(
+                self._logger.warning(
                     "Updating number of layers to reflect the length of the layer thickness array"
                 )
             n_add_layers = len(add_layers)
         else:
             add_layers = np.arange(
                 0, n_add_layers * layer_thickness, layer_thickness
             )
@@ -822,16 +819,15 @@
             "".join([f"{abs(znode):>12.3f}" for znode in self.nodes_z])
         )
 
         # write the resistivity in log e format
         if self.res_scale.lower() == "loge":
             write_res_model = np.log(self.res_model[::-1, :, :])
         elif (
-            self.res_scale.lower() == "log"
-            or self.res_scale.lower() == "log10"
+            self.res_scale.lower() == "log" or self.res_scale.lower() == "log10"
         ):
             write_res_model = np.log10(self.res_model[::-1, :, :])
         elif self.res_scale.lower() == "linear":
             write_res_model = self.res_model[::-1, :, :]
         else:
             raise ValueError(
                 f'resistivity scale "{self.res_scale}" is not supported.'
@@ -941,17 +937,15 @@
         # get nodes
         self.nodes_north = np.array(
             [float(nn) for nn in ilines[2].strip().split()]
         )
         self.nodes_east = np.array(
             [float(nn) for nn in ilines[3].strip().split()]
         )
-        self.nodes_z = np.array(
-            [float(nn) for nn in ilines[4].strip().split()]
-        )
+        self.nodes_z = np.array([float(nn) for nn in ilines[4].strip().split()])
 
         self.res_model = np.zeros((n_north, n_east, n_z))
 
         # get model
         count_z = 0
         line_index = 6
         count_e = 0
@@ -1627,18 +1621,18 @@
         else:
             raise ValueError(
                 "'topography_file', 'surface' or "
                 + "topography_array must be provided"
             )
 
         if self.n_air_layers is None or self.n_air_layers == 0:
-            self._logger.warn(
+            self._logger.warning(
                 "No air layers specified, so will not add air/topography !!!"
             )
-            self._logger.warn(
+            self._logger.warning(
                 "Only bathymetry will be added below according to the topofile: sea-water low resistivity!!!"
             )
 
         elif (
             self.n_air_layers > 0
         ):  # FZ: new logic, add equal blocksize air layers on top of the simple flat-earth grid
             # get grid centre
@@ -1675,17 +1669,15 @@
                 # make a new mesh
                 n_layers = self.n_layers + self.n_air_layers
                 self.nodes_z, z_grid = self.make_z_mesh(n_layers)
 
                 # adjust level to topography min
                 if max_elev is not None:
                     self.grid_z -= max_elev
-                    ztops = np.where(
-                        self.surface_dict["topography"] > max_elev
-                    )
+                    ztops = np.where(self.surface_dict["topography"] > max_elev)
                     self.surface_dict["topography"][ztops] = max_elev
                 else:
                     self.grid_z -= topo_core.max()
 
             elif airlayer_type == "constant":
                 if max_elev is not None:
                     air_cell_thickness = np.ceil(
@@ -2766,15 +2758,15 @@
         info = mlines[0].strip().split()
         iteration_number = int(info[2])
         rms = float(info[5])
         try:
             lagrange = float(info[8])
         except IndexError:
             self._logger.warning("Did not get Lagrange Multiplier")
-            lagrange = 1.
+            lagrange = 1.0
 
         # get lengths of things
         n_north, n_east, n_z, n_res = np.array(
             mlines[1].strip().split(), dtype=int
         )
 
         # make empty arrays to put stuff into
@@ -2788,24 +2780,24 @@
         count_n = 0  # number of north nodes found
         while count_n < n_north:
             mline = mlines[line_index].strip().split()
             for north_node in mline:
                 self._nodes_north[count_n] = float(north_node)
                 count_n += 1
             line_index += 1
-        self.grid_north = np.insert(np.cumsum(self.nodes_north),0,0)
+        self.grid_north = np.insert(np.cumsum(self.nodes_north), 0, 0)
 
         count_e = 0  # number of east nodes found
         while count_e < n_east:
             mline = mlines[line_index].strip().split()
             for east_node in mline:
                 self._nodes_east[count_e] = float(east_node)
                 count_e += 1
             line_index += 1
-        self.grid_east = np.insert(np.cumsum(self.nodes_east),0,0)
+        self.grid_east = np.insert(np.cumsum(self.nodes_east), 0, 0)
 
         count_z = 0  # number of vertical nodes
         zdep = 0
         while count_z < n_z:
             mline = mlines[line_index].strip().split()
             for z_node in mline:
                 self.grid_z[count_z] = zdep
```

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/winglink.py` & `mtpy-v2-2.0.7/mtpy/modeling/winglink.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/winglinktools.py` & `mtpy-v2-2.0.7/mtpy/modeling/winglinktools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/__init__.py` & `mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/data.py` & `mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/data.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/startup.py` & `mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/startup.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/modeling/ws3dinv/stations.py` & `mtpy-v2-2.0.7/mtpy/modeling/ws3dinv/stations.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/mtpy_globals.py` & `mtpy-v2-2.0.7/mtpy/mtpy_globals.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/processing/birrp.py` & `mtpy-v2-2.0.7/mtpy/processing/birrp.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/processing/filter.py` & `mtpy-v2-2.0.7/mtpy/processing/filter.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/processing/tf.py` & `mtpy-v2-2.0.7/mtpy/processing/tf.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/__init__.py` & `mtpy-v2-2.0.7/mtpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/array2raster.py` & `mtpy-v2-2.0.7/mtpy/utils/array2raster.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/basemap_tools.py` & `mtpy-v2-2.0.7/mtpy/utils/basemap_tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/calculator.py` & `mtpy-v2-2.0.7/mtpy/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/concatenate_input.py` & `mtpy-v2-2.0.7/mtpy/utils/concatenate_input.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/configfile.py` & `mtpy-v2-2.0.7/mtpy/utils/configfile.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/convert_modem_data_to_geogrid.py` & `mtpy-v2-2.0.7/mtpy/utils/convert_modem_data_to_geogrid.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/edi_folders.py` & `mtpy-v2-2.0.7/mtpy/utils/edi_folders.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/exceptions.py` & `mtpy-v2-2.0.7/mtpy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/filehandling.py` & `mtpy-v2-2.0.7/mtpy/utils/filehandling.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/gis_tools.py` & `mtpy-v2-2.0.7/mtpy/utils/gis_tools.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/mtpy_decorator.py` & `mtpy-v2-2.0.7/mtpy/utils/mtpy_decorator.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/plot_rms_iterations.py` & `mtpy-v2-2.0.7/mtpy/utils/plot_rms_iterations.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/sensor_orientation_correction.py` & `mtpy-v2-2.0.7/mtpy/utils/sensor_orientation_correction.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/shapefiles.py` & `mtpy-v2-2.0.7/mtpy/utils/shapefiles.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy/utils/shapefiles_creator.py` & `mtpy-v2-2.0.7/mtpy/utils/shapefiles_creator.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/mtpy_v2.egg-info/PKG-INFO` & `mtpy-v2-2.0.7/mtpy_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtpy-v2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python toolkit for standard magnetotelluric data processing.
 Home-page: https://github.com/MTgeophysics/mtpy-v2
 Author: Jared Peacock, Alison Kirkby, Fei Zhang, Rakib Hassan, Lars Krieger, Stephan Thiel
 Author-email: jpeacock@usgs.gov
 License: MIT
 Keywords: magnetotellurics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,15 +25,15 @@
 [![PyPi version](https://img.shields.io/pypi/v/mtpy-v2.svg)](https://pypi.python.org/pypi/mtpy-v2)
 [![Latest conda|conda-forge version](https://img.shields.io/conda/v/conda-forge/mtpy-v2.svg)](https://anaconda.org/conda-forge/mtpy-v2)
 [![codecov](https://codecov.io/gh/MTgeophysics/mtpy-v2/graph/badge.svg?token=TQPFBFMYDQ)](https://codecov.io/gh/MTgeophysics/mtpy-v2)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/mtpy-v2/badge/?version=latest)](https://mtpy-v2.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MTgeophysics/mtpy-v2/main)
 
-## Version 2.0.6
+## Version 2.0.7
 
 # Description
  
 `mtpy` provides tools for working with magnetotelluric (MT) data.  MTpy-v2 is an updated version of [mtpy](https://github.com/MTgeophysics/mtpy). Many things have changed under the hood and usage is different from mtpy v1. The main difference is that there is a central data type that can hold transfer functions and then read/write to your modeling program, plot, and analyze your data.  No longer will you need a directory of EDI files and then read them in everytime you want to do something.  You only need to build a project once and save it to an MTH5 file and you are ready to go. All metadata uses [mt-metadata](https://github.com/kujaku11/mt-metadata).
 
 # Installation
```

### Comparing `mtpy-v2-2.0.6/mtpy_v2.egg-info/SOURCES.txt` & `mtpy-v2-2.0.7/mtpy_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/setup.py` & `mtpy-v2-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,11 +61,11 @@
     keywords="magnetotellurics",
     name="mtpy-v2",
     packages=find_packages(include=["mtpy", "mtpy.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/MTgeophysics/mtpy-v2",
-    version="2.0.6",
+    version="2.0.7",
     zip_safe=False,
     package_data={"": []},
 )
```

### Comparing `mtpy-v2-2.0.6/tests/__init__.py` & `mtpy-v2-2.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/test_mt.py` & `mtpy-v2-2.0.7/tests/core/test_mt.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/test_mt_collection.py` & `mtpy-v2-2.0.7/tests/core/test_mt_collection.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/test_mt_dataframe.py` & `mtpy-v2-2.0.7/tests/core/test_mt_dataframe.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/test_mt_location.py` & `mtpy-v2-2.0.7/tests/core/test_mt_location.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @author: jpeacock
 """
 
 # =============================================================================
 # Imports
 # =============================================================================
 import unittest
+from pathlib import Path
 
 from mtpy.core.mt_location import MTLocation
 
 # =============================================================================
 
 
 class TestMTLocation(unittest.TestCase):
@@ -94,14 +95,31 @@
 
         with self.subTest("longitude"):
             self.assertAlmostEqual(self.loc.longitude, self.true_lon)
 
         with self.subTest("utm zone"):
             self.assertEqual(self.loc.utm_zone, self.utm_zone)
 
+    def test_to_from_json(self):
+        fn = Path().cwd().joinpath("test.json")
+
+        loc_og = MTLocation(
+            latitude=self.true_lat,
+            longitude=self.true_lon,
+            utm_epsg=self.utm_epsg,
+        )
+        loc_og.to_json(fn)
+
+        loc_new = MTLocation()
+        loc_new.from_json(fn)
+
+        self.assertEqual(loc_og, loc_new)
+
+        fn.unlink()
+
 
 class TestMTLocationModelLocation(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         self.true_lat = 40.0
         self.true_lon = -120.0
         self.utm_epsg = 32611
```

### Comparing `mtpy-v2-2.0.6/tests/core/test_mt_stations.py` & `mtpy-v2-2.0.7/tests/core/test_mt_stations.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/transfer_function/test_pt.py` & `mtpy-v2-2.0.7/tests/core/transfer_function/test_pt.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/transfer_function/test_tf_base.py` & `mtpy-v2-2.0.7/tests/core/transfer_function/test_tf_base.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/transfer_function/test_tipper.py` & `mtpy-v2-2.0.7/tests/core/transfer_function/test_tipper.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/core/transfer_function/test_z.py` & `mtpy-v2-2.0.7/tests/core/transfer_function/test_z.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/imaging/test_plot_mt_response.py` & `mtpy-v2-2.0.7/tests/imaging/test_plot_mt_response.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/modeling/__init__.py` & `mtpy-v2-2.0.7/tests/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/modeling/test_errors.py` & `mtpy-v2-2.0.7/tests/modeling/test_errors.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/utils/test_calculator.py` & `mtpy-v2-2.0.7/tests/utils/test_calculator.py`

 * *Files identical despite different names*

### Comparing `mtpy-v2-2.0.6/tests/utils/test_gis_tools.py` & `mtpy-v2-2.0.7/tests/utils/test_gis_tools.py`

 * *Files identical despite different names*

