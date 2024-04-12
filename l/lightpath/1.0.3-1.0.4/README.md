# Comparing `tmp/lightpath-1.0.3.tar.gz` & `tmp/lightpath-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightpath-1.0.3.tar", last modified: Thu Sep 14 21:21:35 2023, max compression
+gzip compressed data, was "lightpath-1.0.4.tar", last modified: Fri Apr 12 22:28:36 2024, max compression
```

## Comparing `lightpath-1.0.3.tar` & `lightpath-1.0.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.894442 lightpath-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-09-14 21:21:11.000000 lightpath-1.0.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-09-14 21:21:11.000000 lightpath-1.0.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-14 21:21:11.000000 lightpath-1.0.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-14 21:21:11.000000 lightpath-1.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.874442 lightpath-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-14 21:21:11.000000 lightpath-1.0.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-14 21:21:11.000000 lightpath-1.0.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.874442 lightpath-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-14 21:21:11.000000 lightpath-1.0.3/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-14 21:21:11.000000 lightpath-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-09-14 21:21:11.000000 lightpath-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-14 21:21:11.000000 lightpath-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-09-14 21:21:11.000000 lightpath-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-09-14 21:21:11.000000 lightpath-1.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-14 21:21:11.000000 lightpath-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-09-14 21:21:35.894442 lightpath-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-09-14 21:21:11.000000 lightpath-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.874442 lightpath-1.0.3/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-14 21:21:11.000000 lightpath-1.0.3/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-14 21:21:11.000000 lightpath-1.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.874442 lightpath-1.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)      901 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.878442 lightpath-1.0.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/controller.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8573 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/path.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.878442 lightpath-1.0.3/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/source/upcoming_release_notes/template-short.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.878442 lightpath-1.0.3/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   101190 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/static/LCLS_beamline_map.png
--rw-r--r--   0 runner    (1001) docker     (127)   268651 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs/static/LCLS_beamline_map.svg
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-14 21:21:11.000000 lightpath-1.0.3/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.882442 lightpath-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-14 21:21:11.000000 lightpath-1.0.3/examples/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.882442 lightpath-1.0.3/lightpath/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       43 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23594 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.886442 lightpath-1.0.3/lightpath/happi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17247 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/mock_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    22616 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.886442 lightpath-1.0.3/lightpath/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/conf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    42695 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/path.json
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/tests/test_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.890442 lightpath-1.0.3/lightpath/ui/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/ui/device.ui
--rw-r--r--   0 runner    (1001) docker     (127)    17352 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/ui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/ui/lightapp.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-09-14 21:21:11.000000 lightpath-1.0.3/lightpath/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 21:21:35.886442 lightpath-1.0.3/lightpath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-14 21:21:35.000000 lightpath-1.0.3/lightpath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-09-14 21:21:11.000000 lightpath-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-09-14 21:21:11.000000 lightpath-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 21:21:35.894442 lightpath-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.885446 lightpath-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 22:28:24.000000 lightpath-1.0.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 22:28:24.000000 lightpath-1.0.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 22:28:24.000000 lightpath-1.0.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 22:28:24.000000 lightpath-1.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.877446 lightpath-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 22:28:24.000000 lightpath-1.0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 22:28:24.000000 lightpath-1.0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.877446 lightpath-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 22:28:24.000000 lightpath-1.0.4/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 22:28:24.000000 lightpath-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 22:28:24.000000 lightpath-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 22:28:24.000000 lightpath-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-12 22:28:24.000000 lightpath-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 22:28:24.000000 lightpath-1.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 22:28:24.000000 lightpath-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-12 22:28:36.885446 lightpath-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 22:28:24.000000 lightpath-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.877446 lightpath-1.0.4/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 22:28:24.000000 lightpath-1.0.4/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 22:28:24.000000 lightpath-1.0.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.877446 lightpath-1.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.877446 lightpath-1.0.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/controller.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/path.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.881446 lightpath-1.0.4/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/source/upcoming_release_notes/template-short.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.881446 lightpath-1.0.4/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   101190 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/static/LCLS_beamline_map.png
+-rw-r--r--   0 runner    (1001) docker     (127)   268651 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs/static/LCLS_beamline_map.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 22:28:24.000000 lightpath-1.0.4/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.881446 lightpath-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-12 22:28:24.000000 lightpath-1.0.4/examples/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.881446 lightpath-1.0.4/lightpath/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.885446 lightpath-1.0.4/lightpath/happi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/mock_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.885446 lightpath-1.0.4/lightpath/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/conf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42695 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/path.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.885446 lightpath-1.0.4/lightpath/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/ui/device.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    17352 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/ui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/ui/lightapp.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-12 22:28:24.000000 lightpath-1.0.4/lightpath/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:28:36.885446 lightpath-1.0.4/lightpath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 22:28:36.000000 lightpath-1.0.4/lightpath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-12 22:28:24.000000 lightpath-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 22:28:24.000000 lightpath-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:28:36.889446 lightpath-1.0.4/setup.cfg
```

### Comparing `lightpath-1.0.3/.flake8` & `lightpath-1.0.4/.flake8`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/.github/ISSUE_TEMPLATE.md` & `lightpath-1.0.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/.github/PULL_REQUEST_TEMPLATE.md` & `lightpath-1.0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/.github/workflows/standard.yml` & `lightpath-1.0.4/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/.gitignore` & `lightpath-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/.pre-commit-config.yaml` & `lightpath-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/CONTRIBUTING.rst` & `lightpath-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/LICENSE.md` & `lightpath-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/PKG-INFO` & `lightpath-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightpath
-Version: 1.0.3
+Version: 1.0.4
 Summary: {{ cookiecutter.description }}
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `lightpath-1.0.3/README.rst` & `lightpath-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/conda-recipe/meta.yaml` & `lightpath-1.0.4/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/Makefile` & `lightpath-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/pre-release-notes.sh` & `lightpath-1.0.4/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/release_notes.py` & `lightpath-1.0.4/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/source/conf.py` & `lightpath-1.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/source/interface.rst` & `lightpath-1.0.4/docs/source/interface.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/source/releases.rst` & `lightpath-1.0.4/docs/source/releases.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 Release History
 ###############
 
 
+v1.0.4 (2024-04-12)
+===================
+
+Maintenance
+-----------
+- Remove hard failure when a lightpath-active device is malformed.  Instead of throwing an
+  exception, simply omit it from the facility graph
+- Trim beam paths before BeamPath objects are created, when device names are gathered into paths
+
+Contributors
+------------
+- tangkong
+
+
+
 v1.0.3 (2023-09-14)
 ===================
 
 Maintenance
 -----------
 - Update build requirements to use pip-provided extras for documentation and test builds.
 - Fix some tests, adding assert statements with timeouts.
```

### Comparing `lightpath-1.0.3/docs/source/tutorial.rst` & `lightpath-1.0.4/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/source/upcoming_release_notes/template-full.rst` & `lightpath-1.0.4/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/static/LCLS_beamline_map.png` & `lightpath-1.0.4/docs/static/LCLS_beamline_map.png`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/docs/static/LCLS_beamline_map.svg` & `lightpath-1.0.4/docs/static/LCLS_beamline_map.svg`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/examples/demo.py` & `lightpath-1.0.4/examples/demo.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/controller.py` & `lightpath-1.0.4/lightpath/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,19 @@
             raise ValueError('No lightpath-active devices found')
         # gather devices by branch
         branch_dict = {}
         for res in results:
             for branch_set in (res.metadata.get('input_branches', []),
                                res.metadata.get('output_branches', [])):
                 if branch_set is None:
-                    raise ValueError(
-                        f'device {res.item.name} has no branch information, '
+                    logger.warning(
+                        f'device ({res.item.name}) missing branch information, '
                         'check to make sure your happi database is '
                         'correctly implementing its container.')
+                    break
                 for branch in branch_set:
                     branch_dict.setdefault(branch, set()).add(res)
 
         # Construct subgraphs and merge
         subgraphs = []
         for branch_name, branch_devs in branch_dict.items():
             subgraph = self.make_graph(
@@ -142,15 +143,15 @@
         Load a beamline given the facility graph.  Finds all possible
         paths from facility sources to the endstation's branch.
         Branches are mapped to endstations in the config.
         Each branch can be optionally mapped to a final z to
         consider part of the path.
 
         Loads valid beampaths into the LightController.beamlines
-        attribute for latedr access.
+        attribute for later access.
 
         Parameters
         ----------
         endstation : str
             Name of endstation to load
         """
         try:
@@ -161,26 +162,54 @@
             return
 
         paths = list()
         for branch in end_branches:
             # Find the paths from each source to the desired line
             for src in self.sources:
                 try:
-                    if nx.has_path(self.graph, src, branch):
-                        found_paths = nx.all_simple_paths(self.graph,
-                                                          source=src,
-                                                          target=branch)
-                        paths.extend(found_paths)
-                    else:
-                        logger.debug(f'No path between {src} and {branch}')
+                    path_exists: bool = nx.has_path(self.graph, src, branch)
                 except NodeNotFound:
                     logger.debug(f'Either source {src} or target {branch} '
                                  'not found.')
+                    path_exists = False
+
+                if path_exists:
+                    found_paths = nx.all_simple_paths(self.graph,
+                                                      source=src,
+                                                      target=branch)
+
+                    # Trim beamline based on z-positions
+                    if isinstance(end_branches, dict):
+                        new_paths = list()
+                        for found_path in found_paths:
+                            end_z = end_branches[branch]
+                            if end_z is not None:
+                                # Only filter internal devices
+                                truncated_path = [
+                                    name for name in found_path[1:-1]
+                                    if self.graph.nodes[name]['md'].res['z'] < end_z
+                                ]
+                                truncated_path.append(found_path[-1])
+                                truncated_path.insert(0, found_path[0])
+                                new_paths.append(truncated_path)
+                            else:
+                                new_paths.append(found_path)
 
-        self.beamlines[endstation] = paths
+                        paths.extend(new_paths)
+                    elif isinstance(end_branches, list):
+                        paths.extend(found_paths)
+                    else:
+                        raise TypeError('config is incorrectly formatted '
+                                        f'(found mapping from {endstation} to '
+                                        f'{type(end_branches)}).')
+
+                else:
+                    logger.debug(f'No path between {src} and {branch}')
+
+                self.beamlines[endstation] = paths
 
     def get_paths(self, endstation: str) -> list[BeamPath]:
         """
         Returns the BeamPaths for a specified endstation.
         Create and fill the BeamPaths if they have not been already
 
         Parameters
@@ -196,44 +225,28 @@
         # if path exists, return it
         paths = self.beamlines[endstation]
 
         if all([isinstance(path, BeamPath) for path in paths]):
             return paths
 
         # create the BeamPaths if they have not been already
-        end_branches = self.beamline_config[endstation]
+        # end_branches = self.beamline_config[endstation]
         filled_paths = []
         for path in paths:
             subgraph = self.graph.subgraph(path)
             devices = [self.get_device(dev_name)
                        for dev_name, data in subgraph.nodes.data()
                        if data['md'].res is not None]
             bp = BeamPath(
                 *devices,
                 name=endstation,
                 minimum_transmission=self.min_trans
             )
 
-            if isinstance(end_branches, dict):
-                # access the last z for this branch
-                # if end_branches is Dict[BranchName, end_z], grab last
-                # allowable z with the branch name (last node in path)
-                last_z = end_branches[path[-1]]
-                if last_z:
-                    # append path with all devices before last z
-                    filled_paths.append(bp.split(last_z)[0])
-                else:
-                    filled_paths.append(bp)
-            elif isinstance(end_branches, list):
-                # end_branches is a simple list, no splitting needed
-                filled_paths.append(bp)
-            else:
-                raise TypeError('config is incorrectly formatted '
-                                f'(found mapping from {endstation} to '
-                                f'{type(end_branches)}).')
+            filled_paths.append(bp)
 
         self.beamlines[endstation] = filled_paths
         return filled_paths
 
     @staticmethod
     def imped_z(path: BeamPath) -> float:
         """
```

### Comparing `lightpath-1.0.3/lightpath/happi/containers.py` & `lightpath-1.0.4/lightpath/happi/containers.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/main.py` & `lightpath-1.0.4/lightpath/main.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/mock_devices.py` & `lightpath-1.0.4/lightpath/mock_devices.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/path.py` & `lightpath-1.0.4/lightpath/path.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/conftest.py` & `lightpath-1.0.4/lightpath/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/path.json` & `lightpath-1.0.4/lightpath/tests/path.json`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/test_cli.py` & `lightpath-1.0.4/lightpath/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/test_controller.py` & `lightpath-1.0.4/lightpath/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/test_gui.py` & `lightpath-1.0.4/lightpath/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/test_path.py` & `lightpath-1.0.4/lightpath/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/tests/test_widgets.py` & `lightpath-1.0.4/lightpath/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/ui/device.ui` & `lightpath-1.0.4/lightpath/ui/device.ui`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/ui/gui.py` & `lightpath-1.0.4/lightpath/ui/gui.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/ui/lightapp.ui` & `lightpath-1.0.4/lightpath/ui/lightapp.ui`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/ui/widgets.py` & `lightpath-1.0.4/lightpath/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath/version.py` & `lightpath-1.0.4/lightpath/version.py`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/lightpath.egg-info/PKG-INFO` & `lightpath-1.0.4/lightpath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightpath
-Version: 1.0.3
+Version: 1.0.4
 Summary: {{ cookiecutter.description }}
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `lightpath-1.0.3/lightpath.egg-info/SOURCES.txt` & `lightpath-1.0.4/lightpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightpath-1.0.3/pyproject.toml` & `lightpath-1.0.4/pyproject.toml`

 * *Files identical despite different names*

