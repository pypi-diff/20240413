# Comparing `tmp/aurora-0.3.6.tar.gz` & `tmp/aurora-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora-0.3.6.tar", last modified: Tue Nov  7 21:07:24 2023, max compression
+gzip compressed data, was "aurora-0.3.7.tar", last modified: Thu Nov  9 02:17:53 2023, max compression
```

## Comparing `aurora-0.3.6.tar` & `aurora-0.3.7.tar`

### file list

```diff
@@ -1,168 +1,186 @@
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.945517 aurora-0.3.6/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1063 2023-11-07 21:06:48.000000 aurora-0.3.6/LICENSE
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      245 2023-11-07 21:06:48.000000 aurora-0.3.6/MANIFEST.in
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1130 2023-11-07 21:07:24.945517 aurora-0.3.6/PKG-INFO
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      409 2023-11-07 21:06:48.000000 aurora-0.3.6/README.rst
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.929517 aurora-0.3.6/aurora/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       22 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/__init__.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.929517 aurora-0.3.6/aurora/config/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      142 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7283 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/config_creator.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.929517 aurora-0.3.6/aurora/config/emtf_band_setup/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      314 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/emtf_band_setup/__init__.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.929517 aurora-0.3.6/aurora/config/metadata/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      137 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/metadata/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1769 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/metadata/decimation_level.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5777 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/metadata/processing.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4985 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/config/metadata/station.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3878 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/general_helper_functions.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/pipelines/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11148 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/fourier_coefficients.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      819 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14821 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/process_mth5.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    12275 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/run_summary.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14296 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/time_series_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8622 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/transfer_function_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    25524 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/pipelines/transfer_function_kernel.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/sandbox/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1679 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/butterworth_filters.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1651 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/debug_mt_metadata_issue_85.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/sandbox/io_helpers/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4052 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/emtf_band_setup.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2410 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/fdsn_dataset.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5247 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/inventory_review.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3253 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/make_mth5_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14886 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/io_helpers/zfile_murphy.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2508 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/mth5_channel_summary_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5964 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/mth5_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2590 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/obspy_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8027 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/plot_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1721 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/sandbox/triage_metadata.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/time_series/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7905 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/apodization_window.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1466 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/decorators.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/time_series/filters/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/filters/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2460 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/filters/filter_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3457 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/frequency_band_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3316 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/time_axis_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    13627 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/window_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     6713 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/windowed_time_series.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    16797 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/windowing_scheme.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4246 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/time_series/xarray_helpers.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/transfer_function/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4144 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/TTFZ.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     9545 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/base.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4234 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/emtf_z_file_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    20433 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/kernel_dataset.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.933517 aurora-0.3.6/aurora/transfer_function/plot/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/plot/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3845 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/plot/comparison_plots.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1200 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/plot/error_bar_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      931 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/plot/rho_phi_helpers.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11579 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/plot/rho_plot.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/aurora/transfer_function/regression/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5489 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/TRME.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3406 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/TRME_RR.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    10816 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/base.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1478 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/helper_functions.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5089 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/iter_control.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11411 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/regression/m_estimator.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11707 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/transfer_function_collection.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/aurora/transfer_function/weights/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/weights/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4098 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/weights/coherence_weights.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     9650 2023-11-07 21:06:48.000000 aurora-0.3.6/aurora/transfer_function/weights/edf_weights.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.929517 aurora-0.3.6/aurora.egg-info/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1130 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/PKG-INFO
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4892 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/SOURCES.txt
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        1 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/dependency_links.txt
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        1 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/not-zip-safe
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       77 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/requires.txt
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        7 2023-11-07 21:07:24.000000 aurora-0.3.6/aurora.egg-info/top_level.txt
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/docs/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      634 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/Makefile
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/docs/api/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      189 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/api/general_helper_functions.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      232 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/api/index.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      494 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/api/pipelines.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1545 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/api/time_series.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1237 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/api/transfer_function.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3673 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/conf.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/docs/figures/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)   118395 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/figures/aurora_logo.png
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      503 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/index.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      795 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/make.bat
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/docs/user-docs/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      881 2023-11-07 21:06:48.000000 aurora-0.3.6/docs/user-docs/installing.rst
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       38 2023-11-07 21:07:24.945517 aurora-0.3.6/setup.cfg
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1530 2023-11-07 21:06:48.000000 aurora-0.3.6/setup.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/tests/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/__init__.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/tests/cas04/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5515 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/01_make_cas04_mth5.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11733 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/02b_process_cas04_mth5.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      229 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/band_setup_emtf_nims.txt
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    62719 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/cas04_from_tim_20211203.xml
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/tests/cas04/emtf_results/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    19670 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/emtf_results/CAS04-CAS04bcd_REV06-CAS04bcd_NVR08.zmm
--rwxrwxr-x   0 kkappler  (1001) kkappler  (1001)    19644 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/emtf_results/CAS04bcd_REV06.zrr
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      549 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cas04/helper_functions.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74206 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cfg1.xml
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74206 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/cfg2.xml
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.937517 aurora-0.3.6/tests/config/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1845 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/config/test_config_creator.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74293 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/emtfxml_test.xml
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/io/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    10610 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/io/IAK34_struct_zss.mat
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    15757 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/io/archived_from_matlab.zss
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2587 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/io/test_issue_139.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      267 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/io/test_matlab_zfile_reader.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/parkfield/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      797 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/bf4_9819.csv
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/parkfield/config/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4804 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/config/pkd_test_run_config.json
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1064 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/config/test_single_decimation_level.cfg
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/parkfield/emtf_results/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11926 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/emtf_results/PKD_272_00.zrr
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3057 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/make_parkfield_mth5_from_local_data.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1194 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/readme
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1303 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/set_up_raw_data.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2645 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/test_calibrate_parkfield.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3087 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/test_process_parkfield_run.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3350 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/parkfield/test_process_parkfield_run_rr.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/pipelines/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/pipelines/__init__.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      913 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/pipelines/test_run_summary.py
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.941517 aurora-0.3.6/tests/synthetic/
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.945517 aurora-0.3.6/tests/synthetic/data/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)  1440000 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/data/test1.asc
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)  1440000 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/data/test2.asc
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.945517 aurora-0.3.6/tests/synthetic/emtf_output/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    15714 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/emtf_output/from_matlab_256_26.zss
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/emtf_output/test1.zss
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/emtf_output/test2.zss
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/emtf_output/test2r1.zrr
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2992 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/plot_helpers_synthetic.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      388 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/readme
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     6770 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_compare_aurora_vs_archived_emtf.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1343 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_define_frequency_bands.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5663 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_fourier_coefficients.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      974 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_make_h5s.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1525 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_metadata_values_set_correctly.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4775 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_multi_run.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11932 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_processing.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1547 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_run_ts_slice.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3314 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/synthetic/test_stft_methods_agree.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      723 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/test_doc_build.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1151 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/test_general_helper_functions.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      633 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/test_run_on_commit.ipynb
-drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-07 21:07:24.945517 aurora-0.3.6/tests/time_series/
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2735 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/time_series/test_apodization_window.py
--rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8792 2023-11-07 21:06:48.000000 aurora-0.3.6/tests/time_series/test_windowing_scheme.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.404672 aurora-0.3.7/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1063 2023-11-09 02:17:19.000000 aurora-0.3.7/LICENSE
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      245 2023-11-09 02:17:19.000000 aurora-0.3.7/MANIFEST.in
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1130 2023-11-09 02:17:53.400673 aurora-0.3.7/PKG-INFO
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      409 2023-11-09 02:17:19.000000 aurora-0.3.7/README.rst
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.380673 aurora-0.3.7/aurora/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       22 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/__init__.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.380673 aurora-0.3.7/aurora/config/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      142 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7283 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/config_creator.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/config/emtf_band_setup/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      314 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/emtf_band_setup/__init__.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/config/metadata/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      137 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/metadata/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1769 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/metadata/decimation_level.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5777 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/metadata/processing.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4985 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/config/metadata/station.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3878 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/general_helper_functions.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/pipelines/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11148 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/fourier_coefficients.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      819 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14821 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/process_mth5.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    12275 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/run_summary.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14296 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/time_series_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8622 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/transfer_function_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    25524 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/pipelines/transfer_function_kernel.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/sandbox/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1679 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/butterworth_filters.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1651 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/debug_mt_metadata_issue_85.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/sandbox/io_helpers/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4052 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/emtf_band_setup.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2410 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/fdsn_dataset.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5247 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/inventory_review.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3253 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/make_mth5_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14886 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/io_helpers/zfile_murphy.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2508 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/mth5_channel_summary_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5964 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/mth5_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2590 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/obspy_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8027 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/plot_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1721 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/sandbox/triage_metadata.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/test_utils/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7864 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/dataset_definitions.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/test_utils/mth5/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/mth5/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      664 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/mth5/fc_helpers.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/test_utils/parkfield/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/parkfield/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7281 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/parkfield/calibration_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1988 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/parkfield/make_parkfield_mth5.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      477 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/parkfield/path_helpers.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.384673 aurora-0.3.7/aurora/test_utils/synthetic/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    12329 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/make_mth5_from_asc.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5303 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/make_processing_configs.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      393 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/paths.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1789 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/processing_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3614 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/rms_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8716 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/test_utils/synthetic/station_config.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/time_series/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     7905 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/apodization_window.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1466 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/decorators.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/time_series/filters/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/filters/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2460 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/filters/filter_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3457 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/frequency_band_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3316 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/time_axis_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    13642 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/window_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     6713 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/windowed_time_series.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    16797 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/windowing_scheme.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4246 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/time_series/xarray_helpers.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/transfer_function/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4144 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/TTFZ.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     9545 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/base.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4234 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/emtf_z_file_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    20433 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/kernel_dataset.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/transfer_function/plot/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/plot/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3845 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/plot/comparison_plots.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1200 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/plot/error_bar_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      931 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/plot/rho_phi_helpers.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11579 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/plot/rho_plot.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/transfer_function/regression/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5489 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/TRME.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3406 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/TRME_RR.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    10816 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/base.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1478 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/helper_functions.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5089 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/iter_control.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11411 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/regression/m_estimator.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11707 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/transfer_function_collection.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/aurora/transfer_function/weights/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/weights/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4098 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/weights/coherence_weights.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     9650 2023-11-09 02:17:19.000000 aurora-0.3.7/aurora/transfer_function/weights/edf_weights.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.380673 aurora-0.3.7/aurora.egg-info/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1130 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/PKG-INFO
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5487 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/SOURCES.txt
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        1 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/dependency_links.txt
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        1 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/not-zip-safe
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       18 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/requires.txt
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        7 2023-11-09 02:17:53.000000 aurora-0.3.7/aurora.egg-info/top_level.txt
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/docs/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      634 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/Makefile
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.388673 aurora-0.3.7/docs/api/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      189 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/api/general_helper_functions.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      232 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/api/index.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      494 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/api/pipelines.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1545 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/api/time_series.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1237 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/api/transfer_function.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3673 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/conf.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/docs/figures/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)   118395 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/figures/aurora_logo.png
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      503 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/index.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      795 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/make.bat
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/docs/user-docs/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      881 2023-11-09 02:17:19.000000 aurora-0.3.7/docs/user-docs/installing.rst
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)       38 2023-11-09 02:17:53.404672 aurora-0.3.7/setup.cfg
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1422 2023-11-09 02:17:19.000000 aurora-0.3.7/setup.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/__init__.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/cas04/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5515 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/01_make_cas04_mth5.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11733 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/02b_process_cas04_mth5.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      229 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/band_setup_emtf_nims.txt
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    62719 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/cas04_from_tim_20211203.xml
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/cas04/emtf_results/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    19670 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/emtf_results/CAS04-CAS04bcd_REV06-CAS04bcd_NVR08.zmm
+-rwxrwxr-x   0 kkappler  (1001) kkappler  (1001)    19644 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/emtf_results/CAS04bcd_REV06.zrr
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      549 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cas04/helper_functions.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74206 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cfg1.xml
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74206 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/cfg2.xml
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/config/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1845 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/config/test_config_creator.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    74293 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/emtfxml_test.xml
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/io/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    10610 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/io/IAK34_struct_zss.mat
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    15757 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/io/archived_from_matlab.zss
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2587 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/io/test_issue_139.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      267 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/io/test_matlab_zfile_reader.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/parkfield/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      797 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/bf4_9819.csv
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.392673 aurora-0.3.7/tests/parkfield/config/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4804 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/config/pkd_test_run_config.json
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1064 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/config/test_single_decimation_level.cfg
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.396673 aurora-0.3.7/tests/parkfield/emtf_results/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11926 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/emtf_results/PKD_272_00.zrr
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1194 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/readme
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1303 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/set_up_raw_data.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2645 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/test_calibrate_parkfield.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3087 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/test_process_parkfield_run.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3350 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/parkfield/test_process_parkfield_run_rr.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.396673 aurora-0.3.7/tests/pipelines/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/pipelines/__init__.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      913 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/pipelines/test_run_summary.py
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.396673 aurora-0.3.7/tests/synthetic/
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.400673 aurora-0.3.7/tests/synthetic/data/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)  1440000 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/data/test1.asc
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)  1440000 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/data/test2.asc
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.400673 aurora-0.3.7/tests/synthetic/emtf_output/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    15714 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/emtf_output/from_matlab_256_26.zss
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/emtf_output/test1.zss
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/emtf_output/test2.zss
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    14993 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/emtf_output/test2r1.zrr
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2992 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/plot_helpers_synthetic.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      388 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/readme
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     6770 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_compare_aurora_vs_archived_emtf.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1343 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_define_frequency_bands.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     5663 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_fourier_coefficients.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      974 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_make_h5s.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1525 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_metadata_values_set_correctly.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     4775 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_multi_run.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)    11932 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_processing.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1547 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_run_ts_slice.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     3314 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/synthetic/test_stft_methods_agree.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      723 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/test_doc_build.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     1151 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/test_general_helper_functions.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)      633 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/test_run_on_commit.ipynb
+drwxrwxr-x   0 kkappler  (1001) kkappler  (1001)        0 2023-11-09 02:17:53.400673 aurora-0.3.7/tests/time_series/
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     2735 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/time_series/test_apodization_window.py
+-rw-rw-r--   0 kkappler  (1001) kkappler  (1001)     8792 2023-11-09 02:17:19.000000 aurora-0.3.7/tests/time_series/test_windowing_scheme.py
```

### Comparing `aurora-0.3.6/LICENSE` & `aurora-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/PKG-INFO` & `aurora-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora
-Version: 0.3.6
+Version: 0.3.7
 Summary: Processing Codes for Magnetotelluric Data
 Home-page: https://github.com/simpeg/aurora
 Author: Karl Kappler
 Author-email: karl.kappler@berkeley.edu
 License: MIT license
 Keywords: aurora
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 License-File: LICENSE
 
 .. image:: ../docs/figures/aurora_logo.png
    :width: 900
    :alt: AURORA
 
 |
```

### Comparing `aurora-0.3.6/aurora/config/config_creator.py` & `aurora-0.3.7/aurora/config/config_creator.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/config/metadata/decimation_level.py` & `aurora-0.3.7/aurora/config/metadata/decimation_level.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/config/metadata/processing.py` & `aurora-0.3.7/aurora/config/metadata/processing.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/config/metadata/station.py` & `aurora-0.3.7/aurora/config/metadata/station.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/general_helper_functions.py` & `aurora-0.3.7/aurora/general_helper_functions.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/fourier_coefficients.py` & `aurora-0.3.7/aurora/pipelines/fourier_coefficients.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/helpers.py` & `aurora-0.3.7/aurora/pipelines/helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/process_mth5.py` & `aurora-0.3.7/aurora/pipelines/process_mth5.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/run_summary.py` & `aurora-0.3.7/aurora/pipelines/run_summary.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/time_series_helpers.py` & `aurora-0.3.7/aurora/pipelines/time_series_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/transfer_function_helpers.py` & `aurora-0.3.7/aurora/pipelines/transfer_function_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/pipelines/transfer_function_kernel.py` & `aurora-0.3.7/aurora/pipelines/transfer_function_kernel.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/butterworth_filters.py` & `aurora-0.3.7/aurora/sandbox/butterworth_filters.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/debug_mt_metadata_issue_85.py` & `aurora-0.3.7/aurora/sandbox/debug_mt_metadata_issue_85.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/io_helpers/emtf_band_setup.py` & `aurora-0.3.7/aurora/sandbox/io_helpers/emtf_band_setup.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/io_helpers/fdsn_dataset.py` & `aurora-0.3.7/aurora/sandbox/io_helpers/fdsn_dataset.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/io_helpers/inventory_review.py` & `aurora-0.3.7/aurora/sandbox/io_helpers/inventory_review.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/io_helpers/make_mth5_helpers.py` & `aurora-0.3.7/aurora/sandbox/io_helpers/make_mth5_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/io_helpers/zfile_murphy.py` & `aurora-0.3.7/aurora/sandbox/io_helpers/zfile_murphy.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/mth5_channel_summary_helpers.py` & `aurora-0.3.7/aurora/sandbox/mth5_channel_summary_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/mth5_helpers.py` & `aurora-0.3.7/aurora/sandbox/mth5_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/obspy_helpers.py` & `aurora-0.3.7/aurora/sandbox/obspy_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/plot_helpers.py` & `aurora-0.3.7/aurora/sandbox/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/sandbox/triage_metadata.py` & `aurora-0.3.7/aurora/sandbox/triage_metadata.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/apodization_window.py` & `aurora-0.3.7/aurora/time_series/apodization_window.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/decorators.py` & `aurora-0.3.7/aurora/time_series/decorators.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/filters/filter_helpers.py` & `aurora-0.3.7/aurora/time_series/filters/filter_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/frequency_band_helpers.py` & `aurora-0.3.7/aurora/time_series/frequency_band_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/time_axis_helpers.py` & `aurora-0.3.7/aurora/time_series/time_axis_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/window_helpers.py` & `aurora-0.3.7/aurora/time_series/window_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         output_array[i, :] = data[
             i * num_samples_advance : i * num_samples_advance + num_samples_window
         ]
 
     return output_array
 
 
-@jit
+@jit(nopython=True)
 def sliding_window_numba(data, num_samples_window, num_samples_advance, num_windows):
     """
 
     Parameters
     ----------
     data: np.ndarray
         The time series data to be windowed
```

### Comparing `aurora-0.3.6/aurora/time_series/windowed_time_series.py` & `aurora-0.3.7/aurora/time_series/windowed_time_series.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/windowing_scheme.py` & `aurora-0.3.7/aurora/time_series/windowing_scheme.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/time_series/xarray_helpers.py` & `aurora-0.3.7/aurora/time_series/xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/TTFZ.py` & `aurora-0.3.7/aurora/transfer_function/TTFZ.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/base.py` & `aurora-0.3.7/aurora/transfer_function/base.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/emtf_z_file_helpers.py` & `aurora-0.3.7/aurora/transfer_function/emtf_z_file_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/kernel_dataset.py` & `aurora-0.3.7/aurora/transfer_function/kernel_dataset.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/plot/comparison_plots.py` & `aurora-0.3.7/aurora/transfer_function/plot/comparison_plots.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/plot/error_bar_helpers.py` & `aurora-0.3.7/aurora/transfer_function/plot/error_bar_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/plot/rho_phi_helpers.py` & `aurora-0.3.7/aurora/transfer_function/plot/rho_phi_helpers.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/plot/rho_plot.py` & `aurora-0.3.7/aurora/transfer_function/plot/rho_plot.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/TRME.py` & `aurora-0.3.7/aurora/transfer_function/regression/TRME.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/TRME_RR.py` & `aurora-0.3.7/aurora/transfer_function/regression/TRME_RR.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/base.py` & `aurora-0.3.7/aurora/transfer_function/regression/base.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/helper_functions.py` & `aurora-0.3.7/aurora/transfer_function/regression/helper_functions.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/iter_control.py` & `aurora-0.3.7/aurora/transfer_function/regression/iter_control.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/regression/m_estimator.py` & `aurora-0.3.7/aurora/transfer_function/regression/m_estimator.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/transfer_function_collection.py` & `aurora-0.3.7/aurora/transfer_function/transfer_function_collection.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/weights/coherence_weights.py` & `aurora-0.3.7/aurora/transfer_function/weights/coherence_weights.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora/transfer_function/weights/edf_weights.py` & `aurora-0.3.7/aurora/transfer_function/weights/edf_weights.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/aurora.egg-info/PKG-INFO` & `aurora-0.3.7/aurora.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora
-Version: 0.3.6
+Version: 0.3.7
 Summary: Processing Codes for Magnetotelluric Data
 Home-page: https://github.com/simpeg/aurora
 Author: Karl Kappler
 Author-email: karl.kappler@berkeley.edu
 License: MIT license
 Keywords: aurora
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 License-File: LICENSE
 
 .. image:: ../docs/figures/aurora_logo.png
    :width: 900
    :alt: AURORA
 
 |
```

### Comparing `aurora-0.3.6/aurora.egg-info/SOURCES.txt` & `aurora-0.3.7/aurora.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,29 @@
 aurora/sandbox/triage_metadata.py
 aurora/sandbox/io_helpers/__init__.py
 aurora/sandbox/io_helpers/emtf_band_setup.py
 aurora/sandbox/io_helpers/fdsn_dataset.py
 aurora/sandbox/io_helpers/inventory_review.py
 aurora/sandbox/io_helpers/make_mth5_helpers.py
 aurora/sandbox/io_helpers/zfile_murphy.py
+aurora/test_utils/__init__.py
+aurora/test_utils/dataset_definitions.py
+aurora/test_utils/mth5/__init__.py
+aurora/test_utils/mth5/fc_helpers.py
+aurora/test_utils/parkfield/__init__.py
+aurora/test_utils/parkfield/calibration_helpers.py
+aurora/test_utils/parkfield/make_parkfield_mth5.py
+aurora/test_utils/parkfield/path_helpers.py
+aurora/test_utils/synthetic/__init__.py
+aurora/test_utils/synthetic/make_mth5_from_asc.py
+aurora/test_utils/synthetic/make_processing_configs.py
+aurora/test_utils/synthetic/paths.py
+aurora/test_utils/synthetic/processing_helpers.py
+aurora/test_utils/synthetic/rms_helpers.py
+aurora/test_utils/synthetic/station_config.py
 aurora/time_series/__init__.py
 aurora/time_series/apodization_window.py
 aurora/time_series/decorators.py
 aurora/time_series/frequency_band_helpers.py
 aurora/time_series/time_axis_helpers.py
 aurora/time_series/window_helpers.py
 aurora/time_series/windowed_time_series.py
@@ -98,15 +113,14 @@
 tests/cas04/emtf_results/CAS04bcd_REV06.zrr
 tests/config/test_config_creator.py
 tests/io/IAK34_struct_zss.mat
 tests/io/archived_from_matlab.zss
 tests/io/test_issue_139.py
 tests/io/test_matlab_zfile_reader.py
 tests/parkfield/bf4_9819.csv
-tests/parkfield/make_parkfield_mth5_from_local_data.py
 tests/parkfield/readme
 tests/parkfield/set_up_raw_data.py
 tests/parkfield/test_calibrate_parkfield.py
 tests/parkfield/test_process_parkfield_run.py
 tests/parkfield/test_process_parkfield_run_rr.py
 tests/parkfield/config/pkd_test_run_config.json
 tests/parkfield/config/test_single_decimation_level.cfg
```

### Comparing `aurora-0.3.6/docs/Makefile` & `aurora-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/api/time_series.rst` & `aurora-0.3.7/docs/api/time_series.rst`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/api/transfer_function.rst` & `aurora-0.3.7/docs/api/transfer_function.rst`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/conf.py` & `aurora-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/figures/aurora_logo.png` & `aurora-0.3.7/docs/figures/aurora_logo.png`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/make.bat` & `aurora-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/docs/user-docs/installing.rst` & `aurora-0.3.7/docs/user-docs/installing.rst`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/setup.py` & `aurora-0.3.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,38 +7,31 @@
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 # with open("HISTORY.rst") as history_file:
 #    history = history_file.read()
 
 requirements = [
-    "matplotlib",
     "mth5",
-    "mt_metadata",
-    "numpy",
     "numba",
-    "obspy",
     "psutil",
-    "pandas<1.5",
-    "scipy",
-    "xarray",
 ]
 
 setup_requirements = [
     "pytest-runner",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
     author="Karl Kappler",
     author_email="karl.kappler@berkeley.edu",
-    python_requires=">=3.5",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
@@ -54,10 +47,10 @@
     keywords="aurora",
     name="aurora",
     packages=find_packages(include=["aurora", "aurora.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/simpeg/aurora",
-    version="0.3.6",
+    version="0.3.7",
     zip_safe=False,
 )
```

### Comparing `aurora-0.3.6/tests/cas04/01_make_cas04_mth5.py` & `aurora-0.3.7/tests/cas04/01_make_cas04_mth5.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cas04/02b_process_cas04_mth5.py` & `aurora-0.3.7/tests/cas04/02b_process_cas04_mth5.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cas04/cas04_from_tim_20211203.xml` & `aurora-0.3.7/tests/cas04/cas04_from_tim_20211203.xml`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cas04/emtf_results/CAS04-CAS04bcd_REV06-CAS04bcd_NVR08.zmm` & `aurora-0.3.7/tests/cas04/emtf_results/CAS04-CAS04bcd_REV06-CAS04bcd_NVR08.zmm`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cas04/emtf_results/CAS04bcd_REV06.zrr` & `aurora-0.3.7/tests/cas04/emtf_results/CAS04bcd_REV06.zrr`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cas04/helper_functions.py` & `aurora-0.3.7/tests/cas04/helper_functions.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cfg1.xml` & `aurora-0.3.7/tests/cfg1.xml`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/cfg2.xml` & `aurora-0.3.7/tests/cfg2.xml`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/config/test_config_creator.py` & `aurora-0.3.7/tests/config/test_config_creator.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/emtfxml_test.xml` & `aurora-0.3.7/tests/emtfxml_test.xml`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/io/IAK34_struct_zss.mat` & `aurora-0.3.7/tests/io/IAK34_struct_zss.mat`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/io/archived_from_matlab.zss` & `aurora-0.3.7/tests/io/archived_from_matlab.zss`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/io/test_issue_139.py` & `aurora-0.3.7/tests/io/test_issue_139.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/bf4_9819.csv` & `aurora-0.3.7/tests/parkfield/bf4_9819.csv`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/config/pkd_test_run_config.json` & `aurora-0.3.7/tests/parkfield/config/pkd_test_run_config.json`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/config/test_single_decimation_level.cfg` & `aurora-0.3.7/tests/parkfield/config/test_single_decimation_level.cfg`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/emtf_results/PKD_272_00.zrr` & `aurora-0.3.7/tests/parkfield/emtf_results/PKD_272_00.zrr`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/readme` & `aurora-0.3.7/tests/parkfield/readme`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/set_up_raw_data.py` & `aurora-0.3.7/tests/parkfield/set_up_raw_data.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/test_calibrate_parkfield.py` & `aurora-0.3.7/tests/parkfield/test_calibrate_parkfield.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/test_process_parkfield_run.py` & `aurora-0.3.7/tests/parkfield/test_process_parkfield_run.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/parkfield/test_process_parkfield_run_rr.py` & `aurora-0.3.7/tests/parkfield/test_process_parkfield_run_rr.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/pipelines/test_run_summary.py` & `aurora-0.3.7/tests/pipelines/test_run_summary.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/data/test1.asc` & `aurora-0.3.7/tests/synthetic/data/test1.asc`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/data/test2.asc` & `aurora-0.3.7/tests/synthetic/data/test2.asc`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/emtf_output/from_matlab_256_26.zss` & `aurora-0.3.7/tests/synthetic/emtf_output/from_matlab_256_26.zss`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/emtf_output/test1.zss` & `aurora-0.3.7/tests/synthetic/emtf_output/test1.zss`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/emtf_output/test2.zss` & `aurora-0.3.7/tests/synthetic/emtf_output/test2.zss`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/emtf_output/test2r1.zrr` & `aurora-0.3.7/tests/synthetic/emtf_output/test2r1.zrr`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/plot_helpers_synthetic.py` & `aurora-0.3.7/tests/synthetic/plot_helpers_synthetic.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_compare_aurora_vs_archived_emtf.py` & `aurora-0.3.7/tests/synthetic/test_compare_aurora_vs_archived_emtf.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_define_frequency_bands.py` & `aurora-0.3.7/tests/synthetic/test_define_frequency_bands.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_fourier_coefficients.py` & `aurora-0.3.7/tests/synthetic/test_fourier_coefficients.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_make_h5s.py` & `aurora-0.3.7/tests/synthetic/test_make_h5s.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_metadata_values_set_correctly.py` & `aurora-0.3.7/tests/synthetic/test_metadata_values_set_correctly.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_multi_run.py` & `aurora-0.3.7/tests/synthetic/test_multi_run.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_processing.py` & `aurora-0.3.7/tests/synthetic/test_processing.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_run_ts_slice.py` & `aurora-0.3.7/tests/synthetic/test_run_ts_slice.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/synthetic/test_stft_methods_agree.py` & `aurora-0.3.7/tests/synthetic/test_stft_methods_agree.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/test_doc_build.py` & `aurora-0.3.7/tests/test_doc_build.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/test_general_helper_functions.py` & `aurora-0.3.7/tests/test_general_helper_functions.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/test_run_on_commit.ipynb` & `aurora-0.3.7/tests/test_run_on_commit.ipynb`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/time_series/test_apodization_window.py` & `aurora-0.3.7/tests/time_series/test_apodization_window.py`

 * *Files identical despite different names*

### Comparing `aurora-0.3.6/tests/time_series/test_windowing_scheme.py` & `aurora-0.3.7/tests/time_series/test_windowing_scheme.py`

 * *Files identical despite different names*

