# Comparing `tmp/emphases-0.0.1.tar.gz` & `tmp/emphases-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emphases-0.0.1.tar", last modified: Thu Dec 21 22:12:52 2023, max compression
+gzip compressed data, was "emphases-0.0.2.tar", last modified: Fri Apr 12 23:46:32 2024, max compression
```

## Comparing `emphases-0.0.1.tar` & `emphases-0.0.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.564167 emphases-0.0.1/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1078 2023-03-30 23:00:58.000000 emphases-0.0.1/LICENSE
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    11017 2023-12-21 22:12:52.564167 emphases-0.0.1/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    10239 2023-12-21 22:12:11.000000 emphases-0.0.1/README.md
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.540166 emphases-0.0.1/emphases/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      860 2023-10-11 16:34:32.000000 emphases-0.0.1/emphases/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1477 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/__main__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.540166 emphases-0.0.1/emphases/annotate/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/annotate/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1390 2023-09-12 01:41:51.000000 emphases-0.0.1/emphases/annotate/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1894 2023-09-12 01:41:38.000000 emphases-0.0.1/emphases/annotate/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.536167 emphases-0.0.1/emphases/assets/
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.540166 emphases-0.0.1/emphases/assets/checkpoints/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)  3043923 2023-09-13 14:40:11.000000 emphases-0.0.1/emphases/assets/checkpoints/checkpoint.pt
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.548167 emphases-0.0.1/emphases/assets/configs/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     7152 2023-09-13 14:44:15.000000 emphases-0.0.1/emphases/assets/configs/annotate.yaml
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.552167 emphases-0.0.1/emphases/assets/partitions/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   130095 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/assets/partitions/automatic.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      277 2023-09-22 13:19:05.000000 emphases-0.0.1/emphases/assets/partitions/buckeye.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   130095 2023-09-12 15:26:36.000000 emphases-0.0.1/emphases/assets/partitions/crowdsource.json
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)   130095 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/assets/partitions/libritts.json
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.552167 emphases-0.0.1/emphases/baselines/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       86 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/__init__.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.552167 emphases-0.0.1/emphases/baselines/duration_variance/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/duration_variance/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      671 2023-04-13 20:25:09.000000 emphases-0.0.1/emphases/baselines/duration_variance/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.552167 emphases-0.0.1/emphases/baselines/pitch_variance/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/pitch_variance/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1544 2023-09-03 16:47:45.000000 emphases-0.0.1/emphases/baselines/pitch_variance/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.556167 emphases-0.0.1/emphases/baselines/prominence/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      238 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4148 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/baselines/prominence/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4716 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/cwt_utils.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4492 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/duration_processing.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      601 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/energy_processing.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3900 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/f0_processing.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1419 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/filter.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5762 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/loma.py
--rwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)     4956 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/pitch_tracker.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2494 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/baselines/prominence/smooth_and_interp.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.556167 emphases-0.0.1/emphases/config/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        0 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/config/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5938 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/config/defaults.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1395 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/config/static.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      942 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/convert.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    19228 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.556167 emphases-0.0.1/emphases/data/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      162 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/data/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2154 2023-11-10 19:32:20.000000 emphases-0.0.1/emphases/data/collate.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3535 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/dataset.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.556167 emphases-0.0.1/emphases/data/download/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/data/download/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      699 2023-09-06 02:12:24.000000 emphases-0.0.1/emphases/data/download/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)    18936 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/download/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      665 2023-09-01 20:35:17.000000 emphases-0.0.1/emphases/data/loader.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.560166 emphases-0.0.1/emphases/data/preprocess/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       62 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/data/preprocess/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      697 2023-09-04 17:07:25.000000 emphases-0.0.1/emphases/data/preprocess/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4567 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/preprocess/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3479 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/preprocess/loudness.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3029 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/preprocess/mels.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2384 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/data/sampler.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.560166 emphases-0.0.1/emphases/evaluate/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       71 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/evaluate/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      843 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/evaluate/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     3719 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/evaluate/core.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2909 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/evaluate/metrics.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      405 2023-09-13 14:30:38.000000 emphases-0.0.1/emphases/load.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.560166 emphases-0.0.1/emphases/model/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       64 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/model/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     5096 2023-09-04 20:21:47.000000 emphases-0.0.1/emphases/model/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.560166 emphases-0.0.1/emphases/model/layers/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      382 2023-09-04 18:15:33.000000 emphases-0.0.1/emphases/model/layers/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1048 2023-09-04 18:14:56.000000 emphases-0.0.1/emphases/model/layers/convolution.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1715 2023-08-29 22:34:24.000000 emphases-0.0.1/emphases/model/layers/transformer.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.560166 emphases-0.0.1/emphases/partition/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/partition/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      429 2023-08-23 21:44:50.000000 emphases-0.0.1/emphases/partition/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     4770 2023-09-13 15:28:31.000000 emphases-0.0.1/emphases/partition/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.564167 emphases-0.0.1/emphases/plot/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       42 2023-04-13 20:25:09.000000 emphases-0.0.1/emphases/plot/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1581 2023-04-13 20:25:09.000000 emphases-0.0.1/emphases/plot/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.564167 emphases-0.0.1/emphases/plot/scaling/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       19 2023-04-13 20:25:09.000000 emphases-0.0.1/emphases/plot/scaling/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1619 2023-09-11 22:03:38.000000 emphases-0.0.1/emphases/plot/scaling/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2364 2023-09-11 22:03:25.000000 emphases-0.0.1/emphases/plot/scaling/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.564167 emphases-0.0.1/emphases/train/
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       20 2023-03-30 23:00:58.000000 emphases-0.0.1/emphases/train/__init__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1302 2023-12-21 22:12:11.000000 emphases-0.0.1/emphases/train/__main__.py
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     9746 2023-11-16 16:54:03.000000 emphases-0.0.1/emphases/train/core.py
-drwxrwxr-x   0 mrm5248   (1001) mrm5248   (1001)        0 2023-12-21 22:12:52.564167 emphases-0.0.1/emphases.egg-info/
--rw-r--r--   0 mrm5248   (1001) mrm5248   (1001)    11017 2023-12-21 22:12:52.000000 emphases-0.0.1/emphases.egg-info/PKG-INFO
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     2347 2023-12-21 22:12:52.000000 emphases-0.0.1/emphases.egg-info/SOURCES.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        1 2023-12-21 22:12:52.000000 emphases-0.0.1/emphases.egg-info/dependency_links.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)      120 2023-12-21 22:12:52.000000 emphases-0.0.1/emphases.egg-info/requires.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)        9 2023-12-21 22:12:52.000000 emphases-0.0.1/emphases.egg-info/top_level.txt
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)       38 2023-12-21 22:12:52.564167 emphases-0.0.1/setup.cfg
--rw-rw-r--   0 mrm5248   (1001) mrm5248   (1001)     1044 2023-12-21 22:12:11.000000 emphases-0.0.1/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.524789 emphases-0.0.2/
+-rw-rw-r--   0 max       (1000) max       (1000)     1078 2024-04-12 22:46:00.000000 emphases-0.0.2/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)    11695 2024-04-12 23:46:32.524789 emphases-0.0.2/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)    10895 2024-04-12 22:46:00.000000 emphases-0.0.2/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.512789 emphases-0.0.2/emphases/
+-rw-rw-r--   0 max       (1000) max       (1000)      860 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1477 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/__main__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.512789 emphases-0.0.2/emphases/annotate/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/annotate/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1390 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/annotate/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1894 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/annotate/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.512789 emphases-0.0.2/emphases/assets/
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.512789 emphases-0.0.2/emphases/assets/checkpoints/
+-rw-rw-r--   0 max       (1000) max       (1000)  3043923 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/checkpoints/checkpoint.pt
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.516789 emphases-0.0.2/emphases/assets/configs/
+-rw-rw-r--   0 max       (1000) max       (1000)     7152 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/configs/annotate.yaml
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.516789 emphases-0.0.2/emphases/assets/partitions/
+-rw-rw-r--   0 max       (1000) max       (1000)   130095 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/partitions/automatic.json
+-rw-rw-r--   0 max       (1000) max       (1000)      277 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/partitions/buckeye.json
+-rw-rw-r--   0 max       (1000) max       (1000)   130095 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/partitions/crowdsource.json
+-rw-rw-r--   0 max       (1000) max       (1000)   130095 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/assets/partitions/libritts.json
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.516789 emphases-0.0.2/emphases/baselines/
+-rw-rw-r--   0 max       (1000) max       (1000)       86 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.516789 emphases-0.0.2/emphases/baselines/duration_variance/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/duration_variance/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      671 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/duration_variance/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.516789 emphases-0.0.2/emphases/baselines/pitch_variance/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/pitch_variance/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1544 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/pitch_variance/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/baselines/prominence/
+-rw-rw-r--   0 max       (1000) max       (1000)      238 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4148 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4716 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/cwt_utils.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4492 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/duration_processing.py
+-rw-rw-r--   0 max       (1000) max       (1000)      601 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/energy_processing.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3900 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/f0_processing.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1419 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/filter.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5762 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/loma.py
+-rwxrwxr-x   0 max       (1000) max       (1000)     4956 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/pitch_tracker.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2494 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/baselines/prominence/smooth_and_interp.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/config/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/config/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5952 2024-04-12 23:16:56.000000 emphases-0.0.2/emphases/config/defaults.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1395 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/config/static.py
+-rw-rw-r--   0 max       (1000) max       (1000)      942 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/convert.py
+-rw-rw-r--   0 max       (1000) max       (1000)    19228 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/data/
+-rw-rw-r--   0 max       (1000) max       (1000)      162 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2154 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/collate.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3535 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/dataset.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/data/download/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/download/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      699 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/download/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    18936 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/download/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)      665 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/loader.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/data/preprocess/
+-rw-rw-r--   0 max       (1000) max       (1000)       62 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/preprocess/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      697 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/preprocess/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4567 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/preprocess/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3479 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/preprocess/loudness.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3029 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/preprocess/mels.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2481 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/data/sampler.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/evaluate/
+-rw-rw-r--   0 max       (1000) max       (1000)       71 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/evaluate/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      843 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/evaluate/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3719 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/evaluate/core.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2909 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/evaluate/metrics.py
+-rw-rw-r--   0 max       (1000) max       (1000)      405 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/load.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/model/
+-rw-rw-r--   0 max       (1000) max       (1000)       64 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/model/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5096 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/model/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/model/layers/
+-rw-rw-r--   0 max       (1000) max       (1000)      382 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/model/layers/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1048 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/model/layers/convolution.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1715 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/model/layers/transformer.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/partition/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/partition/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      429 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/partition/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4770 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/partition/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/plot/
+-rw-rw-r--   0 max       (1000) max       (1000)       42 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/plot/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1581 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/plot/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.520789 emphases-0.0.2/emphases/plot/scaling/
+-rw-rw-r--   0 max       (1000) max       (1000)       19 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/plot/scaling/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1619 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/plot/scaling/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2364 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/plot/scaling/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.524789 emphases-0.0.2/emphases/train/
+-rw-rw-r--   0 max       (1000) max       (1000)       20 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/train/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1302 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/train/__main__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     9746 2024-04-12 22:46:00.000000 emphases-0.0.2/emphases/train/core.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-04-12 23:46:32.524789 emphases-0.0.2/emphases.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    11695 2024-04-12 23:46:32.000000 emphases-0.0.2/emphases.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     2347 2024-04-12 23:46:32.000000 emphases-0.0.2/emphases.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2024-04-12 23:46:32.000000 emphases-0.0.2/emphases.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      127 2024-04-12 23:46:32.000000 emphases-0.0.2/emphases.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        9 2024-04-12 23:46:32.000000 emphases-0.0.2/emphases.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2024-04-12 23:46:32.524789 emphases-0.0.2/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)     1062 2024-04-12 23:17:52.000000 emphases-0.0.2/setup.py
```

### Comparing `emphases-0.0.1/LICENSE` & `emphases-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/PKG-INFO` & `emphases-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,24 @@
-Metadata-Version: 2.1
-Name: emphases
-Version: 0.0.1
-Summary: Crowdsourced and Automatic Speech Prominence Estimation
-Home-page: https://github.com/interactiveaudiolab/emphases
-Author: Interactive Audio Lab
-Author-email: interactiveaudiolab@gmail.com
-License: MIT
-Keywords: annotatation,audio,emphasis,prominence,speech
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: huggingface-hub
-Requires-Dist: librosa
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: penn
-Requires-Dist: pycwt
-Requires-Dist: pyfoal
-Requires-Dist: pypar
-Requires-Dist: pyyaml
-Requires-Dist: reseval
-Requires-Dist: scipy
-Requires-Dist: torch
-Requires-Dist: torchutil
-Requires-Dist: torchaudio
-Requires-Dist: yapecs
-
 <h1 align="center">Crowdsourced and Automatic Speech Prominence Estimation</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/emphases.svg)](https://pypi.python.org/pypi/emphases)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/emphases)](https://pepy.tech/project/emphases)
 
 Annotation, training, evaluation and inference of speech prominence
 
-`pip install emphases`
-
-[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation)
+[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation) [Dataset](https://zenodo.org/records/10402793)
 
 </div>
 
 
 ## Table of contents
 
+- [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface](#application-programming-interface)
         * [`emphases.from_alignment_and_audio`](#emphasesfrom_alignment_and_audio)
         * [`emphases.from_text_and_audio`](#emphasesfrom_text_and_audio)
         * [`emphases.from_file`](#emphasesfrom_file)
         * [`emphases.from_file_to_file`](#emphasesfrom_file_to_file)
         * [`emphases.from_files_to_files`](#emphasesfrom_files_to_files)
@@ -61,14 +32,26 @@
     * [Monitor](#monitor)
 - [Evaluation](#reproducing-results)
     * [Evaluate](#evaluate)
     * [Analyze](#analyze)
 - [Citation](#citation)
 
 
+## Installation
+
+`pip install emphases`
+
+By default, we use the Penn Phonetic Forced Aligner (P2FA) via the [`pyfoal`](https://github.com/maxrmorrison/pyfoal/)
+repo to perform word alignments. This requires installing HTK. See [the HTK
+installation instructions](https://github.com/maxrmorrison/pyfoal/tree/main?tab=readme-ov-file#penn-phonetic-forced-aligner-p2fa)
+provided by `pyfoal`. Alternatively, you can use a different forced aligner
+and either pass the alignment as a [`pypar.Alignment`](https://github.com/maxrmorrison/pypar/tree/main)
+object or save the alignment as a `.TextGrid` file.
+
+
 ## Inference
 
 Perform automatic emphasis annotation using our best pretrained model
 
 ```python
 import emphases
 
@@ -112,14 +95,15 @@
         gpu: The index of the gpu to run inference on
 
     Returns:
         scores: The float-valued emphasis scores for each word
     """
 ```
 
+
 #### `emphases.from_text_and_audio`
 
 ```python
 def from_text_and_audio(
     text: str,
     audio: torch.Tensor,
     sample_rate: int,
```

### Comparing `emphases-0.0.1/README.md` & `emphases-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,53 @@
+Metadata-Version: 2.1
+Name: emphases
+Version: 0.0.2
+Summary: Crowdsourced and Automatic Speech Prominence Estimation
+Home-page: https://github.com/interactiveaudiolab/emphases
+Author: Interactive Audio Lab
+Author-email: interactiveaudiolab@gmail.com
+License: MIT
+Keywords: annotatation,audio,emphasis,prominence,speech
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: GPUtil
+Requires-Dist: huggingface-hub
+Requires-Dist: librosa
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: penn
+Requires-Dist: pycwt
+Requires-Dist: pyfoal
+Requires-Dist: pypar
+Requires-Dist: pyyaml
+Requires-Dist: reseval
+Requires-Dist: scipy
+Requires-Dist: torch
+Requires-Dist: torchutil
+Requires-Dist: torchaudio
+Requires-Dist: yapecs
+
 <h1 align="center">Crowdsourced and Automatic Speech Prominence Estimation</h1>
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/emphases.svg)](https://pypi.python.org/pypi/emphases)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/emphases)](https://pepy.tech/project/emphases)
 
 Annotation, training, evaluation and inference of speech prominence
 
-`pip install emphases`
-
-[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation)
+[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation) [Dataset](https://zenodo.org/records/10402793)
 
 </div>
 
 
 ## Table of contents
 
+- [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface](#application-programming-interface)
         * [`emphases.from_alignment_and_audio`](#emphasesfrom_alignment_and_audio)
         * [`emphases.from_text_and_audio`](#emphasesfrom_text_and_audio)
         * [`emphases.from_file`](#emphasesfrom_file)
         * [`emphases.from_file_to_file`](#emphasesfrom_file_to_file)
         * [`emphases.from_files_to_files`](#emphasesfrom_files_to_files)
@@ -33,14 +61,26 @@
     * [Monitor](#monitor)
 - [Evaluation](#reproducing-results)
     * [Evaluate](#evaluate)
     * [Analyze](#analyze)
 - [Citation](#citation)
 
 
+## Installation
+
+`pip install emphases`
+
+By default, we use the Penn Phonetic Forced Aligner (P2FA) via the [`pyfoal`](https://github.com/maxrmorrison/pyfoal/)
+repo to perform word alignments. This requires installing HTK. See [the HTK
+installation instructions](https://github.com/maxrmorrison/pyfoal/tree/main?tab=readme-ov-file#penn-phonetic-forced-aligner-p2fa)
+provided by `pyfoal`. Alternatively, you can use a different forced aligner
+and either pass the alignment as a [`pypar.Alignment`](https://github.com/maxrmorrison/pypar/tree/main)
+object or save the alignment as a `.TextGrid` file.
+
+
 ## Inference
 
 Perform automatic emphasis annotation using our best pretrained model
 
 ```python
 import emphases
 
@@ -84,14 +124,15 @@
         gpu: The index of the gpu to run inference on
 
     Returns:
         scores: The float-valued emphasis scores for each word
     """
 ```
 
+
 #### `emphases.from_text_and_audio`
 
 ```python
 def from_text_and_audio(
     text: str,
     audio: torch.Tensor,
     sample_rate: int,
```

### Comparing `emphases-0.0.1/emphases/__init__.py` & `emphases-0.0.2/emphases/__init__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/__main__.py` & `emphases-0.0.2/emphases/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/annotate/__main__.py` & `emphases-0.0.2/emphases/annotate/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/annotate/core.py` & `emphases-0.0.2/emphases/annotate/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/assets/checkpoints/checkpoint.pt` & `emphases-0.0.2/emphases/assets/checkpoints/checkpoint.pt`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/assets/configs/annotate.yaml` & `emphases-0.0.2/emphases/assets/configs/annotate.yaml`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/assets/partitions/automatic.json` & `emphases-0.0.2/emphases/assets/partitions/automatic.json`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/assets/partitions/crowdsource.json` & `emphases-0.0.2/emphases/assets/partitions/crowdsource.json`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/assets/partitions/libritts.json` & `emphases-0.0.2/emphases/assets/partitions/libritts.json`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/duration_variance/core.py` & `emphases-0.0.2/emphases/baselines/duration_variance/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/pitch_variance/core.py` & `emphases-0.0.2/emphases/baselines/pitch_variance/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/core.py` & `emphases-0.0.2/emphases/baselines/prominence/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/cwt_utils.py` & `emphases-0.0.2/emphases/baselines/prominence/cwt_utils.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/duration_processing.py` & `emphases-0.0.2/emphases/baselines/prominence/duration_processing.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/energy_processing.py` & `emphases-0.0.2/emphases/baselines/prominence/energy_processing.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/f0_processing.py` & `emphases-0.0.2/emphases/baselines/prominence/f0_processing.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/filter.py` & `emphases-0.0.2/emphases/baselines/prominence/filter.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/loma.py` & `emphases-0.0.2/emphases/baselines/prominence/loma.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/pitch_tracker.py` & `emphases-0.0.2/emphases/baselines/prominence/pitch_tracker.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/baselines/prominence/smooth_and_interp.py` & `emphases-0.0.2/emphases/baselines/prominence/smooth_and_interp.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/config/defaults.py` & `emphases-0.0.2/emphases/config/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from pathlib import Path
 
 import torch
+import GPUtil
 
 
 ###############################################################################
 # Metadata
 ###############################################################################
```

### Comparing `emphases-0.0.1/emphases/config/static.py` & `emphases-0.0.2/emphases/config/static.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/convert.py` & `emphases-0.0.2/emphases/convert.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/core.py` & `emphases-0.0.2/emphases/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/collate.py` & `emphases-0.0.2/emphases/data/collate.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/dataset.py` & `emphases-0.0.2/emphases/data/dataset.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/download/__main__.py` & `emphases-0.0.2/emphases/data/download/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/download/core.py` & `emphases-0.0.2/emphases/data/download/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/loader.py` & `emphases-0.0.2/emphases/data/loader.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/preprocess/__main__.py` & `emphases-0.0.2/emphases/data/preprocess/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/preprocess/core.py` & `emphases-0.0.2/emphases/data/preprocess/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/preprocess/loudness.py` & `emphases-0.0.2/emphases/data/preprocess/loudness.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/preprocess/mels.py` & `emphases-0.0.2/emphases/data/preprocess/mels.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/data/sampler.py` & `emphases-0.0.2/emphases/data/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,18 @@
                 ):
                     batches.append(batch)
                     max_length = length
                     batch = [index]
                 else:
                     batch.append(index)
 
+            # Don't drop last batch
+            if batch:
+                batches.append(batch)
+
         # Shuffle
         return [
             batches[i] for i in
             torch.randperm(len(batches), generator=generator).tolist()]
 
     def set_epoch(self, epoch):
         self.epoch = epoch
```

### Comparing `emphases-0.0.1/emphases/evaluate/__main__.py` & `emphases-0.0.2/emphases/evaluate/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/evaluate/core.py` & `emphases-0.0.2/emphases/evaluate/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/evaluate/metrics.py` & `emphases-0.0.2/emphases/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/model/core.py` & `emphases-0.0.2/emphases/model/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/model/layers/convolution.py` & `emphases-0.0.2/emphases/model/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/model/layers/transformer.py` & `emphases-0.0.2/emphases/model/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/partition/core.py` & `emphases-0.0.2/emphases/partition/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/plot/core.py` & `emphases-0.0.2/emphases/plot/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/plot/scaling/__main__.py` & `emphases-0.0.2/emphases/plot/scaling/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/plot/scaling/core.py` & `emphases-0.0.2/emphases/plot/scaling/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/train/__main__.py` & `emphases-0.0.2/emphases/train/__main__.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases/train/core.py` & `emphases-0.0.2/emphases/train/core.py`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/emphases.egg-info/PKG-INFO` & `emphases-0.0.2/emphases.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: emphases
-Version: 0.0.1
+Version: 0.0.2
 Summary: Crowdsourced and Automatic Speech Prominence Estimation
 Home-page: https://github.com/interactiveaudiolab/emphases
 Author: Interactive Audio Lab
 Author-email: interactiveaudiolab@gmail.com
 License: MIT
 Keywords: annotatation,audio,emphasis,prominence,speech
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: GPUtil
 Requires-Dist: huggingface-hub
 Requires-Dist: librosa
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: penn
 Requires-Dist: pycwt
 Requires-Dist: pyfoal
@@ -31,23 +32,22 @@
 
 [![PyPI](https://img.shields.io/pypi/v/emphases.svg)](https://pypi.python.org/pypi/emphases)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/badge/emphases)](https://pepy.tech/project/emphases)
 
 Annotation, training, evaluation and inference of speech prominence
 
-`pip install emphases`
-
-[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation)
+[Paper](https://www.maxrmorrison.com/pdfs/morrison2024crowdsourced.pdf) [Website](https://www.maxrmorrison.com/sites/prominence-estimation) [Dataset](https://zenodo.org/records/10402793)
 
 </div>
 
 
 ## Table of contents
 
+- [Installation](#installation)
 - [Inference](#inference)
     * [Application programming interface](#application-programming-interface)
         * [`emphases.from_alignment_and_audio`](#emphasesfrom_alignment_and_audio)
         * [`emphases.from_text_and_audio`](#emphasesfrom_text_and_audio)
         * [`emphases.from_file`](#emphasesfrom_file)
         * [`emphases.from_file_to_file`](#emphasesfrom_file_to_file)
         * [`emphases.from_files_to_files`](#emphasesfrom_files_to_files)
@@ -61,14 +61,26 @@
     * [Monitor](#monitor)
 - [Evaluation](#reproducing-results)
     * [Evaluate](#evaluate)
     * [Analyze](#analyze)
 - [Citation](#citation)
 
 
+## Installation
+
+`pip install emphases`
+
+By default, we use the Penn Phonetic Forced Aligner (P2FA) via the [`pyfoal`](https://github.com/maxrmorrison/pyfoal/)
+repo to perform word alignments. This requires installing HTK. See [the HTK
+installation instructions](https://github.com/maxrmorrison/pyfoal/tree/main?tab=readme-ov-file#penn-phonetic-forced-aligner-p2fa)
+provided by `pyfoal`. Alternatively, you can use a different forced aligner
+and either pass the alignment as a [`pypar.Alignment`](https://github.com/maxrmorrison/pypar/tree/main)
+object or save the alignment as a `.TextGrid` file.
+
+
 ## Inference
 
 Perform automatic emphasis annotation using our best pretrained model
 
 ```python
 import emphases
 
@@ -112,14 +124,15 @@
         gpu: The index of the gpu to run inference on
 
     Returns:
         scores: The float-valued emphasis scores for each word
     """
 ```
 
+
 #### `emphases.from_text_and_audio`
 
 ```python
 def from_text_and_audio(
     text: str,
     audio: torch.Tensor,
     sample_rate: int,
```

### Comparing `emphases-0.0.1/emphases.egg-info/SOURCES.txt` & `emphases-0.0.2/emphases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emphases-0.0.1/setup.py` & `emphases-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 with open('README.md', encoding='utf8') as file:
     long_description = file.read()
 
 
 setup(
     name='emphases',
     description='Crowdsourced and Automatic Speech Prominence Estimation',
-    version='0.0.1',
+    version='0.0.2',
     author='Interactive Audio Lab',
     author_email='interactiveaudiolab@gmail.com',
     url='https://github.com/interactiveaudiolab/emphases',
     install_requires=[
+        'GPUtil',
         'huggingface-hub',
         'librosa',
         'matplotlib',
         'numpy',
         'penn',
         'pycwt',
         'pyfoal',
```

