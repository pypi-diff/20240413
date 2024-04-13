# Comparing `tmp/jxtr-2.0.2.tar.gz` & `tmp/jxtr-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jxtr-2.0.2.tar", last modified: Sat Dec 28 22:37:42 2019, max compression
+gzip compressed data, was "jxtr-2.1.5.tar", last modified: Sat Apr 13 21:07:18 2024, max compression
```

## Comparing `jxtr-2.0.2.tar` & `jxtr-2.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-28 22:37:42.000000 jxtr-2.0.2/
--rw-r--r--   0 root         (0) root         (0)       79 2019-12-28 22:37:42.000000 jxtr-2.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-28 22:37:42.000000 jxtr-2.0.2/jxtr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      194 2019-12-28 22:37:41.000000 jxtr-2.0.2/jxtr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        5 2019-12-28 22:37:41.000000 jxtr-2.0.2/jxtr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-28 22:37:41.000000 jxtr-2.0.2/jxtr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-12-28 22:37:41.000000 jxtr-2.0.2/jxtr.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      280 2019-12-28 22:37:41.000000 jxtr-2.0.2/jxtr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2698 2019-12-28 22:25:27.000000 jxtr-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-28 22:37:42.000000 jxtr-2.0.2/jxtr/
--rw-r--r--   0 root         (0) root         (0)     8811 2019-12-28 22:23:07.000000 jxtr-2.0.2/jxtr/t.py
--rw-r--r--   0 root         (0) root         (0)       15 2019-12-28 22:23:07.000000 jxtr-2.0.2/jxtr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      575 2019-12-28 22:37:33.000000 jxtr-2.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      280 2019-12-28 22:37:42.000000 jxtr-2.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:07:18.305047 jxtr-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-13 21:07:18.305047 jxtr-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-13 21:07:07.000000 jxtr-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:07:18.301047 jxtr-2.1.5/jxtr/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 21:07:07.000000 jxtr-2.1.5/jxtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-13 21:07:07.000000 jxtr-2.1.5/jxtr/t.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:07:18.305047 jxtr-2.1.5/jxtr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-13 21:07:18.000000 jxtr-2.1.5/jxtr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 21:07:18.000000 jxtr-2.1.5/jxtr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:07:18.000000 jxtr-2.1.5/jxtr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:07:18.000000 jxtr-2.1.5/jxtr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 21:07:18.000000 jxtr-2.1.5/jxtr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 21:07:18.305047 jxtr-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-13 21:07:07.000000 jxtr-2.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jxtr-2.0.2/README.md` & `jxtr-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jxtr-2.0.2/jxtr/t.py` & `jxtr-2.1.5/jxtr/t.py`

 * *Files identical despite different names*

