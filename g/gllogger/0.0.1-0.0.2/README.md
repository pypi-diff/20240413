# Comparing `tmp/gllogger-0.0.1.tar.gz` & `tmp/gllogger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gllogger-0.0.1.tar", last modified: Fri Apr 12 00:36:49 2024, max compression
+gzip compressed data, was "gllogger-0.0.2.tar", last modified: Sat Apr 13 01:58:05 2024, max compression
```

## Comparing `gllogger-0.0.1.tar` & `gllogger-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:36:49.852829 gllogger-0.0.1/
--rw-rw-rw-   0        0        0      282 2024-04-12 00:36:49.852829 gllogger-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      336 2024-04-12 00:36:30.000000 gllogger-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 00:36:49.852829 gllogger-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 00:36:49.837211 gllogger-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 00:36:49.852829 gllogger-0.0.1/src/gllogger.egg-info/
--rw-rw-rw-   0        0        0      282 2024-04-12 00:36:49.000000 gllogger-0.0.1/src/gllogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-04-12 00:36:49.000000 gllogger-0.0.1/src/gllogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:36:49.000000 gllogger-0.0.1/src/gllogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 00:36:49.000000 gllogger-0.0.1/src/gllogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6542 2024-04-12 00:25:25.000000 gllogger-0.0.1/src/gllogger.py
+drwxrwxrwx   0        0        0        0 2024-04-13 01:58:05.660803 gllogger-0.0.2/
+-rw-rw-rw-   0        0        0      282 2024-04-13 01:58:05.659727 gllogger-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-13 01:53:52.000000 gllogger-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 01:58:05.660803 gllogger-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 01:58:05.643017 gllogger-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 01:58:05.658726 gllogger-0.0.2/src/gllogger.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-04-13 01:58:05.000000 gllogger-0.0.2/src/gllogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-04-13 01:58:05.000000 gllogger-0.0.2/src/gllogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 01:58:05.000000 gllogger-0.0.2/src/gllogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 01:58:05.000000 gllogger-0.0.2/src/gllogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17421 2024-04-13 01:53:08.000000 gllogger-0.0.2/src/gllogger.py
```

