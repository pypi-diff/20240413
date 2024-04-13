# Comparing `tmp/siggen-2.0.20231009.tar.gz` & `tmp/siggen-2.1.20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siggen-2.0.20231009.tar", last modified: Mon Oct  9 15:05:21 2023, max compression
+gzip compressed data, was "siggen-2.1.20240412.tar", last modified: Sat Apr 13 02:53:29 2024, max compression
```

## Comparing `siggen-2.0.20231009.tar` & `siggen-2.1.20240412.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2023-04-18 15:20:01.000000 siggen-2.0.20231009/CODE_OF_CONDUCT.md
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    19353 2023-10-09 15:04:36.000000 siggen-2.0.20231009/HISTORY.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2023-04-18 15:20:01.000000 siggen-2.0.20231009/LICENSE
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      265 2023-04-18 16:10:15.000000 siggen-2.0.20231009/MANIFEST.in
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      722 2023-04-18 15:43:39.000000 siggen-2.0.20231009/Makefile
--rw-r--r--   0 willkg    (1000) willkg    (1000)    12032 2023-10-09 15:05:21.731248 siggen-2.0.20231009/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    10971 2023-10-09 15:04:36.000000 siggen-2.0.20231009/README.rst
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/bin/
--rwxrwxr-x   0 willkg    (1000) willkg    (1000)      516 2023-04-18 15:20:01.000000 siggen-2.0.20231009/bin/run_cmd_tests.sh
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1054 2023-10-03 17:33:57.000000 siggen-2.0.20231009/pyproject.toml
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      165 2023-10-09 15:04:36.000000 siggen-2.0.20231009/requirements-dev.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2023-10-09 15:05:21.731248 siggen-2.0.20231009/setup.cfg
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2098 2023-10-03 17:33:57.000000 siggen-2.0.20231009/setup.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/siggen/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      276 2023-10-09 15:04:36.000000 siggen-2.0.20231009/siggen/__init__.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2863 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/cmd_doc.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4452 2023-04-18 15:20:01.000000 siggen-2.0.20231009/siggen/cmd_fetch_data.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8348 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/cmd_signature.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1939 2023-04-18 15:20:01.000000 siggen-2.0.20231009/siggen/cmd_signify.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4684 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/generator.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     3924 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/pipeline.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    40097 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/rules.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8905 2023-10-09 15:04:36.000000 siggen-2.0.20231009/siggen/schema.rst
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/siggen/siglists/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     6836 2023-04-18 15:20:01.000000 siggen-2.0.20231009/siggen/siglists/README.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     6522 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/siglists/irrelevant_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4998 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/siglists/prefix_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1095 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/siglists/signature_sentinels.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      241 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/siglists/signatures_with_line_numbers_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      702 2023-04-18 15:20:01.000000 siggen-2.0.20231009/siggen/siglists/trim_dll_signature_re.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2941 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/siglists_utils.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       40 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/socorro_sha.txt
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/siggen/tests/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      200 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/__init__.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/siggen/tests/siglists/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/siglists/test-invalid-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/siglists/test-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      108 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/siglists/test-valid-sig-list.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    77931 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/tests/test_rules.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2056 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/test_siglists.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2234 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/test_signature_generator.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    14493 2023-10-09 14:29:34.000000 siggen-2.0.20231009/siggen/tests/test_utils.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    13243 2023-10-09 14:43:50.000000 siggen-2.0.20231009/siggen/utils.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-10-09 15:05:21.731248 siggen-2.0.20231009/siggen.egg-info/
--rw-r--r--   0 willkg    (1000) willkg    (1000)    12032 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1093 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/SOURCES.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/dependency_links.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      130 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/entry_points.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       43 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/requires.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        7 2023-10-09 15:05:21.000000 siggen-2.0.20231009/siggen.egg-info/top_level.txt
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.455435 siggen-2.1.20240412/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2023-04-18 15:20:01.000000 siggen-2.1.20240412/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    20073 2024-04-13 02:52:42.000000 siggen-2.1.20240412/HISTORY.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2023-04-18 15:20:01.000000 siggen-2.1.20240412/LICENSE
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      220 2024-04-13 02:46:11.000000 siggen-2.1.20240412/MANIFEST.in
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      808 2024-04-13 01:33:47.000000 siggen-2.1.20240412/Makefile
+-rw-r--r--   0 willkg    (1000) willkg    (1000)    12526 2024-04-13 02:53:29.455435 siggen-2.1.20240412/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    10971 2023-10-09 15:04:36.000000 siggen-2.1.20240412/README.rst
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.451435 siggen-2.1.20240412/bin/
+-rwxrwxr-x   0 willkg    (1000) willkg    (1000)      516 2023-04-18 15:20:01.000000 siggen-2.1.20240412/bin/run_cmd_tests.sh
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2549 2024-04-13 02:52:42.000000 siggen-2.1.20240412/pyproject.toml
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2024-04-13 02:53:29.455435 siggen-2.1.20240412/setup.cfg
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.451435 siggen-2.1.20240412/siggen/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      404 2024-04-13 02:46:11.000000 siggen-2.1.20240412/siggen/__init__.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2863 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/cmd_doc.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4466 2024-04-13 01:33:47.000000 siggen-2.1.20240412/siggen/cmd_fetch_data.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8348 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/cmd_signature.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1939 2023-04-18 15:20:01.000000 siggen-2.1.20240412/siggen/cmd_signify.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4684 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/generator.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     3924 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/pipeline.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    40097 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/rules.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8905 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/schema.rst
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.455435 siggen-2.1.20240412/siggen/siglists/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     6836 2023-04-18 15:20:01.000000 siggen-2.1.20240412/siggen/siglists/README.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     6639 2024-04-13 01:23:19.000000 siggen-2.1.20240412/siggen/siglists/irrelevant_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     5145 2024-04-13 01:23:19.000000 siggen-2.1.20240412/siggen/siglists/prefix_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1095 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/siglists/signature_sentinels.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      241 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/siglists/signatures_with_line_numbers_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      702 2023-04-18 15:20:01.000000 siggen-2.1.20240412/siggen/siglists/trim_dll_signature_re.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     3106 2024-04-13 01:23:19.000000 siggen-2.1.20240412/siggen/siglists_utils.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       40 2024-04-13 01:23:19.000000 siggen-2.1.20240412/siggen/socorro_sha.txt
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.455435 siggen-2.1.20240412/siggen/tests/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      200 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/__init__.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.455435 siggen-2.1.20240412/siggen/tests/siglists/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/siglists/test-invalid-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       77 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/siglists/test-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      108 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/siglists/test-valid-sig-list.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    77931 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/test_rules.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2056 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/test_siglists.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2234 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/test_signature_generator.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    14493 2024-04-13 01:14:12.000000 siggen-2.1.20240412/siggen/tests/test_utils.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    13243 2024-04-13 01:23:19.000000 siggen-2.1.20240412/siggen/utils.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-13 02:53:29.455435 siggen-2.1.20240412/siggen.egg-info/
+-rw-r--r--   0 willkg    (1000) willkg    (1000)    12526 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1063 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/SOURCES.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/dependency_links.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      130 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/entry_points.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      152 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/requires.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        7 2024-04-13 02:53:29.000000 siggen-2.1.20240412/siggen.egg-info/top_level.txt
```

### Comparing `siggen-2.0.20231009/CODE_OF_CONDUCT.md` & `siggen-2.1.20240412/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/HISTORY.rst` & `siggen-2.1.20240412/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 =======
 History
 =======
 
+2.1.20240412 (April 12th, 2024)
+===============================
+
+Bug fixes:
+
+* bug-1889120: add Rust sub-slice access frames to prefix signature list
+* Bug 1885351 - Add ``nsCOMPtr<T>:: and nsMaybeWeakPtr<T>::`` to the irrelevant signature list.
+* Bug 1884689 - Add ``nsDocShell::GetBrowsingContext`` to the prefix list.
+* Bug 1882088 - Move ``nsTArray`` OOM things to the irrelevant list.
+* bug-1850981: update to python 3.11
+* bug-1876623: Treat ``<.plt ELF section...>`` as prefix signature
+* bug-1799125: switch from ``urlparse`` from ``urllib.parse`` to ``urlsplit``
+* Bug 1866857 - Ignore ``mozilla::Monitor::Lock`` when generating crash signatures
+* Bug 1862460 - Add ``mozilla::Vector<T>`` to the prefix list.
+
+
 2.0.20231009 (October 9th, 2023)
 ================================
 
 Big changes:
 
 * bug 1847429: implement signature generation for ``JavaException``
 * Drop support for Python 3.7 (#109)
```

### Comparing `siggen-2.0.20231009/LICENSE` & `siggen-2.1.20240412/LICENSE`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/Makefile` & `siggen-2.1.20240412/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 .PHONY: clean
 clean:  ## Clean build artifacts
 	rm -rf build dist ${PROJECT}.egg-info .tox .pytest-cache
 	rm -rf docs/_build/*
 	find ${PROJECT}/ tests/ -name __pycache__ | xargs rm -rf
 	find ${PROJECT}/ tests/ -name '*.pyc' | xargs rm -rf
 
+.PHONY: format
+format:  ## Format Python files
+	tox exec -e py39-lint -- ruff format
+
 .PHONY: lint
 lint:  ## Lint files
 	tox -e py39-lint
 
 .PHONY: test
 test:  ## Run tests
 	tox
```

### Comparing `siggen-2.0.20231009/PKG-INFO` & `siggen-2.1.20240412/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: siggen
-Version: 2.0.20231009
-Summary: Experimental extraction of Socorro signature generation
-Home-page: https://github.com/willkg/socorro-siggen
-Maintainer: Will Kahn-Greene
-Maintainer-email: willkg@mozilla.com
-License: Mozilla Public License v2
+Version: 2.1.20240412
+Summary: Socorro signature generation extracted as a Python library
+Author: Will Kahn-Greene
+License: MPLv2
+Project-URL: Homepage, https://github.com/willkg/socorro-siggen
+Project-URL: Source, https://github.com/willkg/socorro-siggen
+Project-URL: Issues, https://github.com/willkg/socorro-siggen
+Keywords: socorro
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: glom
-Requires-Dist: importlib_resources
+Requires-Dist: importlib_resources; python_version < "3.9"
 Provides-Extra: cli
 Requires-Dist: requests<3; extra == "cli"
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: requests<3; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-gh-actions; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
 ==============
 socorro-siggen
 ==============
 
 This is an extraction of the Socorro crash signature generation code.
```

### Comparing `siggen-2.0.20231009/README.rst` & `siggen-2.1.20240412/README.rst`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/bin/run_cmd_tests.sh` & `siggen-2.1.20240412/bin/run_cmd_tests.sh`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/setup.py` & `siggen-2.1.20240412/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,112 @@
-#!/usr/bin/env python
-
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-import codecs
-import os
-import re
-
-from setuptools import setup, find_packages
-
-
-def get_long_desc():
-    return codecs.open("README.rst", encoding="utf-8").read()
-
-
-def get_version():
-    fn = os.path.join("siggen", "__init__.py")
-    vsre = r"""^__version__ = ['"]([^'"]*)['"]"""
-    version_file = codecs.open(fn, mode="r", encoding="utf-8").read()
-    return re.search(vsre, version_file, re.M).group(1)
-
-
-INSTALL_REQUIRES = [
+[project]
+name = "siggen"
+description = "Socorro signature generation extracted as a Python library"
+# x.y.YYYYMMDD or x.y.YYYYMMDD.dev0 -- calver
+version = "2.1.20240412"
+readme = "README.rst"
+keywords = ["socorro"]
+authors = [{name = "Will Kahn-Greene"}]
+license = {text = "MPLv2"}
+requires-python = ">=3.8"
+dependencies = [
     "glom",
-    "importlib_resources",
+    "importlib_resources; python_version < '3.9'",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+urls.Homepage = "https://github.com/willkg/socorro-siggen"
+urls.Source = "https://github.com/willkg/socorro-siggen"
+urls.Issues = "https://github.com/willkg/socorro-siggen"
+
+[project.scripts]
+signify = "siggen.cmd_signify:main"
+fetch-data = "siggen.cmd_fetch_data:main"
+signature = "siggen.cmd_signature:main"
+
+[project.optional-dependencies]
+cli = [
+    "requests<3",
 ]
-EXTRAS_REQUIRE = {
-    "cli": [
-        "requests<3",
-    ],
-}
-
-
-setup(
-    name="siggen",
-    version=get_version(),
-    description="Experimental extraction of Socorro signature generation",
-    long_description=get_long_desc(),
-    long_description_content_type="text/x-rst",
-    maintainer="Will Kahn-Greene",
-    maintainer_email="willkg@mozilla.com",
-    url="https://github.com/willkg/socorro-siggen",
-    license="Mozilla Public License v2",
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=INSTALL_REQUIRES,
-    extras_require=EXTRAS_REQUIRE,
-    python_requires=">=3.8",
-    entry_points="""
-        [console_scripts]
-        signify=siggen.cmd_signify:main
-        fetch-data=siggen.cmd_fetch_data:main
-        signature=siggen.cmd_signature:main
-    """,
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-)
+dev = [
+    "build",
+    "check-manifest",
+    "pytest",
+    "requests<3",
+    "ruff",
+    "tox",
+    "tox-gh-actions",
+    "twine",
+    "wheel",
+]
+
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+
+[tool.ruff]
+line-length = 88
+target-version = "py38"
+src = ["setup.py", "siggen"]
+
+[tool.ruff.lint]
+# Enable pycodestyle (E), pyflakes (F), and bugbear (B) rules
+select = ["E", "F", "B"]
+ignore = ["E501"]
+
+[tool.ruff.lint.flake8-quotes]
+docstring-quotes = "double"
+
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = True
+envlist =
+    py38
+    py39
+    py310
+    py311
+    py312
+    py39-lint
+    py39-norequests
+
+[gh-actions]
+python =
+    3.8: py38
+    3.9: py39, py39-lint, py39-norequests
+    3.10: py310
+    3.11: py311
+    3.12: py312
+
+[testenv]
+extras = dev,cli
+allowlist_externals = {toxinidir}/bin/run_cmd_tests.sh
+commands = 
+    pytest {posargs}
+    {toxinidir}/bin/run_cmd_tests.sh
+
+[testenv:py39-lint]
+extras = dev,cli
+commands =
+    ruff format --check siggen
+    ruff check siggen
+
+[testenv:py39-norequests]
+extras =
+install_command = pip install {packages}
+allowlist_externals = {toxinidir}/bin/run_cmd_tests.sh
+commands =
+    {toxinidir}/bin/run_cmd_tests.sh --no-requests
+"""
```

### Comparing `siggen-2.0.20231009/siggen/cmd_doc.py` & `siggen-2.1.20240412/siggen/cmd_doc.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/cmd_fetch_data.py` & `siggen-2.1.20240412/siggen/cmd_fetch_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import json
 import os
 import sys
 
 try:
     import requests
 except ImportError:
-    print("Error importing requests. You need to install the cli extras.", file=sys.stderr)
+    print(
+        "Error importing requests. You need to install the cli extras.", file=sys.stderr
+    )
     print("Try: pip install 'siggen[cli]'", file=sys.stderr)
     sys.exit(1)
 
 from .utils import convert_to_crash_data
 
 
 class WrappedTextHelpFormatter(argparse.HelpFormatter):
```

### Comparing `siggen-2.0.20231009/siggen/cmd_signature.py` & `siggen-2.1.20240412/siggen/cmd_signature.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/cmd_signify.py` & `siggen-2.1.20240412/siggen/cmd_signify.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/generator.py` & `siggen-2.1.20240412/siggen/generator.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/pipeline.rst` & `siggen-2.1.20240412/siggen/pipeline.rst`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/rules.py` & `siggen-2.1.20240412/siggen/rules.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/schema.rst` & `siggen-2.1.20240412/siggen/schema.rst`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/siglists/README.rst` & `siggen-2.1.20240412/siggen/siglists/README.rst`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/siglists/irrelevant_signature_re.txt` & `siggen-2.1.20240412/siggen/siglists/irrelevant_signature_re.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 mach_msg_trap
 __memcmp
 __memcpy
 __memmove
 __memset
 mnt@asec@org\.mozilla\.f.*\.apk@classes\.dex@0x
 MOZ_Crash
+mozalloc_abort
 mozalloc_handle_oom
 mozglue_static::oom_hook::hook
 mozglue_static::panic_hook
 mozcrt19.dll@0x
 mozilla::AlignedBuffer<T>::Data
 mozilla::ArrayIterator<T>
 mozilla::Atomic<T>::Atomic
@@ -131,14 +132,15 @@
 mozilla::dom::ThreadSafeRequestHandle::GetContext
 mozilla::gfx::Log<
 mozilla::ipc::IPDLParamTraits<T>::Write
 mozilla::ipc::WriteIPDLParam
 mozilla::HashMap
 mozilla::HashSet
 mozilla::MediaRawData::Data
+mozilla::Monitor::Lock
 mozilla::Monitor::Wait
 mozilla::MozPromiseHolderBase
 mozilla::MozPromiseRefcountable::Release
 mozilla::MozPromiseRequestHolder<T>::Track
 mozilla::MozPromise<T>::AssertIsDead
 mozilla::MozPromise<T>::~MozPromise
 mozilla::MozPromise<T>::Private
@@ -160,20 +162,25 @@
 mozilla::TaskController::GetRunnableForMTTask
 mozilla::TaskQueue::
 mozilla::ThreadEventQueue
 mozilla::ThreadSafeAutoRefCnt
 mozilla::UniquePtr
 mozilla::widget::WlCrashHandler
 mozilla::wr::RenderThread::AddRef
-nsCOMPtr<T>::~nsCOMPtr
+moz_xmalloc
+moz_xrealloc
+nsCOMPtr<T>::
 nsCOMPtr_base::~nsCOMPtr_base
+nsMaybeWeakPtr<T>::
 nsQueryObject<T>::operator
 nsRunnableMethodReceiver<T>::nsRunnableMethodReceiver
 ns.*Hashtable
 nsTArrayElementTraits
+nsTArrayInfallibleAllocator
+nsTArray_base<
 nsThread::GetEvent
 nsThread::ProcessNextEvent
 NS_ProcessNextEvent
 (Nt|Zw)?WaitForKeyedEvent
 (Nt|Zw)?WaitForSingleObject(Ex)?
 (Nt|Zw)?WaitForMultipleObjects(Ex)?
 (Nt|Zw)?WaitForAlertByThreadId
```

### Comparing `siggen-2.0.20231009/siggen/siglists/prefix_signature_re.txt` & `siggen-2.1.20240412/siggen/siglists/prefix_signature_re.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 CleanupPerAppKey
 core::ops::function::Fn::call<T>
 core::option::expect_failed
 core::option::expect_none_failed
 core::ptr::drop_in_place
 core::ptr::real_drop_in_place
 core::result::unwrap_failed
+<core::ops::range::Range<usize> as core::slice::index::SliceIndex<\[T\]>>::index
+core::slice::index::<impl core::ops::index::Index<I> for \[T\]>::index
 core::str::slice_error_fail
 CreateFileMappingA
 __cxxabiv1::failed_throw
 CxxThrowException
 __delayLoadHelper2
 dlmalloc
 dvm
@@ -61,14 +63,15 @@
 gsignal
 handle_response
 HandleInvalidParameter
 hashbrown::raw::Fallibility::alloc_err
 hashbrown::raw::RawTable<T>::new_uninitialized<T>
 HeapFree
 huge_dalloc
+InfallibleAllocPolicy
 InvalidArrayIndex_CRASH
 invalid_parameter_noinfo
 _invalid_parameter_noinfo
 je_
 _JNIEnv
 js::AutoEnterOOMUnsafeRegion::crash
 js::LifoAlloc::getOrCreateChunk
@@ -88,16 +91,14 @@
 _MD_
 memcmp
 memcpy
 memmove
 memset
 MessageLoop::PostTask_Helper
 MessageLoop::PostTask
-mozalloc_abort
-mozalloc_handle_oom
 moz_malloc_size_of
 mozilla::CheckCheckedUnsafePtrs<T>::Check
 mozilla::CheckedInt
 mozilla::detail::InvalidArrayIndex_CRASH
 mozilla::detail::nsTStringRepr<T>::
 mozilla::dom::AutoJSAPI::Init
 mozilla::dom::Promise::
@@ -121,61 +122,60 @@
 mozilla::ipc::RPCChannel::CxxStackFrame::CxxStackFrame
 mozilla::ipc::SentinelReadError
 mozilla::ipc::Shmem::OpenExisting
 mozilla::ipc::IProtocol::ChannelSend
 mozilla::ipc::IToplevelProtocol::ShmemCreated
 mozilla::layers::CompositorD3D11::Failed
 mozilla::SpinEventLoopUntil
+mozilla::Vector<T>
 mozilla::WrapNotNull<
 mozilla.*FatalError
-moz_xmalloc
-moz_xrealloc
 MOZ_CrashPrintf
 msvcr120\.dll@0x
 \<name omitted\>
 new\[\]
 NP_Shutdown
 (NS_)?(Lossy)?(Copy|Append|Convert).*UTF
 NS_CycleCollectorSuspect3
 -\[NSApplication _crashOnException:\]
 nsCRT::strcmp
 -\[NSObject doesNotRecognizeSelector:\]
-nsTArrayInfallibleAllocator
 NS_strcmp
 NS_strlen
 nsCOMPtr
 NS_ABORT_OOM
 NS_DebugBreak
 nsDebugImpl::Abort
+nsDocShell::GetBrowsingContext
 nsINode::GetParentNode
 nsThread::GetEvent
 [-+]\[NSException raise(:format:(arguments:)?)?\]
 nsINode::Slots
 nsObserverService
 nsTSubstring<.*>::
 NS_QuickSort
 NSS
 nss
 nsStringBuffer::
 nsTArray<
-nsTArray_base<
 nsTArray_Impl<
 nsThread::Shutdown
 NtUser
 objc_exception_rethrow
 objc_exception_throw
 objc_addExceptionHandler
 objc_msgSend
 objc_release
 objc_retain
 operator new
 o_strcat_s
 <.*>::operator()
 pages_commit
 PL_
+<\.plt ELF section in .*>
 port_
 PORT_
 _PR_
 PR_
 .*ProcessNextEvent
 pthread_cond_signal_thread_np
 pthread_mutex_lock
```

### Comparing `siggen-2.0.20231009/siggen/siglists/signature_sentinels.txt` & `siggen-2.1.20240412/siggen/siglists/signature_sentinels.txt`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/siglists/trim_dll_signature_re.txt` & `siggen-2.1.20240412/siggen/siglists/trim_dll_signature_re.txt`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/siglists_utils.py` & `siggen-2.1.20240412/siggen/siglists_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from pathlib import Path
 import re
 
-import importlib_resources
+# Use importlib_resources if it's there. Otherwise use the built-in version.
+try:
+    import importlib_resources
+except ImportError:
+    from importlib import resources as importlib_resources
 
 
 # This is a hack because sentinels can be a tuple, with the second item being
 # a function to verify if the sentinel applies. It's quite hard to express
 # that in a .txt file, so this special value is here. This list should not
 # grow much, and if it does, we should find a better solution for handling
 # these special values.
```

### Comparing `siggen-2.0.20231009/siggen/tests/test_rules.py` & `siggen-2.1.20240412/siggen/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/tests/test_siglists.py` & `siggen-2.1.20240412/siggen/tests/test_siglists.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/tests/test_signature_generator.py` & `siggen-2.1.20240412/siggen/tests/test_signature_generator.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/tests/test_utils.py` & `siggen-2.1.20240412/siggen/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `siggen-2.0.20231009/siggen/utils.py` & `siggen-2.1.20240412/siggen/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 
 import contextlib
 import copy
 import re
-from urllib.parse import urlparse
+from urllib.parse import urlsplit
 
 from glom import glom, assign
 
 
 def int_or_none(data):
     try:
         return int(data)
@@ -407,15 +407,15 @@
     if is_crash_id_valid(item):
         return item
 
     if item.startswith("bp-") and is_crash_id_valid(item[3:]):
         return item[3:]
 
     if item.startswith("http"):
-        parsed = urlparse(item)
+        parsed = urlsplit(item)
         path = parsed.path
         if path.startswith("/report/index"):
             crash_id = path.split("/")[-1]
             if is_crash_id_valid(crash_id):
                 return crash_id
```

### Comparing `siggen-2.0.20231009/siggen.egg-info/PKG-INFO` & `siggen-2.1.20240412/siggen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 Metadata-Version: 2.1
 Name: siggen
-Version: 2.0.20231009
-Summary: Experimental extraction of Socorro signature generation
-Home-page: https://github.com/willkg/socorro-siggen
-Maintainer: Will Kahn-Greene
-Maintainer-email: willkg@mozilla.com
-License: Mozilla Public License v2
+Version: 2.1.20240412
+Summary: Socorro signature generation extracted as a Python library
+Author: Will Kahn-Greene
+License: MPLv2
+Project-URL: Homepage, https://github.com/willkg/socorro-siggen
+Project-URL: Source, https://github.com/willkg/socorro-siggen
+Project-URL: Issues, https://github.com/willkg/socorro-siggen
+Keywords: socorro
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: glom
-Requires-Dist: importlib_resources
+Requires-Dist: importlib_resources; python_version < "3.9"
 Provides-Extra: cli
 Requires-Dist: requests<3; extra == "cli"
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: requests<3; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-gh-actions; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
 ==============
 socorro-siggen
 ==============
 
 This is an extraction of the Socorro crash signature generation code.
```

### Comparing `siggen-2.0.20231009/siggen.egg-info/SOURCES.txt` & `siggen-2.1.20240412/siggen.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 CODE_OF_CONDUCT.md
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 pyproject.toml
-requirements-dev.txt
-setup.py
 bin/run_cmd_tests.sh
 siggen/__init__.py
 siggen/cmd_doc.py
 siggen/cmd_fetch_data.py
 siggen/cmd_signature.py
 siggen/cmd_signify.py
 siggen/generator.py
```

