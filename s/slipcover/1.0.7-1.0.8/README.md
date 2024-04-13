# Comparing `tmp/slipcover-1.0.7.tar.gz` & `tmp/slipcover-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-1.0.7.tar", last modified: Fri Apr 12 16:27:24 2024, max compression
+gzip compressed data, was "slipcover-1.0.8.tar", last modified: Sat Apr 13 00:19:34 2024, max compression
```

## Comparing `slipcover-1.0.7.tar` & `slipcover-1.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-12 16:27:24.191671 slipcover-1.0.7/
--rw-r--r--   0 runner     (501) staff       (20)    11358 2024-04-12 16:27:01.000000 slipcover-1.0.7/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-04-12 16:27:01.000000 slipcover-1.0.7/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     9403 2024-04-12 16:27:24.190746 slipcover-1.0.7/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     8234 2024-04-12 16:27:01.000000 slipcover-1.0.7/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-12 16:27:24.191784 slipcover-1.0.7/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     4379 2024-04-12 16:27:01.000000 slipcover-1.0.7/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-12 16:27:24.176975 slipcover-1.0.7/src/
--rw-r--r--   0 runner     (501) staff       (20)     5478 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/probe.cxx
--rw-r--r--   0 runner     (501) staff       (20)      865 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/pyptr.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-12 16:27:24.181012 slipcover-1.0.7/src/slipcover/
--rw-r--r--   0 runner     (501) staff       (20)      168 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9365 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     6472 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/branch.py
--rw-r--r--   0 runner     (501) staff       (20)    21990 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/fuzz.py
--rw-r--r--   0 runner     (501) staff       (20)     9302 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/importer.py
--rw-r--r--   0 runner     (501) staff       (20)     2171 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/isolate.py
--rw-r--r--   0 runner     (501) staff       (20)    25397 2024-04-12 16:27:01.000000 slipcover-1.0.7/src/slipcover/slipcover.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-12 16:27:24.190208 slipcover-1.0.7/src/slipcover.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9403 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      716 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-04-12 16:27:24.000000 slipcover-1.0.7/src/slipcover.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-12 16:27:24.189765 slipcover-1.0.7/tests/
--rw-r--r--   0 runner     (501) staff       (20)    15650 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_branch.py
--rw-r--r--   0 runner     (501) staff       (20)    22245 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_bytecode.py
--rw-r--r--   0 runner     (501) staff       (20)    28457 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_coverage.py
--rw-r--r--   0 runner     (501) staff       (20)     9528 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_importer.py
--rw-r--r--   0 runner     (501) staff       (20)    17508 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_instrumentation.py
--rw-r--r--   0 runner     (501) staff       (20)     5065 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/test_isolate.py
--rw-r--r--   0 runner     (501) staff       (20)     1313 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/testme-class.py
--rw-r--r--   0 runner     (501) staff       (20)     1422 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/testme-inner.py
--rw-r--r--   0 runner     (501) staff       (20)     1279 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/testme-partial.py
--rw-r--r--   0 runner     (501) staff       (20)     1269 2024-04-12 16:27:01.000000 slipcover-1.0.7/tests/testme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 00:19:15.000000 slipcover-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 00:19:15.000000 slipcover-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-13 00:19:34.279439 slipcover-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-13 00:19:15.000000 slipcover-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 00:19:34.283439 slipcover-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-13 00:19:15.000000 slipcover-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.275439 slipcover-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/probe.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/pyptr.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/src/slipcover/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21990 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/slipcover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/src/slipcover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15650 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28457 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme.py
```

### Comparing `slipcover-1.0.7/LICENSE` & `slipcover-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/PKG-INFO` & `slipcover-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.7
+Version: 1.0.8
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.7/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.8/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -58,16 +58,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.7/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.7/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -87,15 +87,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.7/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.8/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.7/README.md` & `slipcover-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/setup.py` & `slipcover-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 def get_version():
     import re
     v = re.findall(r"\nVERSION *= *\"([^\"]+)\"", Path("src/slipcover/slipcover.py").read_text())[0]
     return v
 
+PYTHON_VERSION = sys.version_info[0:2]
 VERSION = get_version()
 REPO_URL = "https://github.com/plasma-umass/slipcover"
 
 def get_description():
 #    from pathlib import Path
     import re
     readme_md = Path("README.md")
@@ -70,15 +71,15 @@
     sources=['src/probe.cxx'],
     extra_compile_args=cxx_version('c++17') + platform_compile_args() + limited_api_args(),
     extra_link_args=platform_link_args(),
     py_limited_api=bool(limited_api_args()),
     language='c++',
 )
 
-if sys.argv[1].startswith('bdist') and sys.platform == 'darwin' and \
+if sys.argv[1].startswith('bdist') and sys.platform == 'darwin' and PYTHON_VERSION < (3,12) and\
    sum(arg == '-arch' for arg in platform_compile_args()) > 1:
     # Build universal wheels on MacOS.
     # ---
     # On MacOS >= 11, all builds are compatible for a major MacOS version, so Python "floors"
     # all minor versions to 0, leading to tags like like "macosx_11_0_universal2". If you use
     # the actual (non-0) minor name in the build platform, pip doesn't install it.
     import platform as p
@@ -95,15 +96,17 @@
     long_description_content_type="text/markdown",
     url="https://github.com/plasma-umass/slipcover",
     author="Juan Altmayer Pizzorno, Emery Berger",
     author_email="juan@altmayer.com, emery@cs.umass.edu",
     license="Apache License 2.0",
     packages=['slipcover'],
     package_dir={'': 'src'},
-    ext_modules=([probe]),
+    ext_modules=([probe] if PYTHON_VERSION < (3,12) else []),
+#    python_requires=f">=3.{PYTHON_VERSION[1]},<3.{PYTHON_VERSION[1]+1}" if PYTHON_VERSION < (3,12) \
+#                    else ">=3.12,<3.14",
     python_requires=">=3.8,<3.14",
     install_requires=[
         "tabulate"
     ],
     entry_points={
         "console_scripts": [
             "slipcover=slipcover.__main__:main",
```

### Comparing `slipcover-1.0.7/src/probe.cxx` & `slipcover-1.0.8/src/probe.cxx`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/pyptr.h` & `slipcover-1.0.8/src/pyptr.h`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/__main__.py` & `slipcover-1.0.8/src/slipcover/__main__.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/branch.py` & `slipcover-1.0.8/src/slipcover/branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/bytecode.py` & `slipcover-1.0.8/src/slipcover/bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/importer.py` & `slipcover-1.0.8/src/slipcover/importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/isolate.py` & `slipcover-1.0.8/src/slipcover/isolate.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/src/slipcover/slipcover.py` & `slipcover-1.0.8/src/slipcover/slipcover.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import dis
 import types
 from typing import Dict, Set, List, Tuple
 from collections import defaultdict, Counter
 import threading
 
 if sys.version_info[0:2] < (3,12):
-    from . import probe
+    try:
+        from . import probe
+    except ImportError:
+        raise RuntimeError("You probably have the wrong package; " + \
+                           "SlipCover for Python <3.12 requires version-specific builds")
     from . import bytecode as bc
 
 from pathlib import Path
 from . import branch as br
 
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 
 # FIXME provide __all__
 
 # Counter.total() is new in 3.10
 if sys.version_info[0:2] < (3,10):
     def counter_total(self: Counter) -> int:
         return sum([self[n] for n in self])
```

### Comparing `slipcover-1.0.7/src/slipcover.egg-info/PKG-INFO` & `slipcover-1.0.8/src/slipcover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.7
+Version: 1.0.8
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.7/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.8/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -58,16 +58,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.7/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.7/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -87,15 +87,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.7/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.8/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.7/src/slipcover.egg-info/SOURCES.txt` & `slipcover-1.0.8/src/slipcover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_branch.py` & `slipcover-1.0.8/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_bytecode.py` & `slipcover-1.0.8/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_coverage.py` & `slipcover-1.0.8/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_importer.py` & `slipcover-1.0.8/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_instrumentation.py` & `slipcover-1.0.8/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/test_isolate.py` & `slipcover-1.0.8/tests/test_isolate.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/testme-class.py` & `slipcover-1.0.8/tests/testme-class.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/testme-inner.py` & `slipcover-1.0.8/tests/testme-inner.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/testme-partial.py` & `slipcover-1.0.8/tests/testme-partial.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.7/tests/testme.py` & `slipcover-1.0.8/tests/testme.py`

 * *Files identical despite different names*

