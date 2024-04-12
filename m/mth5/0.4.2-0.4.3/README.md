# Comparing `tmp/mth5-0.4.2.tar.gz` & `tmp/mth5-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mth5-0.4.2.tar", last modified: Fri Mar  8 18:37:43 2024, max compression
+gzip compressed data, was "mth5-0.4.3.tar", last modified: Fri Apr 12 22:23:06 2024, max compression
```

## Comparing `mth5-0.4.2.tar` & `mth5-0.4.3.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:43.252352 mth5-0.4.2/
--rw-rw-rw-   0        0        0      957 2023-03-27 21:53:07.000000 mth5-0.4.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3568 2022-07-05 20:34:49.000000 mth5-0.4.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     2641 2024-02-29 19:32:28.000000 mth5-0.4.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1080 2024-03-01 22:34:42.000000 mth5-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     1096 2024-03-08 18:36:07.000000 mth5-0.4.2/LICENSE.md
--rw-rw-rw-   0        0        0      394 2024-03-01 22:41:22.000000 mth5-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0    13355 2024-03-08 18:37:43.252352 mth5-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     9855 2024-03-08 18:36:12.000000 mth5-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:39.813363 mth5-0.4.2/docs/
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:39.813363 mth5-0.4.2/docs/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0      958 2023-04-15 00:16:51.000000 mth5-0.4.2/docs/.ipynb_checkpoints/index-checkpoint.rst
--rw-rw-rw-   0        0        0      625 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/Makefile
--rw-rw-rw-   0        0        0    10259 2024-03-08 18:36:12.000000 mth5-0.4.2/docs/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:39.628660 mth5-0.4.2/docs/_build/
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:39.613048 mth5-0.4.2/docs/_build/doctrees/
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.145371 mth5-0.4.2/docs/_build/doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    25869 2023-03-23 22:52:43.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_14_1.png
--rw-rw-rw-   0        0        0    16079 2023-03-23 22:52:43.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_18_1.png
--rw-rw-rw-   0        0        0    32094 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_10_0.png
--rw-rw-rw-   0        0        0    23186 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_14_0.png
--rw-rw-rw-   0        0        0    19789 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_18_0.png
--rw-rw-rw-   0        0        0    25725 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_23_1.png
--rw-rw-rw-   0        0        0    57694 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_28_1.png
--rw-rw-rw-   0        0        0    10774 2023-03-23 22:52:46.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_6_0.png
--rw-rw-rw-   0        0        0    49505 2023-03-23 22:52:48.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_29_1.png
--rw-rw-rw-   0        0        0   172207 2023-03-23 22:52:48.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_30_1.png
--rw-rw-rw-   0        0        0   103555 2023-03-23 22:52:48.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_33_0.png
--rw-rw-rw-   0        0        0    93180 2023-03-23 22:52:48.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_35_1.png
--rw-rw-rw-   0        0        0    49505 2023-03-23 22:52:49.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_29_1.png
--rw-rw-rw-   0        0        0   172207 2023-03-23 22:52:49.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_30_1.png
--rw-rw-rw-   0        0        0   103555 2023-03-23 22:52:49.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_33_0.png
--rw-rw-rw-   0        0        0    93180 2023-03-23 22:52:49.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_35_1.png
--rw-rw-rw-   0        0        0    70575 2022-09-09 23:37:55.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_1.png
--rw-rw-rw-   0        0        0   107717 2022-09-09 23:37:55.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_3.png
--rw-rw-rw-   0        0        0   251042 2022-09-09 23:37:55.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_45_0.png
--rw-rw-rw-   0        0        0    29529 2023-03-23 22:52:50.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_geomag_12_0.png
--rw-rw-rw-   0        0        0    37779 2023-03-23 22:52:52.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_nims_16_0.png
--rw-rw-rw-   0        0        0    30162 2023-03-23 22:52:59.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_15_0.png
--rw-rw-rw-   0        0        0    30162 2022-09-08 01:52:17.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_16_0.png
--rw-rw-rw-   0        0        0   169002 2023-03-23 22:52:59.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_17_0.png
--rw-rw-rw-   0        0        0    48807 2023-03-23 22:52:59.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_19_1.png
--rw-rw-rw-   0        0        0   205524 2022-09-08 01:52:17.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_2.png
--rw-rw-rw-   0        0        0    64999 2022-09-08 01:52:17.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_4.png
--rw-rw-rw-   0        0        0    52127 2023-03-23 22:53:00.000000 mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_run_ts_example_14_0.png
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:39.628660 mth5-0.4.2/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.330295 mth5-0.4.2/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   192616 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/_build/html/_images/cas04_run_a_plot.png
--rw-rw-rw-   0        0        0   263672 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/_build/html/_images/cas04_run_a_plot_zoom.png
--rw-rw-rw-   0        0        0    25869 2022-09-12 23:31:54.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_channel_ts_example_14_1.png
--rw-rw-rw-   0        0        0    16079 2022-09-12 23:31:54.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_channel_ts_example_18_1.png
--rw-rw-rw-   0        0        0    32094 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_10_0.png
--rw-rw-rw-   0        0        0    23186 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_14_0.png
--rw-rw-rw-   0        0        0    19789 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_18_0.png
--rw-rw-rw-   0        0        0    25725 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_23_1.png
--rw-rw-rw-   0        0        0    57694 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_28_1.png
--rw-rw-rw-   0        0        0    10774 2022-09-08 01:52:11.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_6_0.png
--rw-rw-rw-   0        0        0    29529 2023-03-23 22:52:50.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_make_mth5_from_geomag_12_0.png
--rw-rw-rw-   0        0        0    37779 2022-09-08 01:52:13.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_make_mth5_from_nims_16_0.png
--rw-rw-rw-   0        0        0    30162 2022-09-12 23:32:00.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_15_0.png
--rw-rw-rw-   0        0        0    30162 2022-09-08 01:52:17.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_16_0.png
--rw-rw-rw-   0        0        0    52127 2022-09-08 01:52:18.000000 mth5-0.4.2/docs/_build/html/_images/examples_notebooks_run_ts_example_14_0.png
--rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/_build/html/_images/mth5_logo.png
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.377128 mth5-0.4.2/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2022-06-17 07:51:38.000000 mth5-0.4.2/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-06-17 07:51:38.000000 mth5-0.4.2/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/_build/html/_static/mth5_logo.png
--rw-rw-rw-   0        0        0       90 2022-06-17 07:51:38.000000 mth5-0.4.2/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/authors.rst
--rw-rw-rw-   0        0        0     5829 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/history.rst
--rw-rw-rw-   0        0        0      958 2024-02-29 19:32:29.000000 mth5-0.4.2/docs/index.rst
--rwxrwxrwx   0        0        0      802 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/make.bat
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.784724 mth5-0.4.2/docs/source/
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.784724 mth5-0.4.2/docs/source/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0      212 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/.ipynb_checkpoints/mt_metadata_guide-checkpoint.rst
--rw-rw-rw-   0        0        0     3571 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/conventions.rst
--rw-rw-rw-   0        0        0      260 2024-02-29 19:32:29.000000 mth5-0.4.2/docs/source/examples.rst
--rw-rw-rw-   0        0        0    10202 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/file_readers.rst
--rw-rw-rw-   0        0        0     1945 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/gotchas.rst
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.815974 mth5-0.4.2/docs/source/images/
--rw-rw-rw-   0        0        0   192616 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/images/cas04_run_a_plot.png
--rw-rw-rw-   0        0        0   263672 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/images/cas04_run_a_plot_zoom.png
--rw-rw-rw-   0        0        0   169249 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/images/example_mt_file_structure.png
--rw-rw-rw-   0        0        0   554935 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/images/example_mt_file_structure_v2.png
--rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/images/mth5_logo.png
--rw-rw-rw-   0        0        0     1653 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/installation.rst
--rw-rw-rw-   0        0        0       56 2022-09-08 19:16:29.000000 mth5-0.4.2/docs/source/modules.rst
--rw-rw-rw-   0        0        0      212 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/mt_metadata_guide.rst
--rw-rw-rw-   0        0        0      360 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.clients.rst
--rw-rw-rw-   0        0        0     1428 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.groups.filter_groups.rst
--rw-rw-rw-   0        0        0     1798 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.groups.rst
--rw-rw-rw-   0        0        0      535 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.lemi.rst
--rw-rw-rw-   0        0        0      379 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.miniseed.rst
--rw-rw-rw-   0        0        0     1011 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.nims.rst
--rw-rw-rw-   0        0        0      548 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.phoenix.readers.contiguous.rst
--rw-rw-rw-   0        0        0      480 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.phoenix.readers.native.rst
--rw-rw-rw-   0        0        0      966 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.phoenix.readers.rst
--rw-rw-rw-   0        0        0      539 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.phoenix.readers.segmented.rst
--rw-rw-rw-   0        0        0      653 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.phoenix.rst
--rw-rw-rw-   0        0        0      647 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.rst
--rw-rw-rw-   0        0        0      403 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.usgs_ascii.rst
--rw-rw-rw-   0        0        0     1192 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.io.zen.rst
--rw-rw-rw-   0        0        0      587 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.rst
--rw-rw-rw-   0        0        0      690 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.tables.rst
--rw-rw-rw-   0        0        0      723 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.timeseries.rst
--rw-rw-rw-   0        0        0      829 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/mth5.utils.rst
--rw-rw-rw-   0        0        0      222 2024-02-29 19:32:29.000000 mth5-0.4.2/docs/source/parallel.rst
--rw-rw-rw-   0        0        0     3536 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/runs.rst
--rw-rw-rw-   0        0        0     5786 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/stations.rst
--rw-rw-rw-   0        0        0     2968 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/structure.rst
--rw-rw-rw-   0        0        0     4096 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/surveys.rst
--rw-rw-rw-   0        0        0     1596 2022-07-05 20:34:49.000000 mth5-0.4.2/docs/source/ts.rst
--rw-rw-rw-   0        0        0     1625 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/usage.rst
--rw-rw-rw-   0        0        0     1859 2023-03-27 21:53:07.000000 mth5-0.4.2/docs/source/usage_v2.rst
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.862837 mth5-0.4.2/mth5/
--rw-rw-rw-   0        0        0     3190 2024-03-08 18:36:12.000000 mth5-0.4.2/mth5/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.000846 mth5-0.4.2/mth5/clients/
--rw-rw-rw-   0        0        0      249 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/__init__.py
--rw-rw-rw-   0        0        0    28087 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/fdsn.py
--rw-rw-rw-   0        0        0    20578 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/geomag.py
--rw-rw-rw-   0        0        0     6844 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/make_mth5.py
--rw-rw-rw-   0        0        0     6244 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/phoenix.py
--rw-rw-rw-   0        0        0     7870 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/clients/zen.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.201330 mth5-0.4.2/mth5/groups/
--rw-rw-rw-   0        0        0     1256 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/__init__.py
--rw-rw-rw-   0        0        0    13430 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/base.py
--rw-rw-rw-   0        0        0    45480 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/channel_dataset.py
--rw-rw-rw-   0        0        0     8921 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/estimate_dataset.py
--rw-rw-rw-   0        0        0     3558 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/groups/experiment.py
--rw-rw-rw-   0        0        0    11324 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/fc_dataset.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.301812 mth5-0.4.2/mth5/groups/filter_groups/
--rw-rw-rw-   0        0        0      416 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/groups/filter_groups/__init__.py
--rw-rw-rw-   0        0        0     3374 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/groups/filter_groups/coefficient_filter_group.py
--rw-rw-rw-   0        0        0     5449 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/filter_groups/fap_filter_group.py
--rw-rw-rw-   0        0        0     4067 2023-03-27 21:53:07.000000 mth5-0.4.2/mth5/groups/filter_groups/fir_filter_group.py
--rw-rw-rw-   0        0        0     3704 2023-03-27 21:53:07.000000 mth5-0.4.2/mth5/groups/filter_groups/time_delay_filter_group.py
--rw-rw-rw-   0        0        0     5494 2023-03-27 21:53:07.000000 mth5-0.4.2/mth5/groups/filter_groups/zpk_filter_group.py
--rw-rw-rw-   0        0        0     5798 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/filters.py
--rw-rw-rw-   0        0        0    21261 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/fourier_coefficients.py
--rw-rw-rw-   0        0        0     1667 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/groups/reports.py
--rw-rw-rw-   0        0        0    29329 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/run.py
--rw-rw-rw-   0        0        0     7644 2024-03-08 18:36:12.000000 mth5-0.4.2/mth5/groups/standards.py
--rw-rw-rw-   0        0        0    25419 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/station.py
--rw-rw-rw-   0        0        0    20306 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/survey.py
--rw-rw-rw-   0        0        0    20284 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/groups/transfer_function.py
--rw-rw-rw-   0        0        0     8840 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.337098 mth5-0.4.2/mth5/io/
--rw-rw-rw-   0        0        0      126 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/__init__.py
--rw-rw-rw-   0        0        0     7549 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/collection.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.368340 mth5-0.4.2/mth5/io/lemi/
--rw-rw-rw-   0        0        0      166 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/lemi/__init__.py
--rw-rw-rw-   0        0        0    21752 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/lemi/lemi424.py
--rw-rw-rw-   0        0        0     5262 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/lemi/lemi_collection.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.401597 mth5-0.4.2/mth5/io/miniseed/
--rw-rw-rw-   0        0        0       86 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/miniseed/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/miniseed/miniseed.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.501839 mth5-0.4.2/mth5/io/nims/
--rw-rw-rw-   0        0        0      339 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/nims/__init__.py
--rw-rw-rw-   0        0        0    17046 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/nims/gps.py
--rw-rw-rw-   0        0        0     8123 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/nims/header.py
--rw-rw-rw-   0        0        0    44984 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/nims/nims.py
--rw-rw-rw-   0        0        0     4300 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/nims/nims_collection.py
--rw-rw-rw-   0        0        0     7827 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/nims/response_filters.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.548703 mth5-0.4.2/mth5/io/phoenix/
--rw-rw-rw-   0        0        0      300 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/__init__.py
--rw-rw-rw-   0        0        0    10739 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/phoenix_collection.py
--rw-rw-rw-   0        0        0     1558 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/read.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.648948 mth5-0.4.2/mth5/io/phoenix/readers/
--rw-rw-rw-   0        0        0      554 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/__init__.py
--rw-rw-rw-   0        0        0    13264 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/base.py
--rw-rw-rw-   0        0        0     5464 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/calibrations.py
--rw-rw-rw-   0        0        0     3132 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/config.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.686701 mth5-0.4.2/mth5/io/phoenix/readers/contiguous/
--rw-rw-rw-   0        0        0      111 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/phoenix/readers/contiguous/__init__.py
--rw-rw-rw-   0        0        0     5005 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/contiguous/decimated_continuous_reader.py
--rw-rw-rw-   0        0        0    22418 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/header.py
--rw-rw-rw-   0        0        0      717 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.717950 mth5-0.4.2/mth5/io/phoenix/readers/native/
--rw-rw-rw-   0        0        0       71 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/phoenix/readers/native/__init__.py
--rw-rw-rw-   0        0        0     9989 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/native/native_reader.py
--rw-rw-rw-   0        0        0     7579 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/receiver_metadata.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.749193 mth5-0.4.2/mth5/io/phoenix/readers/segmented/
--rw-rw-rw-   0        0        0      108 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/phoenix/readers/segmented/__init__.py
--rw-rw-rw-   0        0        0     9585 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/phoenix/readers/segmented/decimated_segmented_reader.py
--rw-rw-rw-   0        0        0     4714 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/reader.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.824980 mth5-0.4.2/mth5/io/usgs_ascii/
--rw-rw-rw-   0        0        0      235 2023-03-27 21:53:08.000000 mth5-0.4.2/mth5/io/usgs_ascii/__init__.py
--rw-rw-rw-   0        0        0    14414 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/usgs_ascii/header.py
--rw-rw-rw-   0        0        0    13248 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/usgs_ascii/usgs_ascii.py
--rw-rw-rw-   0        0        0     4306 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/usgs_ascii/usgs_ascii_collection.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.933635 mth5-0.4.2/mth5/io/zen/
--rw-rw-rw-   0        0        0      383 2023-08-15 22:49:23.000000 mth5-0.4.2/mth5/io/zen/__init__.py
--rw-rw-rw-   0        0        0     7270 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/coil_response.py
--rw-rw-rw-   0        0        0     6122 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/z3d_collection.py
--rw-rw-rw-   0        0        0     7158 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/z3d_header.py
--rw-rw-rw-   0        0        0    12593 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/z3d_metadata.py
--rw-rw-rw-   0        0        0     4791 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/z3d_schedule.py
--rw-rw-rw-   0        0        0    41414 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/zen.py
--rw-rw-rw-   0        0        0    24152 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/io/zen/zen_tools.py
--rw-rw-rw-   0        0        0    60607 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/mth5.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:41.964878 mth5-0.4.2/mth5/tables/
--rw-rw-rw-   0        0        0      205 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/tables/__init__.py
--rw-rw-rw-   0        0        0     3944 2024-03-08 18:36:12.000000 mth5-0.4.2/mth5/tables/channel_table.py
--rw-rw-rw-   0        0        0    12443 2024-03-08 18:36:12.000000 mth5-0.4.2/mth5/tables/mth5_table.py
--rw-rw-rw-   0        0        0     5764 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/tables/tf_table.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.065118 mth5-0.4.2/mth5/timeseries/
--rw-rw-rw-   0        0        0       98 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/timeseries/__init__.py
--rw-rw-rw-   0        0        0    60621 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/timeseries/channel_ts.py
--rw-rw-rw-   0        0        0    47411 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/timeseries/run_ts.py
--rw-rw-rw-   0        0        0    23734 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/timeseries/scipy_filters.py
--rw-rw-rw-   0        0        0    26574 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/timeseries/ts_filters.py
--rw-rw-rw-   0        0        0     4220 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/timeseries/ts_helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.134121 mth5-0.4.2/mth5/utils/
--rw-rw-rw-   0        0        0       16 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/utils/__init__.py
--rw-rw-rw-   0        0        0      364 2022-07-05 20:34:49.000000 mth5-0.4.2/mth5/utils/exceptions.py
--rw-rw-rw-   0        0        0     7770 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/utils/fdsn_tools.py
--rw-rw-rw-   0        0        0     6078 2024-02-29 19:32:29.000000 mth5-0.4.2/mth5/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:40.900606 mth5-0.4.2/mth5.egg-info/
--rw-rw-rw-   0        0        0    13355 2024-03-08 18:37:38.000000 mth5-0.4.2/mth5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10142 2024-03-08 18:37:39.000000 mth5-0.4.2/mth5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 18:37:38.000000 mth5-0.4.2/mth5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-09 00:23:08.000000 mth5-0.4.2/mth5.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2024-03-08 18:37:38.000000 mth5-0.4.2/mth5.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-08 18:37:38.000000 mth5-0.4.2/mth5.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-03-08 18:37:43.252352 mth5-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1568 2024-03-08 18:36:12.000000 mth5-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.203117 mth5-0.4.2/tests/
--rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.265603 mth5-0.4.2/tests/clients/
--rw-rw-rw-   0        0        0        0 2023-04-15 00:16:51.000000 mth5-0.4.2/tests/clients/__init__.py
--rw-rw-rw-   0        0        0     4696 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/clients/test_geomag.py
--rw-rw-rw-   0        0        0    12543 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/clients/test_geomag_client.py
--rw-rw-rw-   0        0        0     2600 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/clients/test_makemth5.py
--rw-rw-rw-   0        0        0     9178 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/example_lemi.txt
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.287732 mth5-0.4.2/tests/helpers/
--rw-rw-rw-   0        0        0     2776 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/helpers/test_initialize_mth5.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.338476 mth5-0.4.2/tests/io/
--rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/__init__.py
--rw-rw-rw-   0        0        0     9178 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/example_lemi.txt
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.371111 mth5-0.4.2/tests/io/lemi/
--rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/lemi/__init__.py
--rw-rw-rw-   0        0        0    17660 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/lemi/test_lemi.py
--rw-rw-rw-   0        0        0     4066 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/lemi/test_lemi_collection.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.434612 mth5-0.4.2/tests/io/nims/
--rw-rw-rw-   0        0        0     3062 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/nims/test_nims_collection.py
--rw-rw-rw-   0        0        0     6133 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/nims/test_nims_gps.py
--rw-rw-rw-   0        0        0     3551 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/nims/test_nims_response.py
--rw-rw-rw-   0        0        0    19225 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/nims/test_read_nims.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.566095 mth5-0.4.2/tests/io/phoenix/
--rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/phoenix/__init__.py
--rw-rw-rw-   0        0        0    37444 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/example_rxcal.json
--rw-rw-rw-   0        0        0    13710 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_base_reader.py
--rw-rw-rw-   0        0        0     3982 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_phoenix_collection.py
--rw-rw-rw-   0        0        0     2922 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_phx_calibration.py
--rw-rw-rw-   0        0        0     7934 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_read_phoenix_continuous.py
--rw-rw-rw-   0        0        0     8809 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_read_phoenix_native.py
--rw-rw-rw-   0        0        0     8644 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/phoenix/test_read_phoenix_segmented.py
--rw-rw-rw-   0        0        0     1940 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/test_reader.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.603854 mth5-0.4.2/tests/io/usgs_ascii/
--rw-rw-rw-   0        0        0     2874 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/usgs_ascii/test_ascii.py
--rw-rw-rw-   0        0        0     3131 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/usgs_ascii/test_ascii_collection.py
--rw-rw-rw-   0        0        0    13936 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/usgs_ascii/test_header.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.704099 mth5-0.4.2/tests/io/zen/
--rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/zen/__init__.py
--rw-rw-rw-   0        0        0    27603 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/zen/test_z3d.py
--rw-rw-rw-   0        0        0     3142 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/zen/test_z3d_collection.py
--rw-rw-rw-   0        0        0     4581 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/zen/test_z3d_header.py
--rw-rw-rw-   0        0        0    14131 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/zen/test_z3d_metadata.py
--rw-rw-rw-   0        0        0     3481 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/io/zen/test_z3d_schedule.py
--rw-rw-rw-   0        0        0     3681 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/io/zen/test_zen_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.735341 mth5-0.4.2/tests/tables/
--rw-rw-rw-   0        0        0      349 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/tables/__init__.py
--rw-rw-rw-   0        0        0     8484 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/tables/test_mth5_table.py
--rw-rw-rw-   0        0        0     5742 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/test_channel_slice.py
--rw-rw-rw-   0        0        0     7583 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/test_mth5_basics.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.878560 mth5-0.4.2/tests/timeseries/
--rw-rw-rw-   0        0        0    33626 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_channel_ts.py
--rw-rw-rw-   0        0        0     3466 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_remove_response.py
--rw-rw-rw-   0        0        0    31650 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_runts.py
--rw-rw-rw-   0        0        0     4909 2024-01-25 19:34:44.000000 mth5-0.4.2/tests/timeseries/test_runts_02.py
--rw-rw-rw-   0        0        0     7698 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_ts_filters.py
--rw-rw-rw-   0        0        0     4693 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_ts_helpers.py
--rw-rw-rw-   0        0        0     2619 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/timeseries/test_xr_scipy.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:42.889632 mth5-0.4.2/tests/utils/
--rw-rw-rw-   0        0        0     5613 2023-03-27 21:53:08.000000 mth5-0.4.2/tests/utils/test_fdsn_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:43.120868 mth5-0.4.2/tests/version_1/
--rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.2/tests/version_1/__init__.py
--rw-rw-rw-   0        0        0     8050 2022-07-05 20:34:49.000000 mth5-0.4.2/tests/version_1/expected.csv
--rw-rw-rw-   0        0        0   105049 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test1_dec_level_3.csv
--rw-rw-rw-   0        0        0    12546 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_build_from_experiment.py
--rw-rw-rw-   0        0        0     8896 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_fcs.py
--rw-rw-rw-   0        0        0     3491 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_filters.py
--rw-rw-rw-   0        0        0     3756 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_from_fap_stationxml.py
--rw-rw-rw-   0        0        0     7288 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_from_stationxml.py
--rw-rw-rw-   0        0        0    11581 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_make_mth5.py
--rw-rw-rw-   0        0        0    18537 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_make_mth5_geomag.py
--rw-rw-rw-   0        0        0    10723 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_make_mth5_ofr.py
--rw-rw-rw-   0        0        0    17171 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_mth5.py
--rw-rw-rw-   0        0        0    15229 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_1/test_transfer_function.py
-drwxrwxrwx   0        0        0        0 2024-03-08 18:37:43.252352 mth5-0.4.2/tests/version_2/
--rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.2/tests/version_2/__init__.py
--rw-rw-rw-   0        0        0    13449 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_build_from_experiment.py
--rw-rw-rw-   0        0        0     3587 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_filters.py
--rw-rw-rw-   0        0        0     4458 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_from_fap_stationxml.py
--rw-rw-rw-   0        0        0     6995 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_from_stationxml.py
--rw-rw-rw-   0        0        0    12452 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_make_mth5.py
--rw-rw-rw-   0        0        0    18785 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_make_mth5_geomag.py
--rw-rw-rw-   0        0        0    18849 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_mth5.py
--rw-rw-rw-   0        0        0    14352 2024-02-29 19:32:30.000000 mth5-0.4.2/tests/version_2/test_transfer_function.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:06.264196 mth5-0.4.3/
+-rw-rw-rw-   0        0        0      957 2023-03-27 21:53:07.000000 mth5-0.4.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3568 2022-07-05 20:34:49.000000 mth5-0.4.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     2641 2024-02-29 19:32:28.000000 mth5-0.4.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1080 2024-03-01 22:34:42.000000 mth5-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     1096 2024-04-12 22:09:38.000000 mth5-0.4.3/LICENSE.md
+-rw-rw-rw-   0        0        0      394 2024-03-01 22:41:22.000000 mth5-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    13355 2024-04-12 22:23:06.264196 mth5-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9855 2024-04-12 22:10:12.000000 mth5-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.610270 mth5-0.4.3/docs/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.610270 mth5-0.4.3/docs/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0      958 2023-04-15 00:16:51.000000 mth5-0.4.3/docs/.ipynb_checkpoints/index-checkpoint.rst
+-rw-rw-rw-   0        0        0      625 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/Makefile
+-rw-rw-rw-   0        0        0    10259 2024-04-12 22:10:12.000000 mth5-0.4.3/docs/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.441361 mth5-0.4.3/docs/_build/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.441361 mth5-0.4.3/docs/_build/doctrees/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.926727 mth5-0.4.3/docs/_build/doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    25869 2023-03-23 22:52:43.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_14_1.png
+-rw-rw-rw-   0        0        0    16079 2023-03-23 22:52:43.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_18_1.png
+-rw-rw-rw-   0        0        0    32094 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_10_0.png
+-rw-rw-rw-   0        0        0    23186 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_14_0.png
+-rw-rw-rw-   0        0        0    19789 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_18_0.png
+-rw-rw-rw-   0        0        0    25725 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_23_1.png
+-rw-rw-rw-   0        0        0    57694 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_28_1.png
+-rw-rw-rw-   0        0        0    10774 2023-03-23 22:52:46.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_6_0.png
+-rw-rw-rw-   0        0        0    49505 2023-03-23 22:52:48.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_29_1.png
+-rw-rw-rw-   0        0        0   172207 2023-03-23 22:52:48.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_30_1.png
+-rw-rw-rw-   0        0        0   103555 2023-03-23 22:52:48.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_33_0.png
+-rw-rw-rw-   0        0        0    93180 2023-03-23 22:52:48.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_35_1.png
+-rw-rw-rw-   0        0        0    49505 2023-03-23 22:52:49.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_29_1.png
+-rw-rw-rw-   0        0        0   172207 2023-03-23 22:52:49.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_30_1.png
+-rw-rw-rw-   0        0        0   103555 2023-03-23 22:52:49.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_33_0.png
+-rw-rw-rw-   0        0        0    93180 2023-03-23 22:52:49.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_35_1.png
+-rw-rw-rw-   0        0        0    70575 2022-09-09 23:37:55.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_1.png
+-rw-rw-rw-   0        0        0   107717 2022-09-09 23:37:55.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_3.png
+-rw-rw-rw-   0        0        0   251042 2022-09-09 23:37:55.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_45_0.png
+-rw-rw-rw-   0        0        0    29529 2023-03-23 22:52:50.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_geomag_12_0.png
+-rw-rw-rw-   0        0        0    37779 2023-03-23 22:52:52.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_nims_16_0.png
+-rw-rw-rw-   0        0        0    30162 2023-03-23 22:52:59.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_15_0.png
+-rw-rw-rw-   0        0        0    30162 2022-09-08 01:52:17.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_16_0.png
+-rw-rw-rw-   0        0        0   169002 2023-03-23 22:52:59.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_17_0.png
+-rw-rw-rw-   0        0        0    48807 2023-03-23 22:52:59.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_19_1.png
+-rw-rw-rw-   0        0        0   205524 2022-09-08 01:52:17.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_2.png
+-rw-rw-rw-   0        0        0    64999 2022-09-08 01:52:17.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_4.png
+-rw-rw-rw-   0        0        0    52127 2023-03-23 22:53:00.000000 mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_run_ts_example_14_0.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:02.441361 mth5-0.4.3/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.111464 mth5-0.4.3/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   192616 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/_build/html/_images/cas04_run_a_plot.png
+-rw-rw-rw-   0        0        0   263672 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/_build/html/_images/cas04_run_a_plot_zoom.png
+-rw-rw-rw-   0        0        0    25869 2022-09-12 23:31:54.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_channel_ts_example_14_1.png
+-rw-rw-rw-   0        0        0    16079 2022-09-12 23:31:54.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_channel_ts_example_18_1.png
+-rw-rw-rw-   0        0        0    32094 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_10_0.png
+-rw-rw-rw-   0        0        0    23186 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_14_0.png
+-rw-rw-rw-   0        0        0    19789 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_18_0.png
+-rw-rw-rw-   0        0        0    25725 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_23_1.png
+-rw-rw-rw-   0        0        0    57694 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_28_1.png
+-rw-rw-rw-   0        0        0    10774 2022-09-08 01:52:11.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_6_0.png
+-rw-rw-rw-   0        0        0    29529 2023-03-23 22:52:50.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_make_mth5_from_geomag_12_0.png
+-rw-rw-rw-   0        0        0    37779 2022-09-08 01:52:13.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_make_mth5_from_nims_16_0.png
+-rw-rw-rw-   0        0        0    30162 2022-09-12 23:32:00.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_15_0.png
+-rw-rw-rw-   0        0        0    30162 2022-09-08 01:52:17.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_16_0.png
+-rw-rw-rw-   0        0        0    52127 2022-09-08 01:52:18.000000 mth5-0.4.3/docs/_build/html/_images/examples_notebooks_run_ts_example_14_0.png
+-rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/_build/html/_images/mth5_logo.png
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.142722 mth5-0.4.3/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2022-06-17 07:51:38.000000 mth5-0.4.3/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-06-17 07:51:38.000000 mth5-0.4.3/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/_build/html/_static/mth5_logo.png
+-rw-rw-rw-   0        0        0       90 2022-06-17 07:51:38.000000 mth5-0.4.3/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     5829 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/history.rst
+-rw-rw-rw-   0        0        0      958 2024-02-29 19:32:29.000000 mth5-0.4.3/docs/index.rst
+-rwxrwxrwx   0        0        0      802 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/make.bat
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.559085 mth5-0.4.3/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.559085 mth5-0.4.3/docs/source/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0      212 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/.ipynb_checkpoints/mt_metadata_guide-checkpoint.rst
+-rw-rw-rw-   0        0        0     3571 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/conventions.rst
+-rw-rw-rw-   0        0        0      260 2024-02-29 19:32:29.000000 mth5-0.4.3/docs/source/examples.rst
+-rw-rw-rw-   0        0        0    10202 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/file_readers.rst
+-rw-rw-rw-   0        0        0     1945 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/gotchas.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.628080 mth5-0.4.3/docs/source/images/
+-rw-rw-rw-   0        0        0   192616 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/images/cas04_run_a_plot.png
+-rw-rw-rw-   0        0        0   263672 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/images/cas04_run_a_plot_zoom.png
+-rw-rw-rw-   0        0        0   169249 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/images/example_mt_file_structure.png
+-rw-rw-rw-   0        0        0   554935 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/images/example_mt_file_structure_v2.png
+-rw-rw-rw-   0        0        0    83174 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/images/mth5_logo.png
+-rw-rw-rw-   0        0        0     1653 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       56 2022-09-08 19:16:29.000000 mth5-0.4.3/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      212 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/mt_metadata_guide.rst
+-rw-rw-rw-   0        0        0      360 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.clients.rst
+-rw-rw-rw-   0        0        0     1428 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.groups.filter_groups.rst
+-rw-rw-rw-   0        0        0     1798 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.groups.rst
+-rw-rw-rw-   0        0        0      535 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.lemi.rst
+-rw-rw-rw-   0        0        0      379 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.miniseed.rst
+-rw-rw-rw-   0        0        0     1011 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.nims.rst
+-rw-rw-rw-   0        0        0      548 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.phoenix.readers.contiguous.rst
+-rw-rw-rw-   0        0        0      480 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.phoenix.readers.native.rst
+-rw-rw-rw-   0        0        0      966 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.phoenix.readers.rst
+-rw-rw-rw-   0        0        0      539 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.phoenix.readers.segmented.rst
+-rw-rw-rw-   0        0        0      653 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.phoenix.rst
+-rw-rw-rw-   0        0        0      647 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.rst
+-rw-rw-rw-   0        0        0      403 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.usgs_ascii.rst
+-rw-rw-rw-   0        0        0     1192 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.io.zen.rst
+-rw-rw-rw-   0        0        0      587 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.rst
+-rw-rw-rw-   0        0        0      690 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.tables.rst
+-rw-rw-rw-   0        0        0      723 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.timeseries.rst
+-rw-rw-rw-   0        0        0      829 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/mth5.utils.rst
+-rw-rw-rw-   0        0        0      222 2024-02-29 19:32:29.000000 mth5-0.4.3/docs/source/parallel.rst
+-rw-rw-rw-   0        0        0     3536 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/runs.rst
+-rw-rw-rw-   0        0        0     5786 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/stations.rst
+-rw-rw-rw-   0        0        0     2968 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/structure.rst
+-rw-rw-rw-   0        0        0     4096 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/surveys.rst
+-rw-rw-rw-   0        0        0     1596 2022-07-05 20:34:49.000000 mth5-0.4.3/docs/source/ts.rst
+-rw-rw-rw-   0        0        0     1625 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/usage.rst
+-rw-rw-rw-   0        0        0     1859 2023-03-27 21:53:07.000000 mth5-0.4.3/docs/source/usage_v2.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.659324 mth5-0.4.3/mth5/
+-rw-rw-rw-   0        0        0     3259 2024-04-12 22:10:12.000000 mth5-0.4.3/mth5/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.812611 mth5-0.4.3/mth5/clients/
+-rw-rw-rw-   0        0        0      249 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/clients/__init__.py
+-rw-rw-rw-   0        0        0    28087 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/clients/fdsn.py
+-rw-rw-rw-   0        0        0    20578 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/clients/geomag.py
+-rw-rw-rw-   0        0        0     6844 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/clients/make_mth5.py
+-rw-rw-rw-   0        0        0     7761 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/clients/phoenix.py
+-rw-rw-rw-   0        0        0     7870 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/clients/zen.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.044347 mth5-0.4.3/mth5/groups/
+-rw-rw-rw-   0        0        0     1256 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/__init__.py
+-rw-rw-rw-   0        0        0    13430 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/base.py
+-rw-rw-rw-   0        0        0    45480 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/channel_dataset.py
+-rw-rw-rw-   0        0        0     8921 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/estimate_dataset.py
+-rw-rw-rw-   0        0        0     3558 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/groups/experiment.py
+-rw-rw-rw-   0        0        0    11324 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/fc_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.160215 mth5-0.4.3/mth5/groups/filter_groups/
+-rw-rw-rw-   0        0        0      416 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/groups/filter_groups/__init__.py
+-rw-rw-rw-   0        0        0     3374 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/groups/filter_groups/coefficient_filter_group.py
+-rw-rw-rw-   0        0        0     5449 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/filter_groups/fap_filter_group.py
+-rw-rw-rw-   0        0        0     4067 2023-03-27 21:53:07.000000 mth5-0.4.3/mth5/groups/filter_groups/fir_filter_group.py
+-rw-rw-rw-   0        0        0     3704 2023-03-27 21:53:07.000000 mth5-0.4.3/mth5/groups/filter_groups/time_delay_filter_group.py
+-rw-rw-rw-   0        0        0     5494 2023-03-27 21:53:07.000000 mth5-0.4.3/mth5/groups/filter_groups/zpk_filter_group.py
+-rw-rw-rw-   0        0        0     5798 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/filters.py
+-rw-rw-rw-   0        0        0    21386 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/groups/fourier_coefficients.py
+-rw-rw-rw-   0        0        0     1667 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/groups/reports.py
+-rw-rw-rw-   0        0        0    29329 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/run.py
+-rw-rw-rw-   0        0        0     7644 2024-03-08 18:36:12.000000 mth5-0.4.3/mth5/groups/standards.py
+-rw-rw-rw-   0        0        0    25419 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/station.py
+-rw-rw-rw-   0        0        0    20306 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/survey.py
+-rw-rw-rw-   0        0        0    20284 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/groups/transfer_function.py
+-rw-rw-rw-   0        0        0     8840 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.213587 mth5-0.4.3/mth5/io/
+-rw-rw-rw-   0        0        0      126 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/__init__.py
+-rw-rw-rw-   0        0        0     7549 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/collection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.265740 mth5-0.4.3/mth5/io/lemi/
+-rw-rw-rw-   0        0        0      166 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/lemi/__init__.py
+-rw-rw-rw-   0        0        0    21752 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/lemi/lemi424.py
+-rw-rw-rw-   0        0        0     5262 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/lemi/lemi_collection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.290413 mth5-0.4.3/mth5/io/miniseed/
+-rw-rw-rw-   0        0        0       86 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/miniseed/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/miniseed/miniseed.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.391660 mth5-0.4.3/mth5/io/nims/
+-rw-rw-rw-   0        0        0      339 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/nims/__init__.py
+-rw-rw-rw-   0        0        0    17046 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/nims/gps.py
+-rw-rw-rw-   0        0        0     8123 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/nims/header.py
+-rw-rw-rw-   0        0        0    44984 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/nims/nims.py
+-rw-rw-rw-   0        0        0     4300 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/nims/nims_collection.py
+-rw-rw-rw-   0        0        0     7827 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/nims/response_filters.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.429420 mth5-0.4.3/mth5/io/phoenix/
+-rw-rw-rw-   0        0        0      300 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/__init__.py
+-rw-rw-rw-   0        0        0    11097 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/io/phoenix/phoenix_collection.py
+-rw-rw-rw-   0        0        0     1558 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/read.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.560908 mth5-0.4.3/mth5/io/phoenix/readers/
+-rw-rw-rw-   0        0        0      554 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/__init__.py
+-rw-rw-rw-   0        0        0    13264 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/base.py
+-rw-rw-rw-   0        0        0     5464 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/calibrations.py
+-rw-rw-rw-   0        0        0     3132 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/config.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.592163 mth5-0.4.3/mth5/io/phoenix/readers/contiguous/
+-rw-rw-rw-   0        0        0      111 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/phoenix/readers/contiguous/__init__.py
+-rw-rw-rw-   0        0        0     5005 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/contiguous/decimated_continuous_reader.py
+-rw-rw-rw-   0        0        0    22418 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/header.py
+-rw-rw-rw-   0        0        0      717 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.614283 mth5-0.4.3/mth5/io/phoenix/readers/native/
+-rw-rw-rw-   0        0        0       71 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/phoenix/readers/native/__init__.py
+-rw-rw-rw-   0        0        0     9989 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/native/native_reader.py
+-rw-rw-rw-   0        0        0     7579 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/receiver_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.645532 mth5-0.4.3/mth5/io/phoenix/readers/segmented/
+-rw-rw-rw-   0        0        0      108 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/phoenix/readers/segmented/__init__.py
+-rw-rw-rw-   0        0        0     9585 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/phoenix/readers/segmented/decimated_segmented_reader.py
+-rw-rw-rw-   0        0        0     4714 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/reader.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.714526 mth5-0.4.3/mth5/io/usgs_ascii/
+-rw-rw-rw-   0        0        0      235 2023-03-27 21:53:08.000000 mth5-0.4.3/mth5/io/usgs_ascii/__init__.py
+-rw-rw-rw-   0        0        0    14414 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/usgs_ascii/header.py
+-rw-rw-rw-   0        0        0    13248 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/usgs_ascii/usgs_ascii.py
+-rw-rw-rw-   0        0        0     4306 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/usgs_ascii/usgs_ascii_collection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.876909 mth5-0.4.3/mth5/io/zen/
+-rw-rw-rw-   0        0        0      383 2023-08-15 22:49:23.000000 mth5-0.4.3/mth5/io/zen/__init__.py
+-rw-rw-rw-   0        0        0     7270 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/coil_response.py
+-rw-rw-rw-   0        0        0     6122 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/z3d_collection.py
+-rw-rw-rw-   0        0        0     7158 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/z3d_header.py
+-rw-rw-rw-   0        0        0    12593 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/z3d_metadata.py
+-rw-rw-rw-   0        0        0     4791 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/z3d_schedule.py
+-rw-rw-rw-   0        0        0    41414 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/zen.py
+-rw-rw-rw-   0        0        0    24152 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/io/zen/zen_tools.py
+-rw-rw-rw-   0        0        0    60641 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/mth5.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:04.930289 mth5-0.4.3/mth5/tables/
+-rw-rw-rw-   0        0        0      205 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/tables/__init__.py
+-rw-rw-rw-   0        0        0     4128 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/tables/channel_table.py
+-rw-rw-rw-   0        0        0    12443 2024-03-08 18:36:12.000000 mth5-0.4.3/mth5/tables/mth5_table.py
+-rw-rw-rw-   0        0        0     5764 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/tables/tf_table.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.046157 mth5-0.4.3/mth5/timeseries/
+-rw-rw-rw-   0        0        0       98 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/timeseries/__init__.py
+-rw-rw-rw-   0        0        0    60621 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/timeseries/channel_ts.py
+-rw-rw-rw-   0        0        0    47411 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/timeseries/run_ts.py
+-rw-rw-rw-   0        0        0    23734 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/timeseries/scipy_filters.py
+-rw-rw-rw-   0        0        0    26574 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/timeseries/ts_filters.py
+-rw-rw-rw-   0        0        0     4220 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/timeseries/ts_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.093022 mth5-0.4.3/mth5/utils/
+-rw-rw-rw-   0        0        0       16 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/utils/__init__.py
+-rw-rw-rw-   0        0        0      364 2022-07-05 20:34:49.000000 mth5-0.4.3/mth5/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7770 2024-02-29 19:32:29.000000 mth5-0.4.3/mth5/utils/fdsn_tools.py
+-rw-rw-rw-   0        0        0     6269 2024-04-12 22:09:24.000000 mth5-0.4.3/mth5/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:03.733557 mth5-0.4.3/mth5.egg-info/
+-rw-rw-rw-   0        0        0    13355 2024-04-12 22:23:00.000000 mth5-0.4.3/mth5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10142 2024-04-12 22:23:02.000000 mth5-0.4.3/mth5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 22:23:01.000000 mth5-0.4.3/mth5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 22:23:01.000000 mth5-0.4.3/mth5.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2024-04-12 22:23:01.000000 mth5-0.4.3/mth5.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-12 22:23:01.000000 mth5-0.4.3/mth5.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-12 22:23:06.264196 mth5-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2024-04-12 22:10:12.000000 mth5-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.146403 mth5-0.4.3/tests/
+-rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.215409 mth5-0.4.3/tests/clients/
+-rw-rw-rw-   0        0        0        0 2023-04-15 00:16:51.000000 mth5-0.4.3/tests/clients/__init__.py
+-rw-rw-rw-   0        0        0     4696 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/clients/test_geomag.py
+-rw-rw-rw-   0        0        0    12543 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/clients/test_geomag_client.py
+-rw-rw-rw-   0        0        0     2600 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/clients/test_makemth5.py
+-rw-rw-rw-   0        0        0     9178 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/example_lemi.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.231037 mth5-0.4.3/tests/helpers/
+-rw-rw-rw-   0        0        0     2776 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/helpers/test_initialize_mth5.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.262280 mth5-0.4.3/tests/io/
+-rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/__init__.py
+-rw-rw-rw-   0        0        0     9178 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/example_lemi.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.321421 mth5-0.4.3/tests/io/lemi/
+-rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/lemi/__init__.py
+-rw-rw-rw-   0        0        0    17660 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/lemi/test_lemi.py
+-rw-rw-rw-   0        0        0     4066 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/lemi/test_lemi_collection.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.385976 mth5-0.4.3/tests/io/nims/
+-rw-rw-rw-   0        0        0     3062 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/nims/test_nims_collection.py
+-rw-rw-rw-   0        0        0     6133 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/nims/test_nims_gps.py
+-rw-rw-rw-   0        0        0     3551 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/nims/test_nims_response.py
+-rw-rw-rw-   0        0        0    19225 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/nims/test_read_nims.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.515847 mth5-0.4.3/tests/io/phoenix/
+-rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/phoenix/__init__.py
+-rw-rw-rw-   0        0        0    37444 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/example_rxcal.json
+-rw-rw-rw-   0        0        0    13710 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_base_reader.py
+-rw-rw-rw-   0        0        0     3982 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_phoenix_collection.py
+-rw-rw-rw-   0        0        0     2922 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_phx_calibration.py
+-rw-rw-rw-   0        0        0     7934 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_read_phoenix_continuous.py
+-rw-rw-rw-   0        0        0     8809 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_read_phoenix_native.py
+-rw-rw-rw-   0        0        0     8644 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/phoenix/test_read_phoenix_segmented.py
+-rw-rw-rw-   0        0        0     1940 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/test_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.578339 mth5-0.4.3/tests/io/usgs_ascii/
+-rw-rw-rw-   0        0        0     2874 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/usgs_ascii/test_ascii.py
+-rw-rw-rw-   0        0        0     3131 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/usgs_ascii/test_ascii_collection.py
+-rw-rw-rw-   0        0        0    13936 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/usgs_ascii/test_header.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.678585 mth5-0.4.3/tests/io/zen/
+-rw-rw-rw-   0        0        0       35 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/zen/__init__.py
+-rw-rw-rw-   0        0        0    27603 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/zen/test_z3d.py
+-rw-rw-rw-   0        0        0     3142 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/zen/test_z3d_collection.py
+-rw-rw-rw-   0        0        0     4581 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/zen/test_z3d_header.py
+-rw-rw-rw-   0        0        0    14131 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/zen/test_z3d_metadata.py
+-rw-rw-rw-   0        0        0     3481 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/io/zen/test_z3d_schedule.py
+-rw-rw-rw-   0        0        0     3681 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/io/zen/test_zen_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.716337 mth5-0.4.3/tests/tables/
+-rw-rw-rw-   0        0        0      349 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/tables/__init__.py
+-rw-rw-rw-   0        0        0     8484 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/tables/test_mth5_table.py
+-rw-rw-rw-   0        0        0     5742 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/test_channel_slice.py
+-rw-rw-rw-   0        0        0     7583 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/test_mth5_basics.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.856753 mth5-0.4.3/tests/timeseries/
+-rw-rw-rw-   0        0        0    33626 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_channel_ts.py
+-rw-rw-rw-   0        0        0     3466 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_remove_response.py
+-rw-rw-rw-   0        0        0    31650 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_runts.py
+-rw-rw-rw-   0        0        0     4909 2024-01-25 19:34:44.000000 mth5-0.4.3/tests/timeseries/test_runts_02.py
+-rw-rw-rw-   0        0        0     7698 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_ts_filters.py
+-rw-rw-rw-   0        0        0     4693 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_ts_helpers.py
+-rw-rw-rw-   0        0        0     2619 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/timeseries/test_xr_scipy.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:05.888000 mth5-0.4.3/tests/utils/
+-rw-rw-rw-   0        0        0     5613 2023-03-27 21:53:08.000000 mth5-0.4.3/tests/utils/test_fdsn_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:06.093937 mth5-0.4.3/tests/version_1/
+-rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.3/tests/version_1/__init__.py
+-rw-rw-rw-   0        0        0     8050 2022-07-05 20:34:49.000000 mth5-0.4.3/tests/version_1/expected.csv
+-rw-rw-rw-   0        0        0   105049 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test1_dec_level_3.csv
+-rw-rw-rw-   0        0        0    12546 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_build_from_experiment.py
+-rw-rw-rw-   0        0        0    12298 2024-04-12 22:09:24.000000 mth5-0.4.3/tests/version_1/test_fcs.py
+-rw-rw-rw-   0        0        0     3491 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_filters.py
+-rw-rw-rw-   0        0        0     3756 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_from_fap_stationxml.py
+-rw-rw-rw-   0        0        0     7288 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_from_stationxml.py
+-rw-rw-rw-   0        0        0    11581 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_make_mth5.py
+-rw-rw-rw-   0        0        0    18537 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_make_mth5_geomag.py
+-rw-rw-rw-   0        0        0    10723 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_make_mth5_ofr.py
+-rw-rw-rw-   0        0        0    17171 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_mth5.py
+-rw-rw-rw-   0        0        0    15229 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_1/test_transfer_function.py
+drwxrwxrwx   0        0        0        0 2024-04-12 22:23:06.264196 mth5-0.4.3/tests/version_2/
+-rw-rw-rw-   0        0        0       35 2022-07-05 20:34:49.000000 mth5-0.4.3/tests/version_2/__init__.py
+-rw-rw-rw-   0        0        0    13449 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_build_from_experiment.py
+-rw-rw-rw-   0        0        0     3587 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_filters.py
+-rw-rw-rw-   0        0        0     4458 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_from_fap_stationxml.py
+-rw-rw-rw-   0        0        0     6995 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_from_stationxml.py
+-rw-rw-rw-   0        0        0    12452 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_make_mth5.py
+-rw-rw-rw-   0        0        0    18785 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_make_mth5_geomag.py
+-rw-rw-rw-   0        0        0    18849 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_mth5.py
+-rw-rw-rw-   0        0        0    14352 2024-02-29 19:32:30.000000 mth5-0.4.3/tests/version_2/test_transfer_function.py
```

### Comparing `mth5-0.4.2/AUTHORS.rst` & `mth5-0.4.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/CONTRIBUTING.rst` & `mth5-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/HISTORY.rst` & `mth5-0.4.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/LICENSE` & `mth5-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/LICENSE.md` & `mth5-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/PKG-INFO` & `mth5-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mth5
-Version: 0.4.2
+Version: 0.4.3
 Summary: Archivable and exchangeable format for magnetotelluric data
 Home-page: https://github.com/kujaku11/mth5
 Author: Jared Peacock
 Author-email: jpeacock@usgs.gov
 License: MIT license
 Keywords: mth5
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,15 +35,15 @@
 
 MTH5 is an HDF5 data container for magnetotelluric time series data, but could be extended to other data types.  This package provides tools for reading/writing/manipulating MTH5 files.
 
 MTH5 uses [h5py](https://www.h5py.org/) to interact with the HDF5 file, [xarray](http://xarray.pydata.org/en/stable/) to interact with the data in a nice way, and all metadata use [mt_metadata](https://github.com/kujaku11/mt_metadata). 
 This project is in cooperation with the Incorporated Research Institutes of Seismology, the U.S. Geological Survey, and other collaborators.  Facilities of the IRIS Consortium are supported by the National Science Foundationâ€™s Seismological Facilities for the Advancement of Geoscience (SAGE) Award under Cooperative Support Agreement EAR-1851048.  USGS is partially funded through the Community for Data Integration and IMAGe through the Minerals Resources Program.  
 
 
-* **Version**: 0.4.2
+* **Version**: 0.4.3
 * **Free software**: MIT license
 * **Documentation**: https://mth5.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **docs/examples/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 Features
```

### Comparing `mth5-0.4.2/README.md` & `mth5-0.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 MTH5 is an HDF5 data container for magnetotelluric time series data, but could be extended to other data types.  This package provides tools for reading/writing/manipulating MTH5 files.
 
 MTH5 uses [h5py](https://www.h5py.org/) to interact with the HDF5 file, [xarray](http://xarray.pydata.org/en/stable/) to interact with the data in a nice way, and all metadata use [mt_metadata](https://github.com/kujaku11/mt_metadata). 
 This project is in cooperation with the Incorporated Research Institutes of Seismology, the U.S. Geological Survey, and other collaborators.  Facilities of the IRIS Consortium are supported by the National Science Foundation’s Seismological Facilities for the Advancement of Geoscience (SAGE) Award under Cooperative Support Agreement EAR-1851048.  USGS is partially funded through the Community for Data Integration and IMAGe through the Minerals Resources Program.  
 
 
-* **Version**: 0.4.2
+* **Version**: 0.4.3
 * **Free software**: MIT license
 * **Documentation**: https://mth5.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **docs/examples/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 Features
```

### Comparing `mth5-0.4.2/docs/.ipynb_checkpoints/index-checkpoint.rst` & `mth5-0.4.3/docs/.ipynb_checkpoints/index-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/Makefile` & `mth5-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/README.rst` & `mth5-0.4.3/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 MTH5 is an HDF5 data container for magnetotelluric time series data, but could be extended to other data types.  This package provides tools for reading/writing/manipulating MTH5 files.
 
 MTH5 uses `h5py <https://www.h5py.org/>`_ to interact with the HDF5 file, `xarray <http://xarray.pydata.org/en/stable/>`_ to interact with the data in a nice way, and all metadata use `mt_metadata <https://github.com/kujaku11/mt_metadata>`_. 
 
 This project is in cooperation with the Incorporated Research Institutes of Seismology, the U.S. Geological Survey, and other collaborators.  Facilities of the IRIS Consortium are supported by the National Science Foundation’s Seismological Facilities for the Advancement of Geoscience (SAGE) Award under Cooperative Support Agreement EAR-1851048.  USGS is partially funded through the Community for Data Integration and IMAGe through the Minerals Resources Program.  
 
-* **Version**: 0.4.2
+* **Version**: 0.4.3
 * **Free software**: MIT license
 * **Documentation**: `<https://mth5.readthedocs.io>`_.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **docs/examples/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 Features
```

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_14_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_14_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_18_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_channel_ts_example_18_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_10_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_10_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_14_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_18_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_18_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_23_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_23_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_28_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_28_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_6_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_filters_example_6_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_29_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_29_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_30_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_30_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_33_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_33_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_35_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.1.0_35_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_29_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_29_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_30_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_30_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_33_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_33_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_35_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_35_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_3.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_43_3.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_45_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_driver_v0.2.0_45_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_geomag_12_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_geomag_12_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_nims_16_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_make_mth5_from_nims_16_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_15_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_15_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_16_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_16_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_17_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_17_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_19_1.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_19_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_2.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_2.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_4.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_remove_instrument_response_example_24_4.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/doctrees/nbsphinx/examples_notebooks_run_ts_example_14_0.png` & `mth5-0.4.3/docs/_build/doctrees/nbsphinx/examples_notebooks_run_ts_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/cas04_run_a_plot.png` & `mth5-0.4.3/docs/_build/html/_images/cas04_run_a_plot.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/cas04_run_a_plot_zoom.png` & `mth5-0.4.3/docs/_build/html/_images/cas04_run_a_plot_zoom.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_channel_ts_example_14_1.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_channel_ts_example_14_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_channel_ts_example_18_1.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_channel_ts_example_18_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_10_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_10_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_14_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_18_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_18_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_23_1.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_23_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_28_1.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_28_1.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_filters_example_6_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_filters_example_6_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_make_mth5_from_geomag_12_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_make_mth5_from_geomag_12_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_make_mth5_from_nims_16_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_make_mth5_from_nims_16_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_15_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_15_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_16_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_remove_instrument_response_example_16_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/examples_notebooks_run_ts_example_14_0.png` & `mth5-0.4.3/docs/_build/html/_images/examples_notebooks_run_ts_example_14_0.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_images/mth5_logo.png` & `mth5-0.4.3/docs/_build/html/_images/mth5_logo.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/_build/html/_static/mth5_logo.png` & `mth5-0.4.3/docs/_build/html/_static/mth5_logo.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/conf.py` & `mth5-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/index.rst` & `mth5-0.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/make.bat` & `mth5-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/conventions.rst` & `mth5-0.4.3/docs/source/conventions.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/file_readers.rst` & `mth5-0.4.3/docs/source/file_readers.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/gotchas.rst` & `mth5-0.4.3/docs/source/gotchas.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/images/cas04_run_a_plot.png` & `mth5-0.4.3/docs/source/images/cas04_run_a_plot.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/images/cas04_run_a_plot_zoom.png` & `mth5-0.4.3/docs/source/images/cas04_run_a_plot_zoom.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/images/example_mt_file_structure.png` & `mth5-0.4.3/docs/source/images/example_mt_file_structure.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/images/example_mt_file_structure_v2.png` & `mth5-0.4.3/docs/source/images/example_mt_file_structure_v2.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/images/mth5_logo.png` & `mth5-0.4.3/docs/source/images/mth5_logo.png`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/installation.rst` & `mth5-0.4.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.groups.filter_groups.rst` & `mth5-0.4.3/docs/source/mth5.groups.filter_groups.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.groups.rst` & `mth5-0.4.3/docs/source/mth5.groups.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.lemi.rst` & `mth5-0.4.3/docs/source/mth5.io.lemi.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.nims.rst` & `mth5-0.4.3/docs/source/mth5.io.nims.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.phoenix.readers.contiguous.rst` & `mth5-0.4.3/docs/source/mth5.io.phoenix.readers.contiguous.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.phoenix.readers.rst` & `mth5-0.4.3/docs/source/mth5.io.phoenix.readers.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.phoenix.readers.segmented.rst` & `mth5-0.4.3/docs/source/mth5.io.phoenix.readers.segmented.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.phoenix.rst` & `mth5-0.4.3/docs/source/mth5.io.phoenix.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.rst` & `mth5-0.4.3/docs/source/mth5.io.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.io.zen.rst` & `mth5-0.4.3/docs/source/mth5.io.zen.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.rst` & `mth5-0.4.3/docs/source/mth5.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.tables.rst` & `mth5-0.4.3/docs/source/mth5.tables.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.timeseries.rst` & `mth5-0.4.3/docs/source/mth5.timeseries.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/mth5.utils.rst` & `mth5-0.4.3/docs/source/mth5.utils.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/runs.rst` & `mth5-0.4.3/docs/source/runs.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/stations.rst` & `mth5-0.4.3/docs/source/stations.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/structure.rst` & `mth5-0.4.3/docs/source/structure.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/surveys.rst` & `mth5-0.4.3/docs/source/surveys.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/ts.rst` & `mth5-0.4.3/docs/source/ts.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/usage.rst` & `mth5-0.4.3/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/docs/source/usage_v2.rst` & `mth5-0.4.3/docs/source/usage_v2.rst`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/__init__.py` & `mth5-0.4.3/mth5/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # =============================================================================
 # Package Variables
 # =============================================================================
 
 __author__ = """Jared Peacock"""
 __email__ = "jpeacock@usgs.gov"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 
 # =============================================================================
 # Initialize Loggers
 # =============================================================================
 config = {
     "handlers": [
@@ -42,14 +42,15 @@
 xr.set_options(keep_attrs=True)
 
 # =============================================================================
 # Defualt Parameters
 # =============================================================================
 CHUNK_SIZE = 8196
 ACCEPTABLE_FILE_TYPES = ["mth5", "MTH5", "h5", "H5"]
+ACCEPTABLE_FILE_SUFFIXES = [f".{x}" for x in ACCEPTABLE_FILE_TYPES]
 ACCEPTABLE_FILE_VERSIONS = ["0.1.0", "0.2.0"]
 ACCEPTABLE_DATA_LEVELS = [0, 1, 2, 3]
 
 ### transfer function summary table dtype
 TF_DTYPE_LIST = [
     ("station", "S30"),
     ("survey", "S50"),
```

### Comparing `mth5-0.4.2/mth5/clients/fdsn.py` & `mth5-0.4.3/mth5/clients/fdsn.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/clients/geomag.py` & `mth5-0.4.3/mth5/clients/geomag.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/clients/make_mth5.py` & `mth5-0.4.3/mth5/clients/make_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/clients/phoenix.py` & `mth5-0.4.3/mth5/clients/zen.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,37 +7,51 @@
 
 # ## Imports
 
 # =============================================================================
 # Imports
 # =============================================================================
 from pathlib import Path
+from loguru import logger
 
 from mth5.mth5 import MTH5
 from mth5 import read_file
-from mth5.io.phoenix import PhoenixCollection
+from mth5.io.zen import Z3DCollection
 
 # =============================================================================
 
 
-class PhoenixClient:
+class ZenClient:
     def __init__(
         self,
         data_path,
-        sample_rates=[130, 24000],
+        sample_rates=[4096, 1024, 256],
         save_path=None,
         calibration_path=None,
+        **kwargs,
     ):
+        self.logger = logger
         self.data_path = data_path
         self.sample_rates = sample_rates
+        self.mth5_filename = "from_zen.h5"
         self.save_path = save_path
-        self.mth5_filename = "from_phoenix.h5"
         self.calibration_path = calibration_path
 
-        self.collection = PhoenixCollection(self.data_path)
+        self.mth5_version = "0.2.0"
+        self.interact = False
+        self.compression = "gzip"
+        self.compression_opts = 4
+        self.shuffle = True
+        self.fletcher32 = True
+        self.data_level = 1
+
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+        self.collection = Z3DCollection(self.data_path)
 
     @property
     def data_path(self):
         """Path to phoenix data"""
         return self._data_path
 
     @data_path.setter
@@ -52,15 +66,15 @@
         """
 
         if value is not None:
             self._data_path = Path(value)
             if not self._data_path.exists():
                 raise IOError(f"Could not find {self._data_path}")
 
-            self.collection = PhoenixCollection(self.data_path)
+            self.collection = Z3DCollection(self.data_path)
 
         else:
             raise ValueError("data_path cannot be None")
 
     @property
     def calibration_path(self):
         """Path to calibration data"""
@@ -99,20 +113,20 @@
         :type value: TYPE
         :return: DESCRIPTION
         :rtype: TYPE
 
         """
 
         if isinstance(value, (int, float)):
-            self._value = [value]
+            self._sample_rates = [value]
         elif isinstance(value, str):
-            self._value = [float(v) for v in value.split(",")]
+            self._sample_rates = [float(v) for v in value.split(",")]
 
         elif isinstance(value, (tuple, list)):
-            self._value = [float(v) for v in value]
+            self._sample_rates = [float(v) for v in value]
         else:
             raise TypeError(f"Cannot parse {type(value)}")
 
     @property
     def save_path(self):
         """Path to save mth5"""
         return self._save_path
@@ -141,17 +155,39 @@
         Get Run information
 
         :return: DESCRIPTION
         :rtype: TYPE
 
         """
 
-        return self.collection.get_runs(sample_rates=self.sample_rates)
+        return self.collection.get_runs(
+            sample_rates=self.sample_rates,
+            calibration_path=self.calibration_path,
+        )
+
+    def get_survey(self, station_dict):
+        """
+        get survey name from a dictionary of a single station of runs
+        :param station_dict: DESCRIPTION
+        :type station_dict: TYPE
+        :return: DESCRIPTION
+        :rtype: TYPE
 
-    def make_mth5_from_phoenix(self, **kwargs):
+        """
+
+        return list(
+            set(
+                [
+                    station_dict[k].survey.unique()[0]
+                    for k in station_dict.keys()
+                ]
+            )
+        )[0]
+
+    def make_mth5_from_zen(self, survey_id=None, combine=True, **kwargs):
         """
         Make an MTH5 from Phoenix files.  Split into runs, account for filters
 
         :param data_path: DESCRIPTION, defaults to None
         :type data_path: TYPE, optional
         :param sample_rates: DESCRIPTION, defaults to None
         :type sample_rates: TYPE, optional
@@ -162,46 +198,57 @@
 
         """
 
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
-        run_dict = self.get_run_dict()
+        runs = self.get_run_dict()
 
         with MTH5() as m:
-            m.open_mth5(self.save_path, "w")
-
-            for station_id, station_dict in run_dict.items():
-                survey_metadata = self.collection.metadata_dict[
-                    station_id
-                ].survey_metadata
-                survey_group = m.add_survey(survey_metadata.id)
+            m.file_version = self.file_version
+            m.compression = self.compression
+            m.compression_opts = self.comporession_opts
+            m.shuffle = self.shuffle
+            m.fletcher32 = self.fletcher32
+            m.data_level = self.data_level
 
-                station_metadata = self.collection.metadata_dict[
-                    station_id
-                ].station_metadata
+            m.open_mth5(self.save_path, "w")
+            for station_id, station_dict in runs.items():
+                if survey_id is None:
+                    survey_id = self.get_survey(station_dict)
+                survey_group = m.add_survey(survey_id)
                 station_group = survey_group.stations_group.add_station(
-                    station_metadata.id, station_metadata=station_metadata
+                    station_id
+                )
+                station_group.metadata.update(
+                    self.collection.station_metadata_dict[station_id]
                 )
+                station_group.write_metadata()
+                if combine:
+                    run_list = []
                 for run_id, run_df in station_dict.items():
-                    run_metadata = self.collection.metadata_dict[
-                        station_id
-                    ].run_metadata
-                    run_metadata.id = run_id
-                    run_metadata.sample_rate = float(
-                        run_df.sample_rate.unique()[0]
-                    )
-
-                    run_group = station_group.add_run(
-                        run_metadata.id, run_metadata=run_metadata
-                    )
+                    run_group = station_group.add_run(run_id)
                     for row in run_df.itertuples():
-                        ch_ts = read_file(row.fn)
-
-                        # add channel to the run group
+                        ch_ts = read_file(
+                            row.fn,
+                            calibration_fn=row.calibration_fn,
+                        )
                         run_group.from_channel_ts(ch_ts)
-
                     run_group.update_metadata()
-
-            station_group.update_metadata()
+                    if combine:
+                        run_list.append(run_group.to_runts())
+                if combine:
+                    # Combine runs and down sample to 1 second.
+                    combined_run = run_list[0].merge(
+                        run_list[1:], new_sample_rate=1
+                    )
+                    combined_run.run_metadata.id = "sr1_0001"
+                    combined_run_group = station_group.add_run("sr1_0001")
+                    combined_run_group.from_runts(combined_run)
+                    combined_run_group.update_metadata()
+                station_group.update_metadata()
             survey_group.update_metadata()
+
+        self.logger.info(f"Wrote MTH5 file to: {self.save_path}")
+
+        return self.save_path
```

### Comparing `mth5-0.4.2/mth5/groups/__init__.py` & `mth5-0.4.3/mth5/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/base.py` & `mth5-0.4.3/mth5/groups/base.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/channel_dataset.py` & `mth5-0.4.3/mth5/groups/channel_dataset.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/estimate_dataset.py` & `mth5-0.4.3/mth5/groups/estimate_dataset.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/experiment.py` & `mth5-0.4.3/mth5/groups/experiment.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/fc_dataset.py` & `mth5-0.4.3/mth5/groups/fc_dataset.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filter_groups/coefficient_filter_group.py` & `mth5-0.4.3/mth5/groups/filter_groups/coefficient_filter_group.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filter_groups/fap_filter_group.py` & `mth5-0.4.3/mth5/groups/filter_groups/fap_filter_group.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filter_groups/fir_filter_group.py` & `mth5-0.4.3/mth5/groups/filter_groups/fir_filter_group.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filter_groups/time_delay_filter_group.py` & `mth5-0.4.3/mth5/groups/filter_groups/time_delay_filter_group.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filter_groups/zpk_filter_group.py` & `mth5-0.4.3/mth5/groups/filter_groups/zpk_filter_group.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/filters.py` & `mth5-0.4.3/mth5/groups/filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/fourier_coefficients.py` & `mth5-0.4.3/mth5/groups/fourier_coefficients.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,22 +429,24 @@
                     self.remove_channel(ch)
                 # time index should be the first index
                 if data_array[ch].time.size == data_array[ch].shape[0]:
                     self.add_channel(
                         ch,
                         fc_data=data_array[ch].to_numpy(),
                         fc_metadata=ch_metadata,
+                        dtype=data_array[ch].dtype,
                     )
                 elif data_array[ch].time.size == data_array[ch].shape[1]:
                     self.add_channel(
                         ch,
                         fc_data=data_array[ch].to_numpy().T,
                         fc_metadata=ch_metadata,
+                        dtype=data_array[ch].dtype,
                     )
-        return 
+        return
 
     def to_xarray(self, channels=None):
         """
         create an xarray dataset from the desired channels. If none grabs all
         channels in the decimation level.
 
         :param channels: DESCRIPTION, defaults to None
@@ -490,14 +492,15 @@
     def add_channel(
         self,
         fc_name,
         fc_data=None,
         fc_metadata=None,
         max_shape=(None, None),
         chunks=True,
+        dtype=complex,
         **kwargs,
     ):
         """
 
         Add a set of Fourier coefficients for a single channel at a single
         decimation level for a processing run.
 
@@ -544,20 +547,20 @@
                     "Need to input a numpy.array, xarray.DataArray, "
                     f"xr.Dataset, pd.DataFrame not {type(fc_data)}"
                 )
                 self.logger.exception(msg)
                 raise TypeError(msg)
         else:
             chunks = True
-            fc_data = np.zeros((1, 1), dtype=complex)
+            fc_data = np.zeros((1, 1), dtype=dtype)
         try:
             dataset = self.hdf5_group.create_dataset(
                 fc_name,
                 data=fc_data,
-                dtype=complex,
+                dtype=dtype,
                 chunks=chunks,
                 maxshape=max_shape,
                 **self.dataset_options,
             )
 
             fc_dataset = FCChannelDataset(dataset, dataset_metadata=fc_metadata)
         except (OSError, RuntimeError, ValueError) as error:
```

### Comparing `mth5-0.4.2/mth5/groups/reports.py` & `mth5-0.4.3/mth5/groups/reports.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/run.py` & `mth5-0.4.3/mth5/groups/run.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/standards.py` & `mth5-0.4.3/mth5/groups/standards.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/station.py` & `mth5-0.4.3/mth5/groups/station.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/survey.py` & `mth5-0.4.3/mth5/groups/survey.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/groups/transfer_function.py` & `mth5-0.4.3/mth5/groups/transfer_function.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/helpers.py` & `mth5-0.4.3/mth5/helpers.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/collection.py` & `mth5-0.4.3/mth5/io/collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/lemi/lemi424.py` & `mth5-0.4.3/mth5/io/lemi/lemi424.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/lemi/lemi_collection.py` & `mth5-0.4.3/mth5/io/lemi/lemi_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/miniseed/miniseed.py` & `mth5-0.4.3/mth5/io/miniseed/miniseed.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/nims/gps.py` & `mth5-0.4.3/mth5/io/nims/gps.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/nims/header.py` & `mth5-0.4.3/mth5/io/nims/header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/nims/nims.py` & `mth5-0.4.3/mth5/io/nims/nims.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/nims/nims_collection.py` & `mth5-0.4.3/mth5/io/nims/nims_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/nims/response_filters.py` & `mth5-0.4.3/mth5/io/nims/response_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/phoenix_collection.py` & `mth5-0.4.3/mth5/io/phoenix/phoenix_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,20 +114,27 @@
 
         station_folders = self._locate_station_folders()
 
         entries = []
         for folder in station_folders:
             rec_fn = folder.joinpath(self._receiver_metadata_name)
             receiver_metadata = self._read_receiver_metadata_json(rec_fn)
-            self.metadata_dict[
-                receiver_metadata.station_metadata.id
-            ] = receiver_metadata
+            self.metadata_dict[receiver_metadata.station_metadata.id] = (
+                receiver_metadata
+            )
 
             for sr in sample_rates:
-                for fn in folder.rglob(f"*{self._file_extension_map[int(sr)]}"):
+                for fn in folder.rglob(
+                    f"*{self._file_extension_map[int(sr)]}"
+                ):
+                    if "calibration" in fn.as_posix().lower():
+                        self.logger.debug(
+                            f"skipping calibration time series {fn}"
+                        )
+                        continue
                     try:
                         phx_obj = open_phoenix(fn)
                     except OSError:
                         self.logger.warning(f"Skipping {fn.name}")
                         continue
                     if hasattr(phx_obj, "read_segment"):
                         segment = phx_obj.read_segment(metadata_only=True)
@@ -200,15 +207,17 @@
                 if sr < 1000:
                     sdf = rdf.loc[
                         (rdf.station == station) & (rdf.sample_rate == sr)
                     ].sort_values("sequence_number")
                     starts = np.sort(
                         sdf.loc[sdf.sample_rate == sr].start.unique()
                     )
-                    ends = np.sort(sdf.loc[sdf.sample_rate == sr].end.unique())
+                    ends = np.sort(
+                        sdf.loc[sdf.sample_rate == sr].end.unique()
+                    )
 
                     # find any breaks in the data
                     diff = ends[0:-1] - starts[1:]
                     diff = diff.astype("timedelta64[s]").astype(float)
 
                     breaks = np.nonzero(diff)[0]
 
@@ -225,15 +234,16 @@
                                 & (rdf.start == start_breaks[ii])
                                 & (rdf.sample_rate == sr),
                                 "run",
                             ] = f"sr{run_stem}_{count:0{zeros}}"
 
                     else:
                         rdf.loc[
-                            (rdf.station == station) & (rdf.sample_rate == sr),
+                            (rdf.station == station)
+                            & (rdf.sample_rate == sr),
                             "run",
                         ] = f"sr{run_stem}_{count:0{zeros}}"
 
                 # segmented data
                 else:
 
                     starts = rdf.loc[
```

### Comparing `mth5-0.4.2/mth5/io/phoenix/read.py` & `mth5-0.4.3/mth5/io/phoenix/read.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/__init__.py` & `mth5-0.4.3/mth5/io/phoenix/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/base.py` & `mth5-0.4.3/mth5/io/phoenix/readers/base.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/calibrations.py` & `mth5-0.4.3/mth5/io/phoenix/readers/calibrations.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/config.py` & `mth5-0.4.3/mth5/io/phoenix/readers/config.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/contiguous/decimated_continuous_reader.py` & `mth5-0.4.3/mth5/io/phoenix/readers/contiguous/decimated_continuous_reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/header.py` & `mth5-0.4.3/mth5/io/phoenix/readers/header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/helpers.py` & `mth5-0.4.3/mth5/io/phoenix/readers/helpers.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/native/native_reader.py` & `mth5-0.4.3/mth5/io/phoenix/readers/native/native_reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/receiver_metadata.py` & `mth5-0.4.3/mth5/io/phoenix/readers/receiver_metadata.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/phoenix/readers/segmented/decimated_segmented_reader.py` & `mth5-0.4.3/mth5/io/phoenix/readers/segmented/decimated_segmented_reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/reader.py` & `mth5-0.4.3/mth5/io/reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/usgs_ascii/header.py` & `mth5-0.4.3/mth5/io/usgs_ascii/header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/usgs_ascii/usgs_ascii.py` & `mth5-0.4.3/mth5/io/usgs_ascii/usgs_ascii.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/usgs_ascii/usgs_ascii_collection.py` & `mth5-0.4.3/mth5/io/usgs_ascii/usgs_ascii_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/coil_response.py` & `mth5-0.4.3/mth5/io/zen/coil_response.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/z3d_collection.py` & `mth5-0.4.3/mth5/io/zen/z3d_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/z3d_header.py` & `mth5-0.4.3/mth5/io/zen/z3d_header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/z3d_metadata.py` & `mth5-0.4.3/mth5/io/zen/z3d_metadata.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/z3d_schedule.py` & `mth5-0.4.3/mth5/io/zen/z3d_schedule.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/zen.py` & `mth5-0.4.3/mth5/io/zen/zen.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/io/zen/zen_tools.py` & `mth5-0.4.3/mth5/io/zen/zen_tools.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/mth5.py` & `mth5-0.4.3/mth5/mth5.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from mth5 import __version__ as mth5_version
 from mth5 import groups
 from mth5.tables import ChannelSummaryTable, TFSummaryTable
 from mth5 import helpers
 from mth5 import (
     CHANNEL_DTYPE,
     TF_DTYPE,
+    ACCEPTABLE_FILE_SUFFIXES,
     ACCEPTABLE_FILE_TYPES,
     ACCEPTABLE_FILE_VERSIONS,
     ACCEPTABLE_DATA_LEVELS,
 )
 
 from mt_metadata.utils.mttime import get_now_utc
 from mt_metadata.timeseries import Experiment
@@ -330,15 +331,15 @@
     @filename.setter
     def filename(self, value):
         """make sure file has the proper extension"""
         self.__filename = None
         if value is not None:
             if not isinstance(value, Path):
                 value = Path(value)
-            if value.suffix not in ACCEPTABLE_FILE_TYPES:
+            if value.suffix not in ACCEPTABLE_FILE_SUFFIXES:
                 msg = (
                     f"file extension {value.suffix} is not correct. "
                     "Changing to default .h5"
                 )
                 self.logger.info(msg)
                 self.__filename = value.with_suffix(".h5")
             else:
```

### Comparing `mth5-0.4.2/mth5/tables/channel_table.py` & `mth5-0.4.3/mth5/tables/channel_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,16 +43,20 @@
             "station",
             "run",
             "component",
             "measurement_type",
             "units",
         ]:
             setattr(df, key, getattr(df, key).str.decode("utf-8"))
-        df.start = pd.to_datetime(df.start.str.decode("utf-8"), format="mixed")
-        df.end = pd.to_datetime(df.end.str.decode("utf-8"), format="mixed")
+        try:
+            df.start = pd.to_datetime(df.start.str.decode("utf-8"), format="mixed")
+            df.end = pd.to_datetime(df.end.str.decode("utf-8"), format="mixed")
+        except ValueError:
+            df.start = pd.to_datetime(df.start.str.decode("utf-8"))
+            df.end = pd.to_datetime(df.end.str.decode("utf-8"))
 
         return df
 
     def summarize(self):
         """
 
         :return: DESCRIPTION
```

### Comparing `mth5-0.4.2/mth5/tables/mth5_table.py` & `mth5-0.4.3/mth5/tables/mth5_table.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/tables/tf_table.py` & `mth5-0.4.3/mth5/tables/tf_table.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/timeseries/channel_ts.py` & `mth5-0.4.3/mth5/timeseries/channel_ts.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/timeseries/run_ts.py` & `mth5-0.4.3/mth5/timeseries/run_ts.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/timeseries/scipy_filters.py` & `mth5-0.4.3/mth5/timeseries/scipy_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/timeseries/ts_filters.py` & `mth5-0.4.3/mth5/timeseries/ts_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/timeseries/ts_helpers.py` & `mth5-0.4.3/mth5/timeseries/ts_helpers.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/utils/fdsn_tools.py` & `mth5-0.4.3/mth5/utils/fdsn_tools.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/mth5/utils/helpers.py` & `mth5-0.4.3/mth5/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,18 @@
 def get_channel_summary(m, show=True):
     """
     :param mth5_path:
     :return:
     """
     logger.info(f"{m.filename} channel summary")
     df = m.channel_summary.to_dataframe()
+    if len(df) <= 1:
+        logger.warning("channel summary smaller than expected -- re-summarizing")
+        m.channel_summary.summarize()
+        df = m.channel_summary.to_dataframe()
     if show:
         logger.info(f"{df}")
     return df
 
 
 @path_or_mth5_object
 def add_filters(m, filters_list, survey_id=""):
```

### Comparing `mth5-0.4.2/mth5.egg-info/PKG-INFO` & `mth5-0.4.3/mth5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mth5
-Version: 0.4.2
+Version: 0.4.3
 Summary: Archivable and exchangeable format for magnetotelluric data
 Home-page: https://github.com/kujaku11/mth5
 Author: Jared Peacock
 Author-email: jpeacock@usgs.gov
 License: MIT license
 Keywords: mth5
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,15 +35,15 @@
 
 MTH5 is an HDF5 data container for magnetotelluric time series data, but could be extended to other data types.  This package provides tools for reading/writing/manipulating MTH5 files.
 
 MTH5 uses [h5py](https://www.h5py.org/) to interact with the HDF5 file, [xarray](http://xarray.pydata.org/en/stable/) to interact with the data in a nice way, and all metadata use [mt_metadata](https://github.com/kujaku11/mt_metadata). 
 This project is in cooperation with the Incorporated Research Institutes of Seismology, the U.S. Geological Survey, and other collaborators.  Facilities of the IRIS Consortium are supported by the National Science Foundationâ€™s Seismological Facilities for the Advancement of Geoscience (SAGE) Award under Cooperative Support Agreement EAR-1851048.  USGS is partially funded through the Community for Data Integration and IMAGe through the Minerals Resources Program.  
 
 
-* **Version**: 0.4.2
+* **Version**: 0.4.3
 * **Free software**: MIT license
 * **Documentation**: https://mth5.readthedocs.io.
 * **Examples**: Click the `Binder` badge above and Jupyter Notebook examples are in **docs/examples/notebooks**
 * **Suggested Citation**: Peacock, J. R., Kappler, K., Ronan, T., Heagy, L.,  Kelbert, A., Frassetto, A. (2022) MTH5: An archive and exchangeable data format for magnetotelluric time series data, *Computers & Geoscience*, **162**, doi:10.1016/j.cageo.2022.105102
 
 
 Features
```

### Comparing `mth5-0.4.2/mth5.egg-info/SOURCES.txt` & `mth5-0.4.3/mth5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/setup.py` & `mth5-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords="mth5",
     name="mth5",
     packages=find_packages(include=["mth5", "mth5.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/kujaku11/mth5",
-    version="0.4.2",
+    version="0.4.3",
     zip_safe=False,
 )
```

### Comparing `mth5-0.4.2/tests/clients/test_geomag.py` & `mth5-0.4.3/tests/clients/test_geomag.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/clients/test_geomag_client.py` & `mth5-0.4.3/tests/clients/test_geomag_client.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/clients/test_makemth5.py` & `mth5-0.4.3/tests/clients/test_makemth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/example_lemi.txt` & `mth5-0.4.3/tests/example_lemi.txt`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/helpers/test_initialize_mth5.py` & `mth5-0.4.3/tests/helpers/test_initialize_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/example_lemi.txt` & `mth5-0.4.3/tests/io/example_lemi.txt`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/lemi/test_lemi.py` & `mth5-0.4.3/tests/io/lemi/test_lemi.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/lemi/test_lemi_collection.py` & `mth5-0.4.3/tests/io/lemi/test_lemi_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/nims/test_nims_collection.py` & `mth5-0.4.3/tests/io/nims/test_nims_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/nims/test_nims_gps.py` & `mth5-0.4.3/tests/io/nims/test_nims_gps.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/nims/test_nims_response.py` & `mth5-0.4.3/tests/io/nims/test_nims_response.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/nims/test_read_nims.py` & `mth5-0.4.3/tests/io/nims/test_read_nims.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/example_rxcal.json` & `mth5-0.4.3/tests/io/phoenix/example_rxcal.json`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_base_reader.py` & `mth5-0.4.3/tests/io/phoenix/test_base_reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_phoenix_collection.py` & `mth5-0.4.3/tests/io/phoenix/test_phoenix_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_phx_calibration.py` & `mth5-0.4.3/tests/io/phoenix/test_phx_calibration.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_read_phoenix_continuous.py` & `mth5-0.4.3/tests/io/phoenix/test_read_phoenix_continuous.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_read_phoenix_native.py` & `mth5-0.4.3/tests/io/phoenix/test_read_phoenix_native.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/phoenix/test_read_phoenix_segmented.py` & `mth5-0.4.3/tests/io/phoenix/test_read_phoenix_segmented.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/test_reader.py` & `mth5-0.4.3/tests/io/test_reader.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/usgs_ascii/test_ascii.py` & `mth5-0.4.3/tests/io/usgs_ascii/test_ascii.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/usgs_ascii/test_ascii_collection.py` & `mth5-0.4.3/tests/io/usgs_ascii/test_ascii_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/usgs_ascii/test_header.py` & `mth5-0.4.3/tests/io/usgs_ascii/test_header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_z3d.py` & `mth5-0.4.3/tests/io/zen/test_z3d.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_z3d_collection.py` & `mth5-0.4.3/tests/io/zen/test_z3d_collection.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_z3d_header.py` & `mth5-0.4.3/tests/io/zen/test_z3d_header.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_z3d_metadata.py` & `mth5-0.4.3/tests/io/zen/test_z3d_metadata.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_z3d_schedule.py` & `mth5-0.4.3/tests/io/zen/test_z3d_schedule.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/io/zen/test_zen_tools.py` & `mth5-0.4.3/tests/io/zen/test_zen_tools.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/tables/test_mth5_table.py` & `mth5-0.4.3/tests/tables/test_mth5_table.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/test_channel_slice.py` & `mth5-0.4.3/tests/test_channel_slice.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/test_mth5_basics.py` & `mth5-0.4.3/tests/test_mth5_basics.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_channel_ts.py` & `mth5-0.4.3/tests/timeseries/test_channel_ts.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_remove_response.py` & `mth5-0.4.3/tests/timeseries/test_remove_response.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_runts.py` & `mth5-0.4.3/tests/timeseries/test_runts.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_runts_02.py` & `mth5-0.4.3/tests/timeseries/test_runts_02.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_ts_filters.py` & `mth5-0.4.3/tests/timeseries/test_ts_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_ts_helpers.py` & `mth5-0.4.3/tests/timeseries/test_ts_helpers.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/timeseries/test_xr_scipy.py` & `mth5-0.4.3/tests/timeseries/test_xr_scipy.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/utils/test_fdsn_tools.py` & `mth5-0.4.3/tests/utils/test_fdsn_tools.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/expected.csv` & `mth5-0.4.3/tests/version_1/expected.csv`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test1_dec_level_3.csv` & `mth5-0.4.3/tests/version_1/test1_dec_level_3.csv`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_build_from_experiment.py` & `mth5-0.4.3/tests/version_1/test_build_from_experiment.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_filters.py` & `mth5-0.4.3/tests/version_1/test_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_from_fap_stationxml.py` & `mth5-0.4.3/tests/version_1/test_from_fap_stationxml.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_from_stationxml.py` & `mth5-0.4.3/tests/version_1/test_from_stationxml.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_make_mth5.py` & `mth5-0.4.3/tests/version_1/test_make_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_make_mth5_geomag.py` & `mth5-0.4.3/tests/version_1/test_make_mth5_geomag.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_make_mth5_ofr.py` & `mth5-0.4.3/tests/version_1/test_make_mth5_ofr.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_mth5.py` & `mth5-0.4.3/tests/version_1/test_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_1/test_transfer_function.py` & `mth5-0.4.3/tests/version_1/test_transfer_function.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_build_from_experiment.py` & `mth5-0.4.3/tests/version_2/test_build_from_experiment.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_filters.py` & `mth5-0.4.3/tests/version_2/test_filters.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_from_fap_stationxml.py` & `mth5-0.4.3/tests/version_2/test_from_fap_stationxml.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_from_stationxml.py` & `mth5-0.4.3/tests/version_2/test_from_stationxml.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_make_mth5.py` & `mth5-0.4.3/tests/version_2/test_make_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_make_mth5_geomag.py` & `mth5-0.4.3/tests/version_2/test_make_mth5_geomag.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_mth5.py` & `mth5-0.4.3/tests/version_2/test_mth5.py`

 * *Files identical despite different names*

### Comparing `mth5-0.4.2/tests/version_2/test_transfer_function.py` & `mth5-0.4.3/tests/version_2/test_transfer_function.py`

 * *Files identical despite different names*

