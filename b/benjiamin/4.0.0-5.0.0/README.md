# Comparing `tmp/benjiamin-4.0.0.tar.gz` & `tmp/benjiamin-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benjiamin-4.0.0.tar", last modified: Fri Apr 12 20:25:18 2024, max compression
+gzip compressed data, was "benjiamin-5.0.0.tar", last modified: Fri Apr 12 22:04:58 2024, max compression
```

## Comparing `benjiamin-4.0.0.tar` & `benjiamin-5.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 20:25:18.661422 benjiamin-4.0.0/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 20:25:18.661299 benjiamin-4.0.0/PKG-INFO
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 20:25:18.661126 benjiamin-4.0.0/benjiamin.egg-info/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 20:25:18.000000 benjiamin-4.0.0/benjiamin.egg-info/PKG-INFO
--rw-r--r--   0 jli17      (501) staff       (20)      172 2024-04-12 20:25:18.000000 benjiamin-4.0.0/benjiamin.egg-info/SOURCES.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 20:25:18.000000 benjiamin-4.0.0/benjiamin.egg-info/dependency_links.txt
--rw-r--r--   0 jli17      (501) staff       (20)       16 2024-04-12 20:25:18.000000 benjiamin-4.0.0/benjiamin.egg-info/requires.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 20:25:18.000000 benjiamin-4.0.0/benjiamin.egg-info/top_level.txt
--rw-r--r--   0 jli17      (501) staff       (20)       38 2024-04-12 20:25:18.661466 benjiamin-4.0.0/setup.cfg
--rw-r--r--   0 jli17      (501) staff       (20)      773 2024-04-12 20:25:08.000000 benjiamin-4.0.0/setup.py
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:04:58.628835 benjiamin-5.0.0/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:04:58.628703 benjiamin-5.0.0/PKG-INFO
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 22:04:58.628522 benjiamin-5.0.0/benjiamin.egg-info/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 22:04:58.000000 benjiamin-5.0.0/benjiamin.egg-info/PKG-INFO
+-rw-r--r--   0 jli17      (501) staff       (20)      140 2024-04-12 22:04:58.000000 benjiamin-5.0.0/benjiamin.egg-info/SOURCES.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:04:58.000000 benjiamin-5.0.0/benjiamin.egg-info/dependency_links.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 22:04:58.000000 benjiamin-5.0.0/benjiamin.egg-info/top_level.txt
+-rw-r--r--   0 jli17      (501) staff       (20)       38 2024-04-12 22:04:58.628876 benjiamin-5.0.0/setup.cfg
+-rw-r--r--   0 jli17      (501) staff       (20)     1247 2024-04-12 22:04:21.000000 benjiamin-5.0.0/setup.py
```
