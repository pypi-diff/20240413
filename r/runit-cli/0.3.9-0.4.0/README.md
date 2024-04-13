# Comparing `tmp/runit-cli-0.3.9.tar.gz` & `tmp/runit_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runit-cli-0.3.9.tar", last modified: Tue Dec 26 09:26:50 2023, max compression
+gzip compressed data, was "runit_cli-0.4.0.tar", last modified: Sat Apr 13 14:28:36 2024, max compression
```

## Comparing `runit-cli-0.3.9.tar` & `runit_cli-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-26 09:26:40.000000 runit-cli-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2023-12-26 09:26:50.606441 runit-cli-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-26 09:26:40.000000 runit-cli-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.602441 runit-cli-0.3.9/runit/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.602441 runit-cli-0.3.9/runit/languages/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/php.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/languages/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.602441 runit-cli-0.3.9/runit/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/modules/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/runit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.602441 runit-cli-0.3.9/runit/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/.runitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.602441 runit-cli-0.3.9/runit/templates/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/javascript/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/javascript/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/templates/multi/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/index.php
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/request.php
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/multi/test.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/templates/php/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/php/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/php/index.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/python/application.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/request.php
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/templates/runit.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.598441 runit-cli-0.3.9/runit/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/tools/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/javascript/loader.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/javascript/runner.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/tools/php/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/php/loader.php
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/php/manager.php
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/php/runner.php
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit/tools/python/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/python/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-12-26 09:26:40.000000 runit-cli-0.3.9/runit/tools/python/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:26:50.606441 runit-cli-0.3.9/runit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-26 09:26:50.000000 runit-cli-0.3.9/runit_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 09:26:50.606441 runit-cli-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-12-26 09:26:40.000000 runit-cli-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.923806 runit_cli-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-13 14:28:32.000000 runit_cli-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 14:28:36.923806 runit_cli-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-13 14:28:32.000000 runit_cli-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.911805 runit_cli-0.4.0/runit/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/languages/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/modules/account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/plugins/languages/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/plugins/languages/r.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16554 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/runit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/.runitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.915805 runit_cli-0.4.0/runit/templates/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/javascript/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/javascript/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/multi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/index.php
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/multi/test.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/php/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/php/index.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/python/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/request.php
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/templates/runit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.911805 runit_cli-0.4.0/runit/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/javascript/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/javascript/runner.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/php/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/loader.php
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/manager.php
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/php/runner.php
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/runit/tools/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/python/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 14:28:32.000000 runit_cli-0.4.0/runit/tools/python/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.923806 runit_cli-0.4.0/runit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 14:28:36.000000 runit_cli-0.4.0/runit_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:28:36.923806 runit_cli-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-13 14:28:32.000000 runit_cli-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:28:36.919805 runit_cli-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_clone_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_create_new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_create_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_generate_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_publish_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-13 14:28:32.000000 runit_cli-0.4.0/tests/test_run_project.py
```

### Comparing `runit-cli-0.3.9/PKG-INFO` & `runit_cli-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.3.9
+Version: 0.4.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
-Project-URL: Source, https://github.com/theonlyamos/runit/
+Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `runit-cli-0.3.9/README.md` & `runit_cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/Request.py` & `runit_cli-0.4.0/runit/Request.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/cli.py` & `runit_cli-0.4.0/runit/cli.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/constants.py` & `runit_cli-0.4.0/runit/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.3.9"
+VERSION = "0.4.0"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = Path(os.curdir).resolve()
```

### Comparing `runit-cli-0.3.9/runit/core.py` & `runit_cli-0.4.0/runit/core.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/generate.py` & `runit_cli-0.4.0/runit/generate.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/__init__.py` & `runit_cli-0.4.0/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/javascript.py` & `runit_cli-0.4.0/runit/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/multi.py` & `runit_cli-0.4.0/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/php.py` & `runit_cli-0.4.0/runit/languages/php.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/python.py` & `runit_cli-0.4.0/runit/languages/python.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/languages/runtime.py` & `runit_cli-0.4.0/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/modules/account.py` & `runit_cli-0.4.0/runit/modules/account.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/runit.py` & `runit_cli-0.4.0/runit/runit.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,28 +113,28 @@
         '''
         global IS_RUNNING
         try:
             if not IS_RUNNING:
                 IS_RUNNING = True
                 
             while not name:
-                name = str(input('Enter RunIt Name: '))
+                name = str(input('Enter RunIt Project Name: '))
             return name
         except KeyboardInterrupt:
             sys.exit(1)
     
     @staticmethod
     def notfound(format='json'):
         global TEMPLATES_FOLDER
         global NOT_FOUND_FILE
 
         if format == 'json':
             return '404 - Not Found'
 
-        with open(os.path.join(os.curdir, TEMPLATES_FOLDER, NOT_FOUND_FILE),'rt') as file:
+        with open(os.path.join(TEMPLATES_FOLDER, NOT_FOUND_FILE),'rt') as file:
             return file.read()
     
     @staticmethod
     def extract_project(filepath):
         directory = os.path.split(filepath)[0]
     
         with ZipFile(filepath, 'r') as file:
@@ -196,27 +196,27 @@
         bg_thread.start()
         bg_thread.join()
 
     @classmethod
     def is_private(cls, project_id: str, projects_folder: Path | str = PROJECTS_DIR)-> bool:
         global NOT_FOUND_FILE
 
-        os.chdir(projects_folder)
+        os.chdir(Path(projects_folder, project_id))
         
         if not RunIt.has_config_file():
             return False
         
         project = cls(**RunIt.load_config())
         return project.private
 
     @classmethod
     def start(cls, project_id: str, func='index', projects_folder: Path | str = PROJECTS_DIR, args: Optional[Union[dict,list]]=None):
         global NOT_FOUND_FILE
 
-        os.chdir(projects_folder)
+        os.chdir(Path(projects_folder, project_id))
         
         if not RunIt.has_config_file():
             return RunIt.notfound()
         
         project = cls(**RunIt.load_config())
         
         
@@ -228,15 +228,15 @@
 
         args_list = args if type(args) is list  else []
         
         start_file = project.start_file
 
         lang_parser = LanguageParser.detect_language(
             filename=start_file, 
-            runtime=os.getenv('RUNTIME_'+project.language.upper(), project.runtime), 
+            runtime=project.runtime, 
             is_docker=RunIt.DOCKER, 
             project_id=project_id
         )
         lang_parser.current_func = func
         try:
             return getattr(lang_parser, func)(*args_list)
         except AttributeError as e:
@@ -404,34 +404,35 @@
         package_file = open('package.json', 'rt')
         package_details = json.load(package_file)
         package_file.close()
         
         package_details['name'] = self.name
         package_details['author'] = self.author
         
-        package_file = open('package.json', 'wt')
-        json.dump(package_details, package_file, indent=4)
-        package_file.close()
+        with open('package.json', 'wt') as package_file:
+            json.dump(package_details, package_file, indent=4)
+        
         try:
             logger.info('[-] Installing node modules...')
             if RunIt.RUNTIME_ENV == 'client':
                 os.system('npm install')
             else:
                 os.system('bun install')
         except Exception as e:
             logger.exception(str(e))
             logger.error("[!] Couldn't install modules")
             logger.debug(INSTALL_MODULE_LATER_MESSAGE)
         
 
     def update_and_install_composer_json(self):
         logger.info("[-] Creating and updating composer.json")
-        package_file = open('composer.json', 'rt')
-        package_details = json.load(package_file)
-        package_file.close()
+        
+        package_details = {}
+        with open('composer.json', 'rt') as package_file:
+            package_details = json.load(package_file)
         
         package_details['name'] = f"runit/{self.name.replace('-', '_')}"
         package_details['author'] = self.author
         
         with open('composer.json', 'wt') as package_file:
             json.dump(package_details, package_file, indent=4)
```

### Comparing `runit-cli-0.3.9/runit/templates/404.html` & `runit_cli-0.4.0/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/templates/multi/application.py` & `runit_cli-0.4.0/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/templates/python/application.py` & `runit_cli-0.4.0/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/tools/javascript/runner.js` & `runit_cli-0.4.0/runit/tools/javascript/runner.js`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/tools/php/loader.php` & `runit_cli-0.4.0/runit/tools/php/loader.php`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/tools/php/runner.php` & `runit_cli-0.4.0/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit/tools/python/runner.py` & `runit_cli-0.4.0/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `runit-cli-0.3.9/runit_cli.egg-info/PKG-INFO` & `runit_cli-0.4.0/runit_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: runit-cli
-Version: 0.3.9
+Version: 0.4.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
-Project-URL: Source, https://github.com/theonlyamos/runit/
+Project-URL: Source, https://github.com/theonlyamos/runit
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `runit-cli-0.3.9/setup.py` & `runit_cli-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.3.9'
+VERSION = '0.4.0'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='runit-cli',
     version=VERSION,
@@ -16,15 +16,15 @@
     long_description_content_type = "text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=['requests','python-dotenv','fastapi', \
                       'passlib', 'docker', 'uvicorn', 'websockets'],
     keywords='python3 runit developer serverless architecture docker',
     project_urls={
-        'Source': 'https://github.com/theonlyamos/runit/',
+        'Source': 'https://github.com/theonlyamos/runit',
         'Tracker': 'https://github.com/theonlyamos/runit/issues',
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

