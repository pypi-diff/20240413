# Comparing `tmp/kilosort-4.0.3.tar.gz` & `tmp/kilosort-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilosort-4.0.3.tar", last modified: Fri Apr  5 21:03:03 2024, max compression
+gzip compressed data, was "kilosort-4.0.4.tar", last modified: Sat Apr 13 21:11:55 2024, max compression
```

## Comparing `kilosort-4.0.3.tar` & `kilosort-4.0.4.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.940929 kilosort-4.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/installation_issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/ISSUE_TEMPLATE/other.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-05 21:02:45.000000 kilosort-4.0.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-05 21:02:45.000000 kilosort-4.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 21:02:45.000000 kilosort-4.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-05 21:02:45.000000 kilosort-4.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 21:02:45.000000 kilosort-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-05 21:03:03.956929 kilosort-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-05 21:02:45.000000 kilosort-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.944929 kilosort-4.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/drift.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/gui_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/hardware.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/multi_shank.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/parameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.948929 kilosort-4.0.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/load_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/make_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 21:02:45.000000 kilosort-4.0.3/docs/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.948929 kilosort-4.0.3/kilosort/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/CCG.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/clustering_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/datashift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.952929 kilosort-4.0.3/kilosort/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/data_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/header_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/message_log_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/minor_gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/probe_view_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/run_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/sanity_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/settings_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/gui/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)    36385 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/run_kilosort.py
--rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/swarmsplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/template_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-05 21:02:45.000000 kilosort-4.0.3/kilosort/wTEMP.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/kilosort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 21:03:03.000000 kilosort-4.0.3/kilosort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 21:02:45.000000 kilosort-4.0.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 21:03:03.956929 kilosort-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-05 21:02:45.000000 kilosort-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:03:03.956929 kilosort-4.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_full_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 21:02:45.000000 kilosort-4.0.3/tests/test_spikedetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 21:02:45.000000 kilosort-4.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.791759 kilosort-4.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/installation_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/ISSUE_TEMPLATE/other.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.775759 kilosort-4.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-13 21:11:45.000000 kilosort-4.0.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-13 21:11:45.000000 kilosort-4.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-13 21:11:45.000000 kilosort-4.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-13 21:11:45.000000 kilosort-4.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 21:11:45.000000 kilosort-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-13 21:11:55.791759 kilosort-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-13 21:11:45.000000 kilosort-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.779759 kilosort-4.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/drift.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/gui_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/hardware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/multi_shank.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/parameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.779759 kilosort-4.0.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/basic_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/load_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/make_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-13 21:11:45.000000 kilosort-4.0.4/docs/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.783758 kilosort-4.0.4/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/CCG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/clustering_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/datashift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/kilosort/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/data_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/header_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/message_log_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/minor_gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/probe_view_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/run_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/sanity_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33239 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/settings_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/gui/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/run_kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60034 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/swarmsplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/template_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-13 21:11:45.000000 kilosort-4.0.4/kilosort/wTEMP.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/kilosort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 21:11:55.000000 kilosort-4.0.4/kilosort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 21:11:45.000000 kilosort-4.0.4/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:11:55.791759 kilosort-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-13 21:11:45.000000 kilosort-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:11:55.787758 kilosort-4.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_full_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 21:11:45.000000 kilosort-4.0.4/tests/test_spikedetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-13 21:11:45.000000 kilosort-4.0.4/tox.ini
```

### Comparing `kilosort-4.0.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `kilosort-4.0.4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/.github/ISSUE_TEMPLATE/feature_request.yml` & `kilosort-4.0.4/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/.github/ISSUE_TEMPLATE/installation_issue.yml` & `kilosort-4.0.4/.github/ISSUE_TEMPLATE/installation_issue.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/.github/workflows/test_and_deploy.yml` & `kilosort-4.0.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/.gitignore` & `kilosort-4.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/.readthedocs.yml` & `kilosort-4.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/CODE_OF_CONDUCT.md` & `kilosort-4.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/LICENSE` & `kilosort-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/PKG-INFO` & `kilosort-4.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.3
+Version: 4.0.4
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,30 +49,30 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots.
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
-**If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
+**If you use Kilosort1-4, please cite the [paper](https://www.nature.com/articles/s41592-024-02232-7):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks or 2D arrays. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
 
-**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+**Note on reusing parameters from previous versions**: This probably will not work well. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
-**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
+**Warning** :bangbang:: There were two bugs in Kilosort 2, 2.5 and 3 (but not 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch1 releases fix these bugs, please use the new default NT and ntbuff parameters. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04.
```

### Comparing `kilosort-4.0.3/README.md` & `kilosort-4.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots.
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
-**If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
+**If you use Kilosort1-4, please cite the [paper](https://www.nature.com/articles/s41592-024-02232-7):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks or 2D arrays. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
 
-**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+**Note on reusing parameters from previous versions**: This probably will not work well. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
-**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
+**Warning** :bangbang:: There were two bugs in Kilosort 2, 2.5 and 3 (but not 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch1 releases fix these bugs, please use the new default NT and ntbuff parameters. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04.
```

### Comparing `kilosort-4.0.3/docs/Makefile` & `kilosort-4.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/conf.py` & `kilosort-4.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/drift.rst` & `kilosort-4.0.4/docs/drift.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/gui_guide.rst` & `kilosort-4.0.4/docs/gui_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
    :width: 600
 
 If you need to create a new probe layout, select "[new]" to open the probe creation tool. Values for 'x-coordinates' and 'y-coordinates' need to be in microns, and can be specified with numpy expressions. For example, a 1-shank linear probe with 4 channels could have `np.ones(4)` in the 'x-coordinates' field instead of `1, 1, 1, 1`. Each field (except name) must have the same number of elements, corresponding to the number of ephys channels in the data. WHen you are finished setting the values, click "Check" to verify that your inputs are valid. If they are not, an error message will be displayed. Otherwise, the "OK" button will become clickable, which will save the probe to the Kilosort4 probes directory.
 
 .. image:: https://www.kilosort.org/static/images/gui_make_probe.png
    :width: 600
 
-After a probe is selected, you can click "Preview Probe" to see a visualization and verify that the probe geometry looks correct.
+After a probe is selected, you can click "Preview Probe" to see a visualization and verify that the probe geometry looks correct. Checking "True Aspect Ratio" will show a physically proportional representation. Moving the slider will adjust the displayed scale of the contacts.
 
 
 Load the data
 -------------
 After you select a probe, the GUI will attempt to automatically determine the correct value for 'number of channels.' Make sure this correctly reflects the number of channels in your datafile, including non-ephys channels. For example, Neuropixels 1 probes output data with 385 channels. Only 384 of those are the ephys data used for sorting, but 'number of channels' should still be set to 385. You may also need to change the dtype of the data (int16 by default) or the sampling rate (30000hz by default). Additionally, you can choose which computing device. By default, the GUI will select the first CUDA GPU detected by PyTorch, or CPU if no GPU is detected.
 
 When you are satisfied with these settings, click "LOAD" at the top left of the GUI to load the data.
```

### Comparing `kilosort-4.0.3/docs/hardware.rst` & `kilosort-4.0.4/docs/hardware.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/index.rst` & `kilosort-4.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/make.bat` & `kilosort-4.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/multi_shank.rst` & `kilosort-4.0.4/docs/multi_shank.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 .. _multi_shank:
 
 Using probes with multiple shanks
 ==================================
+Update: the latest version of the code addresses this issue. After getting feedback from users, this page will be removed if there are no further issues. For 2D arrays, you may want to set the new `x_centers` parameter (under "Extra Settings" in the GUI) for best results.
+
 Currently, Kilosort4 does not process shanks separately. Until this is added, we recommend changing your probe layout to artificially stack the shanks in a single column with a bit of vertical space (~100um) between each shank.
 
 If that option isn't feasible for some reason, you can also try adjusting the `min_template_size` and/or `dminx` parameters in the GUI, or in the settings argument for `run_kilosort` if you're using the API. Setting `dminx` to around half the total width of the probe seems to be a good starting point, and you can adjust from there.
 
 See `issue 606 <https://github.com/MouseLand/Kilosort/issues/606>`_ and `issue 617 <https://github.com/MouseLand/Kilosort/issues/617>`_ for additional context.
```

### Comparing `kilosort-4.0.3/docs/parameters.rst` & `kilosort-4.0.4/docs/parameters.rst`

 * *Files 5% similar despite different names*

```diff
@@ -45,12 +45,17 @@
 
 
 ``nearest_chans`` and ``nearest_templates``
 -------------------------------------------
 This is the number of nearest channels and template locations, respectively, used when assigning templates to spikes during spike detection. ``nearest_chans`` cannot be larger than the total number of channels on the probe, so it will need to be reduced for probes with less than 10 channels. ``nearest_templates`` does not have this restriction. However, for probes with around 64 channels or less and sparsely spaced contacts, decreasing ``nearest_templates`` to be less than or equal to the number of channels helps avoid numerical instability.
 
 
+``x_centers``
+-------------
+The number of x-positions to use when determining centers for template groupings. Specifically, this is the number of centroids to look for when using k-means to cluster the x-positions for the probe. In most cases you should not need to specify this. However, **for probes with contacts arranged in a 2D grid**, we recommend setting ``x_centers`` such that centers are placed every 200-300um so that there are not too many templates in each group. For example, for an array that is 2000um in width, try ``x_centers = 10``. If contacts are very densely spaced, you may need to use a higher value for better performance.
+
+
 ``duplicate_spike_bins``
 ------------------------
 After sorting has finished, spikes that occur within this number of bins of each other, from the same unit, are assumed to be artifacts and removed. The default of 15 bins corresponds to 0.5ms for a sampling rate of 30000hz. If your sampling rate is different, you may need to increase or decrease this accordingly. If you see otherwise good neurons with large peaks around 0ms when viewing correlograms in Phy, increasing this value can help remove those artifacts.
 
 **Warning!!!** Do not increase this value beyond 0.5ms as it will interfere with the ACG and CCG refractory period estimations (which normally ignores the central 1ms of the correlogram).
```

### Comparing `kilosort-4.0.3/docs/tutorials/basic_example.ipynb` & `kilosort-4.0.4/docs/tutorials/basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/tutorials/load_data.ipynb` & `kilosort-4.0.4/docs/tutorials/load_data.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/docs/tutorials/make_probe.ipynb` & `kilosort-4.0.4/docs/tutorials/make_probe.ipynb`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/CCG.py` & `kilosort-4.0.4/kilosort/CCG.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/bench.py` & `kilosort-4.0.4/kilosort/bench.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/clustering_qr.py` & `kilosort-4.0.4/kilosort/clustering_qr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from io import StringIO
 import numpy as np
 import torch
 from torch import sparse_coo_tensor as coo
-from scipy.sparse import csr_matrix 
+from scipy.sparse import csr_matrix
+from scipy.ndimage import gaussian_filter
+from scipy.signal import find_peaks
+from scipy.cluster.vq import kmeans
 import faiss
 from tqdm import tqdm 
+
 from kilosort import hierarchical, swarmsplitter 
 
+
 def neigh_mat(Xd, nskip=10, n_neigh=30):
     Xsub = Xd[::nskip]
     n_samples, dim = Xd.shape
     n_nodes = Xsub.shape[0]
 
     Xd = np.ascontiguousarray(Xd)
     Xsub = np.ascontiguousarray(Xsub)
@@ -46,14 +50,15 @@
     N = coo(iin, tones, (nclust, 1))
     C = C.to_dense()
     N = N.to_dense()
     mu = C / (1e-6 + N)
 
     return mu, N
 
+
 def assign_iclust(rows_neigh, isub, kn, tones2, nclust, lam, m, ki, kj, device=torch.device('cuda')):
     NN = kn.shape[0]
 
     ij = torch.vstack((rows_neigh.flatten(), isub[kn].flatten()))
     xN = coo(ij, tones2.flatten(), (NN, nclust))
     xN = xN.to_dense()
 
@@ -65,14 +70,15 @@
     
         xN = xN - lam/m * (ki.unsqueeze(-1) * kN.to_dense()) 
     
     iclust = torch.argmax(xN, 1)
 
     return iclust
 
+
 def assign_isub(iclust, kn, tones2, nclust, nsub, lam, m,ki,kj, device=torch.device('cuda')):
     n_neigh = kn.shape[1]
     cols = iclust.unsqueeze(-1).tile((1, n_neigh))
     iis = torch.vstack((kn.flatten(), cols.flatten()))
 
     xS = coo(iis, tones2.flatten(), (nsub, nclust))
     xS = xS.to_dense()
@@ -83,14 +89,15 @@
         ij = torch.vstack((tzeros, iclust))    
         kN = coo(ij, tones, (1, nclust))
         xS = xS - lam / m * (kj.unsqueeze(-1) * kN.to_dense())
 
     isub = torch.argmax(xS, 1)
     return isub
 
+
 def Mstats(M, device=torch.device('cuda')):
     m = M.sum()
     ki = np.array(M.sum(1)).flatten()
     kj = np.array(M.sum(0)).flatten()
     ki = m * ki/ki.sum()
     kj = m * kj/kj.sum()
 
@@ -172,155 +179,206 @@
 
         mu[j] = Xg[ix].mean(0)
         vexp0[ix] = vexp[ix,imax]
         iclust[ix] = j
 
     return iclust
 
+
 def compute_score(mu, mu2, N, ccN, lam):
     mu_pairs  = ((N*mu).unsqueeze(1)  + N*mu)  / (1e-6 + N+N[:,0]).unsqueeze(-1)
     mu2_pairs = ((N*mu2).unsqueeze(1) + N*mu2) / (1e-6 + N+N[:,0]).unsqueeze(-1)
 
     vpair = (mu2_pairs - mu_pairs**2).sum(-1) * (N + N[:,0])
     vsingle = N[:,0] * (mu2 - mu**2).sum(-1)
     dexp = vpair - (vsingle + vsingle.unsqueeze(-1))
 
     dexp = dexp - torch.diag(torch.diag(dexp))
 
     score = (ccN + ccN.T) - lam * dexp
     return score
 
-def run_one(Xd, st0, nskip = 20, lam = 0):
 
+def run_one(Xd, st0, nskip = 20, lam = 0):
     iclust, iclust0, M = cluster(Xd,nskip = nskip, lam = 0, seed = 5)
-
     xtree, tstat, my_clus = hierarchical.maketree(M, iclust, iclust0)
-
-    xtree, tstat = swarmsplitter.split(Xd.numpy(), xtree, tstat, iclust, my_clus, meta = st0)
-
+    xtree, tstat = swarmsplitter.split(Xd.numpy(), xtree, tstat, iclust,
+                                       my_clus, meta = st0)
     iclust1 = swarmsplitter.new_clusters(iclust, my_clus, xtree, tstat)
 
     return iclust1
 
-import time
-
 
 def xy_templates(ops):
     iU = ops['iU'].cpu().numpy()
     iC = ops['iCC'][:, ops['iU']]
     #PID = st[:,5].long()
     xcup, ycup = ops['xc'][iU], ops['yc'][iU]
     xy = np.vstack((xcup, ycup))
     xy = torch.from_numpy(xy)
 
     iU = ops['iU'].cpu().numpy()
     iC = ops['iCC'][:, ops['iU']]    
+
     return xy, iC
 
+
 def xy_up(ops):
     xcup, ycup = ops['xcup'], ops['ycup']
     xy = np.vstack((xcup, ycup))
     xy = torch.from_numpy(xy)
-
     iC = ops['iC'] 
+
     return xy, iC
 
-def xy_c(ops):
-    xcup, ycup = ops['xc'][::4], ops['yc'][::4]    
-    xy = np.vstack((xcup, ycup+10))
-    xy = torch.from_numpy(xy)
 
-    iC = ops['iC']
-    #print(1)
-    return xy, iC
+def x_centers(ops):
+    k = ops.get('x_centers', None)
+    if k is not None:
+        # Use this as the input for k-means, either a number of centers
+        # or initial guesses.
+        approx_centers = k
+    else:
+        # NOTE: This automated method does not work well for 2D array probes.
+        #       We recommend specifying `x_centers` manually for that case.
+        dminx = ops['dminx']
+        min_x = ops['xc'].min()
+        max_x = ops['xc'].max()
+
+        # Make histogram of x-positions with bin size roughly equal to dminx,
+        # with a bit of padding on either end of the probe so that peaks can be
+        # detected at edges.
+        num_bins = int((max_x-min_x)/(dminx)) + 4
+        bins = np.linspace(min_x - dminx*2, max_x + dminx*2, num_bins)
+        hist, edges = np.histogram(ops['xc'], bins=bins)
+        # Apply smoothing to make peak-finding simpler.
+        smoothed = gaussian_filter(hist, sigma=0.5)
+        peaks, _ = find_peaks(smoothed)
+        # peaks are indices, translate back to position in microns
+        approx_centers = [edges[p] for p in peaks]
+        # Use these as initial guesses for centroids in k-means to get
+        # a more accurate value for the actual centers. Or, if there's only 1,
+        # just look for one centroid.
+        if len(approx_centers) == 1: approx_centers = 1
+
+    centers, distortion = kmeans(ops['xc'], approx_centers)
+
+    # TODO: Maybe use distortion to raise warning if it seems too large?
+    # "The mean (non-squared) Euclidean distance between the observations passed
+    #  and the centroids generated. Note the difference to the standard definition
+    #  of distortion in the context of the k-means algorithm, which is the sum of
+    #  the squared distances."
+
+    # For example, could raise a warning if this is greater than dminx*2?
+    # Most probes should satisfy that criteria.
+
+    return centers
+
+
+def y_centers(ops):
+    ycup = ops['ycup']
+    dmin = ops['dmin']
+    # TODO: May want to add the -dmin/2 in the future to center these, but
+    #       this changes the results for testing so we need to wait until we can
+    #       check it with simulations.
+    centers = np.arange(ycup.min()+dmin-1, ycup.max()+dmin+1, 2*dmin)# - dmin/2
+
+    return centers
 
 
 def run(ops, st, tF,  mode = 'template', device=torch.device('cuda'), progress_bar=None):
 
     if mode == 'template':
         xy, iC = xy_templates(ops)
         iclust_template = st[:,1].astype('int32')
         xcup, ycup = ops['xcup'], ops['ycup']
-    elif mode == 'spikes_nn':
-        xy, iC = xy_c(ops)
-        xcup, ycup = ops['xc'][::4], ops['yc'][::4]   
-        iclust_template = st[:,5].astype('int32')
     else:
         xy, iC = xy_up(ops)
         iclust_template = st[:,5].astype('int32')
         xcup, ycup = ops['xcup'], ops['ycup']
 
-    d0 = ops['dmin']
-    ycent = np.arange(ycup.min()+d0-1, ycup.max()+d0+1, 2*d0)
-
-    nsp = st.shape[0]
-    clu = np.zeros(nsp, 'int32')
-    nmax = 0
-
+    dmin = ops['dmin']
+    dminx = ops['dminx']
     nskip = ops['settings']['cluster_downsampling']
     ncomps = ops['settings']['cluster_pcs']
+    ycent = y_centers(ops)
+    xcent = x_centers(ops)
+    nsp = st.shape[0]
 
+    # Get positions of all grouping centers
+    ycent_pos, xcent_pos = np.meshgrid(ycent, xcent)
+    ycent_pos = torch.from_numpy(ycent_pos.flatten())
+    xcent_pos = torch.from_numpy(xcent_pos.flatten())
+    # Compute distances from templates
+    center_distance = (
+        (xy[0,:] - xcent_pos.unsqueeze(-1))**2
+        + (xy[1,:] - ycent_pos.unsqueeze(-1))**2
+        )
+    # Add some randomness in case of ties
+    center_distance += 1e-20*torch.rand(center_distance.shape)
+    # Get flattened index of x-y center that is closest to template
+    minimum_distance = torch.min(center_distance, 0).indices
+    
+    clu = np.zeros(nsp, 'int32')
     Wall = torch.zeros((0, ops['Nchan'], ops['settings']['n_pcs']))
-    t0 = time.time()
     nearby_chans_empty = 0
-    for kk in tqdm(np.arange(len(ycent)), miniters=20 if progress_bar else None, mininterval=10 if progress_bar else None):
-        # get the data
-        #iclust_template = st[:,1].astype('int32')
-
-        Xd, ch_min, ch_max, igood  = get_data_cpu(
-            ops, xy, iC, iclust_template, tF, ycent[kk], xcup.mean(), dmin=d0,
-            dminx = ops['dminx'], ncomps=ncomps
-            )
-
-        if Xd is None:
-            nearby_chans_empty += 1
-            continue
-
-        if Xd.shape[0]<1000:
-            #clu[igood] = nmax
-            #nmax += 1
-            iclust = torch.zeros((Xd.shape[0],))
-        else:
-            if mode == 'template':
-                st0 = st[igood,0]/ops['fs']
-            else:
-                st0 = None
-
-            # find new clusters
-            iclust, iclust0, M, iclust_init = cluster(Xd, nskip=nskip, lam=1,
-                                                      seed=5, device=device)
-
-            xtree, tstat, my_clus = hierarchical.maketree(M, iclust, iclust0)
-
-            xtree, tstat = swarmsplitter.split(Xd.numpy(), xtree, tstat, iclust, my_clus, meta = st0)
-
-            iclust = swarmsplitter.new_clusters(iclust, my_clus, xtree, tstat)
-
-        clu[igood] = iclust + nmax
-        Nfilt = int(iclust.max() + 1)
-        nmax += Nfilt
-
-        # we need the new templates here         
-        W = torch.zeros((Nfilt, ops['Nchan'], ops['settings']['n_pcs']))
-        for j in range(Nfilt):
-            w = Xd[iclust==j].mean(0)
-            W[j, ch_min:ch_max, :] = torch.reshape(w, (-1, ops['settings']['n_pcs'])).cpu()
-        
-        Wall = torch.cat((Wall, W), 0)
+    nmax = 0
 
-        if progress_bar is not None:
-            progress_bar.emit(int((kk+1) / len(ycent) * 100))
-        
-        if 0:#kk%50==0:
-            print(kk, nmax, time.time()-t0)
+    for kk in tqdm(np.arange(len(ycent)), miniters=20 if progress_bar else None,
+                   mininterval=10 if progress_bar else None):
+        for jj in np.arange(len(xcent)):
+            # Get data for all templates that were closest to this x,y center.
+            ii = ii = kk + jj*ycent.size
+            ix = (minimum_distance == ii)
+            Xd, ch_min, ch_max, igood  = get_data_cpu(
+                ops, xy, iC, iclust_template, tF, ycent[kk], xcent[jj], dmin=dmin,
+                dminx=dminx, ncomps=ncomps, ix=ix
+                )
+
+            if Xd is None:
+                nearby_chans_empty += 1
+                continue
+            elif Xd.shape[0]<1000:
+                iclust = torch.zeros((Xd.shape[0],))
+            else:
+                if mode == 'template':
+                    st0 = st[igood,0]/ops['fs']
+                else:
+                    st0 = None
+
+                # find new clusters
+                iclust, iclust0, M, iclust_init = cluster(Xd, nskip=nskip, lam=1,
+                                                        seed=5, device=device)
+
+                xtree, tstat, my_clus = hierarchical.maketree(M, iclust, iclust0)
+
+                xtree, tstat = swarmsplitter.split(Xd.numpy(), xtree, tstat, iclust, my_clus, meta = st0)
+
+                iclust = swarmsplitter.new_clusters(iclust, my_clus, xtree, tstat)
+
+            clu[igood] = iclust + nmax
+            Nfilt = int(iclust.max() + 1)
+            nmax += Nfilt
+
+            # we need the new templates here         
+            W = torch.zeros((Nfilt, ops['Nchan'], ops['settings']['n_pcs']))
+            for j in range(Nfilt):
+                w = Xd[iclust==j].mean(0)
+                W[j, ch_min:ch_max, :] = torch.reshape(w, (-1, ops['settings']['n_pcs'])).cpu()
+            
+            Wall = torch.cat((Wall, W), 0)
+
+            if progress_bar is not None:
+                progress_bar.emit(int((kk+1) / len(ycent) * 100))
+            
 
     if nearby_chans_empty == len(ycent):
         raise ValueError(
             f'`get_data_cpu` never found suitable channels in `clustering_qr.run`.'
-            f'\ndmin, dminx, and xcenter are: {d0, ops["dminx"], xcup.mean()}'
+            f'\ndmin, dminx, and xcenter are: {dmin, dminx, xcup.mean()}'
         )
 
     if Wall.sum() == 0:
         # Wall is empty, unspecified reason
         raise ValueError(
             'Wall is empty after `clustering_qr.run`, cannot continue clustering.'
         )
```

### Comparing `kilosort-4.0.3/kilosort/datashift.py` & `kilosort-4.0.4/kilosort/datashift.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/__init__.py` & `kilosort-4.0.4/kilosort/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/converter.py` & `kilosort-4.0.4/kilosort/gui/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -224,14 +224,16 @@
             write_prb(probe_filename, pg)
             add_probe_to_settings(self.gui.settings_box, probe_filename)
         except ValueError:
             print(
                 'SpikeInterface recording contains no probe information,\n'
                 'could not write .prb file.'
             )
+            self.gui.settings_box.clear_probe_selection()
+
         self.gui.settings_box.check_load()
 
     @QtCore.Slot()
     def convert_to_binary(self):
         # TODO: add option to specify chunksize for conversion
         if None in [self.filename, self.filetype, self.data_dtype]:
             logger.exception(
@@ -265,15 +267,31 @@
         self.conversion_thread.bin_filename = bin_filename
         self.conversion_thread.recording = recording
         self.conversion_thread.start()
         while self.conversion_thread.isRunning():
             QtWidgets.QApplication.processEvents()
         else:
             self.disableInput.emit(False)
+
+        # Get output of conversion, then delete thread.
+        c = self.conversion_thread.c
+        fs = self.conversion_thread.fs
+        probe_filename = self.conversion_thread.probe_filename
         self.conversion_thread = None
+
+        # Update settings with new data file, probe, etc
+        settings = self.gui.settings_box
+        update_settings_box(settings, c, fs, self.data_dtype)
+        if probe_filename is not None:
+            add_probe_to_settings(settings, probe_filename)
+        else:
+            settings.clear_probe_selection()
+        settings.data_file_path_input.setText(bin_filename.as_posix())
+        settings.data_file_path_input.editingFinished.emit()
+        
         self.gui.settings_box.check_load()
 
 
 # NOTE: spikeinterface should not be imported anywhere else in this module to
 #       avoid an explicit dependency.
 def get_recording_extractor(filename, filetype, stream_id=None, stream_name=None):
     '''Load recording by importing an extractor from spikeinterface.'''
@@ -306,20 +324,12 @@
 class ConversionThread(QtCore.QThread):
 
     def __init__(self, parent, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.parent = parent
 
     def run(self):
-        _, N, c, s, fs, probe_filename = spikeinterface_to_binary(
+        _, _, self.c, _, self.fs, self.probe_filename = spikeinterface_to_binary(
             self.recording, self.bin_filename.parent,
             data_name=self.bin_filename.name,
             dtype=self.parent.data_dtype
         )
-
-        settings = self.parent.gui.settings_box
-        update_settings_box(settings, c, fs, self.parent.data_dtype)
-        if probe_filename is not None:
-            add_probe_to_settings(settings, probe_filename)
-
-        settings.data_file_path_input.setText(self.bin_filename.as_posix())
-        settings.data_file_path_input.editingFinished.emit()
```

### Comparing `kilosort-4.0.3/kilosort/gui/data_view_box.py` & `kilosort-4.0.4/kilosort/gui/data_view_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/header_box.py` & `kilosort-4.0.4/kilosort/gui/header_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/launch.py` & `kilosort-4.0.4/kilosort/gui/launch.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/logger.py` & `kilosort-4.0.4/kilosort/gui/logger.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/main.py` & `kilosort-4.0.4/kilosort/gui/main.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/message_log_box.py` & `kilosort-4.0.4/kilosort/gui/message_log_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/minor_gui_elements.py` & `kilosort-4.0.4/kilosort/gui/minor_gui_elements.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/palettes.py` & `kilosort-4.0.4/kilosort/gui/palettes.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/run_box.py` & `kilosort-4.0.4/kilosort/gui/run_box.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/sanity_plots.py` & `kilosort-4.0.4/kilosort/gui/sanity_plots.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/gui/settings_box.py` & `kilosort-4.0.4/kilosort/gui/settings_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logger = setup_logger(__name__)
 
 _DEFAULT_DTYPE = 'int16'
 _ALLOWED_FILE_TYPES = ['.bin', '.dat', '.bat', '.raw']  # For binary data
 
 class SettingsBox(QtWidgets.QGroupBox):
     settingsUpdated = QtCore.Signal()
-    previewProbe = QtCore.Signal(object)
+    previewProbe = QtCore.Signal(object, object)
     dataChanged = QtCore.Signal()
 
     def __init__(self, parent):
         QtWidgets.QGroupBox.__init__(self, parent=parent)
 
         self.gui = parent
         self.load_enabled = False
@@ -470,17 +470,18 @@
             self.settings[k] = getattr(self, k)
         for k in list(EXTRA_PARAMETERS.keys()):
             self.settings[k] = getattr(self.extra_parameters_window, k)
 
         if not self.check_valid_binary_path(self.data_file_path):
             return False
 
-        none_allowed = ['dmin', 'nt0min']
+        none_allowed = ['dmin', 'nt0min', 'max_channel_distance', 'x_centers']
         for k, v in self.settings.items():
             if v is None and k not in none_allowed:
+                print(f'`None` not allowed for parameter {k}.')
                 return False
         return True
     
     @QtCore.Slot()
     def update_parameter(self):
         parameter_key = self.sender().var_name
         parameter_info = MAIN_PARAMETERS[parameter_key]
@@ -496,17 +497,25 @@
                 except Exception as e:
                     logger.exception(e)
                     self.disable_load()
 
             else:
                 self.settingsUpdated.emit()
 
+    def get_probe_template_args(self):
+        epw = self.extra_parameters_window
+        template_args = [
+            epw.nearest_chans, epw.dmin, epw.dminx, 
+            epw.max_channel_distance, epw.x_centers, self.gui.device
+            ]
+        return template_args
+
     @QtCore.Slot()
     def show_probe_layout(self):
-        self.previewProbe.emit(self.probe_layout)
+        self.previewProbe.emit(self.probe_layout, self.get_probe_template_args())
 
     @QtCore.Slot(str)
     def on_probe_layout_selected(self, name):
         if name not in ["", "[new]", "other..."]:
             probe_path = Path(self.gui.new_probe_files_path).joinpath(name)
             try:
                 probe_layout = load_probe(probe_path)
@@ -660,14 +669,20 @@
             ]
             probes_list.extend(probes)
 
         probes_list.sort(key=lambda f: os.path.splitext(f)[1])
         self.probe_layout_selector.addItems([""] + probes_list + ["[new]", "other..."])
         self._probes = probes_list
 
+    def clear_probe_selection(self):
+        self.probe_layout_selector.setCurrentIndex(0)
+        self.gui.qt_settings.setValue('probe_layout', None)
+        self.gui.qt_settings.setValue('probe_name', None)
+        self.disable_preview_probe()
+
     def populate_dtype_selector(self):
         self.dtype_selector.clear()
         supported_dtypes = BinaryRWFile.supported_dtypes
         self.dtype_selector.addItems(supported_dtypes)
 
     def populate_device_selector(self):
         self.device_selector.clear()
@@ -714,19 +729,16 @@
     def reset(self):
         self.data_file_path_input.clear()
         self.data_file_path = None
         self.gui.qt_settings.setValue('data_file_path', None)
         self.results_directory_input.clear()
         self.results_directory_path = None
         self.gui.qt_settings.setValue('results_dir', None)
-        self.probe_layout_selector.setCurrentIndex(0)
-        self.gui.qt_settings.setValue('probe_layout', None)
-        self.gui.qt_settings.setValue('probe_name', None)
+        self.clear_probe_selection()
         self.set_default_field_values()
-        self.disable_preview_probe()
         self.disable_load()
 
     def check_load(self):
         if self.check_settings():
             self.enable_load()
         else:
             self.disable_load()
```

### Comparing `kilosort-4.0.3/kilosort/gui/sorter.py` & `kilosort-4.0.4/kilosort/gui/sorter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/hierarchical.py` & `kilosort-4.0.4/kilosort/hierarchical.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/io.py` & `kilosort-4.0.4/kilosort/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -541,16 +541,22 @@
         
 
 def get_total_samples(filename, n_channels, dtype=np.int16):
     """Count samples in binary file given dtype and number of channels."""
     bytes_per_value = np.dtype(dtype).itemsize
     bytes_per_sample = np.int64(bytes_per_value * n_channels)
     total_bytes = os.path.getsize(filename)
+    samples = (total_bytes / bytes_per_sample)
 
-    return int(total_bytes / bytes_per_sample)
+    if samples%1 != 0:
+        raise ValueError(
+            "Bytes in binary file did not divide evenly, incorrect n_chan_bin."
+        )
+    else:
+        return int(samples)
 
 
 class BinaryFileGroup:
     def __init__(self, file_objects):
         # NOTE: Assumes list order of files matches temporal order for
         #       concatenation.
         self.file_objects = file_objects
```

### Comparing `kilosort-4.0.3/kilosort/parameters.py` & `kilosort-4.0.4/kilosort/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,25 @@
         'description':
             """
             Number of nearest spike template locations to consider when finding
             local maxima during spike detection.
             """
     },
 
+    'max_channel_distance': {
+        'gui_name': 'max channel distance', 'type': float, 'min': 1,
+        'max': np.inf, 'exclude': [], 'default': None, 'step': 'spike detection',
+        'description':
+            """
+            Templates farther away than this from their nearest channel will
+            not be used. Also limits distance between compared channels during
+            clustering.
+            """
+    },
+
     'templates_from_data': {
         'gui_name': 'templates from data', 'type': bool, 'min': None, 'max': None,
         'exclude': [], 'default': True, 'step': 'spike detection',
         'description':
             """
             Indicates whether spike shapes used in universal templates should be 
             estimated from the data or loaded from the predefined templates.
@@ -315,14 +326,27 @@
         'exclude': [], 'default': 64, 'step': 'clustering',
         'description':
             """
             Maximum number of spatiotemporal PC features used for clustering.
             """
     },
 
+    'x_centers': {
+        'gui_name': 'x centers', 'type': int, 'min': 1,
+        'max': np.inf, 'exclude': [], 'default': None, 'step': 'clustering',
+        'description':
+            """
+            Number of x-positions to use when determining center points for
+            template groupings. If None, this will be determined automatically
+            by finding peaks in channel density. For 2D array type probes, we
+            recommend specifying this so that centers are placed every few
+            hundred microns.
+            """
+    },
+
 
     ### POSTPROCESSING
     'duplicate_spike_bins': {
         'gui_name': 'duplicate spike bins', 'type': int, 'min': 0, 'max': np.inf,
         'exclude': [], 'default': 15, 'step': 'postprocessing',
         'description':
             """
```

### Comparing `kilosort-4.0.3/kilosort/postprocessing.py` & `kilosort-4.0.4/kilosort/postprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/preprocessing.py` & `kilosort-4.0.4/kilosort/preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/run_kilosort.py` & `kilosort-4.0.4/kilosort/run_kilosort.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,17 +100,14 @@
         raise ValueError(
             '`n_chan_bin` is a required setting. This is the total number of '
             'channels in the binary file, which may or may not be equal to the '
             'number of channels specified by the probe.'
             )
     settings = {**DEFAULT_SETTINGS, **settings}
 
-    if settings['nt0min'] is None:
-        settings['nt0min'] = int(20 * settings['nt']/61)
-
     if data_dtype is None:
         print("Interpreting binary file as default dtype='int16'. If data was "
                 "saved in a different format, specify `data_dtype`.")
 
     if device is None:
         if torch.cuda.is_available():
             print('Using GPU for PyTorch computations. '
@@ -198,14 +195,16 @@
 
     return filename, data_dir, results_dir, probe
 
 
 def initialize_ops(settings, probe, data_dtype, do_CAR, invert_sign, device) -> dict:
     """Package settings and probe information into a single `ops` dictionary."""
 
+    if settings['nt0min'] is None:
+        settings['nt0min'] = int(20 * settings['nt']/61)
     # TODO: Clean this up during refactor. Lots of confusing duplication here.
     ops = settings  
     ops['settings'] = settings 
     ops['probe'] = probe
     ops['data_dtype'] = data_dtype
     ops['do_CAR'] = do_CAR
     ops['invert_sign'] = invert_sign
```

### Comparing `kilosort-4.0.3/kilosort/simulation.py` & `kilosort-4.0.4/kilosort/simulation.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/spikedetect.py` & `kilosort-4.0.4/kilosort/spikedetect.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,14 +94,18 @@
     ops['dmin'] = dmin
     ops['yup'] = np.arange(ymin, ymax+.00001, dmin//2)
 
     ops['dminx'] = dminx = ops['settings']['dminx']
     nx = np.round((xmax - xmin) / (dminx/2)) + 1
     ops['xup'] = np.linspace(xmin, xmax, int(nx))
 
+    # Set max channel distance based on dmin, dminx, use whichever is greater.
+    if ops.get('max_channel_distance', None) is None:
+        ops['max_channel_distance'] = max(dmin, dminx)
+
     return ops
 
 
 def template_match(X, ops, iC, iC2, weigh, device=torch.device('cuda')):
     NT = X.shape[-1]
     nt = ops['nt']
     Nchan = ops['Nchan']
@@ -157,16 +161,18 @@
 
 
 def nearest_chans(ys, yc, xs, xc, nC, device=torch.device('cuda')):
     ds = (ys - yc[:,np.newaxis])**2 + (xs - xc[:,np.newaxis])**2
     iC = np.argsort(ds, 0)[:nC]
     iC = torch.from_numpy(iC).to(device)
     ds = np.sort(ds, 0)[:nC]
+
     return iC, ds
 
+
 def yweighted(yc, iC, adist, xy, device=torch.device('cuda')):    
 
     yy = torch.from_numpy(yc).to(device)[iC]
     cF0 = torch.nn.functional.relu(adist)
     cF0 = cF0/cF0.sum(0)
 
     yct = (cF0 * yy[:,xy[:,0]]).sum(0)
@@ -186,25 +192,32 @@
             )
     else:
         print('Using built-in universal templates.')
         # Use pre-computed templates.
         ops['wPCA'], ops['wTEMP'] = get_waves(ops, device=device)
 
     ops = template_centers(ops)
-
     [ys, xs] = np.meshgrid(ops['yup'], ops['xup'])
     ys, xs = ys.flatten(), xs.flatten()
-    ops['ycup'], ops['xcup'] = ys, xs
-
     xc, yc = ops['xc'], ops['yc']
     Nfilt = len(ys)
 
     nC = ops['settings']['nearest_chans']
     nC2 = ops['settings']['nearest_templates']
     iC, ds = nearest_chans(ys, yc, xs, xc, nC, device=device)
+
+    # Don't use templates that are too far away from nearest channel
+    # (use square of max distance since ds are squared distances)
+    igood = ds[0,:] <= ops['max_channel_distance']**2
+    iC = iC[:,igood]
+    ds = ds[:,igood]
+    ys = ys[igood]
+    xs = xs[igood]
+    ops['ycup'], ops['xcup'] = ys, xs
+
     iC2, ds2 = nearest_chans(ys, ys, xs, xs, nC2, device=device)
 
     ds_torch = torch.from_numpy(ds).to(device).float()
     template_sizes = sig * (1+torch.arange(nsizes, device=device))
     weigh = torch.exp(-ds_torch.unsqueeze(-1) / template_sizes**2)
     weigh = torch.permute(weigh, (2, 0, 1)).contiguous()
     weigh = weigh / (weigh**2).sum(1).unsqueeze(1)**.5
```

### Comparing `kilosort-4.0.3/kilosort/swarmsplitter.py` & `kilosort-4.0.4/kilosort/swarmsplitter.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/template_matching.py` & `kilosort-4.0.4/kilosort/template_matching.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/utils.py` & `kilosort-4.0.4/kilosort/utils.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort/wTEMP.npz` & `kilosort-4.0.4/kilosort/wTEMP.npz`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/kilosort.egg-info/PKG-INFO` & `kilosort-4.0.4/kilosort.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kilosort
-Version: 4.0.3
+Version: 4.0.4
 Summary: spike sorting pipeline
 Home-page: https://github.com/MouseLand/kilosort
 Author: Marius Pachitariu
 Author-email: pachitarium@janelia.hhmi.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,30 +49,30 @@
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/blob/master/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/kilosort)](https://github.com/MouseLand/kilosort/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/kilosort?style=social)](https://github.com/MouseLand/kilosort/)
 
 
-You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots.
+You can run Kilosort4 without installing it locally using google colab. An example colab notebook is available [here](https://colab.research.google.com/drive/1gFZa8TEBDXmg_CB5RwuT_52Apl3hP0Ie?usp=sharing). It will download some test data, run kilosort4 on it, and show some plots. Talk describing Kilosort4 is [here](https://www.youtube.com/watch?v=LTSmoACr918). 
 
 Example notebooks are provided in the `docs/source/tutorials` folder and in the [docs](https://kilosort.readthedocs.io/en/latest/tutorials/tutorials.html). The notebooks include: 
 
   1. `basic_example`:  sets up run on example data and shows how to modify parameters  
   2. `load_data`:  example data format conversion through SpikeInterface  
   3. `make_probe`:  making a custom probe configuration.
 
-**If you use Kilosort1-4, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.01.07.523036v1):**     
+**If you use Kilosort1-4, please cite the [paper](https://www.nature.com/articles/s41592-024-02232-7):**     
 Pachitariu, M., Sridhar, S., Pennington, J., & Stringer, C. (2024). Spike sorting with Kilosort4.
 
-**Warning** :bangbang:: There was a bug in Kilosort 2.5 and 3 (but not 1,2 and 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch0 releases fix this bug. It is also advised not to manually change the batch size in any Matlab-version of Kilosort (1-3). **Update** :bangbang:: The patch introduced a misalignment of spike times relative to the data, which we are currently working to fix. 
+**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks or 2D arrays. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
 
-**Note on multi-shank probes** : We are aware of some issues with sorting data from probes with multiple shanks. See [documentation here](https://kilosort.readthedocs.io/en/latest/multi_shank.html) for recommended workarounds until the code is updated to handle these probes.
+**Note on reusing parameters from previous versions**: This probably will not work well. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
 
-**Note on reusing parameters from previous versions**: Please don't do this. Kilosort4 is a new algorithm, and the main parameters (the thresholds) can affect the results in a different way for your data. Please start with the default parameters and adjust from there based on what you see in Phy. 
+**Warning** :bangbang:: There were two bugs in Kilosort 2, 2.5 and 3 (but not 4) which caused fewer spikes to be detected in ~7ms periods at batch boundaries (every 2.1866s, issue #594). The patch1 releases fix these bugs, please use the new default NT and ntbuff parameters. 
 
 ## Installation
 
 ### System requirements
 
 Linux and Windows 64-bit are supported for running the code. At least 8GB of GPU RAM is required to run the software (see [docs](https://kilosort.readthedocs.io/en/latest/hardware.html) for more recommendations). The software has been tested on Windows 10 and Ubuntu 20.04.
```

### Comparing `kilosort-4.0.3/kilosort.egg-info/SOURCES.txt` & `kilosort-4.0.4/kilosort.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,14 @@
 kilosort/gui/palettes.py
 kilosort/gui/probe_view_box.py
 kilosort/gui/run_box.py
 kilosort/gui/sanity_plots.py
 kilosort/gui/settings_box.py
 kilosort/gui/sorter.py
 tests/conftest.py
+tests/test_clustering.py
 tests/test_dtype.py
 tests/test_full_pipeline.py
 tests/test_io.py
 tests/test_parameters.py
 tests/test_preprocessing.py
 tests/test_spikedetect.py
```

### Comparing `kilosort-4.0.3/setup.py` & `kilosort-4.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tests/conftest.py` & `kilosort-4.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tests/test_dtype.py` & `kilosort-4.0.4/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tests/test_full_pipeline.py` & `kilosort-4.0.4/tests/test_full_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,18 @@
     # Less than 2.5% difference in spike count, 5% difference in number of units
     # TODO: Make sure these are reasonable error bounds
     spikes_error = np.abs(st.size - st_load.size)/np.max([st.size, st_load.size])
     with capture_mgr.global_and_fixture_disabled():
         print(f'Proportion difference in total spike count: {spikes_error}')
         print(f'Count from run_kilosort: {st.size}')
         print(f'Count from saved test results: {st_load.size}')
-    assert spikes_error <= 0.025
 
     n = np.unique(clu).size
     n_load = np.unique(clu_load).size
     unit_count_error = np.abs(n - n_load)/np.max([n, n_load])
     with capture_mgr.global_and_fixture_disabled():
         print(f'Proportion difference in number of units: {unit_count_error}')
         print(f'Number of units from run_kilosort: {n}')
         print(f'Number of units from saved test results: {n_load}')
+
+    assert spikes_error <= 0.025
     assert unit_count_error <= 0.05
```

### Comparing `kilosort-4.0.3/tests/test_io.py` & `kilosort-4.0.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tests/test_parameters.py` & `kilosort-4.0.4/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tests/test_preprocessing.py` & `kilosort-4.0.4/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kilosort-4.0.3/tox.ini` & `kilosort-4.0.4/tox.ini`

 * *Files identical despite different names*

