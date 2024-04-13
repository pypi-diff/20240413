# Comparing `tmp/HiYaPyCo-0.5.4.tar.gz` & `tmp/HiYaPyCo-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiYaPyCo-0.5.4.tar", last modified: Wed Nov 29 11:47:47 2023, max compression
+gzip compressed data, was "HiYaPyCo-0.5.5.tar", last modified: Sat Apr 13 09:12:19 2024, max compression
```

## Comparing `HiYaPyCo-0.5.4.tar` & `HiYaPyCo-0.5.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11152 2023-11-29 11:47:47.000000 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      489 2023-11-29 11:47:47.000000 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/SOURCES.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2023-11-29 11:47:47.000000 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/dependency_links.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2023-11-29 11:47:47.000000 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/requires.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2023-11-29 11:47:47.000000 HiYaPyCo-0.5.4/HiYaPyCo.egg-info/top_level.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/LICENSE
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/MANIFEST.in
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11152 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10361 2023-11-29 11:44:30.000000 HiYaPyCo-0.5.4/README.rst
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/hiyapyco/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    21689 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.4/hiyapyco/__init__.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2023-11-28 09:37:34.000000 HiYaPyCo-0.5.4/hiyapyco/odyldo.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2023-11-29 11:44:02.000000 HiYaPyCo-0.5.4/hiyapyco/version.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/setup.cfg
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2023-11-29 11:43:56.000000 HiYaPyCo-0.5.4/setup.py
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2023-11-29 11:47:47.454091 HiYaPyCo-0.5.4/test/
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_castinterpolated.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_interpolation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_interpolationunicode.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_invocation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.4/test/test_merge.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_missingfiles.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_multiple.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.5.4/test/test_odict.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.4/test/test_simple.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.197439 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11195 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      489 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/SOURCES.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/dependency_links.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/requires.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/top_level.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/LICENSE
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/MANIFEST.in
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11195 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10404 2024-04-13 08:55:30.000000 HiYaPyCo-0.5.5/README.rst
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.197439 HiYaPyCo-0.5.5/hiyapyco/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    21689 2024-04-13 08:37:16.000000 HiYaPyCo-0.5.5/hiyapyco/__init__.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2024-04-13 08:37:32.000000 HiYaPyCo-0.5.5/hiyapyco/odyldo.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2024-04-13 08:39:01.000000 HiYaPyCo-0.5.5/hiyapyco/version.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/setup.cfg
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2024-04-13 08:39:36.000000 HiYaPyCo-0.5.5/setup.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/test/
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_castinterpolated.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_interpolation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_interpolationunicode.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_invocation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.5/test/test_merge.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_missingfiles.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_multiple.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.5.5/test/test_odict.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_simple.py
```

### Comparing `HiYaPyCo-0.5.4/HiYaPyCo.egg-info/PKG-INFO` & `HiYaPyCo-0.5.5/HiYaPyCo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.4
+Version: 0.5.5
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -334,28 +334,33 @@
 
 An `AUR package <https://aur.archlinux.org/packages/python-hiyapyco/>`_
 is available (provided by `Pete Crighton <https://github.com/PeteCrighton>`_ and not always up to date).
 
 License
 -------
 
-Copyright |copy| 2014 - 2023 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
+Copyright |copy| 2014 - 2024 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
 
 .. |copy| unicode:: 0xA9 .. copyright sign
 
 This package is free software.
 This software is licensed under the terms of the GNU GENERAL PUBLIC
 LICENSE version 3 or later, as published by the Free Software
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
+0.5.5
+~~~~~~
+
+FIXED: #67 cosmetic changes
+
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
 
 IMPROVED: testing and python support (3.11)
```

### Comparing `HiYaPyCo-0.5.4/LICENSE` & `HiYaPyCo-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/PKG-INFO` & `HiYaPyCo-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.4
+Version: 0.5.5
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -334,28 +334,33 @@
 
 An `AUR package <https://aur.archlinux.org/packages/python-hiyapyco/>`_
 is available (provided by `Pete Crighton <https://github.com/PeteCrighton>`_ and not always up to date).
 
 License
 -------
 
-Copyright |copy| 2014 - 2023 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
+Copyright |copy| 2014 - 2024 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
 
 .. |copy| unicode:: 0xA9 .. copyright sign
 
 This package is free software.
 This software is licensed under the terms of the GNU GENERAL PUBLIC
 LICENSE version 3 or later, as published by the Free Software
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
+0.5.5
+~~~~~~
+
+FIXED: #67 cosmetic changes
+
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
 
 IMPROVED: testing and python support (3.11)
```

### Comparing `HiYaPyCo-0.5.4/README.rst` & `HiYaPyCo-0.5.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -313,28 +313,33 @@
 
 An `AUR package <https://aur.archlinux.org/packages/python-hiyapyco/>`_
 is available (provided by `Pete Crighton <https://github.com/PeteCrighton>`_ and not always up to date).
 
 License
 -------
 
-Copyright |copy| 2014 - 2023 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
+Copyright |copy| 2014 - 2024 Klaus Zerwes `zero-sys.net <https://zero-sys.net>`_
 
 .. |copy| unicode:: 0xA9 .. copyright sign
 
 This package is free software.
 This software is licensed under the terms of the GNU GENERAL PUBLIC
 LICENSE version 3 or later, as published by the Free Software
 Foundation.
 See
 `https://www.gnu.org/licenses/gpl.html <https://www.gnu.org/licenses/gpl.html>`_
 
 Changelog
 ---------
 
+0.5.5
+~~~~~~
+
+FIXED: #67 cosmetic changes
+
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
 
 IMPROVED: testing and python support (3.11)
```

### Comparing `HiYaPyCo-0.5.4/hiyapyco/__init__.py` & `HiYaPyCo-0.5.5/hiyapyco/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ===============================
 
 A simple python lib allowing hierarchical config files in YAML syntax.
 
 License
 -------
 
-(c) 2014 - 2023 Klaus Zerwes zero-sys.net
+(c) 2014 - 2024 Klaus Zerwes zero-sys.net
 This package is free software.
 This software is licensed under the terms of the
 GNU GENERAL PUBLIC LICENSE version 3 or later,
 as published by the Free Software Foundation.
 See https://www.gnu.org/licenses/gpl.html
 """
```

### Comparing `HiYaPyCo-0.5.4/hiyapyco/odyldo.py` & `HiYaPyCo-0.5.5/hiyapyco/odyldo.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 ODYLDo - Ordered Dict Yaml Loader / Dumper
 ------------------------------------------
 
 a simple implementation of a Ordered Dict Loader for PyYAML;
 because chaos is fun but order matters on loading dicts from a yaml file;
 
-(c) 2014 - 2023 Klaus Zerwes zero-sys.net
+(c) 2014 - 2024 Klaus Zerwes zero-sys.net
 This package is free software.
 This software is licensed under the terms of the
 GNU GENERAL PUBLIC LICENSE version 3 or later,
 as published by the Free Software Foundation.
 See https://www.gnu.org/licenses/gpl.html
 """
```

### Comparing `HiYaPyCo-0.5.4/setup.py` & `HiYaPyCo-0.5.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from setuptools import setup
 
 basepath = os.path.dirname(os.path.realpath(__file__))
 sys.path.insert(0, os.path.dirname(basepath))
 
-HIYAPYCOVERSION='0.5.4'
+HIYAPYCOVERSION='0.5.5'
 
 long_description = open('README.rst').read()
 
 installrequires = [
     'PyYAML<7',
     'Jinja2>3,<4',
     'MarkupSafe<3'
```

### Comparing `HiYaPyCo-0.5.4/test/test_castinterpolated.py` & `HiYaPyCo-0.5.5/test/test_castinterpolated.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_interpolation.py` & `HiYaPyCo-0.5.5/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_interpolationunicode.py` & `HiYaPyCo-0.5.5/test/test_interpolationunicode.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_invocation.py` & `HiYaPyCo-0.5.5/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_merge.py` & `HiYaPyCo-0.5.5/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_missingfiles.py` & `HiYaPyCo-0.5.5/test/test_missingfiles.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_multiple.py` & `HiYaPyCo-0.5.5/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_odict.py` & `HiYaPyCo-0.5.5/test/test_odict.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.4/test/test_simple.py` & `HiYaPyCo-0.5.5/test/test_simple.py`

 * *Files identical despite different names*

