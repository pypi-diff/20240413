# Comparing `tmp/QuartzFramework-0.2.tar.gz` & `tmp/QuartzFramework-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuartzFramework-0.2.tar", last modified: Fri Apr 12 09:29:24 2024, max compression
+gzip compressed data, was "QuartzFramework-0.3.tar", last modified: Sat Apr 13 05:14:13 2024, max compression
```

## Comparing `QuartzFramework-0.2.tar` & `QuartzFramework-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:29:24.381589 QuartzFramework-0.2/
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-12 09:29:24.381589 QuartzFramework-0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:29:24.381589 QuartzFramework-0.2/QuartzFramework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-12 09:29:24.000000 QuartzFramework-0.2/QuartzFramework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      206 2024-04-12 09:29:24.000000 QuartzFramework-0.2/QuartzFramework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:29:24.000000 QuartzFramework-0.2/QuartzFramework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-12 09:29:24.000000 QuartzFramework-0.2/QuartzFramework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-12 09:29:24.000000 QuartzFramework-0.2/QuartzFramework.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 09:29:24.381589 QuartzFramework-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-12 09:29:12.000000 QuartzFramework-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:14:13.094982 QuartzFramework-0.3/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-13 05:14:13.094982 QuartzFramework-0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:14:13.094982 QuartzFramework-0.3/QuartzFramework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-13 05:14:13.000000 QuartzFramework-0.3/QuartzFramework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-13 05:14:13.000000 QuartzFramework-0.3/QuartzFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 05:14:13.000000 QuartzFramework-0.3/QuartzFramework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-13 05:14:13.000000 QuartzFramework-0.3/QuartzFramework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-13 05:14:13.000000 QuartzFramework-0.3/QuartzFramework.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 05:14:13.094982 QuartzFramework-0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-13 05:14:09.000000 QuartzFramework-0.3/setup.py
```

