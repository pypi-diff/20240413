# Comparing `tmp/masspds2024-0.0.1.tar.gz` & `tmp/masspds2024-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masspds2024-0.0.1.tar", last modified: Sat Apr 13 04:15:36 2024, max compression
+gzip compressed data, was "masspds2024-0.0.2.tar", last modified: Sat Apr 13 04:57:00 2024, max compression
```

## Comparing `masspds2024-0.0.1.tar` & `masspds2024-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 04:15:36.731744 masspds2024-0.0.1/
--rw-rw-rw-   0        0        0      379 2024-04-13 04:15:36.729208 masspds2024-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 04:15:36.728207 masspds2024-0.0.1/masspds2024.egg-info/
--rw-rw-rw-   0        0        0      379 2024-04-13 04:15:36.000000 masspds2024-0.0.1/masspds2024.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2024-04-13 04:15:36.000000 masspds2024-0.0.1/masspds2024.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 04:15:36.000000 masspds2024-0.0.1/masspds2024.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 04:15:36.000000 masspds2024-0.0.1/masspds2024.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 04:15:36.732743 masspds2024-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      493 2024-04-13 04:14:45.000000 masspds2024-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:57:00.949254 masspds2024-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2024-04-13 04:56:25.000000 masspds2024-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      637 2024-04-13 04:57:00.948256 masspds2024-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       79 2024-04-13 04:55:53.000000 masspds2024-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-13 04:55:16.000000 masspds2024-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      755 2024-04-13 04:57:00.952474 masspds2024-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 04:57:00.913415 masspds2024-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 04:57:00.930794 masspds2024-0.0.2/src/data_generation/
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:33:04.000000 masspds2024-0.0.2/src/data_generation/__init__.py
+-rw-rw-rw-   0        0        0     3262 2024-04-13 04:33:15.000000 masspds2024-0.0.2/src/data_generation/data_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-13 04:57:00.945796 masspds2024-0.0.2/src/masspds2024.egg-info/
+-rw-rw-rw-   0        0        0      637 2024-04-13 04:57:00.000000 masspds2024-0.0.2/src/masspds2024.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-13 04:57:00.000000 masspds2024-0.0.2/src/masspds2024.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 04:57:00.000000 masspds2024-0.0.2/src/masspds2024.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-13 04:57:00.000000 masspds2024-0.0.2/src/masspds2024.egg-info/top_level.txt
```

