# Comparing `tmp/blastpipe-2024.0.3.tar.gz` & `tmp/blastpipe-2024.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.0.3.tar", last modified: Thu Apr  4 03:34:55 2024, max compression
+gzip compressed data, was "blastpipe-2024.0.4.tar", last modified: Sat Apr 13 18:59:40 2024, max compression
```

## Comparing `blastpipe-2024.0.3.tar` & `blastpipe-2024.0.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:34:55.091736 blastpipe-2024.0.3/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)    11661 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)    64567 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-04 03:34:55.091736 blastpipe-2024.0.3/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/mixin.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     2943 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4648 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8557 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-04 03:29:19.000000 blastpipe-2024.0.3/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:59:40.217923 blastpipe-2024.0.4/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2889 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5869 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3061 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)    69217 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-13 18:59:40.217923 blastpipe-2024.0.4/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     4528 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1235 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/mixin.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3175 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8329 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      122 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      813 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-04-13 18:54:08.000000 blastpipe-2024.0.4/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.0.3/.github/workflows/codeql.yml` & `blastpipe-2024.0.4/.github/workflows/codeql.yml`

 * *Files 9% similar despite different names*

```diff
@@ -46,33 +46,33 @@
           egress-policy: audit
 
       - name: Checkout repository
         uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@8a470fddafa5cbb6266ee11b37ef4d8aae19c571 # v3.24.6
+        uses: github/codeql-action/init@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@8a470fddafa5cbb6266ee11b37ef4d8aae19c571 # v3.24.6
+        uses: github/codeql-action/autobuild@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@8a470fddafa5cbb6266ee11b37ef4d8aae19c571 # v3.24.6
+        uses: github/codeql-action/analyze@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `blastpipe-2024.0.3/.github/workflows/dependency-review.yml` & `blastpipe-2024.0.4/.github/workflows/dependency-review.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         uses: step-security/harden-runner@63c24ba6bd7ba022e95695ff85de572c04a18142 # v2.7.0
         with:
           egress-policy: audit
 
       - name: 'Checkout Repository'
         uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # v4.1.1
       - name: 'Dependency Review'
-        uses: actions/dependency-review-action@9129d7d40b8c12c1ed0f60400d00c92d437adcce # v4.1.3
+        uses: actions/dependency-review-action@5bbc3ba658137598168acb2ab73b21c432dd411b # v4.2.5
```

### Comparing `blastpipe-2024.0.3/.github/workflows/scorecards.yml` & `blastpipe-2024.0.4/.github/workflows/scorecards.yml`

 * *Files 10% similar despite different names*

```diff
@@ -59,18 +59,18 @@
           #   - `publish_results` will always be set to `false`, regardless
           #     of the value entered here.
           publish_results: true
 
       # Upload the results as artifacts (optional). Commenting out will disable uploads of run results in SARIF
       # format to the repository Actions tab.
       - name: "Upload artifact"
-        uses: actions/upload-artifact@a8a3f3ad30e3422c9c7b888a15615d19a852ae32 # v3.1.3
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # v4.3.1
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@8a470fddafa5cbb6266ee11b37ef4d8aae19c571 # v3.24.6
+        uses: github/codeql-action/upload-sarif@4355270be187e1b672a7a1c7c7bae5afdc1ab94a # v3.24.10
         with:
           sarif_file: results.sarif
```

### Comparing `blastpipe-2024.0.3/.gitignore` & `blastpipe-2024.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/CHANGELOG.md` & `blastpipe-2024.0.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,79 @@
 # CHANGELOG
 
 
 
+## v2024.0.4 (2024-04-13)
+
+### :arrow_up:
+
+* :arrow_up: Bump OZI-Project/release from 0.1.13 to 0.1.14
+
+Bumps [OZI-Project/release](https://github.com/ozi-project/release) from 0.1.13 to 0.1.14.
+- [Release notes](https://github.com/ozi-project/release/releases)
+- [Commits](https://github.com/ozi-project/release/compare/9a404fb06ef2b5c1634518720f8cdafa41539f77...945b312031019d0d85c5674721327f894131d898)
+
+---
+updated-dependencies:
+- dependency-name: OZI-Project/release
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`1b019b0`](https://github.com/OZI-Project/blastpipe/commit/1b019b04ecfaf30b25a05d9c092ee213a10a0fd5))
+
+* :arrow_up: Bump github/codeql-action from 3.24.6 to 3.24.10
+
+Bumps [github/codeql-action](https://github.com/github/codeql-action) from 3.24.6 to 3.24.10.
+- [Release notes](https://github.com/github/codeql-action/releases)
+- [Changelog](https://github.com/github/codeql-action/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/github/codeql-action/compare/8a470fddafa5cbb6266ee11b37ef4d8aae19c571...4355270be187e1b672a7a1c7c7bae5afdc1ab94a)
+
+---
+updated-dependencies:
+- dependency-name: github/codeql-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`d8e7924`](https://github.com/OZI-Project/blastpipe/commit/d8e7924033adcf052e320a2a5e8057833616d53c))
+
+### :hammer:
+
+* :hammer: bump to lastest OZI. ([`912190a`](https://github.com/OZI-Project/blastpipe/commit/912190ae91ffc5645f00396b76e5e3adab643228))
+
+### :pencil2:
+
+* :pencil2: Remove unused option variables. ([`71e885f`](https://github.com/OZI-Project/blastpipe/commit/71e885fc0a179846bc02034430beabbd68068992))
+
+* :pencil2: fix missing envs. ([`b59bc1c`](https://github.com/OZI-Project/blastpipe/commit/b59bc1ca1f3db7ad58858c0ccf8af9e586a1b574))
+
+### Other
+
+* Merge pull request #55 from OZI-Project/dependabot/github_actions/OZI-Project/release-0.1.14
+
+⬆️ Bump OZI-Project/release from 0.1.13 to 0.1.14 ([`d4871e4`](https://github.com/OZI-Project/blastpipe/commit/d4871e4fe9345716add535a6755dace925dd5230))
+
+* :rotating_light: Fix quoted type annotations.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`988f9f2`](https://github.com/OZI-Project/blastpipe/commit/988f9f2b8697ce6569b456ebf1343b952d4fdb0c))
+
+* Merge pull request #50 from OZI-Project/dependabot/github_actions/actions/dependency-review-action-4.2.5
+
+⬆️ Bump actions/dependency-review-action from 4.1.3 to 4.2.5 ([`d3113fe`](https://github.com/OZI-Project/blastpipe/commit/d3113fe1200a1c6bb7822d96351e1820a18a56f8))
+
+* Merge pull request #54 from OZI-Project/dependabot/github_actions/github/codeql-action-3.24.10
+
+⬆️ Bump github/codeql-action from 3.24.6 to 3.24.10 ([`e34440b`](https://github.com/OZI-Project/blastpipe/commit/e34440bb02c1e4750e0acadf2d1fa76f9ae2cf82))
+
+* Merge pull request #52 from OZI-Project/dependabot/github_actions/actions/upload-artifact-4.3.1
+
+⬆️ Bump actions/upload-artifact from 3.1.3 to 4.3.1 ([`389ac50`](https://github.com/OZI-Project/blastpipe/commit/389ac505d22f1a893e3e4423ee8fee49706739aa))
+
+
 ## v2024.0.3 (2024-04-04)
 
 ### :hammer:
 
 * :hammer: Add install-subprojects option.
 
 Signed-off-by: rjdbcm &lt;rjdbcm@mail.umkc.edu&gt; ([`af8f951`](https://github.com/OZI-Project/blastpipe/commit/af8f9519a11ed5efd9a86fc6089afb543688a46e))
@@ -49,14 +117,44 @@
 * Don&#39;t install when run as subproject. ([`a5dfcbc`](https://github.com/OZI-Project/blastpipe/commit/a5dfcbc7ced9f710b01285b704cc4a54538416ec))
 
 
 ## v2024.0.0 (2024-04-03)
 
 ### :arrow_up:
 
+* :arrow_up: Bump actions/dependency-review-action from 4.1.3 to 4.2.5
+
+Bumps [actions/dependency-review-action](https://github.com/actions/dependency-review-action) from 4.1.3 to 4.2.5.
+- [Release notes](https://github.com/actions/dependency-review-action/releases)
+- [Commits](https://github.com/actions/dependency-review-action/compare/9129d7d40b8c12c1ed0f60400d00c92d437adcce...5bbc3ba658137598168acb2ab73b21c432dd411b)
+
+---
+updated-dependencies:
+- dependency-name: actions/dependency-review-action
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`4ae3417`](https://github.com/OZI-Project/blastpipe/commit/4ae34177e2cdc72d9333e924c0e3d31d838d5f9f))
+
+* :arrow_up: Bump actions/upload-artifact from 3.1.3 to 4.3.1
+
+Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 3.1.3 to 4.3.1.
+- [Release notes](https://github.com/actions/upload-artifact/releases)
+- [Commits](https://github.com/actions/upload-artifact/compare/a8a3f3ad30e3422c9c7b888a15615d19a852ae32...5d5d22a31266ced268874388b861e4b58bb5c2f3)
+
+---
+updated-dependencies:
+- dependency-name: actions/upload-artifact
+  dependency-type: direct:production
+  update-type: version-update:semver-major
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`0f33c02`](https://github.com/OZI-Project/blastpipe/commit/0f33c02f27db5a22221b8cd106a214f5b47be0e0))
+
 * :arrow_up: Bump pypa/gh-action-pypi-publish from 1.8.12 to 1.8.14
 
 Bumps [pypa/gh-action-pypi-publish](https://github.com/pypa/gh-action-pypi-publish) from 1.8.12 to 1.8.14.
 - [Release notes](https://github.com/pypa/gh-action-pypi-publish/releases)
 - [Commits](https://github.com/pypa/gh-action-pypi-publish/compare/e53eb8b103ffcb59469888563dc324e3c8ba6f06...81e9d935c883d0b210363ab89cf05f3894778450)
 
 ---
```

### Comparing `blastpipe-2024.0.3/LICENSE.txt` & `blastpipe-2024.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/NOTICE.md` & `blastpipe-2024.0.4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/PKG-INFO` & `blastpipe-2024.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.0.3
+Version: 2024.0.4
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.3.tar.gz
+Download-URL: https://github.com//blastpipe/archive/refs/tags/2024.0.4.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `blastpipe-2024.0.3/README.rst` & `blastpipe-2024.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/__init__.py` & `blastpipe-2024.0.4/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/backports.py` & `blastpipe-2024.0.4/blastpipe/backports.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 from .mixin import mixin
 
 
 class IsTemplatePre311(Protocol):
     """Protocol to check if a Template is pre-3.11"""
 
     delimiter: str
-    idpattern: r'str'
-    braceidpattern: r'Optional[str]'
+    idpattern: str
+    braceidpattern: Optional[str]
     flags: int
     pattern: re.Pattern[str]
     template: str
 
     def safe_substitute(self: Any) -> Optional[str]:
         """Abstract method to be implemented by base"""
 
@@ -54,16 +54,16 @@
 _T = TypeVar('_T', bound='string.Template')
 
 
 class TemplateGetIdentifiersMixin(Mixin[Any]):
     """Example Template mixin with preferred way of typing and using mixins"""
 
     delimiter: str
-    idpattern: r'str'
-    braceidpattern: r'Optional[str]'
+    idpattern: str
+    braceidpattern: Optional[str]
     flags: int
     pattern: re.Pattern[str]
     template: str
 
     def safe_substitute(self: object) -> Optional[str]:
         """Abstract method to be implemented by base"""
```

### Comparing `blastpipe-2024.0.3/blastpipe/backports.pyi` & `blastpipe-2024.0.4/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/buffer.py` & `blastpipe-2024.0.4/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/loop.py` & `blastpipe-2024.0.4/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/malloc.py` & `blastpipe-2024.0.4/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/meson.build` & `blastpipe-2024.0.4/blastpipe/meson.build`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-python_files = [
+source_files = [
     '__init__.py',
     'backports.py',
     'buffer.py',
     'loop.py',
     'malloc.py',
     'mixin.py',
     'sequence.py',
@@ -27,23 +27,17 @@
     'loop.pyi',
     'malloc.pyi',
     'mixin.pyi',
     'sequence.pyi',
     'tailcall.pyi',
     'py.typed',
 ]
-foreach file: python_files
+foreach file: source_files
     fs.copyfile(file)
     if not meson.is_subproject() or get_option('install-subprojects').enabled()
         python.install_sources(file, subdir: project_name)
     endif
 endforeach
-if false
-    executable('source_files', python_files)
-endif
-children = []
-foreach child: children
+source_children = []
+foreach child: source_children
     subdir(child)
-endforeach
-if false
-    executable('source_children', children)
-endif
+endforeach
```

### Comparing `blastpipe-2024.0.3/blastpipe/mixin.py` & `blastpipe-2024.0.4/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/sequence.py` & `blastpipe-2024.0.4/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/blastpipe/tailcall.py` & `blastpipe-2024.0.4/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/meson.build` & `blastpipe-2024.0.4/meson.build`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,27 @@
 )
 env = environment()
 fs = import('fs')
 pymod = import('python')
 project_name = meson.project_name()
 docs_source = 'subprojects/docs'
 pip_compile = find_program('pip-compile', required: true)
-requirements = ['requirements.in']
+root_files = [
+    'README.rst',
+    'CHANGELOG.md',
+    'LICENSE.txt',
+    'requirements.in',
+    'pyproject.toml',
+    '.gitignore',
+    '.pre-commit-config.yaml',
+    'NOTICE.md',
+]
 custom_target(
     'requirements-blastpipe',
-    input: requirements,
+    input: root_files[3],
     output: 'requirements.txt',
     build_always_stale: true,
     build_by_default: true,
     command: [
         'pip-compile',
         '--allow-unsafe',
         '--strip-extras',
@@ -62,37 +71,33 @@
 pyproject_config.set('REQUIREMENTS_IN', '\n'.join(required))
 pyproject_config.set('LICENSE', meson.project_license()[0])
 configure_file(
     input: 'pyproject.toml',
     output: 'pyproject.toml',
     configuration: pyproject_config
 )
-vcs_tag(input: 'pyproject.toml', output: 'pyproject.toml')
-root_files = [
-    'README.rst',
-    'CHANGELOG.md',
-    'LICENSE.txt',
-    'requirements.in',
-    'NOTICE.md',
-]
+vcs_tag(input: 'pyproject.toml', output: 'pyproject.orig.toml')
 foreach source : root_files
-    fs.copyfile(source)
+    if source not in ['pyproject.toml', '.gitignore']
+        fs.copyfile(source)
+    endif
 endforeach
-if false
-    executable('root_files', root_files)
-endif
 root_children = [
     'blastpipe',
     'tests',
 ]
 foreach child: root_children
     subdir(child)
 endforeach
 if false
+    executable('root_files', root_files)
     executable('root_children', root_children)
+    executable('source_files', source_files)
+    executable('source_children', source_children)
+    executable('test_files', test_files)
 endif
 if not meson.is_subproject()
     dev = subproject('ozi')
     foreach var : get_option('variables')
         name = var.replace('-', '_')
         set_variable(name, dev.get_variable(name))
     endforeach
```

### Comparing `blastpipe-2024.0.3/meson.options` & `blastpipe-2024.0.4/meson.options`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,14 @@
         'python',
         'metadata-version',
         'namespace',
         'should-fail',
         'unhashable',
         'plugin-only',
         'no-version',
-        'emoji-dist',
-        'emoji-lint',
-        'emoji-test',
-        'emoji-no-version',
-        'emoji-metadata-version',
         'dist-exclude-suites',
         'lint-exclude-suites',
         'test-exclude-suites'
     ]
 )
 option(
     'dist-suite',
```

### Comparing `blastpipe-2024.0.3/pyproject.toml` & `blastpipe-2024.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -324,77 +324,62 @@
 parentdir_prefix_version = "blastpipe-"
 tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist = True
-envlist = py310,py311,py312
 
 [gh]
 python =
-   3.12 = py312
-   3.11 = py311
-   3.10 = py310
-[testenv:dist]
+   3.12 = dist,lint,test
+   3.11 = dist,lint,test
+   3.10 = dist,lint,test
+
+[testenv]
 allowlist_externals = rm
 package = wheel
 deps =
    mesonpep517>=0.2
    meson[ninja]>=1.1.0
    pip-tools>=7
    setuptools>=64
    setuptools_scm>=8.0
    tomli>=2.0.0;python_version<"3.11"
    -r requirements.in
 commands =
-   meson setup {env_tmp_dir} -Dozi:dist=enabled --reconfigure
    meson compile -C {env_tmp_dir}
    rm -rf {env_tmp_dir}/.gitignore
-   meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=dist
+
+[testenv:dist]
+commands_pre = meson setup {env_tmp_dir} -Dozi:dist=enabled --reconfigure
+commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=dist
+
 [testenv:lint]
-allowlist_externals = rm
-package = wheel
-deps =
-   mesonpep517>=0.2
-   meson[ninja]>=1.1.0
-   pip-tools>=7
-   setuptools>=64
-   setuptools_scm>=8.0
-   tomli>=2.0.0;python_version<"3.11"
-   -r requirements.in
-commands =
-   meson setup {env_tmp_dir} -Dozi:lint=enabled --reconfigure
-   meson compile -C {env_tmp_dir}
-   rm -rf {env_tmp_dir}/.gitignore
-   meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=lint
+commands_pre = meson setup {env_tmp_dir} -Dozi:lint=enabled --reconfigure
+commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=lint
+
 [testenv:test]
-allowlist_externals = rm
-package = wheel
-deps =
-   mesonpep517>=0.2
-   meson[ninja]>=1.1.0
-   pip-tools>=7
-   setuptools>=64
-   setuptools_scm>=8.0
-   tomli>=2.0.0;python_version<"3.11"
-   -r requirements.in
-commands =
-   meson setup {env_tmp_dir} -Dozi:test=enabled --reconfigure
-   meson compile -C {env_tmp_dir}
-   rm -rf {env_tmp_dir}/.gitignore
-   meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=test
+commands_pre = meson setup {env_tmp_dir} -Dozi:test=enabled --reconfigure
+commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=test
 
 [testenv:fix]
-description = quickly fix minor source issues 
+description = OZI project fix issues utility (black, isort, autoflake, ruff)
 deps = 
-     black
+     black>=24.3
      isort
      autoflake
      ruff
 skip_install = true
 commands =
-     black -v -S .
-     isort .
-     autoflake -i -vv -r .
-     ruff check blastpipe --fix
+     {env_python} -m black -S .
+     {env_python} -m isort .
+     {env_python} -m autoflake -i -r .
+     {env_python} -m ruff check blastpipe --fix
+
+[testenv:scm]
+description = OZI supply chain management (setuptools_scm)
+deps =
+     setuptools_scm[toml]>=8
+commands =
+     {env_python} -m setuptools_scm {posargs}
 """
```

### Comparing `blastpipe-2024.0.3/subprojects/docs/LICENSE.txt` & `blastpipe-2024.0.4/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.0.4/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.0.4/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/_static/meson.build` & `blastpipe-2024.0.4/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/_templates/layout.html` & `blastpipe-2024.0.4/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/_templates/meson.build` & `blastpipe-2024.0.4/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/conf.cfg` & `blastpipe-2024.0.4/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/index.rst` & `blastpipe-2024.0.4/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/meson.build` & `blastpipe-2024.0.4/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/subprojects/docs/meson.options` & `blastpipe-2024.0.4/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/tests/meson.build` & `blastpipe-2024.0.4/tests/meson.build`

 * *Files 11% similar despite different names*

```diff
@@ -17,10 +17,7 @@
  'test_fuzz.py',
  'test_tailcall.py',
 ]
 foreach file: test_files
   fs.copyfile(file)
   python.install_sources(file, subdir: project_name/'tests')
 endforeach
-if false
-  executable('test_files', test_files)
-endif
```

### Comparing `blastpipe-2024.0.3/tests/test_backports.py` & `blastpipe-2024.0.4/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/tests/test_fuzz.py` & `blastpipe-2024.0.4/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.0.3/tests/test_tailcall.py` & `blastpipe-2024.0.4/tests/test_tailcall.py`

 * *Files identical despite different names*

