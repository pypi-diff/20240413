# Comparing `tmp/pyfoal-1.0.0.tar.gz` & `tmp/pyfoal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfoal-1.0.0.tar", last modified: Thu Sep 14 09:03:23 2023, max compression
+gzip compressed data, was "pyfoal-1.0.1.tar", last modified: Fri Apr 12 23:11:58 2024, max compression
```

## Comparing `pyfoal-1.0.0.tar` & `pyfoal-1.0.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1090 2023-09-14 09:02:43.000000 pyfoal-1.0.0/LICENSE
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)     8983 2023-09-14 09:03:23.736395 pyfoal-1.0.0/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8260 2023-09-14 09:02:43.000000 pyfoal-1.0.0/README.md
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.720395 pyfoal-1.0.0/pyfoal/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1041 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1449 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/__main__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.720395 pyfoal-1.0.0/pyfoal/assets/
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.720395 pyfoal-1.0.0/pyfoal/assets/g2p/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      372 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/g2p/phonemes.csv
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.728395 pyfoal-1.0.0/pyfoal/assets/p2fa/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      288 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/p2fa/config
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  8119146 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/p2fa/hmmdefs
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      598 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/p2fa/macros
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      257 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/p2fa/monophones
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.728395 pyfoal-1.0.0/pyfoal/assets/partitions/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   182013 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/partitions/arctic.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  3687171 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/assets/partitions/libritts.json
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.732396 pyfoal-1.0.0/pyfoal/baselines/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       37 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/baselines/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4445 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/baselines/mfa.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     8364 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/baselines/p2fa.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1489 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/checkpoint.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/config/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/config/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4160 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/config/defaults.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      712 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/config/static.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4203 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/convert.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10226 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/data/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      162 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2169 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/collate.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3286 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/dataset.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/data/download/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/download/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      567 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/download/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9899 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/download/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      655 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/loader.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/data/preprocess/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       58 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/preprocess/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      547 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/preprocess/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1163 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/preprocess/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2041 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/preprocess/mels.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1557 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/preprocess/prior.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2740 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/data/sampler.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/evaluate/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       70 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/evaluate/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      838 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/evaluate/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2939 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/evaluate/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4018 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/evaluate/metrics.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/g2p/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/g2p/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2079 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/g2p/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2833 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/interpolate.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1920 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/load.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1971 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/loudness.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4595 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/model.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/partition/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/partition/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      383 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/partition/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2381 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/partition/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/plot/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/plot/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      841 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/plot/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3425 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/plot/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1272 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/time.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.736395 pyfoal-1.0.0/pyfoal/train/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/train/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1355 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/train/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    11646 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/train/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4276 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/viterbi.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1483 2023-09-14 09:02:43.000000 pyfoal-1.0.0/pyfoal/write.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-09-14 09:03:23.720395 pyfoal-1.0.0/pyfoal.egg-info/
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)     8983 2023-09-14 09:03:23.000000 pyfoal-1.0.0/pyfoal.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1503 2023-09-14 09:03:23.000000 pyfoal-1.0.0/pyfoal.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-09-14 09:03:23.000000 pyfoal-1.0.0/pyfoal.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      132 2023-09-14 09:03:23.000000 pyfoal-1.0.0/pyfoal.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        7 2023-09-14 09:03:23.000000 pyfoal-1.0.0/pyfoal.egg-info/top_level.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-09-14 09:03:23.736395 pyfoal-1.0.0/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1055 2023-09-14 09:02:43.000000 pyfoal-1.0.0/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/
+-rw-rw-r--   0 max       (1000) max       (1000)     1090 2024-04-12 22:46:07.000000 pyfoal-1.0.1/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     8994 2024-04-12 23:11:58.290866 pyfoal-1.0.1/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     8260 2024-04-12 22:46:07.000000 pyfoal-1.0.1/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.274866 pyfoal-1.0.1/pyfoal/
+-rw-rw-r--   0 max       (1000) max       (1000)     1041 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1449 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/__main__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.274866 pyfoal-1.0.1/pyfoal/assets/
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.274866 pyfoal-1.0.1/pyfoal/assets/g2p/
+-rw-rw-r--   0 max       (1000) max       (1000)      372 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/g2p/phonemes.csv
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.282866 pyfoal-1.0.1/pyfoal/assets/p2fa/
+-rw-rw-r--   0 max       (1000) max       (1000)      288 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/p2fa/config
+-rw-rw-r--   0 max       (1000) max       (1000)  8119146 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/p2fa/hmmdefs
+-rw-rw-r--   0 max       (1000) max       (1000)      598 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/p2fa/macros
+-rw-rw-r--   0 max       (1000) max       (1000)      257 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/p2fa/monophones
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.286867 pyfoal-1.0.1/pyfoal/assets/partitions/
+-rw-rw-r--   0 max       (1000) max       (1000)   182013 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/partitions/arctic.json
+-rw-rw-r--   0 max       (1000) max       (1000)  3687171 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/assets/partitions/libritts.json
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/baselines/
+-rw-rw-r--   0 max       (1000) max       (1000)       37 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/baselines/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4445 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/baselines/mfa.py
+-rw-rw-r--   0 max       (1000) max       (1000)     8359 2024-04-12 23:00:41.000000 pyfoal-1.0.1/pyfoal/baselines/p2fa.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1489 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/checkpoint.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/config/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/config/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4160 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/config/defaults.py
+-rw-rw-r--   0 max       (1000) max       (1000)      712 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/config/static.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4203 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/convert.py
+-rw-rw-r--   0 max       (1000) max       (1000)    10226 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/data/
+-rw-rw-r--   0 max       (1000) max       (1000)      162 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2169 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/collate.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3286 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/dataset.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/data/download/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/download/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      567 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/download/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     9899 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/download/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)      655 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/loader.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/data/preprocess/
+-rw-rw-r--   0 max       (1000) max       (1000)       58 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/preprocess/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      547 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/preprocess/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1163 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/preprocess/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2041 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/preprocess/mels.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1557 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/preprocess/prior.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2740 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/data/sampler.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/evaluate/
+-rw-rw-r--   0 max       (1000) max       (1000)       70 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/evaluate/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      838 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/evaluate/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2939 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/evaluate/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4018 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/evaluate/metrics.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/g2p/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/g2p/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2079 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/g2p/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2833 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/interpolate.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1920 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/load.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1971 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/loudness.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4595 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/model.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/partition/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/partition/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      383 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/partition/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2381 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/partition/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/plot/
+-rw-rw-r--   0 max       (1000) max       (1000)       19 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/plot/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      841 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/plot/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3425 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/plot/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1272 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/time.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal/train/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/train/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1355 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/train/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    11646 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/train/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4276 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/viterbi.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1483 2024-04-12 22:46:07.000000 pyfoal-1.0.1/pyfoal/write.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:11:58.290866 pyfoal-1.0.1/pyfoal.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     8994 2024-04-12 23:11:58.000000 pyfoal-1.0.1/pyfoal.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1503 2024-04-12 23:11:58.000000 pyfoal-1.0.1/pyfoal.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2024-04-12 23:11:58.000000 pyfoal-1.0.1/pyfoal.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      128 2024-04-12 23:11:58.000000 pyfoal-1.0.1/pyfoal.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        7 2024-04-12 23:11:58.000000 pyfoal-1.0.1/pyfoal.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2024-04-12 23:11:58.290866 pyfoal-1.0.1/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)     1062 2024-04-12 23:08:10.000000 pyfoal-1.0.1/setup.py
```

### Comparing `pyfoal-1.0.0/LICENSE` & `pyfoal-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/PKG-INFO` & `pyfoal-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: pyfoal
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python forced aligner
 Home-page: https://github.com/maxrmorrison/pyfoal
 Author: Max Morrison
 Author-email: maxrmorrison@gmail.com
 License: MIT
 Keywords: align,alignment,attention,duration,phoneme,speech,word
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g2p_en
+Requires-Dist: librosa
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: phonemizer
 Requires-Dist: pypar
 Requires-Dist: requests
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: soundfile
 Requires-Dist: tensorboard
-Requires-Dist: torch<2.0.0
-Requires-Dist: torchaudio<2.0.0
+Requires-Dist: torch
+Requires-Dist: torchaudio
 Requires-Dist: tqdm
 Requires-Dist: yapecs
 
 <h1 align="center">Python forced alignment</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/pyfoal.svg)](https://pypi.python.org/pypi/pyfoal)
```

### Comparing `pyfoal-1.0.0/README.md` & `pyfoal-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/__init__.py` & `pyfoal-1.0.1/pyfoal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/__main__.py` & `pyfoal-1.0.1/pyfoal/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/assets/p2fa/hmmdefs` & `pyfoal-1.0.1/pyfoal/assets/p2fa/hmmdefs`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/assets/p2fa/macros` & `pyfoal-1.0.1/pyfoal/assets/p2fa/macros`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/assets/partitions/arctic.json` & `pyfoal-1.0.1/pyfoal/assets/partitions/arctic.json`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/assets/partitions/libritts.json` & `pyfoal-1.0.1/pyfoal/assets/partitions/libritts.json`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/baselines/mfa.py` & `pyfoal-1.0.1/pyfoal/baselines/mfa.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/baselines/p2fa.py` & `pyfoal-1.0.1/pyfoal/baselines/p2fa.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     def format(self, directory, audio, script_file):
         """Write HTK arguments and convert data to HTK format"""
         # Save audio to disk
         audiofile = directory / 'sound.wav'
         soundfile.write(
             str(audiofile),
-            audio.cpu().squeeze().numpy().astype(np.float32),
+            audio.cpu().squeeze().numpy().astype(float),
             SAMPLE_RATE)
 
         # Save HTK process metadata
         code_file = directory / 'codetr.scp'
         plp_file = directory / 'tmp.plp'
         with open(code_file, 'w') as file:
             file.write(f'{audiofile} {plp_file}\n')
```

### Comparing `pyfoal-1.0.0/pyfoal/checkpoint.py` & `pyfoal-1.0.1/pyfoal/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/config/defaults.py` & `pyfoal-1.0.1/pyfoal/config/defaults.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/config/static.py` & `pyfoal-1.0.1/pyfoal/config/static.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/convert.py` & `pyfoal-1.0.1/pyfoal/convert.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/core.py` & `pyfoal-1.0.1/pyfoal/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/collate.py` & `pyfoal-1.0.1/pyfoal/data/collate.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/dataset.py` & `pyfoal-1.0.1/pyfoal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/download/__main__.py` & `pyfoal-1.0.1/pyfoal/data/download/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/download/core.py` & `pyfoal-1.0.1/pyfoal/data/download/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/loader.py` & `pyfoal-1.0.1/pyfoal/data/loader.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/preprocess/__main__.py` & `pyfoal-1.0.1/pyfoal/data/preprocess/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/preprocess/core.py` & `pyfoal-1.0.1/pyfoal/data/preprocess/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/preprocess/mels.py` & `pyfoal-1.0.1/pyfoal/data/preprocess/mels.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/preprocess/prior.py` & `pyfoal-1.0.1/pyfoal/data/preprocess/prior.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/data/sampler.py` & `pyfoal-1.0.1/pyfoal/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/evaluate/__main__.py` & `pyfoal-1.0.1/pyfoal/evaluate/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/evaluate/core.py` & `pyfoal-1.0.1/pyfoal/evaluate/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/evaluate/metrics.py` & `pyfoal-1.0.1/pyfoal/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/g2p/core.py` & `pyfoal-1.0.1/pyfoal/g2p/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/interpolate.py` & `pyfoal-1.0.1/pyfoal/interpolate.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/load.py` & `pyfoal-1.0.1/pyfoal/load.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/loudness.py` & `pyfoal-1.0.1/pyfoal/loudness.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/model.py` & `pyfoal-1.0.1/pyfoal/model.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/partition/core.py` & `pyfoal-1.0.1/pyfoal/partition/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/plot/__main__.py` & `pyfoal-1.0.1/pyfoal/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/plot/core.py` & `pyfoal-1.0.1/pyfoal/plot/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/time.py` & `pyfoal-1.0.1/pyfoal/time.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/train/__main__.py` & `pyfoal-1.0.1/pyfoal/train/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/train/core.py` & `pyfoal-1.0.1/pyfoal/train/core.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/viterbi.py` & `pyfoal-1.0.1/pyfoal/viterbi.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal/write.py` & `pyfoal-1.0.1/pyfoal/write.py`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/pyfoal.egg-info/PKG-INFO` & `pyfoal-1.0.1/pyfoal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: pyfoal
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python forced aligner
 Home-page: https://github.com/maxrmorrison/pyfoal
 Author: Max Morrison
 Author-email: maxrmorrison@gmail.com
 License: MIT
 Keywords: align,alignment,attention,duration,phoneme,speech,word
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: g2p_en
+Requires-Dist: librosa
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: phonemizer
 Requires-Dist: pypar
 Requires-Dist: requests
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: soundfile
 Requires-Dist: tensorboard
-Requires-Dist: torch<2.0.0
-Requires-Dist: torchaudio<2.0.0
+Requires-Dist: torch
+Requires-Dist: torchaudio
 Requires-Dist: tqdm
 Requires-Dist: yapecs
 
 <h1 align="center">Python forced alignment</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/pyfoal.svg)](https://pypi.python.org/pypi/pyfoal)
```

### Comparing `pyfoal-1.0.0/pyfoal.egg-info/SOURCES.txt` & `pyfoal-1.0.1/pyfoal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfoal-1.0.0/setup.py` & `pyfoal-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='pyfoal',
     description='Python forced aligner',
-    version='1.0.0',
+    version='1.0.1',
     author='Max Morrison',
     author_email='maxrmorrison@gmail.com',
     url='https://github.com/maxrmorrison/pyfoal',
     install_requires=[
         'g2p_en',
+        'librosa',
         'matplotlib',
         'numpy',
         'phonemizer',
         'pypar',
         'requests',
         'scikit-learn',
         'scipy',
         'soundfile',
         'tensorboard',
-        'torch<2.0.0',
-        'torchaudio<2.0.0',
+        'torch',
+        'torchaudio',
         'tqdm',
         'yapecs'],
     packages=find_packages(),
     package_data={'pyfoal': ['assets/*', 'assets/*/*']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=[
```

