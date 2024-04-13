# Comparing `tmp/rack-0.0.1.tar.gz` & `tmp/rack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rack-0.0.1.tar", last modified: Fri Apr  4 17:02:18 2014, max compression
+gzip compressed data, was "rack-0.0.2.tar", last modified: Sat Apr 13 05:28:37 2024, max compression
```

## Comparing `rack-0.0.1.tar` & `rack-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-04-04 17:02:18.000000 rack-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-04-04 17:02:18.000000 rack-0.0.1/rack/
--rwxrwxrwx   0 thom      (1000) thom      (1000)       38 2014-04-04 16:56:23.000000 rack-0.0.1/rack/rack
--rw-rw-rw-   0 thom      (1000) thom      (1000)       32 2014-04-04 16:45:04.000000 rack-0.0.1/rack/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2014-04-04 17:02:18.000000 rack-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      265 2014-04-04 17:02:18.000000 rack-0.0.1/PKG-INFO
--rw-rw-r--   0 thom      (1000) thom      (1000)      365 2014-04-04 16:57:10.000000 rack-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2014-04-04 17:02:18.000000 rack-0.0.1/rack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      265 2014-04-04 17:02:16.000000 rack-0.0.1/rack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2014-04-04 17:02:16.000000 rack-0.0.1/rack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2014-04-04 17:02:16.000000 rack-0.0.1/rack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      174 2014-04-04 17:02:16.000000 rack-0.0.1/rack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2014-04-04 16:57:20.000000 rack-0.0.1/rack.egg-info/not-zip-safe
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:28:37.778361 rack-0.0.2/
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        0 2024-04-13 01:18:37.000000 rack-0.0.2/LICENSE
+-rw-r--r--   0 cJ        (1000) cJ        (1000)      696 2024-04-13 05:28:37.778361 rack-0.0.2/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      202 2024-04-13 05:28:30.000000 rack-0.0.2/README.rst
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      108 2024-04-13 00:59:20.000000 rack-0.0.2/__init__.py
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      584 2024-04-13 05:27:02.000000 rack-0.0.2/pyproject.toml
+drwxrwxr-x   0 cJ        (1000) cJ        (1000)        0 2024-04-13 05:28:37.778361 rack-0.0.2/rack.egg-info/
+-rw-r--r--   0 cJ        (1000) cJ        (1000)      696 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/PKG-INFO
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      168 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        1 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)        5 2024-04-13 05:28:37.000000 rack-0.0.2/rack.egg-info/top_level.txt
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)       38 2024-04-13 05:28:37.778361 rack-0.0.2/setup.cfg
+-rw-rw-r--   0 cJ        (1000) cJ        (1000)      425 2024-04-13 05:25:37.000000 rack-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

