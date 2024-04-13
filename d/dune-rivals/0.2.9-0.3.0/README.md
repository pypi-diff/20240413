# Comparing `tmp/dune_rivals-0.2.9.tar.gz` & `tmp/dune_rivals-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.9.tar", last modified: Fri Apr 12 21:11:54 2024, max compression
+gzip compressed data, was "dune_rivals-0.3.0.tar", last modified: Sat Apr 13 16:30:13 2024, max compression
```

## Comparing `dune_rivals-0.2.9.tar` & `dune_rivals-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:11:54.210576 dune_rivals-0.2.9/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:11:54.210170 dune_rivals-0.2.9/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.9/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:11:54.209751 dune_rivals-0.2.9/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 21:11:54.000000 dune_rivals-0.2.9/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10823 2024-04-12 21:10:43.000000 dune_rivals-0.2.9/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 21:11:48.000000 dune_rivals-0.2.9/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 21:11:54.210666 dune_rivals-0.2.9/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 16:30:13.085917 dune_rivals-0.3.0/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 16:30:13.085515 dune_rivals-0.3.0/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.3.0/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-13 16:30:13.085087 dune_rivals-0.3.0/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-13 16:30:13.000000 dune_rivals-0.3.0/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-13 16:30:13.000000 dune_rivals-0.3.0/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-13 16:30:13.000000 dune_rivals-0.3.0/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-13 16:30:13.000000 dune_rivals-0.3.0/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    15944 2024-04-13 16:29:27.000000 dune_rivals-0.3.0/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-13 16:29:58.000000 dune_rivals-0.3.0/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-13 16:30:13.086009 dune_rivals-0.3.0/setup.cfg
```

