# Comparing `tmp/unscribe-0.0.1.tar.gz` & `tmp/unscribe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unscribe-0.0.1.tar", last modified: Thu Apr 11 23:19:25 2024, max compression
+gzip compressed data, was "unscribe-0.0.2.tar", last modified: Sat Apr 13 16:58:12 2024, max compression
```

## Comparing `unscribe-0.0.1.tar` & `unscribe-0.0.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.096012 unscribe-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 23:19:21.000000 unscribe-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-11 23:19:25.096012 unscribe-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-11 23:19:21.000000 unscribe-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:19:25.096012 unscribe-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-11 23:19:21.000000 unscribe-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.076012 unscribe-0.0.1/unscribe/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/cpu_refiner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.076012 unscribe-0.0.1/unscribe/saicinpainting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.080012 unscribe-0.0.1/unscribe/saicinpainting/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.080012 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23234 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/base_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.080012 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/fid_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/inception.py
--rw-r--r--   0 runner    (1001) docker     (127)    33621 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.084012 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.084012 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/countless2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/countless3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/evaluation/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.084012 unscribe-0.0.1/unscribe/saicinpainting/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.084012 unscribe-0.0.1/unscribe/saicinpainting/training/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/data/aug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/data/masks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.088012 unscribe-0.0.1/unscribe/saicinpainting/training/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/feature_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/losses/style_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.092012 unscribe-0.0.1/unscribe/saicinpainting/training/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/depthwise_sep_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/fake_fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/ffc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/multidilated_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/multiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)    27991 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/pix2pixhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/spatial_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/modules/squeeze_excitation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.092012 unscribe-0.0.1/unscribe/saicinpainting/training/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/trainers/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.092012 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/saicinpainting/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-11 23:19:21.000000 unscribe-0.0.1/unscribe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:19:25.096012 unscribe-0.0.1/unscribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-11 23:19:25.000000 unscribe-0.0.1/unscribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-11 23:19:25.000000 unscribe-0.0.1/unscribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:19:25.000000 unscribe-0.0.1/unscribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 23:19:25.000000 unscribe-0.0.1/unscribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 23:19:25.000000 unscribe-0.0.1/unscribe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.920349 unscribe-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 16:58:08.000000 unscribe-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-13 16:58:12.920349 unscribe-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-13 16:58:08.000000 unscribe-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:58:12.920349 unscribe-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-13 16:58:08.000000 unscribe-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.900349 unscribe-0.0.2/unscribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/cpu_refiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.900349 unscribe-0.0.2/unscribe/saicinpainting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.904349 unscribe-0.0.2/unscribe/saicinpainting/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.904349 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23234 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/base_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.908349 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12179 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/fid_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/inception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33621 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.908349 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.908349 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/countless2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-13 16:58:08.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/countless3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/evaluation/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.908349 unscribe-0.0.2/unscribe/saicinpainting/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.912349 unscribe-0.0.2/unscribe/saicinpainting/training/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/data/aug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13706 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/data/masks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.912349 unscribe-0.0.2/unscribe/saicinpainting/training/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/feature_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/losses/style_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.916349 unscribe-0.0.2/unscribe/saicinpainting/training/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/depthwise_sep_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/fake_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/ffc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/multidilated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/multiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27991 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/pix2pixhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/spatial_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/modules/squeeze_excitation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.916349 unscribe-0.0.2/unscribe/saicinpainting/training/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/trainers/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.920349 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/saicinpainting/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-13 16:58:09.000000 unscribe-0.0.2/unscribe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:58:12.920349 unscribe-0.0.2/unscribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-13 16:58:12.000000 unscribe-0.0.2/unscribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-13 16:58:12.000000 unscribe-0.0.2/unscribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:58:12.000000 unscribe-0.0.2/unscribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 16:58:12.000000 unscribe-0.0.2/unscribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 16:58:12.000000 unscribe-0.0.2/unscribe.egg-info/top_level.txt
```

### Comparing `unscribe-0.0.1/LICENSE` & `unscribe-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/PKG-INFO` & `unscribe-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unscribe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A straightforward text remover and/or scrambler using LaMa inpainting and CRAFT text-detection
 Home-page: https://github.com/manbehindthemadness/modern-craft
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,15 @@
 Requires-Dist: wldhx.yadisk-direct
 Requires-Dist: tensorflow
 Requires-Dist: opencv-python>=3.4.2.17
 Requires-Dist: torch>=2.0.0
 Requires-Dist: pytorch-lightning==1.2.9
 Requires-Dist: kornia==0.5.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 # Unscribe
 
 Unscribe is a Python library for text removal and scrambling in images using LaMa inpainting and CRAFT text detection.
 
 ## Diagrams:
 ### The following techniques were used in the creation of this project:
```

### Comparing `unscribe-0.0.1/README.md` & `unscribe-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/setup.py` & `unscribe-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     'packaging',
     'wldhx.yadisk-direct',
     'tensorflow',
     'opencv-python>=3.4.2.17',
     'torch>=2.0.0',
     'pytorch-lightning==1.2.9',
     'kornia==0.5.0',
-    'torchvision>=0.17.0'
+    'torchvision>=0.17.0',
+    'quickdl',
 ]
 
 exclusions = [
     'torch',
     'torchvision',
     'kornia',
     'tensorflow',
@@ -46,15 +47,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='unscribe',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

### Comparing `unscribe-0.0.1/unscribe/cpu_refiner.py` & `unscribe-0.0.2/unscribe/cpu_refiner.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/main.py` & `unscribe-0.0.2/unscribe/main.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/__init__.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/data.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/data.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/evaluator.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/base_loss.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/base_loss.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/fid_score.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/fid_score.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/fid/inception.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/fid/inception.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/lpips.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/losses/ssim.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/losses/ssim.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/countless2d.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/countless2d.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/countless3d.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/countless3d.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/countless/test.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/countless/test.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/masks/mask.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/masks/mask.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/refinement.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/refinement.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/utils.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/evaluation/vis.py` & `unscribe-0.0.2/unscribe/saicinpainting/evaluation/vis.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/data/aug.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/data/aug.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/data/datasets.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/data/datasets.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/data/masks.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/data/masks.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/adversarial.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/adversarial.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/constants.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/constants.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/distance_weighting.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/feature_matching.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/feature_matching.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/perceptual.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/perceptual.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/segmentation.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/segmentation.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/losses/style_loss.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/losses/style_loss.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/__init__.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/base.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/base.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/depthwise_sep_conv.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/depthwise_sep_conv.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/fake_fakes.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/fake_fakes.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/ffc.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/ffc.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/multidilated_conv.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/multidilated_conv.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/multiscale.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/multiscale.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/pix2pixhd.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/pix2pixhd.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/spatial_transform.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/spatial_transform.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/modules/squeeze_excitation.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/modules/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/trainers/__init__.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/trainers/base.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/trainers/base.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/trainers/default.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/trainers/default.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/base.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/base.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/colors.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/colors.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/training/visualizers/directory.py` & `unscribe-0.0.2/unscribe/saicinpainting/training/visualizers/directory.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/saicinpainting/utils.py` & `unscribe-0.0.2/unscribe/saicinpainting/utils.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe/utils.py` & `unscribe-0.0.2/unscribe/utils.py`

 * *Files identical despite different names*

### Comparing `unscribe-0.0.1/unscribe.egg-info/PKG-INFO` & `unscribe-0.0.2/unscribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unscribe
-Version: 0.0.1
+Version: 0.0.2
 Summary: A straightforward text remover and/or scrambler using LaMa inpainting and CRAFT text-detection
 Home-page: https://github.com/manbehindthemadness/modern-craft
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,14 +31,15 @@
 Requires-Dist: wldhx.yadisk-direct
 Requires-Dist: tensorflow
 Requires-Dist: opencv-python>=3.4.2.17
 Requires-Dist: torch>=2.0.0
 Requires-Dist: pytorch-lightning==1.2.9
 Requires-Dist: kornia==0.5.0
 Requires-Dist: torchvision>=0.17.0
+Requires-Dist: quickdl
 
 # Unscribe
 
 Unscribe is a Python library for text removal and scrambling in images using LaMa inpainting and CRAFT text detection.
 
 ## Diagrams:
 ### The following techniques were used in the creation of this project:
```

### Comparing `unscribe-0.0.1/unscribe.egg-info/SOURCES.txt` & `unscribe-0.0.2/unscribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

