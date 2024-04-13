# Comparing `tmp/deshima-sensitivity-0.4.1.tar.gz` & `tmp/deshima_sensitivity-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deshima-sensitivity-0.4.1.tar", max compression
+gzip compressed data, was "deshima_sensitivity-0.4.2.tar", max compression
```

## Comparing `deshima-sensitivity-0.4.1.tar` & `deshima_sensitivity-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1083 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/LICENSE
--rw-r--r--   0        0        0     2958 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/README.md
--rw-r--r--   0        0        0      671 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/deshima_sensitivity/__init__.py
--rw-r--r--   0        0        0     3604 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/deshima_sensitivity/atmosphere.py
--rw-r--r--   0        0        0   632957 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/deshima_sensitivity/data/atm.csv
--rw-r--r--   0        0        0    42575 2022-06-14 16:31:25.795225 deshima-sensitivity-0.4.1/deshima_sensitivity/data/z_Dl.csv
--rw-r--r--   0        0        0     9879 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/filter.py
--rw-r--r--   0        0        0     3245 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/galaxy.py
--rw-r--r--   0        0        0     4511 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/instruments.py
--rw-r--r--   0        0        0     2582 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/physics.py
--rw-r--r--   0        0        0     7157 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/plotting.py
--rw-r--r--   0        0        0    25713 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/deshima_sensitivity/simulator.py
--rw-r--r--   0        0        0     1418 2022-06-14 16:31:25.799225 deshima-sensitivity-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4243 2022-06-14 16:31:32.481086 deshima-sensitivity-0.4.1/setup.py
--rw-r--r--   0        0        0     4200 2022-06-14 16:31:32.481491 deshima-sensitivity-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2958 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/README.md
+-rw-r--r--   0        0        0      671 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/atmosphere.py
+-rw-r--r--   0        0        0   632957 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/data/atm.csv
+-rw-r--r--   0        0        0    42575 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/data/z_Dl.csv
+-rw-r--r--   0        0        0     9879 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/filter.py
+-rw-r--r--   0        0        0     3245 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/galaxy.py
+-rw-r--r--   0        0        0     4511 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/instruments.py
+-rw-r--r--   0        0        0     2582 2024-04-13 18:50:30.579912 deshima_sensitivity-0.4.2/deshima_sensitivity/physics.py
+-rw-r--r--   0        0        0     7157 2024-04-13 18:50:30.583912 deshima_sensitivity-0.4.2/deshima_sensitivity/plotting.py
+-rw-r--r--   0        0        0    25713 2024-04-13 18:50:30.583912 deshima_sensitivity-0.4.2/deshima_sensitivity/simulator.py
+-rw-r--r--   0        0        0     1468 2024-04-13 18:50:30.583912 deshima_sensitivity-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4251 1970-01-01 00:00:00.000000 deshima_sensitivity-0.4.2/PKG-INFO
```

### Comparing `deshima-sensitivity-0.4.1/LICENSE` & `deshima_sensitivity-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/README.md` & `deshima_sensitivity-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Currently it is mainly used to estimate the observation sensitivity of [DESHIMA](http://deshima.ewi.tudelft.nl) and its successors.
 
 An online Jupyter notebook is available for DESHIMA collaborators to calculate the sensitivity and the mapping speed of the DESHIMA 2.0 by themselves.
 Click the budge below to open it in [Google colaboratory](http://colab.research.google.com/) (a Google account is necessary to re-run it).
 
 ### Stable version (recommended)
 
-[![open stable version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/v0.4.1/sensitivity.ipynb)
+[![open stable version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/v0.4.2/sensitivity.ipynb)
 
 ### Latest version
 
 [![open latest version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/main/sensitivity.ipynb)
 
 In the case of running it in a local Python environment, please follow the requirements and the installation guide below.
```

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/__init__.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 A.  It is included in the main beam efficiency.
     These losses reduce the coupling to a point source,
     but the power (in transmission) couples to the sky.
 
 """
 # flake8: noqa
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 # modules
 from . import atmosphere
 from . import galaxy
 from . import instruments
 from . import physics
```

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/atmosphere.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/atmosphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,11 +115,11 @@
                                      delim_whitespace=True,header=0)
 
         Make function from pandas file::
 
             etafun = desim.eta_atm_interp(eta_atm_df)
 
     """
-    x = np.array(list(eta_atm_dataframe)[1:]).astype(np.float)
+    x = np.array(list(eta_atm_dataframe)[1:]).astype(np.float64)
     y = eta_atm_dataframe["F"].values
     z = eta_atm_dataframe.iloc[:, 1:].values
     return interp2d(x, y, z, kind="cubic")
```

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/data/atm.csv` & `deshima_sensitivity-0.4.2/deshima_sensitivity/data/atm.csv`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/data/z_Dl.csv` & `deshima_sensitivity-0.4.2/deshima_sensitivity/data/z_Dl.csv`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/filter.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/filter.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/galaxy.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/galaxy.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/instruments.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/instruments.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/physics.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/physics.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/plotting.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/plotting.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/deshima_sensitivity/simulator.py` & `deshima_sensitivity-0.4.2/deshima_sensitivity/simulator.py`

 * *Files identical despite different names*

### Comparing `deshima-sensitivity-0.4.1/pyproject.toml` & `deshima_sensitivity-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deshima-sensitivity"
-version = "0.4.1"
+version = "0.4.2"
 description = "Sensitivity calculator for DESHIMA-type spectrometers"
 authors = ["Akira Endo <a.endo@tudelft.nl>"]
 maintainers = [
     "Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>",
     "Yohei Togami <y.togami@a.phys.nagoya-u.ac.jp>",
     "Keiichi Matsuda <matsuda@a.phys.nagoya-u.ac.jp>",
     "Masato Hagimoto <hagimoto@a.phys.nagoya-u.ac.jp>",
@@ -25,23 +25,25 @@
     { version = ">=1.20, <1.22", python = ">=3.7.1, <3.8" },
     { version = "^1.20", python = ">=3.8, <3.11" },
 ]
 pandas = [
     { version = ">=1.3, <1.4", python = ">=3.7.1, <3.8" },
     { version = "^1.3", python = ">=3.8, <3.11" },
 ]
+pandas-dataclasses = "^0.2"
 scipy = "^1.4"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3"
 ipython = [
     { version = "^7.34", python = ">=3.7.1, <3.8" },
     { version = "^8.4", python = ">=3.8, <3.11" },
 ]
 myst-parser = "^0.18"
+pandas-stubs = "^1.2"
 pydata-sphinx-theme = "^0.9"
 pytest = "^7.1"
 sphinx = "^5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `deshima-sensitivity-0.4.1/setup.py` & `deshima_sensitivity-0.4.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: deshima-sensitivity
+Version: 0.4.2
+Summary: Sensitivity calculator for DESHIMA-type spectrometers
+Home-page: https://github.com/deshima-dev/deshima-sensitivity
+License: MIT
+Author: Akira Endo
+Author-email: a.endo@tudelft.nl
+Maintainer: Akio Taniguchi
+Maintainer-email: taniguchi@a.phys.nagoya-u.ac.jp
+Requires-Python: >=3.7.1,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: jupyter-io (>=0.2,<0.3)
+Requires-Dist: lmfit (>=1.0,<2.0)
+Requires-Dist: matplotlib (>=3.2,<4.0)
+Requires-Dist: numpy (>=1.20,<1.22) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: numpy (>=1.20,<2.0) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: pandas (>=1.3,<1.4) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: pandas (>=1.3,<2.0) ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: pandas-dataclasses (>=0.2,<0.3)
+Requires-Dist: scipy (>=1.4,<2.0)
+Project-URL: Documentation, https://deshima-dev.github.io/deshima-sensitivity/
+Description-Content-Type: text/markdown
+
+# deshima-sensitivity
+
+[![Release](https://img.shields.io/pypi/v/deshima-sensitivity?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/deshima-sensitivity/)
+[![Python](https://img.shields.io/pypi/pyversions/deshima-sensitivity?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/deshima-sensitivity/)
+[![Downloads](https://img.shields.io/pypi/dm/deshima-sensitivity?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/deshima-sensitivity)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3966839-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.3966839)
+[![Tests](https://img.shields.io/github/workflow/status/deshima-dev/deshima-sensitivity/Tests?label=Tests&style=flat-square)](https://github.com/deshima-dev/deshima-sensitivity/actions/tests.yml)
+
+Sensitivity calculator for DESHIMA-type spectrometers
+
+## Overview
+
+deshima-sensitivity is a Python package which enables to calculate observation sensitivity of DESHIMA-type spectrometers.
+Currently it is mainly used to estimate the observation sensitivity of [DESHIMA](http://deshima.ewi.tudelft.nl) and its successors.
+
+An online Jupyter notebook is available for DESHIMA collaborators to calculate the sensitivity and the mapping speed of the DESHIMA 2.0 by themselves.
+Click the budge below to open it in [Google colaboratory](http://colab.research.google.com/) (a Google account is necessary to re-run it).
+
+### Stable version (recommended)
+
+[![open stable version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/v0.4.2/sensitivity.ipynb)
+
+### Latest version
+
+[![open latest version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/main/sensitivity.ipynb)
+
+In the case of running it in a local Python environment, please follow the requirements and the installation guide below.
+
+## Requirements
+
+- **Python:** 3.7, 3.8, or 3.9 (tested by the authors)
+- **Dependencies:** See [pyproject.toml](https://github.com/deshima-dev/deshima-sensitivity/blob/main/pyproject.toml)
+
+## Installation
+
+```shell
+$ pip install deshima-sensitivity
+```
+
+## Development environment
+
+The following steps can create a standalone development environment (VS Code + Python).
+
+1. Install [VS Code] and [Docker Desktop], and launch them
+1. Install the [Remote Containers] extension to VS Code
+1. Clone this repository
+1. Open the repository by VS Code
+1. Choose `Reopen in Container` from the [Command Palette]
+
+[Command Palette]: https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette
+[Docker Desktop]: https://www.docker.com/products/docker-desktop
+[Remote Containers]: https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers
+[VS Code]: https://code.visualstudio.com
 
-packages = \
-['deshima_sensitivity']
 
-package_data = \
-{'': ['*'], 'deshima_sensitivity': ['data/*']}
-
-install_requires = \
-['jupyter-io>=0.2,<0.3',
- 'lmfit>=1.0,<2.0',
- 'matplotlib>=3.2,<4.0',
- 'scipy>=1.4,<2.0']
-
-extras_require = \
-{':python_full_version >= "3.7.1" and python_version < "3.8"': ['numpy>=1.20,<1.22',
-                                                                'pandas>=1.3,<1.4'],
- ':python_version >= "3.8" and python_version < "3.11"': ['numpy>=1.20,<2.0',
-                                                          'pandas>=1.3,<2.0']}
-
-setup_kwargs = {
-    'name': 'deshima-sensitivity',
-    'version': '0.4.1',
-    'description': 'Sensitivity calculator for DESHIMA-type spectrometers',
-    'long_description': '# deshima-sensitivity\n\n[![Release](https://img.shields.io/pypi/v/deshima-sensitivity?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/deshima-sensitivity/)\n[![Python](https://img.shields.io/pypi/pyversions/deshima-sensitivity?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/pypi/deshima-sensitivity/)\n[![Downloads](https://img.shields.io/pypi/dm/deshima-sensitivity?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/deshima-sensitivity)\n[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.3966839-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.3966839)\n[![Tests](https://img.shields.io/github/workflow/status/deshima-dev/deshima-sensitivity/Tests?label=Tests&style=flat-square)](https://github.com/deshima-dev/deshima-sensitivity/actions/tests.yml)\n\nSensitivity calculator for DESHIMA-type spectrometers\n\n## Overview\n\ndeshima-sensitivity is a Python package which enables to calculate observation sensitivity of DESHIMA-type spectrometers.\nCurrently it is mainly used to estimate the observation sensitivity of [DESHIMA](http://deshima.ewi.tudelft.nl) and its successors.\n\nAn online Jupyter notebook is available for DESHIMA collaborators to calculate the sensitivity and the mapping speed of the DESHIMA 2.0 by themselves.\nClick the budge below to open it in [Google colaboratory](http://colab.research.google.com/) (a Google account is necessary to re-run it).\n\n### Stable version (recommended)\n\n[![open stable version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/v0.4.1/sensitivity.ipynb)\n\n### Latest version\n\n[![open latest version in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deshima-dev/deshima-sensitivity/blob/main/sensitivity.ipynb)\n\nIn the case of running it in a local Python environment, please follow the requirements and the installation guide below.\n\n## Requirements\n\n- **Python:** 3.7, 3.8, or 3.9 (tested by the authors)\n- **Dependencies:** See [pyproject.toml](https://github.com/deshima-dev/deshima-sensitivity/blob/main/pyproject.toml)\n\n## Installation\n\n```shell\n$ pip install deshima-sensitivity\n```\n\n## Development environment\n\nThe following steps can create a standalone development environment (VS Code + Python).\n\n1. Install [VS Code] and [Docker Desktop], and launch them\n1. Install the [Remote Containers] extension to VS Code\n1. Clone this repository\n1. Open the repository by VS Code\n1. Choose `Reopen in Container` from the [Command Palette]\n\n[Command Palette]: https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette\n[Docker Desktop]: https://www.docker.com/products/docker-desktop\n[Remote Containers]: https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers\n[VS Code]: https://code.visualstudio.com\n\n',
-    'author': 'Akira Endo',
-    'author_email': 'a.endo@tudelft.nl',
-    'maintainer': 'Akio Taniguchi',
-    'maintainer_email': 'taniguchi@a.phys.nagoya-u.ac.jp',
-    'url': 'https://github.com/deshima-dev/deshima-sensitivity',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

