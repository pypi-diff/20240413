# Comparing `tmp/pyprjbtstrptst-0.1.4-py3-none-any.whl.zip` & `tmp/pyprjbtstrptst-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9288 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3513 b- defN 24-Apr-12 23:17 BuildBinary.py
--rw-r--r--  2.0 unx     2552 b- defN 24-Apr-12 23:17 PythonProjectBootstrapperTesting/EntryPoint.py
--rw-r--r--  2.0 unx      947 b- defN 24-Apr-12 23:17 PythonProjectBootstrapperTesting/Math.py
--rw-r--r--  2.0 unx      612 b- defN 24-Apr-12 23:17 PythonProjectBootstrapperTesting/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 24-Apr-12 23:17 pyprjbtstrptst/EntryPoint.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-12 23:17 pyprjbtstrptst/Math.py
--rw-r--r--  2.0 unx      598 b- defN 24-Apr-12 23:18 pyprjbtstrptst/__init__.py
--rw-r--r--  2.0 unx     1091 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6179 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       60 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1142 b- defN 24-Apr-12 23:18 pyprjbtstrptst-0.1.4.dist-info/RECORD
-13 files, 20220 bytes uncompressed, 7348 bytes compressed:  63.7%
+Zip file size: 9090 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3513 b- defN 24-Apr-13 01:58 BuildBinary.py
+-rw-r--r--  2.0 unx     2552 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/EntryPoint.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/Math.py
+-rw-r--r--  2.0 unx      612 b- defN 24-Apr-13 01:58 PythonProjectBootstrapperTesting/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 24-Apr-13 01:58 pyprjbtstrptst/EntryPoint.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-13 01:58 pyprjbtstrptst/Math.py
+-rw-r--r--  2.0 unx      598 b- defN 24-Apr-13 01:58 pyprjbtstrptst/__init__.py
+-rw-r--r--  2.0 unx     1091 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5770 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       60 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1142 b- defN 24-Apr-13 01:58 pyprjbtstrptst-0.1.7.dist-info/RECORD
+13 files, 19699 bytes uncompressed, 7150 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pyprjbtstrptst/Math.py
 Comment: 
 
 Filename: pyprjbtstrptst/__init__.py
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/LICENSE.txt
+Filename: pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/METADATA
+Filename: pyprjbtstrptst-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/WHEEL
+Filename: pyprjbtstrptst-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/entry_points.txt
+Filename: pyprjbtstrptst-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/top_level.txt
+Filename: pyprjbtstrptst-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyprjbtstrptst-0.1.4.dist-info/RECORD
+Filename: pyprjbtstrptst-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## BuildBinary.py

```diff
@@ -1,10 +1,10 @@
 # ----------------------------------------------------------------------
 # |
-# |  Copyright (c) 2024 varun narayan
+# |  Copyright (c) 2024 Varun Narayan
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """Builds the binary for this project."""
 
 import datetime
 import importlib
@@ -47,15 +47,15 @@
     elif current_year // 100 != initial_year // 100:
         year_suffix = str(current_year)
     else:
         year_suffix = "-{}".format(current_year % 100)
 
     return textwrap.dedent(
         f"""\
-        Copyright (c) {initial_year}{year_suffix} varun narayan
+        Copyright (c) {initial_year}{year_suffix} Varun Narayan
 
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

## PythonProjectBootstrapperTesting/Math.py

```diff
@@ -21,12 +21,7 @@
 def Mult(x, y):
     return x * y
 
 
 # ----------------------------------------------------------------------
 def Div(x, y):
     return x / y
-
-
-# ----------------------------------------------------------------------
-def Mod(x, y):
-    return x % y
```

## pyprjbtstrptst/EntryPoint.py

```diff
@@ -1,10 +1,10 @@
 # ----------------------------------------------------------------------
 # |
-# |  Copyright (c) 2024 varun narayan
+# |  Copyright (c) 2024 Varun Narayan
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """This file serves as an example of how to create scripts that can be invoked from the command line once the package is installed."""
 
 import sys
```

## pyprjbtstrptst/Math.py

```diff
@@ -1,10 +1,10 @@
 # ----------------------------------------------------------------------
 # |
-# |  Copyright (c) 2024 varun narayan
+# |  Copyright (c) 2024 Varun Narayan
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 """Basic math functions. This file illustrates how to create a python package that contains functions that can be invoked by other python code."""
 
 
 # ----------------------------------------------------------------------
```

## pyprjbtstrptst/__init__.py

```diff
@@ -1,14 +1,14 @@
 # ----------------------------------------------------------------------
 # |
-# |  Copyright (c) 2024 varun narayan
+# |  Copyright (c) 2024 Varun Narayan
 # |  Distributed under the MIT License.
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.4"
+__version__ = "0.1.7"
 
 from .Math import Add, Sub, Mult, Div
```

## Comparing `pyprjbtstrptst-0.1.4.dist-info/LICENSE.txt` & `pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT LICENSE
 
-Copyright (c) 2024 varun narayan
+Copyright (c) 2024 Varun Narayan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `pyprjbtstrptst-0.1.4.dist-info/METADATA` & `pyprjbtstrptst-0.1.7.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyprjbtstrptst
-Version: 0.1.4
-Summary: python proj test bootstrap
-Author-email: varun narayan <varun646@gmail.com>
+Version: 0.1.7
+Summary: python proj btstrp test
+Author-email: Varun Narayan <varun646@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Documentation, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Repository, https://github.com/varun646/PythonProjectBootstrapperTest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,23 +24,23 @@
 Requires-Dist: build ==1.* ; extra == 'package'
 Requires-Dist: cx-Freeze ==6.* ; extra == 'package'
 Requires-Dist: twine ==4.* ; extra == 'package'
 
 # PythonProjectBootstrapperTest
 
 [![CI](https://github.com/varun646/PythonProjectBootstrapperTest/actions/workflows/standard.yaml/badge.svg?event=push)](https://github.com/varun646/PythonProjectBootstrapperTest/actions/workflows/standard.yaml)
-[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/davidbrownell/2f9d770d13e3a148424f374f74d41f4b/raw/PythonProjectBootstrapperTest_coverage.json)](https://github.com/varun646/PythonProjectBootstrapperTest/actions)
+[![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/varun646/7d3823a2d39ed7fedc159d1391c5f11f/raw/PythonProjectBootstrapperTest_coverage.json)](https://github.com/varun646/PythonProjectBootstrapperTest/actions)
 [![License](https://img.shields.io/github/license/varun646/PythonProjectBootstrapperTest?color=dark-green)](https://github.com/varun646/PythonProjectBootstrapperTest/blob/master/LICENSE.txt)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/varun646/PythonProjectBootstrapperTest?color=dark-green)](https://github.com/varun646/PythonProjectBootstrapperTest/commits/main/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyprjbtstrptst?color=dark-green)](https://pypi.org/project/pyprjbtstrptst/)
 [![PyPI - Version](https://img.shields.io/pypi/v/pyprjbtstrptst?color=dark-green)](https://pypi.org/project/pyprjbtstrptst/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyprjbtstrptst)](https://pypistats.org/packages/pyprjbtstrptst)
 
 # PythonProjectBootstrapperTest
-python proj test bootstrap
+python proj btstrp test
 
 ### Overview
 
 TODO: Complete this section
 
 ### How to use PythonProjectBootstrapperTest
 
@@ -80,16 +80,14 @@
     | `black` | Validates that the source code is formatted by [black](https://github.com/psf/black). | <p>Validation:<br/>`python Build.py black`</p><p>Perform formatting:<br/>`python Build.py black --format`</p> | |
     | `pylint` | Validates the source code using [pylint](https://github.com/pylint-dev/pylint). | `python Build.py pylint` | |
     | `pytest` | Runs automated tests using [pytest](https://docs.pytest.org/). | <p>Without Code Coverage:<br/>`python Build.py pytest`</p><p>With Code Coverage:<br/>`python Build.py pytest --code-coverage`</p> | |
     | `update_version` | Updates the [semantic version](https://semver.org/) of the package based on git commits using [AutoGitSemVer](https://github.com/davidbrownell/AutoGitSemVer). | `python Build.py update_version` | |
     | `package` | Creates a Python wheel package for distribution; outputs to the `/dist` directory. | `python Build.py package` | Requires `--package` when bootstrapping in step #2. |
     | `publish` | Publishes a Python wheel package to [PyPi](https://pypi.org/). | <p>https://test.pypi.org:<br/>`python Build.py publish`</p><p>https://pypi.org:<br/>`python Build.py publish --production`</p> | Requires `--package` when bootstrapping in step #2. |
     | `build_binary` | Builds an executable for your package that can be run on machines without a python installation; outputs to the `/build` directory. | `python Build.py build_binary` | Requires `--package` when bootstrapping in step #2. |
-    | `create_docker_image` | Creates a [Docker](https://www.docker.com/) image based on the current development environment. This supports the "Reusable" aspect of [FAIR principles](https://www.go-fair.org/fair-principles/) by creating a snapshot of the repository and all of its dependencies as they exist in a single moment in time. | `python Build.py create_docker_image` | Requires docker. |
-
 
 5) [Optional] Deactivate the development environment by running...
     | Operating System | Command |
     | --- | --- |
     | Linux / MacOS | `. ./Deactivate.sh` |
     | Windows | `Deactivate.cmd` |
```

## Comparing `pyprjbtstrptst-0.1.4.dist-info/RECORD` & `pyprjbtstrptst-0.1.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-BuildBinary.py,sha256=j15PSyA81YSLJ8ZziP4NqZk-69fqXRuEJ6QerV-Cs48,3513
+BuildBinary.py,sha256=-3ujy6q5GVo6IxSpa4-r8j_6NetO2dvpMi_7bhMBw9U,3513
 PythonProjectBootstrapperTesting/EntryPoint.py,sha256=3Xi6ot1lveR6dzDTSOtfs-N9zqOOM1c75JIRVTrTdvA,2552
-PythonProjectBootstrapperTesting/Math.py,sha256=XZnF-rHcwrp9fwb63pRAVNvpu2XswUexp-ubChWXERU,947
+PythonProjectBootstrapperTesting/Math.py,sha256=Tevmtoshj7XhYUy2Oadws2RIRJMyHMXpEcGtb5I-7OY,835
 PythonProjectBootstrapperTesting/__init__.py,sha256=42TfbLDT-LM5pLO_p7Etv-xmPRH9pjJuaemgso3cMPg,612
-pyprjbtstrptst/EntryPoint.py,sha256=QDkGQG_LjbrpSZPeEMrnXbZH3ZwzKv-2aI1yDo2G-r0,2534
-pyprjbtstrptst/Math.py,sha256=wVHMx-yYuLo9F4iQdwpmML3KN9rpuBjxdGhTYVef13Q,835
-pyprjbtstrptst/__init__.py,sha256=EZi2E7o_Nodxx8ZXFSrAZxC9ZnS_da3nDoNfxxCW4Is,598
-pyprjbtstrptst-0.1.4.dist-info/LICENSE.txt,sha256=ck47cFE0d6sqDBoVjVwmjNZnp_nqmwwMfWAePJ4wuJA,1091
-pyprjbtstrptst-0.1.4.dist-info/METADATA,sha256=7SkJ-oKAVJwnoPt6uLACW4th0YUlZhEfTKjfpHFPSNU,6179
-pyprjbtstrptst-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyprjbtstrptst-0.1.4.dist-info/entry_points.txt,sha256=OJJ4E_AkMaIJS_L9JY-OkG7dNAMUK2vtGEOAgvJWzdE,65
-pyprjbtstrptst-0.1.4.dist-info/top_level.txt,sha256=ugqgXJWGUckZyN2Pm-7sF6RRSnPhorM11ChCP5Yfgcc,60
-pyprjbtstrptst-0.1.4.dist-info/RECORD,,
+pyprjbtstrptst/EntryPoint.py,sha256=GuH9nKqDq5s1MKXgCqZcfkCugnmEZLJURHl2m0-4LBk,2534
+pyprjbtstrptst/Math.py,sha256=Tevmtoshj7XhYUy2Oadws2RIRJMyHMXpEcGtb5I-7OY,835
+pyprjbtstrptst/__init__.py,sha256=mXbzYLxtLWr7sJLXDpNqADrGt21vUnashf8EGNMBU3o,598
+pyprjbtstrptst-0.1.7.dist-info/LICENSE.txt,sha256=zCmegIpsbaajGyBHbV96bjKLKbeSPT9F9LyUbiZZ3-s,1091
+pyprjbtstrptst-0.1.7.dist-info/METADATA,sha256=5Im7v--qovKVDdsF_A7nd4Kb0J7-1Tj40L7FfTpfE1E,5770
+pyprjbtstrptst-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyprjbtstrptst-0.1.7.dist-info/entry_points.txt,sha256=OJJ4E_AkMaIJS_L9JY-OkG7dNAMUK2vtGEOAgvJWzdE,65
+pyprjbtstrptst-0.1.7.dist-info/top_level.txt,sha256=ugqgXJWGUckZyN2Pm-7sF6RRSnPhorM11ChCP5Yfgcc,60
+pyprjbtstrptst-0.1.7.dist-info/RECORD,,
```

