# Comparing `tmp/wristwatch-1.0.0.tar.gz` & `tmp/wristwatch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wristwatch-1.0.0.tar", last modified: Sat Apr 13 17:57:11 2024, max compression
+gzip compressed data, was "wristwatch-1.0.1.tar", last modified: Sat Apr 13 18:44:01 2024, max compression
```

## Comparing `wristwatch-1.0.0.tar` & `wristwatch-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:57:11.908442 wristwatch-1.0.0/
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.0.0/LICENSE
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      157 2024-04-13 17:57:11.908442 wristwatch-1.0.0/PKG-INFO
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1887 2024-04-13 17:52:50.000000 wristwatch-1.0.0/README.md
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-13 17:57:11.908442 wristwatch-1.0.0/setup.cfg
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      281 2024-04-13 17:46:56.000000 wristwatch-1.0.0/setup.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:57:11.908442 wristwatch-1.0.0/wristwatch/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:46:48.000000 wristwatch-1.0.0/wristwatch/__init__.py
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     7381 2024-04-13 17:40:50.000000 wristwatch-1.0.0/wristwatch/wristwatch.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:57:11.908442 wristwatch-1.0.0/wristwatch.egg-info/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      157 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/PKG-INFO
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/entry_points.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       33 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/requires.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-13 17:57:11.000000 wristwatch-1.0.0/wristwatch.egg-info/top_level.txt
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.0.1/LICENSE
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2091 2024-04-13 18:44:01.316981 wristwatch-1.0.1/PKG-INFO
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1887 2024-04-13 17:52:50.000000 wristwatch-1.0.1/README.md
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-13 18:44:01.316981 wristwatch-1.0.1/setup.cfg
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      480 2024-04-13 18:43:17.000000 wristwatch-1.0.1/setup.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/wristwatch/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:46:48.000000 wristwatch-1.0.1/wristwatch/__init__.py
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     7381 2024-04-13 17:40:50.000000 wristwatch-1.0.1/wristwatch/wristwatch.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/wristwatch.egg-info/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2091 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/entry_points.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       56 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/requires.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/top_level.txt
```

### Comparing `wristwatch-1.0.0/LICENSE` & `wristwatch-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wristwatch-1.0.0/README.md` & `wristwatch-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wristwatch-1.0.0/wristwatch/wristwatch.py` & `wristwatch-1.0.1/wristwatch/wristwatch.py`

 * *Files identical despite different names*

