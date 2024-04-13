# Comparing `tmp/wansuite-2.0.tar.gz` & `tmp/wansuite-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wansuite-2.0.tar", last modified: Sat Apr 13 07:09:03 2024, max compression
+gzip compressed data, was "dist\wansuite-2.2.tar", last modified: Sat Apr 13 08:47:40 2024, max compression
```

## Comparing `wansuite-2.0.tar` & `wansuite-2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 07:09:03.806493 wansuite-2.0/
--rw-rw-rw-   0        0        0       94 2024-04-13 07:09:03.805492 wansuite-2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 07:09:03.806493 wansuite-2.0/setup.cfg
--rw-rw-rw-   0        0        0      156 2024-04-13 07:03:17.000000 wansuite-2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:09:03.800494 wansuite-2.0/wansuite/
--rw-rw-rw-   0        0        0       84 2024-03-31 04:27:38.000000 wansuite-2.0/wansuite/__init__.py
--rw-rw-rw-   0        0        0    13166 2023-04-03 00:00:42.000000 wansuite-2.0/wansuite/investing.py
--rw-rw-rw-   0        0        0       89 2023-02-10 12:37:51.000000 wansuite-2.0/wansuite/iofile.py
--rw-rw-rw-   0        0        0     3659 2024-03-07 16:43:29.000000 wansuite-2.0/wansuite/msql.py
--rw-rw-rw-   0        0        0      145 2024-03-08 01:38:27.000000 wansuite-2.0/wansuite/sys.py
--rw-rw-rw-   0        0        0      397 2023-02-08 13:29:16.000000 wansuite-2.0/wansuite/wtime.py
-drwxrwxrwx   0        0        0        0 2024-04-13 07:09:03.804494 wansuite-2.0/wansuite.egg-info/
--rw-rw-rw-   0        0        0       94 2024-04-13 07:09:03.000000 wansuite-2.0/wansuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-13 07:09:03.000000 wansuite-2.0/wansuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 07:09:03.000000 wansuite-2.0/wansuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 07:09:03.000000 wansuite-2.0/wansuite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 08:47:40.000000 wansuite-2.2/
+-rw-rw-rw-   0        0        0      213 2024-04-13 08:47:40.000000 wansuite-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 08:47:40.000000 wansuite-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      155 2024-04-13 08:47:28.000000 wansuite-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite/
+-rw-rw-rw-   0        0        0      195 2024-04-13 08:41:34.000000 wansuite-2.2/wansuite/__init__.py
+-rw-rw-rw-   0        0        0    13166 2023-04-03 00:00:42.000000 wansuite-2.2/wansuite/investing.py
+-rw-rw-rw-   0        0        0       89 2023-02-10 12:37:51.000000 wansuite-2.2/wansuite/iofile.py
+-rw-rw-rw-   0        0        0     3659 2024-03-07 16:43:29.000000 wansuite-2.2/wansuite/msql.py
+-rw-rw-rw-   0        0        0      145 2024-03-08 01:38:27.000000 wansuite-2.2/wansuite/sys.py
+-rw-rw-rw-   0        0        0      397 2023-02-08 13:29:16.000000 wansuite-2.2/wansuite/wtime.py
+drwxrwxrwx   0        0        0        0 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 08:47:40.000000 wansuite-2.2/wansuite.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `wansuite-2.0/wansuite/investing.py` & `wansuite-2.2/wansuite/investing.py`

 * *Files identical despite different names*

### Comparing `wansuite-2.0/wansuite/msql.py` & `wansuite-2.2/wansuite/msql.py`

 * *Files identical despite different names*

