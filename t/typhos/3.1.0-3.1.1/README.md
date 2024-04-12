# Comparing `tmp/typhos-3.1.0.tar.gz` & `tmp/typhos-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typhos-3.1.0.tar", last modified: Wed Dec  6 18:58:11 2023, max compression
+gzip compressed data, was "typhos-3.1.1.tar", last modified: Fri Apr 12 22:32:18 2024, max compression
```

## Comparing `typhos-3.1.0.tar` & `typhos-3.1.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.652828 typhos-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-06 18:57:58.000000 typhos-3.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-12-06 18:57:58.000000 typhos-3.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-06 18:57:58.000000 typhos-3.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-06 18:57:58.000000 typhos-3.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.628828 typhos-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-06 18:57:58.000000 typhos-3.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-06 18:57:58.000000 typhos-3.1.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.628828 typhos-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-06 18:57:58.000000 typhos-3.1.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-12-06 18:57:58.000000 typhos-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-06 18:57:58.000000 typhos-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-06 18:57:58.000000 typhos-3.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2023-12-06 18:57:58.000000 typhos-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-12-06 18:57:58.000000 typhos-3.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-06 18:57:58.000000 typhos-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2023-12-06 18:58:11.652828 typhos-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-12-06 18:57:58.000000 typhos-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.628828 typhos-3.1.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-12-06 18:57:58.000000 typhos-3.1.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-06 18:57:58.000000 typhos-3.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.628828 typhos-3.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)      901 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.632828 typhos-3.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.632828 typhos-3.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   190974 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/_static/device_display.gif
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/_static/expanded.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/_static/function.png
--rw-r--r--   0 runner    (1001) docker     (127)    37320 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/_static/hydra.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   268419 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/_static/kind_panel.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12534 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/display.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/python_methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/save.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.632828 typhos-3.1.0/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/upcoming_release_notes/template-short.rst
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-12-06 18:57:58.000000 typhos-3.1.0/docs/source/widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-06 18:57:58.000000 typhos-3.1.0/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-12-06 18:57:58.000000 typhos-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-06 18:57:58.000000 typhos-3.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-06 18:57:58.000000 typhos-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 18:58:11.652828 typhos-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.636828 typhos-3.1.0/typhos/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.640828 typhos-3.1.0/typhos/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/benchmark/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11271 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    59564 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/dynamic_font.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.640828 typhos-3.1.0/typhos/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/examples/device_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/examples/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/examples/positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29836 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.640828 typhos-3.1.0/typhos/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/plugins/happi.py
--rw-r--r--   0 runner    (1001) docker     (127)    38864 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/related_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    31646 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.644828 typhos-3.1.0/typhos/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/empty_saved_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/happi.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/happi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.644828 typhos-3.1.0/typhos/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/plugins/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/plugins/test_happi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_dynamic_font.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_related_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/test_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.644828 typhos-3.1.0/typhos/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/big_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/env_device_notes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   473831 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/lenna.png
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/python.png
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/sig.ui
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/tiny_stylesheet.qss
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/utils/user_device_notes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tests/variety_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/textedit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tools/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tools/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/tweakable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos/ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos/ui/core/
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/core/detailed_screen.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/core/detailed_tree.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/core/embedded_screen.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/core/engineering_screen.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos/ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/devices/PositionerBase.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/devices/PositionerBase.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    94114 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)    23549 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/widgets/positioner.ui
--rw-r--r--   0 runner    (1001) docker     (127)    39208 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/widgets/positioner_row.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/ui/widgets/tweakable.ui
--rw-r--r--   0 runner    (1001) docker     (127)    54849 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/variety.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/web.py
--rw-r--r--   0 runner    (1001) docker     (127)    40087 2023-12-06 18:57:58.000000 typhos-3.1.0/typhos/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 18:58:11.648828 typhos-3.1.0/typhos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-06 18:58:11.000000 typhos-3.1.0/typhos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.757995 typhos-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 22:32:06.000000 typhos-3.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-12 22:32:06.000000 typhos-3.1.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 22:32:06.000000 typhos-3.1.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 22:32:06.000000 typhos-3.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.733995 typhos-3.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 22:32:06.000000 typhos-3.1.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-12 22:32:06.000000 typhos-3.1.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.733995 typhos-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 22:32:06.000000 typhos-3.1.1/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-12 22:32:06.000000 typhos-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 22:32:06.000000 typhos-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 22:32:06.000000 typhos-3.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-12 22:32:06.000000 typhos-3.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 22:32:06.000000 typhos-3.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 22:32:06.000000 typhos-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-04-12 22:32:18.757995 typhos-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-12 22:32:06.000000 typhos-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.737995 typhos-3.1.1/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-12 22:32:06.000000 typhos-3.1.1/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 22:32:06.000000 typhos-3.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.737995 typhos-3.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.737995 typhos-3.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.737995 typhos-3.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   190974 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/_static/device_display.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/_static/expanded.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/_static/function.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37320 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/_static/hydra.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   268419 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/_static/kind_panel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/display.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/python_methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30966 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/save.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.741995 typhos-3.1.1/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-12 22:32:06.000000 typhos-3.1.1/docs/source/widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 22:32:06.000000 typhos-3.1.1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-12 22:32:06.000000 typhos-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 22:32:06.000000 typhos-3.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-12 22:32:06.000000 typhos-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:32:18.757995 typhos-3.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.741995 typhos-3.1.1/typhos/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.745995 typhos-3.1.1/typhos/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/benchmark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59564 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/dynamic_font.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.745995 typhos-3.1.1/typhos/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/examples/device_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/examples/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/examples/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29836 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.745995 typhos-3.1.1/typhos/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/plugins/happi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38864 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/related_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31646 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.749995 typhos-3.1.1/typhos/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/empty_saved_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/happi.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/happi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.749995 typhos-3.1.1/typhos/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/plugins/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/plugins/test_happi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_dynamic_font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_related_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.749995 typhos-3.1.1/typhos/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/big_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/env_device_notes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   473831 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/lenna.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/sig.ui
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/tiny_stylesheet.qss
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/utils/user_device_notes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tests/variety_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/textedit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tools/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tools/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tools/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/tweakable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos/ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos/ui/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/core/detailed_screen.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/core/detailed_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/core/embedded_screen.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/core/engineering_screen.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos/ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/devices/PositionerBase.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/devices/PositionerBase.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    94114 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/widgets/positioner.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    39202 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/widgets/positioner_row.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/ui/widgets/tweakable.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    54849 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/variety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40087 2024-04-12 22:32:06.000000 typhos-3.1.1/typhos/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:32:18.753995 typhos-3.1.1/typhos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:32:18.000000 typhos-3.1.1/typhos.egg-info/top_level.txt
```

### Comparing `typhos-3.1.0/.flake8` & `typhos-3.1.1/.flake8`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/.github/ISSUE_TEMPLATE.md` & `typhos-3.1.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `typhos-3.1.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/.github/workflows/standard.yml` & `typhos-3.1.1/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/.gitignore` & `typhos-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/.pre-commit-config.yaml` & `typhos-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/CONTRIBUTING.rst` & `typhos-3.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/LICENSE.md` & `typhos-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/PKG-INFO` & `typhos-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typhos
-Version: 3.1.0
+Version: 3.1.1
 Summary: Interface generation for ophyd devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `typhos-3.1.0/README.md` & `typhos-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/conda-recipe/meta.yaml` & `typhos-3.1.1/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/Makefile` & `typhos-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/pre-release-notes.sh` & `typhos-3.1.1/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/release_notes.py` & `typhos-3.1.1/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/_static/device_display.gif` & `typhos-3.1.1/docs/source/_static/device_display.gif`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/_static/expanded.jpg` & `typhos-3.1.1/docs/source/_static/expanded.jpg`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/_static/function.png` & `typhos-3.1.1/docs/source/_static/function.png`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/_static/hydra.jpg` & `typhos-3.1.1/docs/source/_static/hydra.jpg`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/_static/kind_panel.gif` & `typhos-3.1.1/docs/source/_static/kind_panel.gif`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/basic_usage.rst` & `typhos-3.1.1/docs/source/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/conf.py` & `typhos-3.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/connections.rst` & `typhos-3.1.1/docs/source/connections.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/display.rst` & `typhos-3.1.1/docs/source/display.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/index.rst` & `typhos-3.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/plugins.rst` & `typhos-3.1.1/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/python_methods.rst` & `typhos-3.1.1/docs/source/python_methods.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/release_notes.rst` & `typhos-3.1.1/docs/source/release_notes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Release History
 ###############
 
+
+v3.1.1 (2024-04-12)
+===================
+
+Fixes
+-----
+- Change position widget limit colors from yellow off/yellow on to
+  dark gray off/orange on for better contrast.
+
+Contributors
+------------
+- zllentz
+
+
 v3.1.0 (2023-12-05)
 ===================
 
 Features
 --------
 - Add overridable ``find_signal`` method to the ``SignalConnection`` class to allow
   the use of alternate signal registries in subclasses.
```

### Comparing `typhos-3.1.0/docs/source/save.rst` & `typhos-3.1.1/docs/source/save.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/templates.rst` & `typhos-3.1.1/docs/source/templates.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/tools.rst` & `typhos-3.1.1/docs/source/tools.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/upcoming_release_notes/template-full.rst` & `typhos-3.1.1/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/utils.rst` & `typhos-3.1.1/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/docs/source/widgets.rst` & `typhos-3.1.1/docs/source/widgets.rst`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/pyproject.toml` & `typhos-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/__init__.py` & `typhos-3.1.1/typhos/__init__.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/alarm.py` & `typhos-3.1.1/typhos/alarm.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/app.py` & `typhos-3.1.1/typhos/app.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/benchmark/cases.py` & `typhos-3.1.1/typhos/benchmark/cases.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/benchmark/device.py` & `typhos-3.1.1/typhos/benchmark/device.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/benchmark/ioc.py` & `typhos-3.1.1/typhos/benchmark/ioc.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/benchmark/profile.py` & `typhos-3.1.1/typhos/benchmark/profile.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/benchmark/utils.py` & `typhos-3.1.1/typhos/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/cache.py` & `typhos-3.1.1/typhos/cache.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/cli.py` & `typhos-3.1.1/typhos/cli.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/display.py` & `typhos-3.1.1/typhos/display.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/dynamic_font.py` & `typhos-3.1.1/typhos/dynamic_font.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/examples/device_classes.py` & `typhos-3.1.1/typhos/examples/device_classes.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/examples/panel.py` & `typhos-3.1.1/typhos/examples/panel.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/examples/positioner.py` & `typhos-3.1.1/typhos/examples/positioner.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/func.py` & `typhos-3.1.1/typhos/func.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/jira.py` & `typhos-3.1.1/typhos/jira.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/notes.py` & `typhos-3.1.1/typhos/notes.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/panel.py` & `typhos-3.1.1/typhos/panel.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/plugins/core.py` & `typhos-3.1.1/typhos/plugins/core.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/plugins/happi.py` & `typhos-3.1.1/typhos/plugins/happi.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/positioner.py` & `typhos-3.1.1/typhos/positioner.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/related_display.py` & `typhos-3.1.1/typhos/related_display.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/status.py` & `typhos-3.1.1/typhos/status.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/suite.py` & `typhos-3.1.1/typhos/suite.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/conftest.py` & `typhos-3.1.1/typhos/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/happi.json` & `typhos-3.1.1/typhos/tests/happi.json`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/plugins/test_core.py` & `typhos-3.1.1/typhos/tests/plugins/test_core.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/plugins/test_happi.py` & `typhos-3.1.1/typhos/tests/plugins/test_happi.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_alarm.py` & `typhos-3.1.1/typhos/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_benchmark.py` & `typhos-3.1.1/typhos/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_cache.py` & `typhos-3.1.1/typhos/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_cli.py` & `typhos-3.1.1/typhos/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_display.py` & `typhos-3.1.1/typhos/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_dynamic_font.py` & `typhos-3.1.1/typhos/tests/test_dynamic_font.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_func.py` & `typhos-3.1.1/typhos/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_log.py` & `typhos-3.1.1/typhos/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_notes.py` & `typhos-3.1.1/typhos/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_panel.py` & `typhos-3.1.1/typhos/tests/test_panel.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_plot.py` & `typhos-3.1.1/typhos/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_positioner.py` & `typhos-3.1.1/typhos/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_related_display.py` & `typhos-3.1.1/typhos/tests/test_related_display.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_status.py` & `typhos-3.1.1/typhos/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_suite.py` & `typhos-3.1.1/typhos/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_utils.py` & `typhos-3.1.1/typhos/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/test_widgets.py` & `typhos-3.1.1/typhos/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/utils/big_stylesheet.qss` & `typhos-3.1.1/typhos/tests/utils/big_stylesheet.qss`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/utils/lenna.png` & `typhos-3.1.1/typhos/tests/utils/lenna.png`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/utils/python.png` & `typhos-3.1.1/typhos/tests/utils/python.png`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/utils/sig.ui` & `typhos-3.1.1/typhos/tests/utils/sig.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tests/variety_ioc.py` & `typhos-3.1.1/typhos/tests/variety_ioc.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/textedit.py` & `typhos-3.1.1/typhos/textedit.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tools/log.py` & `typhos-3.1.1/typhos/tools/log.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tools/plot.py` & `typhos-3.1.1/typhos/tools/plot.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/tweakable.py` & `typhos-3.1.1/typhos/tweakable.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/core/detailed_screen.ui` & `typhos-3.1.1/typhos/ui/core/detailed_screen.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/core/detailed_tree.ui` & `typhos-3.1.1/typhos/ui/core/detailed_tree.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/core/embedded_screen.ui` & `typhos-3.1.1/typhos/ui/core/embedded_screen.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/core/engineering_screen.ui` & `typhos-3.1.1/typhos/ui/core/engineering_screen.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/devices/PositionerBase.detailed.ui` & `typhos-3.1.1/typhos/ui/devices/PositionerBase.detailed.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/devices/PositionerBase.embedded.ui` & `typhos-3.1.1/typhos/ui/devices/PositionerBase.embedded.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/loading.gif` & `typhos-3.1.1/typhos/ui/loading.gif`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/style.qss` & `typhos-3.1.1/typhos/ui/style.qss`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/ui/widgets/positioner.ui` & `typhos-3.1.1/typhos/ui/widgets/positioner.ui`

 * *Files 2% similar despite different names*

#### Comparing `typhos-3.1.0/typhos/ui/widgets/positioner.ui` & `typhos-3.1.1/typhos/ui/widgets/positioner.ui`

```diff
@@ -122,24 +122,24 @@
     parent : QWidget
         The parent widget for the Label
     init_channel : str, optional
         The channel to be used by the widget.</string>
                         </property>
                         <property name="onColor" stdset="0">
                           <color>
-                            <red>239</red>
-                            <green>246</green>
-                            <blue>20</blue>
+                            <red>255</red>
+                            <green>150</green>
+                            <blue>0</blue>
                           </color>
                         </property>
                         <property name="offColor" stdset="0">
                           <color>
-                            <red>178</red>
-                            <green>188</green>
-                            <blue>17</blue>
+                            <red>50</red>
+                            <green>50</green>
+                            <blue>50</blue>
                           </color>
                         </property>
                         <property name="showLabels" stdset="0">
                           <bool>false</bool>
                         </property>
                         <property name="circles" stdset="0">
                           <bool>true</bool>
@@ -585,24 +585,24 @@
         The channel to be used by the widget.</string>
                         </property>
                         <property name="styleSheet">
                           <string notr="true">margin: 0px;</string>
                         </property>
                         <property name="onColor" stdset="0">
                           <color>
-                            <red>239</red>
-                            <green>246</green>
-                            <blue>20</blue>
+                            <red>255</red>
+                            <green>150</green>
+                            <blue>0</blue>
                           </color>
                         </property>
                         <property name="offColor" stdset="0">
                           <color>
-                            <red>178</red>
-                            <green>188</green>
-                            <blue>17</blue>
+                            <red>50</red>
+                            <green>50</green>
+                            <blue>50</blue>
                           </color>
                         </property>
                         <property name="orientation" stdset="0">
                           <enum>Qt::Vertical</enum>
                         </property>
                         <property name="showLabels" stdset="0">
                           <bool>false</bool>
```

### Comparing `typhos-3.1.0/typhos/ui/widgets/positioner_row.ui` & `typhos-3.1.1/typhos/ui/widgets/positioner_row.ui`

 * *Files 1% similar despite different names*

#### Comparing `typhos-3.1.0/typhos/ui/widgets/positioner_row.ui` & `typhos-3.1.1/typhos/ui/widgets/positioner_row.ui`

```diff
@@ -475,24 +475,24 @@
         The channel to be used by the widget.</string>
                     </property>
                     <property name="alarmSensitiveBorder" stdset="0">
                       <bool>false</bool>
                     </property>
                     <property name="onColor" stdset="0">
                       <color>
-                        <red>239</red>
-                        <green>246</green>
-                        <blue>20</blue>
+                        <red>255</red>
+                        <green>150</green>
+                        <blue>0</blue>
                       </color>
                     </property>
                     <property name="offColor" stdset="0">
                       <color>
-                        <red>178</red>
-                        <green>188</green>
-                        <blue>17</blue>
+                        <red>50</red>
+                        <green>50</green>
+                        <blue>50</blue>
                       </color>
                     </property>
                     <property name="showLabels" stdset="0">
                       <bool>false</bool>
                     </property>
                     <property name="circles" stdset="0">
                       <bool>true</bool>
@@ -769,24 +769,24 @@
                       <string notr="true">margin: 0px;</string>
                     </property>
                     <property name="alarmSensitiveBorder" stdset="0">
                       <bool>false</bool>
                     </property>
                     <property name="onColor" stdset="0">
                       <color>
-                        <red>239</red>
-                        <green>246</green>
-                        <blue>20</blue>
+                        <red>255</red>
+                        <green>150</green>
+                        <blue>0</blue>
                       </color>
                     </property>
                     <property name="offColor" stdset="0">
                       <color>
-                        <red>178</red>
-                        <green>188</green>
-                        <blue>17</blue>
+                        <red>50</red>
+                        <green>50</green>
+                        <blue>50</blue>
                       </color>
                     </property>
                     <property name="orientation" stdset="0">
                       <enum>Qt::Vertical</enum>
                     </property>
                     <property name="showLabels" stdset="0">
                       <bool>false</bool>
@@ -1268,20 +1268,20 @@
     </customwidget>
     <customwidget>
       <class>TyphosDisplaySwitcher</class>
       <extends>QFrame</extends>
       <header>typhos.display</header>
     </customwidget>
     <customwidget>
-      <class>TyphosRelatedSuiteButton</class>
-      <extends>QPushButton</extends>
-      <header>typhos.related_display</header>
-    </customwidget>
-    <customwidget>
       <class>TyphosNotesEdit</class>
       <extends>QLineEdit</extends>
       <header>typhos.notes</header>
     </customwidget>
+    <customwidget>
+      <class>TyphosRelatedSuiteButton</class>
+      <extends>QPushButton</extends>
+      <header>typhos.related_display</header>
+    </customwidget>
   </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `typhos-3.1.0/typhos/ui/widgets/tweakable.ui` & `typhos-3.1.1/typhos/ui/widgets/tweakable.ui`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/utils.py` & `typhos-3.1.1/typhos/utils.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/variety.py` & `typhos-3.1.1/typhos/variety.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/version.py` & `typhos-3.1.1/typhos/version.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/web.py` & `typhos-3.1.1/typhos/web.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos/widgets.py` & `typhos-3.1.1/typhos/widgets.py`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos.egg-info/PKG-INFO` & `typhos-3.1.1/typhos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typhos
-Version: 3.1.0
+Version: 3.1.1
 Summary: Interface generation for ophyd devices
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `typhos-3.1.0/typhos.egg-info/SOURCES.txt` & `typhos-3.1.1/typhos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typhos-3.1.0/typhos.egg-info/entry_points.txt` & `typhos-3.1.1/typhos.egg-info/entry_points.txt`

 * *Files identical despite different names*

