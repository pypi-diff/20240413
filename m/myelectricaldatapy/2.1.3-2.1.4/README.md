# Comparing `tmp/myelectricaldatapy-2.1.3.tar.gz` & `tmp/myelectricaldatapy-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.3.tar", last modified: Thu Feb  8 07:33:44 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.1.4.tar", last modified: Sat Apr 13 15:49:57 2024, max compression
```

## Comparing `myelectricaldatapy-2.1.3.tar` & `myelectricaldatapy-2.1.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.511008 myelectricaldatapy-2.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.511008 myelectricaldatapy-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.511008 myelectricaldatapy-2.1.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-02-08 07:33:44.000000 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-08 07:33:44.000000 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 07:33:44.000000 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-08 07:33:44.000000 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-08 07:33:44.000000 myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-08 07:33:37.000000 myelectricaldatapy-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:44.515008 myelectricaldatapy-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-08 07:33:26.000000 myelectricaldatapy-2.1.3/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.352177 myelectricaldatapy-2.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/dependbot-auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 15:49:57.000000 myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:49:57.360177 myelectricaldatapy-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.356177 myelectricaldatapy-2.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-13 15:49:44.000000 myelectricaldatapy-2.1.4/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.3/.github/dependabot.yml` & `myelectricaldatapy-2.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.3/.github/workflows/lint.yml` & `myelectricaldatapy-2.1.4/.github/workflows/lint.yml`

 * *Files 22% similar despite different names*

```diff
@@ -23,8 +23,8 @@
       - name: 📦 Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
           pip install pylint
 
       - name: Run pre-commit
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
```

### Comparing `myelectricaldatapy-2.1.3/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.1.4/.github/workflows/pythonpublish.yml`

 * *Files 24% similar despite different names*

```diff
@@ -8,18 +8,16 @@
     tags:
       - "*.*.*"
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     name: Deploy to PyPi
-    # Specifying a GitHub environment is optional, but strongly encouraged
     environment: release
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
       - name: 📥 Checkout the repository
         uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
@@ -27,20 +25,14 @@
           python-version: "3.x"
 
       - name: 📦 Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel twine build
 
-      - name: 🔢 Set version number
-        run: |
-          export version=${{ github.ref }}
-          sed -i "s|replace_by_workflow|${version##*/}|" ./pyproject.toml
-          cat ./pyproject.toml
-
       - name: Build package
         shell: bash
         run: |
           python -m build
 
       - name: 🚀 Publish to PyPi
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `myelectricaldatapy-2.1.3/.github/workflows/release.yml` & `myelectricaldatapy-2.1.4/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     runs-on: ubuntu-latest
     steps:
       # To use this repository's private action, you must check out the repository
       - name: Checkout
         uses: actions/checkout@v4
       - name: Generate changelog
         id: changelog
-        uses: metcalfc/changelog-generator@v4.3.0
+        uses: metcalfc/changelog-generator@v4.3.1
         with:
           myToken: ${{ secrets.GITHUB_TOKEN }}
       - name: Create Release
         id: create_release
         uses: actions/create-release@latest
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `myelectricaldatapy-2.1.3/.gitignore` & `myelectricaldatapy-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.3/.pre-commit-config.yaml` & `myelectricaldatapy-2.1.4/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.0
+    rev: v0.3.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
@@ -20,15 +20,15 @@
     rev: v4.5.0
     hooks:
       - id: check-executables-have-shebangs
         stages: [manual]
       - id: check-json
         exclude: (.vscode|.devcontainer)
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.33.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
         exclude: (.github|.vscode|.devcontainer)
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
@@ -43,13 +43,13 @@
         stages: [manual]
         args:
           - --py311-plus
           - --force
           - --keep-updates
         files: ^(/.+)?[^/]+\.py$
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports]
         additional_dependencies: [types-requests==2.28.11.7]
         exclude: tests/
```

### Comparing `myelectricaldatapy-2.1.3/LICENSE` & `myelectricaldatapy-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.3/PKG-INFO` & `myelectricaldatapy-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.3
+Version: 2.1.4
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.3/README.md` & `myelectricaldatapy-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.3/example.py` & `myelectricaldatapy-2.1.4/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-""" Example code."""
+"""Example code."""
 
 import asyncio
 import logging
 from datetime import datetime, timedelta
 
 from myelectricaldatapy import Enedis, EnedisByPDL, EnedisException
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.1.4/myelectricaldatapy/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for analytics."""
+
 from __future__ import annotations
 
 from datetime import datetime as dt, timedelta
 import logging
 import re
 from typing import Any, Collection, Tuple
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.1.4/myelectricaldatapy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for Enedis Authentication (http://www.myelectricaldata.fr)."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import socket
 from typing import Any
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.1.4/myelectricaldatapy/myelectricaldata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for Enedis Gateway (http://www.myelectricaldata.fr)."""
+
 from __future__ import annotations
 
 import logging
 import re
 from datetime import date
 from datetime import datetime as dt
 from datetime import timedelta
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.1.4/myelectricaldatapy/mypdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for my PDL."""
+
 from __future__ import annotations
 
 import logging
 from datetime import date
 from datetime import datetime as dt
 from datetime import timedelta
 from typing import Any, Callable, Tuple
@@ -178,26 +179,38 @@
             self.max_power = {}
             self.has_collected = False
         try:
             self.access = await self._api.async_valid_access(self.pdl)
             if self.access.get("quota_reached", False):
                 detail = self.access.get("information", "Quota reached")
                 raise LimitReached(409, {"detail": detail})
+
             if self.is_connected is False:
                 raise EnedisException(200, {"detail": "Api access not valid"})
+
             if not self.contract:
-                self.contract = await self._api.async_get_contract(self.pdl)
+                try:
+                    self.contract = await self._api.async_get_contract(self.pdl)
+                except EnedisException as error:
+                    _LOGGER.warning(error)
+
             if not self.address:
-                self.address = await self._api.async_get_address(self.pdl)
+                try:
+                    self.address = await self._api.async_get_address(self.pdl)
+                except EnedisException as error:
+                    _LOGGER.warning(error)
+
             if not self.ecowatt and self._ecowatt_subs:
                 self.ecowatt = await self._api.async_get_ecowatt(start, end)
+
             if not self.max_power and self._maxpower_subs:
                 self.max_power = await self._api.async_get_max_power(
                     self.pdl, start, end
                 )
+
             if self.has_parameters and self.has_collected is False:
                 await self.async_update_collects()
                 self.last_refresh = dt.now()
         except EnedisException as error:
             raise error from error
         finally:
             self.last_access = dt.now()
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.3
+Version: 2.1.4
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.3/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.1.4/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MANIFEST.in
 README.md
 example.py
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 .github/dependabot.yml
+.github/workflows/dependbot-auto-approve.yml
 .github/workflows/lint.yml
 .github/workflows/pythonpublish.yml
 .github/workflows/release.yml
 .vscode/settings.json
 myelectricaldatapy/__init__.py
 myelectricaldatapy/analytics.py
 myelectricaldatapy/auth.py
```

### Comparing `myelectricaldatapy-2.1.3/pyproject.toml` & `myelectricaldatapy-2.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.3/tests/conftest.py` & `myelectricaldatapy-2.1.4/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 """Test helpers for MyElectricalData."""
+
 from collections.abc import Generator
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
 import myelectricaldatapy
 
 from .consts import ACCESS, ADDRESS, CONTRACT, DATASET_30, DATASET_DAILY, ECOWATT, TEMPO
 
 
 @pytest.fixture(name="mock_enedis")
 def mock_enedis() -> Generator[AsyncMock, None, None]:
     """Mock a successful connection."""
-    with patch.object(
-        myelectricaldatapy.Enedis,
-        "async_get_daily_consumption",
-        return_value=DATASET_DAILY,
-    ), patch.object(
-        myelectricaldatapy.Enedis,
-        "async_get_daily_production",
-        return_value=DATASET_DAILY,
-    ), patch.object(
-        myelectricaldatapy.Enedis,
-        "async_get_details_consumption",
-        return_value=DATASET_30,
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_valid_access", return_value=ACCESS
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_contract", return_value=CONTRACT
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_address", return_value=ADDRESS
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO
-    ), patch.object(
-        myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=ECOWATT
-    ) as service_mock:
+    with (
+        patch.object(
+            myelectricaldatapy.Enedis,
+            "async_get_daily_consumption",
+            return_value=DATASET_DAILY,
+        ),
+        patch.object(
+            myelectricaldatapy.Enedis,
+            "async_get_daily_production",
+            return_value=DATASET_DAILY,
+        ),
+        patch.object(
+            myelectricaldatapy.Enedis,
+            "async_get_details_consumption",
+            return_value=DATASET_30,
+        ),
+        patch.object(
+            myelectricaldatapy.Enedis, "async_valid_access", return_value=ACCESS
+        ),
+        patch.object(
+            myelectricaldatapy.Enedis, "async_get_contract", return_value=CONTRACT
+        ),
+        patch.object(
+            myelectricaldatapy.Enedis, "async_get_address", return_value=ADDRESS
+        ),
+        patch.object(myelectricaldatapy.Enedis, "async_get_tempo", return_value=TEMPO),
+        patch.object(
+            myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=ECOWATT
+        ) as service_mock,
+    ):
         yield service_mock
```

### Comparing `myelectricaldatapy-2.1.3/tests/consts.py` & `myelectricaldatapy-2.1.4/tests/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test constants."""
+
 PDL = "01234567890"
 TOKEN = "xxxxxxxxxxxxx"
 
 ACCESS = {
     "valid": True,
     "consent_expiration_date": "2026-01-14T15:32:38",
     "call_number": 7,
```

### Comparing `myelectricaldatapy-2.1.3/tests/test_analytics.py` & `myelectricaldatapy-2.1.4/tests/test_analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests analytics."""
+
 from __future__ import annotations
 
 from datetime import datetime as dt
 from typing import Any
 from unittest.mock import Mock, patch
 
 import pytest
```

### Comparing `myelectricaldatapy-2.1.3/tests/test_load_data.py` & `myelectricaldatapy-2.1.4/tests/test_load_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests  Enedis api."""
+
 from __future__ import annotations
 
 from datetime import datetime as dt
 from unittest.mock import Mock, patch
 
 import pytest
 from freezegun import freeze_time
```

