# Comparing `tmp/geotils-0.0.20.tar.gz` & `tmp/geotils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotils-0.0.20.tar", last modified: Fri Mar 22 06:52:23 2024, max compression
+gzip compressed data, was "geotils-0.1.7.tar", last modified: Sat Apr 13 04:18:55 2024, max compression
```

## Comparing `geotils-0.0.20.tar` & `geotils-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:52:23.012396 geotils-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-22 06:52:23.012396 geotils-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 06:52:16.000000 geotils-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:52:23.012396 geotils-0.0.20/geotils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-22 06:52:23.000000 geotils-0.0.20/geotils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-22 06:52:23.000000 geotils-0.0.20/geotils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 06:52:23.000000 geotils-0.0.20/geotils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-22 06:52:23.000000 geotils-0.0.20/geotils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 06:52:23.000000 geotils-0.0.20/geotils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 06:52:23.012396 geotils-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 06:52:16.000000 geotils-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.130694 geotils-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 04:18:46.000000 geotils-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 04:18:55.130694 geotils-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-13 04:18:46.000000 geotils-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.114694 geotils-0.1.7/geotils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.118694 geotils-0.1.7/geotils/ToBeChecked/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.118694 geotils-0.1.7/geotils/ToBeChecked/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/losses/lovasz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.118694 geotils-0.1.7/geotils/ToBeChecked/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/meters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/test_meters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.118694 geotils-0.1.7/geotils/ToBeChecked/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/models/ASPP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/models/OCR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/models/RA_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/models/Unet_W_Mods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/models/pred_SAM.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.122694 geotils-0.1.7/geotils/ToBeChecked/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/utility/modify_contact_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/ToBeChecked/utility/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.122694 geotils-0.1.7/geotils/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25720 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/make_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15714 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/polygon_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/data_processing/transform_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.122694 geotils-0.1.7/geotils/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/dataset/FloodNet_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/dataset/Planet_Dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/dataset/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/dataset/sentinel_1_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10559 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/dataset/sentinel_2_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.126694 geotils-0.1.7/geotils/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/logging/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/logging/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.126694 geotils-0.1.7/geotils/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/adamw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.126694 geotils-0.1.7/geotils/optimizers/over9000/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/adabelief.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/adamod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/adan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/apollo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/diffgrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/madam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/madgrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/radam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/ralamb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/over9000/rangerlars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/optimizers/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.130694 geotils-0.1.7/geotils/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/schedulers/polylr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/schedulers/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.130694 geotils-0.1.7/geotils/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)    25720 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/visualization/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-13 04:18:46.000000 geotils-0.1.7/geotils/visualization/masking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:18:55.130694 geotils-0.1.7/geotils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 04:18:55.000000 geotils-0.1.7/geotils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-13 04:18:46.000000 geotils-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:18:55.130694 geotils-0.1.7/setup.cfg
```

