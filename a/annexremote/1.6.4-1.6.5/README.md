# Comparing `tmp/annexremote-1.6.4.tar.gz` & `tmp/annexremote-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annexremote-1.6.4.tar", last modified: Sat Oct 28 00:20:40 2023, max compression
+gzip compressed data, was "annexremote-1.6.5.tar", last modified: Sat Apr 13 17:05:03 2024, max compression
```

## Comparing `annexremote-1.6.4.tar` & `annexremote-1.6.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.781856 annexremote-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-28 00:20:11.000000 annexremote-1.6.4/.autorc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-28 00:20:11.000000 annexremote-1.6.4/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-28 00:20:11.000000 annexremote-1.6.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.773856 annexremote-1.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-10-28 00:20:11.000000 annexremote-1.6.4/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-28 00:20:11.000000 annexremote-1.6.4/.github/workflows/codespell.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-10-28 00:20:11.000000 annexremote-1.6.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-10-28 00:20:11.000000 annexremote-1.6.4/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-28 00:20:11.000000 annexremote-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-28 00:20:11.000000 annexremote-1.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12388 2023-10-28 00:20:29.000000 annexremote-1.6.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-10-28 00:20:11.000000 annexremote-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-28 00:20:11.000000 annexremote-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2023-10-28 00:20:40.781856 annexremote-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2023-10-28 00:20:11.000000 annexremote-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/annexremote/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-28 00:20:11.000000 annexremote-1.6.4/annexremote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    44421 2023-10-28 00:20:11.000000 annexremote-1.6.4/annexremote/annexremote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/annexremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-28 00:20:40.000000 annexremote-1.6.4/annexremote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/docs/annexremote/
--rw-r--r--   0 runner    (1001) docker     (127)    76316 2023-10-28 00:20:11.000000 annexremote-1.6.4/docs/annexremote/annexremote.html
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-28 00:20:11.000000 annexremote-1.6.4/docs/annexremote/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-10-28 00:20:11.000000 annexremote-1.6.4/docs/config.mako
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-10-28 00:20:11.000000 annexremote-1.6.4/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.777856 annexremote-1.6.4/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4825 2023-10-28 00:20:11.000000 annexremote-1.6.4/examples/git-annex-remote-directory
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-10-28 00:20:11.000000 annexremote-1.6.4/examples/git-annex-remote-example
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-10-28 00:20:11.000000 annexremote-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-28 00:20:11.000000 annexremote-1.6.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 00:20:40.781856 annexremote-1.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:20:40.781856 annexremote-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    44421 2023-10-28 00:20:11.000000 annexremote-1.6.4/tests/annexremote.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-28 00:20:11.000000 annexremote-1.6.4/tests/test_AnnexRemoteSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    29481 2023-10-28 00:20:11.000000 annexremote-1.6.4/tests/test_GitAnnexRequestMessages.py
--rw-r--r--   0 runner    (1001) docker     (127)    16495 2023-10-28 00:20:11.000000 annexremote-1.6.4/tests/test_SpecialRemoteMessages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-10-28 00:20:11.000000 annexremote-1.6.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.231719 annexremote-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-13 17:04:46.000000 annexremote-1.6.5/.autorc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-13 17:04:46.000000 annexremote-1.6.5/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 17:04:46.000000 annexremote-1.6.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.219719 annexremote-1.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.223719 annexremote-1.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 17:04:46.000000 annexremote-1.6.5/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 17:04:46.000000 annexremote-1.6.5/.github/workflows/codespell.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-13 17:04:46.000000 annexremote-1.6.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-13 17:04:46.000000 annexremote-1.6.5/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 17:04:46.000000 annexremote-1.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 17:04:46.000000 annexremote-1.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13585 2024-04-13 17:04:58.000000 annexremote-1.6.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-13 17:04:46.000000 annexremote-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 17:04:46.000000 annexremote-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-04-13 17:05:03.227719 annexremote-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-13 17:04:46.000000 annexremote-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.223719 annexremote-1.6.5/annexremote/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 17:04:46.000000 annexremote-1.6.5/annexremote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-13 17:04:46.000000 annexremote-1.6.5/annexremote/annexremote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.227719 annexremote-1.6.5/annexremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 17:05:03.000000 annexremote-1.6.5/annexremote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.227719 annexremote-1.6.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.227719 annexremote-1.6.5/docs/annexremote/
+-rw-r--r--   0 runner    (1001) docker     (127)    76316 2024-04-13 17:04:46.000000 annexremote-1.6.5/docs/annexremote/annexremote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-13 17:04:46.000000 annexremote-1.6.5/docs/annexremote/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-13 17:04:46.000000 annexremote-1.6.5/docs/config.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-13 17:04:46.000000 annexremote-1.6.5/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.227719 annexremote-1.6.5/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-04-13 17:04:46.000000 annexremote-1.6.5/examples/git-annex-remote-directory
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-13 17:04:46.000000 annexremote-1.6.5/examples/git-annex-remote-example
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-13 17:04:46.000000 annexremote-1.6.5/examples/test_git-annex-remote-directory
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-13 17:04:46.000000 annexremote-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-13 17:04:46.000000 annexremote-1.6.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:05:03.231719 annexremote-1.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:05:03.227719 annexremote-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-13 17:04:46.000000 annexremote-1.6.5/tests/annexremote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-13 17:04:46.000000 annexremote-1.6.5/tests/test_AnnexRemoteSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29481 2024-04-13 17:04:46.000000 annexremote-1.6.5/tests/test_GitAnnexRequestMessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-04-13 17:04:46.000000 annexremote-1.6.5/tests/test_SpecialRemoteMessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-13 17:04:46.000000 annexremote-1.6.5/tests/utils.py
```

### Comparing `annexremote-1.6.4/.github/workflows/release.yml` & `annexremote-1.6.5/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       - name: Download latest auto
         run: |
           auto_download_url="$(curl -fsSL https://api.github.com/repos/intuit/auto/releases/latest | jq -r '.assets[] | select(.name == "auto-linux.gz") | .browser_download_url')"
           wget -O- "$auto_download_url" | gunzip > ~/auto
           chmod a+x ~/auto
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.9
 
       - name: Install build & twine
         run: python -m pip install build twine
 
       - name: Create release
```

### Comparing `annexremote-1.6.4/.github/workflows/unittests.yml` & `annexremote-1.6.5/.github/workflows/unittests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       fail-fast: false
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flake8 pytest pytest-cov
         pip install .
@@ -34,14 +34,21 @@
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
       run: |
         python -m pytest -s -v --cov=annexremote --cov-report=xml tests
+    - name: Install git-annex needed for the next step
+      run: |
+        sudo apt update
+        sudo apt install -y git-annex
+    - name: Test example external remote
+      run: |
+        examples/test_git-annex-remote-directory
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         # token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
         flags: unittests
         fail_ci_if_error: false
```

### Comparing `annexremote-1.6.4/CHANGELOG.md` & `annexremote-1.6.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+# v1.6.5 (Sat Apr 13 2024)
+
+#### 🐛 Bug Fix
+
+- Add listconfigs to examples/git-annex-remote-directory + a test for that [#101](https://github.com/Lykos153/AnnexRemote/pull/101) ([@yarikoptic](https://github.com/yarikoptic))
+- chore(deps): update pre-commit hook psf/black to v24.3.0 [#99](https://github.com/Lykos153/AnnexRemote/pull/99) ([@renovate[bot]](https://github.com/renovate[bot]))
+- chore(deps): update pre-commit hook psf/black to v24 [#98](https://github.com/Lykos153/AnnexRemote/pull/98) ([@renovate[bot]](https://github.com/renovate[bot]))
+- Update pre-commit hook psf/black to v23.12.0 [#95](https://github.com/Lykos153/AnnexRemote/pull/95) ([@renovate[bot]](https://github.com/renovate[bot]))
+- Update actions/setup-python action to v5 [#96](https://github.com/Lykos153/AnnexRemote/pull/96) ([@renovate[bot]](https://github.com/renovate[bot]))
+
+#### 🏠 Internal
+
+- chore(deps): update pre-commit hook psf/black to v24.4.0 [#102](https://github.com/Lykos153/AnnexRemote/pull/102) ([@renovate[bot]](https://github.com/renovate[bot]))
+
+#### Authors: 2
+
+- [@renovate[bot]](https://github.com/renovate[bot])
+- Yaroslav Halchenko ([@yarikoptic](https://github.com/yarikoptic))
+
+---
+
 # v1.6.4 (Sat Oct 28 2023)
 
 #### 🏠 Internal
 
 - Fix build - remove setuptools-git-versioning from pyproject.toml and also versioneer.py from MANIFEST [#94](https://github.com/Lykos153/AnnexRemote/pull/94) ([@yarikoptic](https://github.com/yarikoptic))
 
 #### Authors: 1
```

### Comparing `annexremote-1.6.4/LICENSE` & `annexremote-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/PKG-INFO` & `annexremote-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annexremote
-Version: 1.6.4
+Version: 1.6.5
 Summary: git annex special remotes made easy
 Author-email: Silvio Ankermann <silvio@booq.org>
 License: GPL-3.0-only
 Project-URL: Documentation, https://lykos153.github.io/AnnexRemote
 Project-URL: Source, https://github.com/Lykos153/AnnexRemote
 Keywords: git-annex,remote
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `annexremote-1.6.4/README.md` & `annexremote-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/annexremote/annexremote.py` & `annexremote-1.6.5/annexremote/annexremote.py`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/annexremote.egg-info/PKG-INFO` & `annexremote-1.6.5/annexremote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annexremote
-Version: 1.6.4
+Version: 1.6.5
 Summary: git annex special remotes made easy
 Author-email: Silvio Ankermann <silvio@booq.org>
 License: GPL-3.0-only
 Project-URL: Documentation, https://lykos153.github.io/AnnexRemote
 Project-URL: Source, https://github.com/Lykos153/AnnexRemote
 Keywords: git-annex,remote
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `annexremote-1.6.4/annexremote.egg-info/SOURCES.txt` & `annexremote-1.6.5/annexremote.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 annexremote.egg-info/top_level.txt
 docs/config.mako
 docs/index.html
 docs/annexremote/annexremote.html
 docs/annexremote/index.html
 examples/git-annex-remote-directory
 examples/git-annex-remote-example
+examples/test_git-annex-remote-directory
 tests/annexremote.py
 tests/test_AnnexRemoteSetup.py
 tests/test_GitAnnexRequestMessages.py
 tests/test_SpecialRemoteMessages.py
 tests/utils.py
```

### Comparing `annexremote-1.6.4/docs/annexremote/annexremote.html` & `annexremote-1.6.5/docs/annexremote/annexremote.html`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/docs/annexremote/index.html` & `annexremote-1.6.5/docs/annexremote/index.html`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/docs/config.mako` & `annexremote-1.6.5/docs/config.mako`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/examples/git-annex-remote-directory` & `annexremote-1.6.5/examples/git-annex-remote-directory`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 class DirectoryRemote(ExportRemote):
     def initremote(self):
         self.directory = self.annex.getconfig("directory")
         if not self.directory:
             raise RemoteError("You need to set directory=")
         self._mkdir(self.directory)
 
+    def listconfigs(self):
+        return {"directory": "directory where data is stored"}
+
     def prepare(self):
         self.directory = self.annex.getconfig("directory")
         self.info = {"directory": self.directory}
         if not os.path.exists(self.directory):
             raise RemoteError("{} not found".format(self.directory))
 
     def transfer_store(self, key, filename):
```

### Comparing `annexremote-1.6.4/examples/git-annex-remote-example` & `annexremote-1.6.5/examples/git-annex-remote-example`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/pyproject.toml` & `annexremote-1.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/tests/annexremote.py` & `annexremote-1.6.5/tests/annexremote.py`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/tests/test_GitAnnexRequestMessages.py` & `annexremote-1.6.5/tests/test_GitAnnexRequestMessages.py`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/tests/test_SpecialRemoteMessages.py` & `annexremote-1.6.5/tests/test_SpecialRemoteMessages.py`

 * *Files identical despite different names*

### Comparing `annexremote-1.6.4/tests/utils.py` & `annexremote-1.6.5/tests/utils.py`

 * *Files identical despite different names*

