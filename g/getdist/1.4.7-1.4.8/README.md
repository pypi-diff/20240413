# Comparing `tmp/getdist-1.4.7.tar.gz` & `tmp/getdist-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getdist-1.4.7.tar", last modified: Fri Jan 19 09:28:39 2024, max compression
+gzip compressed data, was "getdist-1.4.8.tar", last modified: Sat Apr 13 08:26:47 2024, max compression
```

## Comparing `getdist-1.4.7.tar` & `getdist-1.4.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.700870 getdist-1.4.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2024-01-19 09:26:04.000000 getdist-1.4.7/GetDistGUI.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68114 2024-01-19 09:26:04.000000 getdist-1.4.7/LICENCE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2024-01-19 09:26:04.000000 getdist-1.4.7/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-01-19 09:28:39.700870 getdist-1.4.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10649 2024-01-19 09:26:04.000000 getdist-1.4.7/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.672868 getdist-1.4.7/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.676868 getdist-1.4.7/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9201 2024-01-19 09:26:05.000000 getdist-1.4.7/docs/source/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.684869 getdist-1.4.7/getdist/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1947 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/analysis_defaults.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/chain_grid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63744 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/chains.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11204 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/cobaya_interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12863 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/command_line.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9222 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/convolve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/covcomb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3901 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/covmat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      778 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/covscale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12283 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/densities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/distparam_template.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    22044 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gaussian_mixtures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.688869 getdist-1.4.7/getdist/gui/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/SyntaxHighlight.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.692870 getdist-1.4.7/getdist/gui/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16164 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/Icon.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/delete.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/delete_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/open.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      809 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/open_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/remove.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/remove_large.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      373 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/save.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/images/save_large.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.672868 getdist-1.4.7/getdist/gui/mac_app/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.692870 getdist-1.4.7/getdist/gui/mac_app/Contents/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1263 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/mac_app/Contents/Info.plist
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.692870 getdist-1.4.7/getdist/gui/mac_app/Contents/MacOS/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      122 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/mac_app/Contents/MacOS/GetDistGUI
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.692870 getdist-1.4.7/getdist/gui/mac_app/Contents/Resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)   559497 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns
--rw-rw-r--   0 travis    (2000) travis    (2000)    96734 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/gui/mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13684 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/inifile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11881 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/kde_bandwidth.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16654 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/matplotlib_ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118646 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/mcsamples.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16211 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/paramnames.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/parampriors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   170183 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/plots.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.696870 getdist-1.4.7/getdist/styles/
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/styles/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5921 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/styles/planck.paramnames
--rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/styles/planck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16929 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/styles/sfmath.sty
--rw-rw-r--   0 travis    (2000) travis    (2000)      517 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/styles/tab10.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.696870 getdist-1.4.7/getdist/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19711 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/tests/getdist_test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16705 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/tests/test_distributions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37192 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2024-01-19 09:26:05.000000 getdist-1.4.7/getdist/yaml_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-01-19 09:28:39.696870 getdist-1.4.7/getdist.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2024-01-19 09:28:39.000000 getdist-1.4.7/getdist.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2024-01-19 09:26:05.000000 getdist-1.4.7/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-01-19 09:28:39.700870 getdist-1.4.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2024-01-19 09:26:05.000000 getdist-1.4.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.395977 getdist-1.4.8/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2024-04-13 08:24:04.000000 getdist-1.4.8/GetDistGUI.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68114 2024-04-13 08:24:04.000000 getdist-1.4.8/LICENCE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2024-04-13 08:24:04.000000 getdist-1.4.8/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-04-13 08:26:47.395977 getdist-1.4.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10649 2024-04-13 08:24:04.000000 getdist-1.4.8/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.375976 getdist-1.4.8/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.379976 getdist-1.4.8/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9201 2024-04-13 08:24:04.000000 getdist-1.4.8/docs/source/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.383976 getdist-1.4.8/getdist/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1947 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3266 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/analysis_defaults.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5938 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/chain_grid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63744 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/chains.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11212 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/cobaya_interface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12863 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/command_line.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9222 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/convolve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covcomb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3901 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covmat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      778 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/covscale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12283 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/densities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2086 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/distparam_template.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22044 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gaussian_mixtures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6626 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/SyntaxHighlight.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/images/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16164 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/Icon.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      337 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/delete.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/delete_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/open.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      809 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/open_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/remove.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/remove_large.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      373 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/save.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      423 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/images/save_large.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.375976 getdist-1.4.8/getdist/gui/mac_app/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1263 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/Info.plist
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/MacOS/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      122 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/MacOS/GetDistGUI
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.387977 getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   559497 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96734 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/gui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13684 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/inifile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11881 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/kde_bandwidth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16654 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/matplotlib_ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118646 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/mcsamples.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16211 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/paramnames.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4158 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/parampriors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   170183 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/plots.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist/styles/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5921 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/planck.paramnames
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2450 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/planck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16929 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/sfmath.sty
+-rw-rw-r--   0 travis    (2000) travis    (2000)      517 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/styles/tab10.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19711 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/getdist_test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16705 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/tests/test_distributions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37192 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2024-04-13 08:24:04.000000 getdist-1.4.8/getdist/yaml_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-13 08:26:47.391977 getdist-1.4.8/getdist.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)    91153 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1552 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2024-04-13 08:26:47.000000 getdist-1.4.8/getdist.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2024-04-13 08:24:04.000000 getdist-1.4.8/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-13 08:26:47.395977 getdist-1.4.8/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3100 2024-04-13 08:24:04.000000 getdist-1.4.8/setup.py
```

### Comparing `getdist-1.4.7/LICENCE.txt` & `getdist-1.4.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/PKG-INFO` & `getdist-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getdist
-Version: 1.4.7
+Version: 1.4.8
 Summary: GetDist Monte Carlo sample analysis, plotting and GUI
 Author: Antony Lewis
 License: GetDist, Copyright (c) 2019, Antony Lewis
         
         Code to find optimal bandwidths for basic kernel density estimators in 1 and 2D
         was adapted from Matlab code by Zdravko Botev. Original code notice:
```

### Comparing `getdist-1.4.7/README.rst` & `getdist-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/docs/source/conf.py` & `getdist-1.4.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/__init__.py` & `getdist-1.4.8/getdist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'Antony Lewis'
-__version__ = "1.4.7"
+__version__ = "1.4.8"
 __url__ = "https://getdist.readthedocs.io"
 
 import os
 import sys
 from getdist.inifile import IniFile
 from getdist.paramnames import ParamInfo, ParamNames
 from getdist.chains import WeightedSamples
```

### Comparing `getdist-1.4.7/getdist/_base.py` & `getdist-1.4.8/getdist/_base.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/analysis_defaults.ini` & `getdist-1.4.8/getdist/analysis_defaults.ini`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/chain_grid.py` & `getdist-1.4.8/getdist/chain_grid.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/chains.py` & `getdist-1.4.8/getdist/chains.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/cobaya_interface.py` & `getdist-1.4.8/getdist/cobaya_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 def get_sampler_temperature(filename_or_info):
     info = yaml_file_or_dict(filename_or_info)
     if _sampler not in info:
         return None
     # post-processed chains have always already been cooled
     if _post in info:
         return 1
-    return info[_sampler][get_sampler_key(info)].get("temperature")
+    return (info[_sampler][get_sampler_key(info)] or {}).get("temperature")
 
 
 def get_sample_label(filename_or_info):
     return yaml_file_or_dict(filename_or_info).get(_label)
 
 
 def get_burn_removed(filename_or_info):
```

### Comparing `getdist-1.4.7/getdist/command_line.py` & `getdist-1.4.8/getdist/command_line.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/convolve.py` & `getdist-1.4.8/getdist/convolve.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/covmat.py` & `getdist-1.4.8/getdist/covmat.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/covscale.py` & `getdist-1.4.8/getdist/covscale.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/densities.py` & `getdist-1.4.8/getdist/densities.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/distparam_template.ini` & `getdist-1.4.8/getdist/distparam_template.ini`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gaussian_mixtures.py` & `getdist-1.4.8/getdist/gaussian_mixtures.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/SyntaxHighlight.py` & `getdist-1.4.8/getdist/gui/SyntaxHighlight.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/images/Icon.png` & `getdist-1.4.8/getdist/gui/images/Icon.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/images/delete_large.png` & `getdist-1.4.8/getdist/gui/images/delete_large.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/images/open_large.png` & `getdist-1.4.8/getdist/gui/images/open_large.png`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/mac_app/Contents/Info.plist` & `getdist-1.4.8/getdist/gui/mac_app/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns` & `getdist-1.4.8/getdist/gui/mac_app/Contents/Resources/GetDistGUI.icns`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/gui/mainwindow.py` & `getdist-1.4.8/getdist/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/inifile.py` & `getdist-1.4.8/getdist/inifile.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/kde_bandwidth.py` & `getdist-1.4.8/getdist/kde_bandwidth.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/matplotlib_ext.py` & `getdist-1.4.8/getdist/matplotlib_ext.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/mcsamples.py` & `getdist-1.4.8/getdist/mcsamples.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/paramnames.py` & `getdist-1.4.8/getdist/paramnames.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/parampriors.py` & `getdist-1.4.8/getdist/parampriors.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/plots.py` & `getdist-1.4.8/getdist/plots.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/styles/planck.paramnames` & `getdist-1.4.8/getdist/styles/planck.paramnames`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/styles/planck.py` & `getdist-1.4.8/getdist/styles/planck.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/styles/sfmath.sty` & `getdist-1.4.8/getdist/styles/sfmath.sty`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/styles/tab10.py` & `getdist-1.4.8/getdist/styles/tab10.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/tests/getdist_test.py` & `getdist-1.4.8/getdist/tests/getdist_test.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/tests/test_distributions.py` & `getdist-1.4.8/getdist/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/types.py` & `getdist-1.4.8/getdist/types.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist/yaml_tools.py` & `getdist-1.4.8/getdist/yaml_tools.py`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/getdist.egg-info/PKG-INFO` & `getdist-1.4.8/getdist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getdist
-Version: 1.4.7
+Version: 1.4.8
 Summary: GetDist Monte Carlo sample analysis, plotting and GUI
 Author: Antony Lewis
 License: GetDist, Copyright (c) 2019, Antony Lewis
         
         Code to find optimal bandwidths for basic kernel density estimators in 1 and 2D
         was adapted from Matlab code by Zdravko Botev. Original code notice:
```

### Comparing `getdist-1.4.7/getdist.egg-info/SOURCES.txt` & `getdist-1.4.8/getdist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/pyproject.toml` & `getdist-1.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdist-1.4.7/setup.py` & `getdist-1.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,13 +85,14 @@
 
     cmd_class = {
         'develop': DevelopCommand,
         'install': InstallCommand,
         'build_py': BuildCommand
     }
 
-setup(zip_safe=False,
+setup(name="getdist",
+      zip_safe=False,
       platforms="any",
       package_data=package_data,
       packages=["getdist", "getdist.gui", "getdist.tests", "getdist.styles"],
       test_suite="getdist.tests",
       cmdclass=cmd_class)
```

