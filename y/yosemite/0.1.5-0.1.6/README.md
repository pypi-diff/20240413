# Comparing `tmp/yosemite-0.1.5.tar.gz` & `tmp/yosemite-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yosemite-0.1.5.tar", last modified: Fri Mar 29 03:43:31 2024, max compression
+gzip compressed data, was "yosemite-0.1.6.tar", last modified: Fri Mar 29 09:12:09 2024, max compression
```

## Comparing `yosemite-0.1.5.tar` & `yosemite-0.1.6.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.343238 yosemite-0.1.5/
--rw-r--r--   0 hammad     (501) staff       (20)      735 2024-03-29 03:43:31.342789 yosemite-0.1.5/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      349 2024-03-28 23:00:14.000000 yosemite-0.1.5/README.md
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-03-29 03:43:31.343333 yosemite-0.1.5/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      826 2024-03-29 03:43:21.000000 yosemite-0.1.5/setup.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.307331 yosemite-0.1.5/tests/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.308656 yosemite-0.1.5/tests/__cli__/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/__cli__/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)      493 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/__cli__/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 14:14:15.000000 yosemite-0.1.5/tests/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.310047 yosemite-0.1.5/tests/llms/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/llms/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     6572 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/llms/llm.py
--rw-r--r--   0 hammad     (501) staff       (20)     3066 2024-03-27 16:44:33.000000 yosemite-0.1.5/tests/main.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.313734 yosemite-0.1.5/tests/ml/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    14751 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/database.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.316192 yosemite-0.1.5/tests/ml/legacy/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/legacy/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8677 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/legacy/database.py
--rw-r--r--   0 hammad     (501) staff       (20)     9176 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/legacy/vector_database.py
--rw-r--r--   0 hammad     (501) staff       (20)     3313 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/text.py
--rw-r--r--   0 hammad     (501) staff       (20)    13062 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/ml/transformers.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.317772 yosemite-0.1.5/tests/prehistoric/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/prehistoric/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8992 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/prehistoric/heat.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.322224 yosemite-0.1.5/tests/tools/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/tools/input.py
--rw-r--r--   0 hammad     (501) staff       (20)     2445 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/tools/lightspeed.py
--rw-r--r--   0 hammad     (501) staff       (20)     5243 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/tools/load.py
--rw-r--r--   0 hammad     (501) staff       (20)     5086 2024-03-27 16:43:45.000000 yosemite-0.1.5/tests/tools/text.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.324685 yosemite-0.1.5/yosemite/
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.328811 yosemite-0.1.5/yosemite/__cli__/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/__cli__/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)      491 2024-03-29 00:55:08.000000 yosemite-0.1.5/yosemite/__cli__/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)       26 2024-03-29 00:05:14.000000 yosemite-0.1.5/yosemite/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.330006 yosemite-0.1.5/yosemite/llms/
--rw-r--r--   0 hammad     (501) staff       (20)       20 2024-03-29 01:48:18.000000 yosemite-0.1.5/yosemite/llms/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     6572 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/llms/llm.py
--rw-r--r--   0 hammad     (501) staff       (20)     3072 2024-03-27 16:22:20.000000 yosemite-0.1.5/yosemite/main.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.331241 yosemite-0.1.5/yosemite/ml/
--rw-r--r--   0 hammad     (501) staff       (20)       82 2024-03-29 02:31:57.000000 yosemite-0.1.5/yosemite/ml/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.332125 yosemite-0.1.5/yosemite/ml/database/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 02:31:29.000000 yosemite-0.1.5/yosemite/ml/database/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    16014 2024-03-29 03:38:17.000000 yosemite-0.1.5/yosemite/ml/database/database.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.334967 yosemite-0.1.5/yosemite/ml/legacy/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/ml/legacy/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8677 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/ml/legacy/database.py
--rw-r--r--   0 hammad     (501) staff       (20)     9176 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/ml/legacy/vector_database.py
--rw-r--r--   0 hammad     (501) staff       (20)     3794 2024-03-29 03:20:31.000000 yosemite-0.1.5/yosemite/ml/text.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.336260 yosemite-0.1.5/yosemite/ml/transform/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 02:31:03.000000 yosemite-0.1.5/yosemite/ml/transform/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)    12830 2024-03-29 02:58:49.000000 yosemite-0.1.5/yosemite/ml/transform/transformers.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.337662 yosemite-0.1.5/yosemite/prehistoric/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/prehistoric/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8992 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/prehistoric/heat.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.341455 yosemite-0.1.5/yosemite/tools/
--rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 00:05:30.000000 yosemite-0.1.5/yosemite/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-03-27 15:27:55.000000 yosemite-0.1.5/yosemite/tools/input.py
--rw-r--r--   0 hammad     (501) staff       (20)     2445 2024-03-27 15:28:04.000000 yosemite-0.1.5/yosemite/tools/lightspeed.py
--rw-r--r--   0 hammad     (501) staff       (20)     5243 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/tools/load.py
--rw-r--r--   0 hammad     (501) staff       (20)     5086 2024-03-27 15:18:05.000000 yosemite-0.1.5/yosemite/tools/text.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 03:43:31.342280 yosemite-0.1.5/yosemite.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      735 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)     1282 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       55 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/entry_points.txt
--rw-r--r--   0 hammad     (501) staff       (20)      165 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2024-03-29 03:43:31.000000 yosemite-0.1.5/yosemite.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.237284 yosemite-0.1.6/
+-rw-r--r--   0 hammad     (501) staff       (20)      735 2024-03-29 09:12:09.236888 yosemite-0.1.6/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      349 2024-03-28 23:00:14.000000 yosemite-0.1.6/README.md
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-03-29 09:12:09.237409 yosemite-0.1.6/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      826 2024-03-29 09:11:39.000000 yosemite-0.1.6/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.212830 yosemite-0.1.6/tests/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.213965 yosemite-0.1.6/tests/__cli__/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/__cli__/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)      493 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/__cli__/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 14:14:15.000000 yosemite-0.1.6/tests/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.214946 yosemite-0.1.6/tests/llms/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/llms/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6572 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/llms/llm.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3066 2024-03-27 16:44:33.000000 yosemite-0.1.6/tests/main.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.217159 yosemite-0.1.6/tests/ml/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    14751 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/database.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.218754 yosemite-0.1.6/tests/ml/legacy/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/legacy/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8677 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/legacy/database.py
+-rw-r--r--   0 hammad     (501) staff       (20)     9176 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/legacy/vector_database.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3313 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13062 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/ml/transformers.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.219403 yosemite-0.1.6/tests/prehistoric/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/prehistoric/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8992 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/prehistoric/heat.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.221837 yosemite-0.1.6/tests/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/tools/input.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2445 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/tools/lightspeed.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5243 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/tools/load.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5086 2024-03-27 16:43:45.000000 yosemite-0.1.6/tests/tools/text.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.222719 yosemite-0.1.6/yosemite/
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.226823 yosemite-0.1.6/yosemite/__cli__/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/__cli__/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)      491 2024-03-29 00:55:08.000000 yosemite-0.1.6/yosemite/__cli__/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)       26 2024-03-29 00:05:14.000000 yosemite-0.1.6/yosemite/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.228304 yosemite-0.1.6/yosemite/llms/
+-rw-r--r--   0 hammad     (501) staff       (20)       45 2024-03-29 08:00:29.000000 yosemite-0.1.6/yosemite/llms/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6572 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/llms/llm.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3655 2024-03-29 08:08:06.000000 yosemite-0.1.6/yosemite/llms/serve.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3072 2024-03-27 16:22:20.000000 yosemite-0.1.6/yosemite/main.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.229132 yosemite-0.1.6/yosemite/ml/
+-rw-r--r--   0 hammad     (501) staff       (20)       82 2024-03-29 02:31:57.000000 yosemite-0.1.6/yosemite/ml/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.230290 yosemite-0.1.6/yosemite/ml/database/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 02:31:29.000000 yosemite-0.1.6/yosemite/ml/database/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    16014 2024-03-29 03:38:17.000000 yosemite-0.1.6/yosemite/ml/database/database.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.231747 yosemite-0.1.6/yosemite/ml/legacy/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/ml/legacy/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8677 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/ml/legacy/database.py
+-rw-r--r--   0 hammad     (501) staff       (20)     9176 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/ml/legacy/vector_database.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3794 2024-03-29 03:20:31.000000 yosemite-0.1.6/yosemite/ml/text.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.232780 yosemite-0.1.6/yosemite/ml/transform/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 02:31:03.000000 yosemite-0.1.6/yosemite/ml/transform/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)    12830 2024-03-29 02:58:49.000000 yosemite-0.1.6/yosemite/ml/transform/transformers.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.233738 yosemite-0.1.6/yosemite/prehistoric/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/prehistoric/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8992 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/prehistoric/heat.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.235895 yosemite-0.1.6/yosemite/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)        0 2024-03-29 00:05:30.000000 yosemite-0.1.6/yosemite/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-03-27 15:27:55.000000 yosemite-0.1.6/yosemite/tools/input.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2445 2024-03-27 15:28:04.000000 yosemite-0.1.6/yosemite/tools/lightspeed.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5243 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/tools/load.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5086 2024-03-27 15:18:05.000000 yosemite-0.1.6/yosemite/tools/text.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-03-29 09:12:09.236415 yosemite-0.1.6/yosemite.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      735 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)     1305 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       55 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/entry_points.txt
+-rw-r--r--   0 hammad     (501) staff       (20)      165 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2024-03-29 09:12:09.000000 yosemite-0.1.6/yosemite.egg-info/top_level.txt
```

### Comparing `yosemite-0.1.5/PKG-INFO` & `yosemite-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yosemite
-Version: 0.1.5
+Version: 0.1.6
 Summary: yosemite
 Author: Hammad Saeed
 Author-email: hammad@supportvectors.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9
```

### Comparing `yosemite-0.1.5/setup.py` & `yosemite-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="yosemite",
-    version="0.1.05",
+    version="0.1.06",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="yosemite",
     entry_points={
         'console_scripts': [
             'yosemite = yosemite.__cli__.cli:main',
         ],
```

### Comparing `yosemite-0.1.5/tests/llms/llm.py` & `yosemite-0.1.6/tests/llms/llm.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/main.py` & `yosemite-0.1.6/tests/main.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/ml/database.py` & `yosemite-0.1.6/tests/ml/database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/ml/legacy/database.py` & `yosemite-0.1.6/tests/ml/legacy/database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/ml/legacy/vector_database.py` & `yosemite-0.1.6/tests/ml/legacy/vector_database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/ml/text.py` & `yosemite-0.1.6/tests/ml/text.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/ml/transformers.py` & `yosemite-0.1.6/tests/ml/transformers.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/prehistoric/heat.py` & `yosemite-0.1.6/tests/prehistoric/heat.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/tools/input.py` & `yosemite-0.1.6/tests/tools/input.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/tools/lightspeed.py` & `yosemite-0.1.6/tests/tools/lightspeed.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/tools/load.py` & `yosemite-0.1.6/tests/tools/load.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/tests/tools/text.py` & `yosemite-0.1.6/tests/tools/text.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/llms/llm.py` & `yosemite-0.1.6/yosemite/llms/llm.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/main.py` & `yosemite-0.1.6/yosemite/main.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/ml/database/database.py` & `yosemite-0.1.6/yosemite/ml/database/database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/ml/legacy/database.py` & `yosemite-0.1.6/yosemite/ml/legacy/database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/ml/legacy/vector_database.py` & `yosemite-0.1.6/yosemite/ml/legacy/vector_database.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/ml/text.py` & `yosemite-0.1.6/yosemite/ml/text.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/ml/transform/transformers.py` & `yosemite-0.1.6/yosemite/ml/transform/transformers.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/prehistoric/heat.py` & `yosemite-0.1.6/yosemite/prehistoric/heat.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/tools/input.py` & `yosemite-0.1.6/yosemite/tools/input.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/tools/lightspeed.py` & `yosemite-0.1.6/yosemite/tools/lightspeed.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/tools/load.py` & `yosemite-0.1.6/yosemite/tools/load.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite/tools/text.py` & `yosemite-0.1.6/yosemite/tools/text.py`

 * *Files identical despite different names*

### Comparing `yosemite-0.1.5/yosemite.egg-info/PKG-INFO` & `yosemite-0.1.6/yosemite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yosemite
-Version: 0.1.5
+Version: 0.1.6
 Summary: yosemite
 Author: Hammad Saeed
 Author-email: hammad@supportvectors.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9
```

### Comparing `yosemite-0.1.5/yosemite.egg-info/SOURCES.txt` & `yosemite-0.1.6/yosemite.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 yosemite.egg-info/entry_points.txt
 yosemite.egg-info/requires.txt
 yosemite.egg-info/top_level.txt
 yosemite/__cli__/__init__.py
 yosemite/__cli__/cli.py
 yosemite/llms/__init__.py
 yosemite/llms/llm.py
+yosemite/llms/serve.py
 yosemite/ml/__init__.py
 yosemite/ml/text.py
 yosemite/ml/database/__init__.py
 yosemite/ml/database/database.py
 yosemite/ml/legacy/__init__.py
 yosemite/ml/legacy/database.py
 yosemite/ml/legacy/vector_database.py
```

