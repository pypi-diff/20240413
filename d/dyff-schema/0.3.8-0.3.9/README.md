# Comparing `tmp/dyff-schema-0.3.8.tar.gz` & `tmp/dyff_schema-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-schema-0.3.8.tar", last modified: Thu Apr 11 02:11:16 2024, max compression
+gzip compressed data, was "dyff_schema-0.3.9.tar", last modified: Sat Apr 13 18:44:26 2024, max compression
```

## Comparing `dyff-schema-0.3.8.tar` & `dyff_schema-0.3.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.320656 dyff-schema-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-11 02:11:16.320656 dyff-schema-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.306656 dyff-schema-0.3.8/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.312656 dyff-schema-0.3.8/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.314656 dyff-schema-0.3.8/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.314656 dyff-schema-0.3.8/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.314656 dyff-schema-0.3.8/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.316656 dyff-schema-0.3.8/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.317656 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.318656 dyff-schema-0.3.8/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    55483 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.320656 dyff-schema-0.3.8/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-11 02:11:16.000000 dyff-schema-0.3.8/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-11 02:11:16.000000 dyff-schema-0.3.8/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:11:16.000000 dyff-schema-0.3.8/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-11 02:11:16.000000 dyff-schema-0.3.8/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-11 02:11:16.000000 dyff-schema-0.3.8/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:11:16.321656 dyff-schema-0.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:11:16.319656 dyff-schema-0.3.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-11 02:11:10.000000 dyff-schema-0.3.8/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.570580 dyff_schema-0.3.9/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.577580 dyff_schema-0.3.9/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.578580 dyff_schema-0.3.9/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.578580 dyff_schema-0.3.9/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.579580 dyff_schema-0.3.9/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.580580 dyff_schema-0.3.9/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.582580 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.582580 dyff_schema-0.3.9/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    56247 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-13 18:44:26.000000 dyff_schema-0.3.9/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 18:44:26.584580 dyff_schema-0.3.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 18:44:26.583580 dyff_schema-0.3.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-13 18:44:20.000000 dyff_schema-0.3.9/tests/test_import.py
```

### Comparing `dyff-schema-0.3.8/.gitlab-ci.yml` & `dyff_schema-0.3.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/.pre-commit-config.yaml` & `dyff_schema-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/.secrets.baseline` & `dyff_schema-0.3.9/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/CODE_OF_CONDUCT.md` & `dyff_schema-0.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/LICENSE` & `dyff_schema-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/PKG-INFO` & `dyff_schema-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.8
+Version: 0.3.9
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.8/README.md` & `dyff_schema-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/__init__.py` & `dyff_schema-0.3.9/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/copydoc.py` & `dyff_schema-0.3.9/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/ids.py` & `dyff_schema-0.3.9/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/quantity.py` & `dyff_schema-0.3.9/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/base.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1328,24 +1328,42 @@
 
 
 class ForeignMethod(DyffModelWithID, MethodBase):
     pass
 
 
 class AnalysisScope(DyffSchemaBaseModel):
-    dataset: Optional[str]
-    inferenceService: Optional[str]
-    evaluation: Optional[str]
-    model: Optional[str]
+    """The specific entities to which the analysis applies.
+
+    When applying an InferenceService-scoped Method, at least
+    ``.inferenceService`` must be set.
+
+    When applying an Evaluation-scoped Method, at least ``.evaluation``,
+    ``.inferenceService``, and ``.dataset`` must be set.
+    """
+
+    dataset: Optional[str] = pydantic.Field(
+        default=None, description="The Dataset to which the analysis applies."
+    )
+    inferenceService: Optional[str] = pydantic.Field(
+        default=None, description="The InferenceService to which the analysis applies."
+    )
+    evaluation: Optional[str] = pydantic.Field(
+        default=None, description="The Evaluation to which the analysis applies."
+    )
+    model: Optional[str] = pydantic.Field(
+        default=None, description="The Model to which the analysis applies."
+    )
 
 
 class AnalysisBase(DyffSchemaBaseModel):
     scope: AnalysisScope = pydantic.Field(
+        default_factory=AnalysisScope,
         description="The specific entities to which the analysis results apply."
-        " At a minimum, the field corresponding to method.scope must be set."
+        " At a minimum, the field corresponding to method.scope must be set.",
     )
 
     arguments: list[AnalysisArgument] = pydantic.Field(
         default_factory=list,
         description="Arguments to pass to the Method implementation.",
     )
```

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/requests.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff/schema/v0/r1/test.py` & `dyff_schema-0.3.9/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.3.9/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.3.8
+Version: 0.3.9
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-schema-0.3.8/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.3.9/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/pyproject.toml` & `dyff_schema-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff-schema-0.3.8/tests/test_import.py` & `dyff_schema-0.3.9/tests/test_import.py`

 * *Files identical despite different names*

