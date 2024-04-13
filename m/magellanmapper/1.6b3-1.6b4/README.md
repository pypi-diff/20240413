# Comparing `tmp/magellanmapper-1.6b3.tar.gz` & `tmp/magellanmapper-1.6b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magellanmapper-1.6b3.tar", last modified: Mon Sep 25 17:56:20 2023, max compression
+gzip compressed data, was "magellanmapper-1.6b4.tar", last modified: Sat Apr 13 18:06:56 2024, max compression
```

## Comparing `magellanmapper-1.6b3.tar` & `magellanmapper-1.6b4.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.473367 magellanmapper-1.6b3/
--rw-r--r--   0 david      (501) staff       (20)     1494 2023-02-23 09:32:04.000000 magellanmapper-1.6b3/LICENSE.txt
--rw-r--r--   0 david      (501) staff       (20)     9493 2023-09-25 17:56:20.472470 magellanmapper-1.6b3/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     5526 2023-09-12 21:28:24.000000 magellanmapper-1.6b3/README.md
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.425330 magellanmapper-1.6b3/magellanmapper.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     9493 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/PKG-INFO
--rwxrwxrwx   0 david      (501) staff       (20)     2299 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/SOURCES.txt
--rwxrwxrwx   0 david      (501) staff       (20)        1 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)       56 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/entry_points.txt
--rwxrwxrwx   0 david      (501) staff       (20)     1474 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/requires.txt
--rwxrwxrwx   0 david      (501) staff       (20)        7 2023-09-25 17:56:20.000000 magellanmapper-1.6b3/magellanmapper.egg-info/top_level.txt
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.425649 magellanmapper-1.6b3/magmap/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/__init__.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.428881 magellanmapper-1.6b3/magmap/atlas/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/atlas/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    81279 2023-05-26 10:20:20.000000 magellanmapper-1.6b3/magmap/atlas/atlas_refiner.py
--rw-r--r--   0 david      (501) staff       (20)    25960 2023-05-26 10:20:20.000000 magellanmapper-1.6b3/magmap/atlas/edge_seg.py
--rw-r--r--   0 david      (501) staff       (20)     3922 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/atlas/labels_meta.py
--rw-r--r--   0 david      (501) staff       (20)    38422 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/atlas/ontology.py
--rw-r--r--   0 david      (501) staff       (20)     2360 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/atlas/reg_tasks.py
--rw-r--r--   0 david      (501) staff       (20)   118340 2023-05-26 10:20:20.000000 magellanmapper-1.6b3/magmap/atlas/register.py
--rw-r--r--   0 david      (501) staff       (20)    15407 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/atlas/transformer.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.429697 magellanmapper-1.6b3/magmap/brain_globe/
--rw-r--r--   0 david      (501) staff       (20)        0 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/brain_globe/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     6795 2023-05-25 02:14:02.000000 magellanmapper-1.6b3/magmap/brain_globe/bg_controller.py
--rw-r--r--   0 david      (501) staff       (20)     3793 2023-05-25 02:14:02.000000 magellanmapper-1.6b3/magmap/brain_globe/bg_model.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.430496 magellanmapper-1.6b3/magmap/cloud/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/cloud/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    17599 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/cloud/aws.py
--rw-r--r--   0 david      (501) staff       (20)     1025 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/cloud/notify.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.433711 magellanmapper-1.6b3/magmap/cv/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/cv/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    16242 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/cv/chunking.py
--rw-r--r--   0 david      (501) staff       (20)    13197 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/cv/classifier.py
--rw-r--r--   0 david      (501) staff       (20)    25002 2023-09-12 21:28:24.000000 magellanmapper-1.6b3/magmap/cv/colocalizer.py
--rw-r--r--   0 david      (501) staff       (20)    48741 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/cv/cv_nd.py
--rw-r--r--   0 david      (501) staff       (20)    44617 2023-03-28 06:06:07.000000 magellanmapper-1.6b3/magmap/cv/detector.py
--rw-r--r--   0 david      (501) staff       (20)    34565 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/cv/segmenter.py
--rw-r--r--   0 david      (501) staff       (20)    38066 2023-03-14 04:55:52.000000 magellanmapper-1.6b3/magmap/cv/stack_detect.py
--rw-r--r--   0 david      (501) staff       (20)    31081 2023-03-01 03:52:31.000000 magellanmapper-1.6b3/magmap/cv/verifier.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.437743 magellanmapper-1.6b3/magmap/gui/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/gui/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    23650 2023-05-23 02:34:50.000000 magellanmapper-1.6b3/magmap/gui/atlas_editor.py
--rw-r--r--   0 david      (501) staff       (20)     3121 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/gui/atlas_threads.py
--rw-r--r--   0 david      (501) staff       (20)     1806 2023-02-23 09:31:38.000000 magellanmapper-1.6b3/magmap/gui/event_handlers.py
--rw-r--r--   0 david      (501) staff       (20)     3615 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/gui/image_viewer.py
--rw-r--r--   0 david      (501) staff       (20)     3978 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/gui/import_threads.py
--rw-r--r--   0 david      (501) staff       (20)     5375 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/gui/pixel_display.py
--rw-r--r--   0 david      (501) staff       (20)    59511 2023-09-21 00:04:33.000000 magellanmapper-1.6b3/magmap/gui/plot_editor.py
--rw-r--r--   0 david      (501) staff       (20)    68950 2023-05-23 02:34:50.000000 magellanmapper-1.6b3/magmap/gui/roi_editor.py
--rw-r--r--   0 david      (501) staff       (20)    10029 2023-05-23 02:34:50.000000 magellanmapper-1.6b3/magmap/gui/verifier_editor.py
--rw-r--r--   0 david      (501) staff       (20)    27143 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/gui/vis_3d.py
--rw-r--r--   0 david      (501) staff       (20)     7879 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/gui/vis_handler.py
--rw-r--r--   0 david      (501) staff       (20)   175982 2023-09-21 17:46:27.000000 magellanmapper-1.6b3/magmap/gui/visualizer.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.443827 magellanmapper-1.6b3/magmap/io/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/io/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    51776 2023-03-01 03:52:31.000000 magellanmapper-1.6b3/magmap/io/cli.py
--rw-r--r--   0 david      (501) staff       (20)    33806 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/io/df_io.py
--rw-r--r--   0 david      (501) staff       (20)    23388 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/io/export_regions.py
--rw-r--r--   0 david      (501) staff       (20)    12799 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/io/export_rois.py
--rw-r--r--   0 david      (501) staff       (20)    30084 2023-03-23 09:27:19.000000 magellanmapper-1.6b3/magmap/io/export_stack.py
--rw-r--r--   0 david      (501) staff       (20)    57289 2023-05-26 08:17:29.000000 magellanmapper-1.6b3/magmap/io/importer.py
--rw-r--r--   0 david      (501) staff       (20)    45460 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/io/libmag.py
--rw-r--r--   0 david      (501) staff       (20)     9040 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/io/load_env.py
--rw-r--r--   0 david      (501) staff       (20)     2019 2023-02-23 09:32:04.000000 magellanmapper-1.6b3/magmap/io/naming.py
--rw-r--r--   0 david      (501) staff       (20)    29200 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/io/np_io.py
--rw-r--r--   0 david      (501) staff       (20)     1306 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/io/packaging.py
--rw-r--r--   0 david      (501) staff       (20)    31994 2023-09-21 00:05:58.000000 magellanmapper-1.6b3/magmap/io/sitk_io.py
--rw-r--r--   0 david      (501) staff       (20)    38964 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/io/sqlite.py
--rw-r--r--   0 david      (501) staff       (20)     3506 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/io/subproc_io.py
--rw-r--r--   0 david      (501) staff       (20)     4464 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/io/yaml_io.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.446516 magellanmapper-1.6b3/magmap/plot/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/plot/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    24433 2023-09-21 17:37:07.000000 magellanmapper-1.6b3/magmap/plot/colormaps.py
--rw-r--r--   0 david      (501) staff       (20)    67349 2023-09-21 17:40:46.000000 magellanmapper-1.6b3/magmap/plot/plot_2d.py
--rw-r--r--   0 david      (501) staff       (20)    21808 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/plot/plot_3d.py
--rw-r--r--   0 david      (501) staff       (20)    63766 2023-05-26 10:20:20.000000 magellanmapper-1.6b3/magmap/plot/plot_support.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.450494 magellanmapper-1.6b3/magmap/settings/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/settings/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    32468 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/settings/atlas_prof.py
--rw-r--r--   0 david      (501) staff       (20)    28302 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/settings/config.py
--rw-r--r--   0 david      (501) staff       (20)     6062 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/settings/grid_search_prof.py
--rw-r--r--   0 david      (501) staff       (20)     5177 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/settings/logs.py
--rw-r--r--   0 david      (501) staff       (20)      737 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/settings/prefs_prof.py
--rw-r--r--   0 david      (501) staff       (20)    11658 2023-03-02 09:33:47.000000 magellanmapper-1.6b3/magmap/settings/profiles.py
--rw-r--r--   0 david      (501) staff       (20)    12968 2023-06-23 03:30:25.000000 magellanmapper-1.6b3/magmap/settings/roi_prof.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.452911 magellanmapper-1.6b3/magmap/stats/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/stats/__init__.py
--rw-r--r--   0 david      (501) staff       (20)    25579 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/stats/atlas_stats.py
--rw-r--r--   0 david      (501) staff       (20)    11323 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/stats/clustering.py
--rw-r--r--   0 david      (501) staff       (20)     7132 2023-03-10 04:16:58.000000 magellanmapper-1.6b3/magmap/stats/mlearn.py
--rw-r--r--   0 david      (501) staff       (20)    57728 2023-04-15 05:02:22.000000 magellanmapper-1.6b3/magmap/stats/vols.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-09-25 17:56:20.457490 magellanmapper-1.6b3/magmap/tests/
--rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/tests/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2561 2023-02-23 09:32:04.000000 magellanmapper-1.6b3/magmap/tests/test_chunking.py
--rw-r--r--   0 david      (501) staff       (20)     1806 2023-03-28 06:06:29.000000 magellanmapper-1.6b3/magmap/tests/test_classifier.py
--rw-r--r--   0 david      (501) staff       (20)     1815 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/tests/test_cv_nd.py
--rw-r--r--   0 david      (501) staff       (20)     2559 2023-03-28 06:06:07.000000 magellanmapper-1.6b3/magmap/tests/test_detector.py
--rw-r--r--   0 david      (501) staff       (20)     1134 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/tests/test_img_equality.py
--rw-r--r--   0 david      (501) staff       (20)     8089 2023-05-25 02:14:09.000000 magellanmapper-1.6b3/magmap/tests/test_libmag.py
--rw-r--r--   0 david      (501) staff       (20)     2481 2023-02-23 09:44:57.000000 magellanmapper-1.6b3/magmap/tests/test_visualizer.py
--rw-r--r--   0 david      (501) staff       (20)     1377 2022-08-03 03:32:45.000000 magellanmapper-1.6b3/magmap/tests/unit_testing.py
--rw-r--r--   0 david      (501) staff       (20)       38 2023-09-25 17:56:20.473533 magellanmapper-1.6b3/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)     4152 2023-09-25 17:56:01.000000 magellanmapper-1.6b3/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.472429 magellanmapper-1.6b4/
+-rw-r--r--   0 david      (501) staff       (20)     1494 2023-02-23 09:32:04.000000 magellanmapper-1.6b4/LICENSE.txt
+-rw-r--r--   0 david      (501) staff       (20)     9563 2024-04-13 18:06:56.471632 magellanmapper-1.6b4/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     5621 2024-04-12 03:36:59.000000 magellanmapper-1.6b4/README.md
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.456241 magellanmapper-1.6b4/magellanmapper.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     9563 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/PKG-INFO
+-rwxrwxrwx   0 david      (501) staff       (20)     2326 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/SOURCES.txt
+-rwxrwxrwx   0 david      (501) staff       (20)        1 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)       56 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/entry_points.txt
+-rwxrwxrwx   0 david      (501) staff       (20)     1482 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/requires.txt
+-rwxrwxrwx   0 david      (501) staff       (20)        7 2024-04-13 18:06:56.000000 magellanmapper-1.6b4/magellanmapper.egg-info/top_level.txt
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.395484 magellanmapper-1.6b4/magmap/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/__init__.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.402122 magellanmapper-1.6b4/magmap/atlas/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/atlas/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    81279 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/atlas/atlas_refiner.py
+-rw-r--r--   0 david      (501) staff       (20)    25960 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/atlas/edge_seg.py
+-rw-r--r--   0 david      (501) staff       (20)     3922 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/atlas/labels_meta.py
+-rw-r--r--   0 david      (501) staff       (20)    38422 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/atlas/ontology.py
+-rw-r--r--   0 david      (501) staff       (20)     2681 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/atlas/reg_tasks.py
+-rw-r--r--   0 david      (501) staff       (20)   118954 2024-04-12 03:16:04.000000 magellanmapper-1.6b4/magmap/atlas/register.py
+-rw-r--r--   0 david      (501) staff       (20)    15407 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/atlas/transformer.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.403954 magellanmapper-1.6b4/magmap/brain_globe/
+-rw-r--r--   0 david      (501) staff       (20)        0 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/brain_globe/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     6795 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/brain_globe/bg_controller.py
+-rw-r--r--   0 david      (501) staff       (20)     3793 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/brain_globe/bg_model.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.406463 magellanmapper-1.6b4/magmap/cloud/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/cloud/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    17599 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/cloud/aws.py
+-rw-r--r--   0 david      (501) staff       (20)     1025 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/cloud/notify.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.415324 magellanmapper-1.6b4/magmap/cv/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/cv/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    16242 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/cv/chunking.py
+-rw-r--r--   0 david      (501) staff       (20)    13197 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/cv/classifier.py
+-rw-r--r--   0 david      (501) staff       (20)    25002 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/cv/colocalizer.py
+-rw-r--r--   0 david      (501) staff       (20)    48741 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/cv/cv_nd.py
+-rw-r--r--   0 david      (501) staff       (20)    44496 2024-03-12 20:40:28.000000 magellanmapper-1.6b4/magmap/cv/detector.py
+-rw-r--r--   0 david      (501) staff       (20)    34565 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/cv/segmenter.py
+-rw-r--r--   0 david      (501) staff       (20)    38066 2024-03-12 02:15:21.000000 magellanmapper-1.6b4/magmap/cv/stack_detect.py
+-rw-r--r--   0 david      (501) staff       (20)    31081 2023-03-01 03:52:31.000000 magellanmapper-1.6b4/magmap/cv/verifier.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.426790 magellanmapper-1.6b4/magmap/gui/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/gui/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    23650 2024-02-09 01:24:46.000000 magellanmapper-1.6b4/magmap/gui/atlas_editor.py
+-rw-r--r--   0 david      (501) staff       (20)     3121 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/gui/atlas_threads.py
+-rw-r--r--   0 david      (501) staff       (20)     1806 2023-02-23 09:31:38.000000 magellanmapper-1.6b4/magmap/gui/event_handlers.py
+-rw-r--r--   0 david      (501) staff       (20)     3615 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/gui/image_viewer.py
+-rw-r--r--   0 david      (501) staff       (20)     3978 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/gui/import_threads.py
+-rw-r--r--   0 david      (501) staff       (20)     5375 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/gui/pixel_display.py
+-rw-r--r--   0 david      (501) staff       (20)    60690 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/gui/plot_editor.py
+-rw-r--r--   0 david      (501) staff       (20)    68953 2024-03-12 20:40:28.000000 magellanmapper-1.6b4/magmap/gui/roi_editor.py
+-rw-r--r--   0 david      (501) staff       (20)    10029 2024-02-09 01:24:46.000000 magellanmapper-1.6b4/magmap/gui/verifier_editor.py
+-rw-r--r--   0 david      (501) staff       (20)    27143 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/gui/vis_3d.py
+-rw-r--r--   0 david      (501) staff       (20)     7879 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/gui/vis_handler.py
+-rw-r--r--   0 david      (501) staff       (20)   178614 2024-02-22 23:25:08.000000 magellanmapper-1.6b4/magmap/gui/visualizer.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.438599 magellanmapper-1.6b4/magmap/io/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/io/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    51776 2023-03-01 03:52:31.000000 magellanmapper-1.6b4/magmap/io/cli.py
+-rw-r--r--   0 david      (501) staff       (20)    33806 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/io/df_io.py
+-rw-r--r--   0 david      (501) staff       (20)    23562 2024-03-12 20:40:28.000000 magellanmapper-1.6b4/magmap/io/export_regions.py
+-rw-r--r--   0 david      (501) staff       (20)    12799 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/io/export_rois.py
+-rw-r--r--   0 david      (501) staff       (20)    30824 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/io/export_stack.py
+-rw-r--r--   0 david      (501) staff       (20)    57289 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/io/importer.py
+-rw-r--r--   0 david      (501) staff       (20)    45460 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/io/libmag.py
+-rw-r--r--   0 david      (501) staff       (20)     9040 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/io/load_env.py
+-rw-r--r--   0 david      (501) staff       (20)     2019 2023-02-23 09:32:04.000000 magellanmapper-1.6b4/magmap/io/naming.py
+-rw-r--r--   0 david      (501) staff       (20)    29614 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/io/np_io.py
+-rw-r--r--   0 david      (501) staff       (20)     1306 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/io/packaging.py
+-rw-r--r--   0 david      (501) staff       (20)    31994 2024-04-12 02:13:23.000000 magellanmapper-1.6b4/magmap/io/sitk_io.py
+-rw-r--r--   0 david      (501) staff       (20)    38964 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/io/sqlite.py
+-rw-r--r--   0 david      (501) staff       (20)     3506 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/io/subproc_io.py
+-rw-r--r--   0 david      (501) staff       (20)     4464 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/io/yaml_io.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.441546 magellanmapper-1.6b4/magmap/plot/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/plot/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    24586 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/plot/colormaps.py
+-rw-r--r--   0 david      (501) staff       (20)    67743 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/plot/plot_2d.py
+-rw-r--r--   0 david      (501) staff       (20)    21808 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/plot/plot_3d.py
+-rw-r--r--   0 david      (501) staff       (20)    64205 2024-03-12 02:15:21.000000 magellanmapper-1.6b4/magmap/plot/plot_support.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.446392 magellanmapper-1.6b4/magmap/settings/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/settings/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    32468 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/settings/atlas_prof.py
+-rw-r--r--   0 david      (501) staff       (20)    28302 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/settings/config.py
+-rw-r--r--   0 david      (501) staff       (20)     6062 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/settings/grid_search_prof.py
+-rw-r--r--   0 david      (501) staff       (20)     5177 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/settings/logs.py
+-rw-r--r--   0 david      (501) staff       (20)      804 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/settings/prefs_prof.py
+-rw-r--r--   0 david      (501) staff       (20)    11658 2023-03-02 09:33:47.000000 magellanmapper-1.6b4/magmap/settings/profiles.py
+-rw-r--r--   0 david      (501) staff       (20)    12939 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/settings/roi_prof.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.449721 magellanmapper-1.6b4/magmap/stats/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/stats/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)    25579 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/stats/atlas_stats.py
+-rw-r--r--   0 david      (501) staff       (20)    11323 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/stats/clustering.py
+-rw-r--r--   0 david      (501) staff       (20)     7132 2023-03-10 04:16:58.000000 magellanmapper-1.6b4/magmap/stats/mlearn.py
+-rw-r--r--   0 david      (501) staff       (20)    57728 2024-02-09 01:23:09.000000 magellanmapper-1.6b4/magmap/stats/vols.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2024-04-13 18:06:56.455460 magellanmapper-1.6b4/magmap/tests/
+-rw-r--r--   0 david      (501) staff       (20)        0 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/tests/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2561 2023-02-23 09:32:04.000000 magellanmapper-1.6b4/magmap/tests/test_chunking.py
+-rw-r--r--   0 david      (501) staff       (20)     1806 2024-02-09 01:23:09.000000 magellanmapper-1.6b4/magmap/tests/test_classifier.py
+-rw-r--r--   0 david      (501) staff       (20)     1815 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/tests/test_cv_nd.py
+-rw-r--r--   0 david      (501) staff       (20)     2559 2024-02-09 01:23:09.000000 magellanmapper-1.6b4/magmap/tests/test_detector.py
+-rw-r--r--   0 david      (501) staff       (20)     1134 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/tests/test_img_equality.py
+-rw-r--r--   0 david      (501) staff       (20)     8089 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/tests/test_libmag.py
+-rw-r--r--   0 david      (501) staff       (20)      840 2024-02-09 01:28:53.000000 magellanmapper-1.6b4/magmap/tests/test_np_io.py
+-rw-r--r--   0 david      (501) staff       (20)     2481 2023-02-23 09:44:57.000000 magellanmapper-1.6b4/magmap/tests/test_visualizer.py
+-rw-r--r--   0 david      (501) staff       (20)     1377 2022-08-03 03:32:45.000000 magellanmapper-1.6b4/magmap/tests/unit_testing.py
+-rw-r--r--   0 david      (501) staff       (20)       38 2024-04-13 18:06:56.472572 magellanmapper-1.6b4/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)     4372 2024-04-13 00:55:35.000000 magellanmapper-1.6b4/setup.py
```

### Comparing `magellanmapper-1.6b3/LICENSE.txt` & `magellanmapper-1.6b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/PKG-INFO` & `magellanmapper-1.6b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magellanmapper
-Version: 1.6b3
+Version: 1.6b4
 Summary: 3D atlas analysis and annotation
 Home-page: https://github.com/sanderslab/magellanmapper
 Author: David Young
 Author-email: david@textflex.com
 License: BSD-3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -43,27 +43,26 @@
 Requires-Dist: tensorflow; extra == "classifier"
 Provides-Extra: gui
 Requires-Dist: PyQt5!=5.15.8; extra == "gui"
 Requires-Dist: pyface; extra == "gui"
 Requires-Dist: traitsui; extra == "gui"
 Provides-Extra: 3d
 Requires-Dist: mayavi; extra == "3d"
+Requires-Dist: vtk<9.3.0; extra == "3d"
 Provides-Extra: itk
-Requires-Dist: itk; extra == "itk"
 Requires-Dist: itk-elastix; extra == "itk"
 Provides-Extra: simplitk
 Requires-Dist: simpleitk==2.0.2rc2.dev785+g8ac4f; python_version < "3.8" and extra == "simplitk"
 Requires-Dist: simpleitk==2.3.0.dev117+g0640d; python_version >= "3.8" and extra == "simplitk"
 Provides-Extra: most
 Requires-Dist: matplotlib_scalebar; extra == "most"
 Requires-Dist: pyamg; extra == "most"
 Requires-Dist: PyQt5!=5.15.8; extra == "most"
 Requires-Dist: pyface; extra == "most"
 Requires-Dist: traitsui; extra == "most"
-Requires-Dist: itk; extra == "most"
 Requires-Dist: itk-elastix; extra == "most"
 Requires-Dist: javabridge==1.0.19.post4+gbebed64; python_version < "3.8" and extra == "most"
 Requires-Dist: javabridge==1.0.19.post9+gc8c12b4; python_version >= "3.8" and extra == "most"
 Requires-Dist: python-bioformats==4.0.5.post2+g51eb88a; python_version < "3.8" and extra == "most"
 Requires-Dist: python-bioformats==4.0.7.post5+g52309d1; python_version >= "3.8" and extra == "most"
 Provides-Extra: all
 Requires-Dist: matplotlib_scalebar; extra == "all"
@@ -71,83 +70,98 @@
 Requires-Dist: seaborn; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: PyQt5!=5.15.8; extra == "all"
 Requires-Dist: pyface; extra == "all"
 Requires-Dist: traitsui; extra == "all"
 Requires-Dist: openpyxl; extra == "all"
 Requires-Dist: jinja2; extra == "all"
-Requires-Dist: itk; extra == "all"
 Requires-Dist: itk-elastix; extra == "all"
 Requires-Dist: javabridge==1.0.19.post4+gbebed64; python_version < "3.8" and extra == "all"
 Requires-Dist: javabridge==1.0.19.post9+gc8c12b4; python_version >= "3.8" and extra == "all"
 Requires-Dist: python-bioformats==4.0.5.post2+g51eb88a; python_version < "3.8" and extra == "all"
 Requires-Dist: python-bioformats==4.0.7.post5+g52309d1; python_version >= "3.8" and extra == "all"
 Requires-Dist: boto3; extra == "all"
 Requires-Dist: awscli; extra == "all"
 Requires-Dist: jupyterlab; extra == "all"
 Requires-Dist: bash_kernel; extra == "all"
 Requires-Dist: mayavi; extra == "all"
+Requires-Dist: vtk<9.3.0; extra == "all"
 
 # MagellanMapper
 
 MagellanMapper is a graphical imaging informatics suite for 3D reconstruction and automated analysis of whole specimens and atlases. Its design philosophy is to make the raw 3D images as accessible as possible, simplify annotation from nuclei to atlases, and scale from the laptop or desktop to the cloud in cross-platform environments.
 
 ![ROI Editor and Atlas Editor screenshots](https://user-images.githubusercontent.com/1258953/195321971-955fc46a-f44d-4282-8c78-21708ebaeef1.png)
 
 <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7781073/"><img align="right" width="200" src="https://user-images.githubusercontent.com/1258953/179440433-0326c4d5-9a9b-4bae-92c7-d09416375bc5.png" title="Current Protocols cover image"></a>
 
 
 ## Quick Reference
 
-- **NEW**: [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
-- [Installation](#installation) (more [details](docs/install.md))
+- [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
+- **NEW**: [Vignette of pipelines](bin/sample_cmds_bash.ipynb)
+- [Installation](#quick-install) (more [details](docs/install.md))
 - [Intro to running MagellanMapper](#run-magellanmapper)
 - [Using the viewers](docs/viewers.md)
 - [Command-line interface](docs/cli.md)
 - [Configuration and settings](docs/settings.md)
 - [Publications](#related-publications-and-datasets)
 
 
-## Installation
+## Quick Install
 
-If you use Conda (available [here](https://docs.conda.io/en/latest/miniconda.html)), you can install MagellanMapper into a new environment:
+Install MagellanMapper with its graphical interface and registration tools:
+
+```shell
+pip install "magellanmapper[gui,itk]"
+```
+
+Then launch MagellanMapper:
+
+```shell
+mm
+```
+
+## Full Install
+
+Alternatively, [Conda](https://docs.conda.io/en/latest/miniconda.html) can be used to install MagellanMapper along with support for importing proprietary image file formats (*note: not currently working on Apple Silicon (Mac M-chip) platforms*):
 
 ```shell
 conda env create -n mag -f https://raw.githubusercontent.com/sanderslab/magellanmapper/master/envs/environment_rel.yml
 ```
 
-To run in this new environment named `mag`<sup>*</sup>:
+Then activate the environment (`mag`) and run MagellanMapper:
 
 ```shell
 conda activate mag
 mm
 ```
 
-<sup>*</sup> `mm` was added in v1.6.0 to launch from installed packages
-
-Or install using Pip ([virtual environment]((https://realpython.com/python-virtual-environments-a-primer/)) recommended):
+If you have [Java](https://www.azul.com/downloads/?package=jdk), you can do the same through Pip:
 
 ```shell
 pip install "magellanmapper[most]" --extra-index-url https://pypi.fury.io/dd8/
 ```
 
 The extra index accesses a few [customized dependencies](docs/install.md#custom-packages) for MagellanMapper.
 
-Conda installs Java to import proprietary image file formats, which can also be installed separately when using Pip (eg from [here](https://www.azul.com/downloads/?package=jdk)).
-
 For the latest updates and fixes, download from Git and install:
 
 ```shell
 git clone https://github.com/sanderslab/magellanmapper.git
+cd magellanmapper
 conda env create -n mag -f environment.yml
-pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
 python run.py
 ```
 
-Or for Pip, replace `"magellanmapper[most]"` with `".[most]"`.
+Or for Pip, replace the `conda` line with:
+
+```shell
+pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
+```
 
 
 ### More ways to install and run
 
 See the [install docs](docs/install.md) for more details, including:
 
 - [Installer scripts](docs/install.md#installer-scripts), which install Miniconda and MagellanMapper without requiring command-line usage
```

### Comparing `magellanmapper-1.6b3/README.md` & `magellanmapper-1.6b4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,60 +5,75 @@
 ![ROI Editor and Atlas Editor screenshots](https://user-images.githubusercontent.com/1258953/195321971-955fc46a-f44d-4282-8c78-21708ebaeef1.png)
 
 <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7781073/"><img align="right" width="200" src="https://user-images.githubusercontent.com/1258953/179440433-0326c4d5-9a9b-4bae-92c7-d09416375bc5.png" title="Current Protocols cover image"></a>
 
 
 ## Quick Reference
 
-- **NEW**: [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
-- [Installation](#installation) (more [details](docs/install.md))
+- [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
+- **NEW**: [Vignette of pipelines](bin/sample_cmds_bash.ipynb)
+- [Installation](#quick-install) (more [details](docs/install.md))
 - [Intro to running MagellanMapper](#run-magellanmapper)
 - [Using the viewers](docs/viewers.md)
 - [Command-line interface](docs/cli.md)
 - [Configuration and settings](docs/settings.md)
 - [Publications](#related-publications-and-datasets)
 
 
-## Installation
+## Quick Install
 
-If you use Conda (available [here](https://docs.conda.io/en/latest/miniconda.html)), you can install MagellanMapper into a new environment:
+Install MagellanMapper with its graphical interface and registration tools:
+
+```shell
+pip install "magellanmapper[gui,itk]"
+```
+
+Then launch MagellanMapper:
+
+```shell
+mm
+```
+
+## Full Install
+
+Alternatively, [Conda](https://docs.conda.io/en/latest/miniconda.html) can be used to install MagellanMapper along with support for importing proprietary image file formats (*note: not currently working on Apple Silicon (Mac M-chip) platforms*):
 
 ```shell
 conda env create -n mag -f https://raw.githubusercontent.com/sanderslab/magellanmapper/master/envs/environment_rel.yml
 ```
 
-To run in this new environment named `mag`<sup>*</sup>:
+Then activate the environment (`mag`) and run MagellanMapper:
 
 ```shell
 conda activate mag
 mm
 ```
 
-<sup>*</sup> `mm` was added in v1.6.0 to launch from installed packages
-
-Or install using Pip ([virtual environment]((https://realpython.com/python-virtual-environments-a-primer/)) recommended):
+If you have [Java](https://www.azul.com/downloads/?package=jdk), you can do the same through Pip:
 
 ```shell
 pip install "magellanmapper[most]" --extra-index-url https://pypi.fury.io/dd8/
 ```
 
 The extra index accesses a few [customized dependencies](docs/install.md#custom-packages) for MagellanMapper.
 
-Conda installs Java to import proprietary image file formats, which can also be installed separately when using Pip (eg from [here](https://www.azul.com/downloads/?package=jdk)).
-
 For the latest updates and fixes, download from Git and install:
 
 ```shell
 git clone https://github.com/sanderslab/magellanmapper.git
+cd magellanmapper
 conda env create -n mag -f environment.yml
-pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
 python run.py
 ```
 
-Or for Pip, replace `"magellanmapper[most]"` with `".[most]"`.
+Or for Pip, replace the `conda` line with:
+
+```shell
+pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
+```
 
 
 ### More ways to install and run
 
 See the [install docs](docs/install.md) for more details, including:
 
 - [Installer scripts](docs/install.md#installer-scripts), which install Miniconda and MagellanMapper without requiring command-line usage
```

#### html2text {}

```diff
@@ -2,46 +2,47 @@
 reconstruction and automated analysis of whole specimens and atlases. Its
 design philosophy is to make the raw 3D images as accessible as possible,
 simplify annotation from nuclei to atlases, and scale from the laptop or
 desktop to the cloud in cross-platform environments. ![ROI Editor and Atlas
 Editor screenshots](https://user-images.githubusercontent.com/1258953/
 195321971-955fc46a-f44d-4282-8c78-21708ebaeef1.png) _[_h_t_t_p_s_:_/_/_u_s_e_r_-
 _i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_1_2_5_8_9_5_3_/_1_7_9_4_4_0_4_3_3_-_0_3_2_6_c_4_d_5_-_9_a_9_b_-_4_b_a_e_-_9_2_c_7_-
-_d_0_9_4_1_6_3_7_5_b_c_5_._p_n_g_]## Quick Reference - **NEW**: [Docs are now on ReadTheDocs!]
-(https://magellanmapper.readthedocs.io/en/latest/) - [Installation]
-(#installation) (more [details](docs/install.md)) - [Intro to running
-MagellanMapper](#run-magellanmapper) - [Using the viewers](docs/viewers.md) -
-[Command-line interface](docs/cli.md) - [Configuration and settings](docs/
-settings.md) - [Publications](#related-publications-and-datasets) ##
-Installation If you use Conda (available [here](https://docs.conda.io/en/
-latest/miniconda.html)), you can install MagellanMapper into a new environment:
-```shell conda env create -n mag -f https://raw.githubusercontent.com/
-sanderslab/magellanmapper/master/envs/environment_rel.yml ``` To run in this
-new environment named `mag`*: ```shell conda activate mag mm ``` * `mm` was
-added in v1.6.0 to launch from installed packages Or install using Pip (
-[virtual environment]((https://realpython.com/python-virtual-environments-a-
-primer/)) recommended): ```shell pip install "magellanmapper[most]" --extra-
-index-url https://pypi.fury.io/dd8/ ``` The extra index accesses a few
-[customized dependencies](docs/install.md#custom-packages) for MagellanMapper.
-Conda installs Java to import proprietary image file formats, which can also be
-installed separately when using Pip (eg from [here](https://www.azul.com/
-downloads/?package=jdk)). For the latest updates and fixes, download from Git
-and install: ```shell git clone https://github.com/sanderslab/
-magellanmapper.git conda env create -n mag -f environment.yml pip install -e ".
-[most]" --extra-index-url https://pypi.fury.io/dd8/ python run.py ``` Or for
-Pip, replace `"magellanmapper[most]"` with `".[most]"`. ### More ways to
-install and run See the [install docs](docs/install.md) for more details,
-including: - [Installer scripts](docs/install.md#installer-scripts), which
-install Miniconda and MagellanMapper without requiring command-line usage -
-[Installer packages](docs/install.md#installer-packages), for point-and-click
-installation ## Using MagellanMapper MagellanMapper consists of a graphical
-user interface (GUI), command-line interface (CLI), and application programming
-interface (API) for Python programmatic access. See the [GUI docs](docs/
-viewers.md) for graphical usage and the [CLI docs](docs/cli.md) for scripting.
-For automated tasks, see the [`sample_cmds_bash.ipynb`](bin/
+_d_0_9_4_1_6_3_7_5_b_c_5_._p_n_g_]## Quick Reference - [Docs are now on ReadTheDocs!](https://
+magellanmapper.readthedocs.io/en/latest/) - **NEW**: [Vignette of pipelines]
+(bin/sample_cmds_bash.ipynb) - [Installation](#quick-install) (more [details]
+(docs/install.md)) - [Intro to running MagellanMapper](#run-magellanmapper) -
+[Using the viewers](docs/viewers.md) - [Command-line interface](docs/cli.md) -
+[Configuration and settings](docs/settings.md) - [Publications](#related-
+publications-and-datasets) ## Quick Install Install MagellanMapper with its
+graphical interface and registration tools: ```shell pip install
+"magellanmapper[gui,itk]" ``` Then launch MagellanMapper: ```shell mm ``` ##
+Full Install Alternatively, [Conda](https://docs.conda.io/en/latest/
+miniconda.html) can be used to install MagellanMapper along with support for
+importing proprietary image file formats (*note: not currently working on Apple
+Silicon (Mac M-chip) platforms*): ```shell conda env create -n mag -f https://
+raw.githubusercontent.com/sanderslab/magellanmapper/master/envs/
+environment_rel.yml ``` Then activate the environment (`mag`) and run
+MagellanMapper: ```shell conda activate mag mm ``` If you have [Java](https://
+www.azul.com/downloads/?package=jdk), you can do the same through Pip: ```shell
+pip install "magellanmapper[most]" --extra-index-url https://pypi.fury.io/dd8/
+``` The extra index accesses a few [customized dependencies](docs/
+install.md#custom-packages) for MagellanMapper. For the latest updates and
+fixes, download from Git and install: ```shell git clone https://github.com/
+sanderslab/magellanmapper.git cd magellanmapper conda env create -n mag -
+f environment.yml python run.py ``` Or for Pip, replace the `conda` line with:
+```shell pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
+``` ### More ways to install and run See the [install docs](docs/install.md)
+for more details, including: - [Installer scripts](docs/install.md#installer-
+scripts), which install Miniconda and MagellanMapper without requiring command-
+line usage - [Installer packages](docs/install.md#installer-packages), for
+point-and-click installation ## Using MagellanMapper MagellanMapper consists of
+a graphical user interface (GUI), command-line interface (CLI), and application
+programming interface (API) for Python programmatic access. See the [GUI docs]
+(docs/viewers.md) for graphical usage and the [CLI docs](docs/cli.md) for
+scripting. For automated tasks, see the [`sample_cmds_bash.ipynb`](bin/
 sample_cmds_bash.ipynb) Jupyter Notebook (or the older [`sample_cmds.sh`](bin/
 sample_cmds.sh) script) that shows examples of running the CLI and exploring
 images in the GUI. See ReadTheDocs for more details, including [viewer
 shortcuts](docs/viewers.md) and customizing [settings](docs/settings.md) for
 your image analysis. Have a question? Found a bug? Want a feature? Please [ask]
 (https://github.com/sanderslab/magellanmapper/issues)! ### Image file import
 Large images or proprietary microscopy formats such as CZI can be imported by
```

### Comparing `magellanmapper-1.6b3/magellanmapper.egg-info/PKG-INFO` & `magellanmapper-1.6b4/magellanmapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magellanmapper
-Version: 1.6b3
+Version: 1.6b4
 Summary: 3D atlas analysis and annotation
 Home-page: https://github.com/sanderslab/magellanmapper
 Author: David Young
 Author-email: david@textflex.com
 License: BSD-3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -43,27 +43,26 @@
 Requires-Dist: tensorflow; extra == "classifier"
 Provides-Extra: gui
 Requires-Dist: PyQt5!=5.15.8; extra == "gui"
 Requires-Dist: pyface; extra == "gui"
 Requires-Dist: traitsui; extra == "gui"
 Provides-Extra: 3d
 Requires-Dist: mayavi; extra == "3d"
+Requires-Dist: vtk<9.3.0; extra == "3d"
 Provides-Extra: itk
-Requires-Dist: itk; extra == "itk"
 Requires-Dist: itk-elastix; extra == "itk"
 Provides-Extra: simplitk
 Requires-Dist: simpleitk==2.0.2rc2.dev785+g8ac4f; python_version < "3.8" and extra == "simplitk"
 Requires-Dist: simpleitk==2.3.0.dev117+g0640d; python_version >= "3.8" and extra == "simplitk"
 Provides-Extra: most
 Requires-Dist: matplotlib_scalebar; extra == "most"
 Requires-Dist: pyamg; extra == "most"
 Requires-Dist: PyQt5!=5.15.8; extra == "most"
 Requires-Dist: pyface; extra == "most"
 Requires-Dist: traitsui; extra == "most"
-Requires-Dist: itk; extra == "most"
 Requires-Dist: itk-elastix; extra == "most"
 Requires-Dist: javabridge==1.0.19.post4+gbebed64; python_version < "3.8" and extra == "most"
 Requires-Dist: javabridge==1.0.19.post9+gc8c12b4; python_version >= "3.8" and extra == "most"
 Requires-Dist: python-bioformats==4.0.5.post2+g51eb88a; python_version < "3.8" and extra == "most"
 Requires-Dist: python-bioformats==4.0.7.post5+g52309d1; python_version >= "3.8" and extra == "most"
 Provides-Extra: all
 Requires-Dist: matplotlib_scalebar; extra == "all"
@@ -71,83 +70,98 @@
 Requires-Dist: seaborn; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: PyQt5!=5.15.8; extra == "all"
 Requires-Dist: pyface; extra == "all"
 Requires-Dist: traitsui; extra == "all"
 Requires-Dist: openpyxl; extra == "all"
 Requires-Dist: jinja2; extra == "all"
-Requires-Dist: itk; extra == "all"
 Requires-Dist: itk-elastix; extra == "all"
 Requires-Dist: javabridge==1.0.19.post4+gbebed64; python_version < "3.8" and extra == "all"
 Requires-Dist: javabridge==1.0.19.post9+gc8c12b4; python_version >= "3.8" and extra == "all"
 Requires-Dist: python-bioformats==4.0.5.post2+g51eb88a; python_version < "3.8" and extra == "all"
 Requires-Dist: python-bioformats==4.0.7.post5+g52309d1; python_version >= "3.8" and extra == "all"
 Requires-Dist: boto3; extra == "all"
 Requires-Dist: awscli; extra == "all"
 Requires-Dist: jupyterlab; extra == "all"
 Requires-Dist: bash_kernel; extra == "all"
 Requires-Dist: mayavi; extra == "all"
+Requires-Dist: vtk<9.3.0; extra == "all"
 
 # MagellanMapper
 
 MagellanMapper is a graphical imaging informatics suite for 3D reconstruction and automated analysis of whole specimens and atlases. Its design philosophy is to make the raw 3D images as accessible as possible, simplify annotation from nuclei to atlases, and scale from the laptop or desktop to the cloud in cross-platform environments.
 
 ![ROI Editor and Atlas Editor screenshots](https://user-images.githubusercontent.com/1258953/195321971-955fc46a-f44d-4282-8c78-21708ebaeef1.png)
 
 <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7781073/"><img align="right" width="200" src="https://user-images.githubusercontent.com/1258953/179440433-0326c4d5-9a9b-4bae-92c7-d09416375bc5.png" title="Current Protocols cover image"></a>
 
 
 ## Quick Reference
 
-- **NEW**: [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
-- [Installation](#installation) (more [details](docs/install.md))
+- [Docs are now on ReadTheDocs!](https://magellanmapper.readthedocs.io/en/latest/)
+- **NEW**: [Vignette of pipelines](bin/sample_cmds_bash.ipynb)
+- [Installation](#quick-install) (more [details](docs/install.md))
 - [Intro to running MagellanMapper](#run-magellanmapper)
 - [Using the viewers](docs/viewers.md)
 - [Command-line interface](docs/cli.md)
 - [Configuration and settings](docs/settings.md)
 - [Publications](#related-publications-and-datasets)
 
 
-## Installation
+## Quick Install
 
-If you use Conda (available [here](https://docs.conda.io/en/latest/miniconda.html)), you can install MagellanMapper into a new environment:
+Install MagellanMapper with its graphical interface and registration tools:
+
+```shell
+pip install "magellanmapper[gui,itk]"
+```
+
+Then launch MagellanMapper:
+
+```shell
+mm
+```
+
+## Full Install
+
+Alternatively, [Conda](https://docs.conda.io/en/latest/miniconda.html) can be used to install MagellanMapper along with support for importing proprietary image file formats (*note: not currently working on Apple Silicon (Mac M-chip) platforms*):
 
 ```shell
 conda env create -n mag -f https://raw.githubusercontent.com/sanderslab/magellanmapper/master/envs/environment_rel.yml
 ```
 
-To run in this new environment named `mag`<sup>*</sup>:
+Then activate the environment (`mag`) and run MagellanMapper:
 
 ```shell
 conda activate mag
 mm
 ```
 
-<sup>*</sup> `mm` was added in v1.6.0 to launch from installed packages
-
-Or install using Pip ([virtual environment]((https://realpython.com/python-virtual-environments-a-primer/)) recommended):
+If you have [Java](https://www.azul.com/downloads/?package=jdk), you can do the same through Pip:
 
 ```shell
 pip install "magellanmapper[most]" --extra-index-url https://pypi.fury.io/dd8/
 ```
 
 The extra index accesses a few [customized dependencies](docs/install.md#custom-packages) for MagellanMapper.
 
-Conda installs Java to import proprietary image file formats, which can also be installed separately when using Pip (eg from [here](https://www.azul.com/downloads/?package=jdk)).
-
 For the latest updates and fixes, download from Git and install:
 
 ```shell
 git clone https://github.com/sanderslab/magellanmapper.git
+cd magellanmapper
 conda env create -n mag -f environment.yml
-pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
 python run.py
 ```
 
-Or for Pip, replace `"magellanmapper[most]"` with `".[most]"`.
+Or for Pip, replace the `conda` line with:
+
+```shell
+pip install -e ".[most]" --extra-index-url https://pypi.fury.io/dd8/
+```
 
 
 ### More ways to install and run
 
 See the [install docs](docs/install.md) for more details, including:
 
 - [Installer scripts](docs/install.md#installer-scripts), which install Miniconda and MagellanMapper without requiring command-line usage
```

### Comparing `magellanmapper-1.6b3/magellanmapper.egg-info/SOURCES.txt` & `magellanmapper-1.6b4/magellanmapper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -81,9 +81,10 @@
 magmap/tests/__init__.py
 magmap/tests/test_chunking.py
 magmap/tests/test_classifier.py
 magmap/tests/test_cv_nd.py
 magmap/tests/test_detector.py
 magmap/tests/test_img_equality.py
 magmap/tests/test_libmag.py
+magmap/tests/test_np_io.py
 magmap/tests/test_visualizer.py
 magmap/tests/unit_testing.py
```

### Comparing `magellanmapper-1.6b3/magellanmapper.egg-info/requires.txt` & `magellanmapper-1.6b4/magellanmapper.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 tifffile
 imagecodecs
 bg-atlasapi
 typing_extensions
 
 [3d]
 mayavi
+vtk<9.3.0
 
 [:python_version < "3.7"]
 dataclasses
 
 [:python_version < "3.8"]
 importlib-metadata>=1.0
 
@@ -23,21 +24,21 @@
 seaborn
 scikit-learn
 PyQt5!=5.15.8
 pyface
 traitsui
 openpyxl
 jinja2
-itk
 itk-elastix
 boto3
 awscli
 jupyterlab
 bash_kernel
 mayavi
+vtk<9.3.0
 
 [all:python_version < "3.8"]
 javabridge==1.0.19.post4+gbebed64
 python-bioformats==4.0.5.post2+g51eb88a
 
 [all:python_version >= "3.8"]
 javabridge==1.0.19.post9+gc8c12b4
@@ -68,28 +69,26 @@
 python-bioformats==4.0.5.post2+g51eb88a
 
 [import:python_version >= "3.8"]
 javabridge==1.0.19.post9+gc8c12b4
 python-bioformats==4.0.7.post5+g52309d1
 
 [itk]
-itk
 itk-elastix
 
 [jupyter]
 jupyterlab
 bash_kernel
 
 [most]
 matplotlib_scalebar
 pyamg
 PyQt5!=5.15.8
 pyface
 traitsui
-itk
 itk-elastix
 
 [most:python_version < "3.8"]
 javabridge==1.0.19.post4+gbebed64
 python-bioformats==4.0.5.post2+g51eb88a
 
 [most:python_version >= "3.8"]
```

### Comparing `magellanmapper-1.6b3/magmap/atlas/atlas_refiner.py` & `magellanmapper-1.6b4/magmap/atlas/atlas_refiner.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/atlas/edge_seg.py` & `magellanmapper-1.6b4/magmap/atlas/edge_seg.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/atlas/labels_meta.py` & `magellanmapper-1.6b4/magmap/atlas/labels_meta.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/atlas/ontology.py` & `magellanmapper-1.6b4/magmap/atlas/ontology.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/atlas/reg_tasks.py` & `magellanmapper-1.6b4/magmap/atlas/reg_tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,51 +8,56 @@
 from magmap.settings import config
 from magmap.stats import vols
 
 _logger = config.logger.getChild(__name__)
 
 
 def build_labels_diff_images(paths: Optional[Sequence[str]] = None):
-    """Build labels difference images for given metrics.
+    """Build labels difference images or regional heat maps for given metrics.
     
-    Replaces each label in an atlas labels image with the value of the effect
-    size of the given metric.
+    Replaces each label in an atlas labels image with the metric value.
     
     :class:`magmap.settings.config.PlotLabels.X_COL` in
     :attr:`magmap.settings.config.plot_labels` can be used to change the
-    metric column.
+    metric column, which otherwise defaults to "vals.effect".
     
     Args:
-        paths: Paths to volume stat files output from the R pipeline.
+        paths: Paths to volume stat files output from the R pipeline or
+            output from the ``--register vol_stats`` pipeline
+            (:meth:`magmap.atlas.register.volumes_by_id`).
 
     """
+    # set the measurement column
+    col_meas = config.plot_labels[config.PlotLabels.X_COL]
+    if not col_meas:
+        col_meas = "vals.effect"
+    
     if paths:
         # set up metrics from filenames after first (image) filename;
         # extract metrics from R stats filename format
         path_dfs = paths
         metrics = [re.search(r"vols_stats_(.*).csv", p) for p in path_dfs]
         metrics = [m.group(1) if m else m for m in metrics]
+        if not metrics[0]:
+            # fall back to the measurement column, eg for metrics from the
+            # vol_stats pipeline
+            metrics[0] = col_meas
     else:
         # set up default metrics and assume corresponding CSVs are in
         # current working directory
         metrics = (
             vols.LabelMetrics.EdgeDistSum.name,
             vols.LabelMetrics.CoefVarNuc.name,
             vols.LabelMetrics.CoefVarIntens.name,
             vols.LabelMetrics.NucCluster.name,
             vols.LabelMetrics.NucClusNoise.name,
             #vols.MetricCombos.HOMOGENEITY.value[0], 
         )
         path_dfs = [f"vols_stats_{m}.csv" for m in metrics]
     
-    # set the measurement column
-    col_meas = config.plot_labels[config.PlotLabels.X_COL]
-    if not col_meas:
-        col_meas = "vals.effect"
-    
     for path_df, metric in zip(path_dfs, metrics):
         if not os.path.exists(path_df):
             # check for existing R stats file
             _logger.warn(f"{path_df} not found, skipping")
             continue
         if not metric:
             # check for extracted metric name
```

### Comparing `magellanmapper-1.6b3/magmap/atlas/register.py` & `magellanmapper-1.6b4/magmap/atlas/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,17 +362,25 @@
         params = transformix_img_filter.GetTransformParameterObject()
         transformix_img_filter = itk.TransformixFilter.New(img_sitk)
         transformix_img_filter.SetTransformParameterObject(params)
         
         # perform the transformation
         transformix_img_filter.UpdateLargestPossibleRegion()
         transf_img = transformix_img_filter.GetOutput()
+        
+        # cast image back to original data type
+        transf_img_orig = transf_img
         cast_filter = itk.CastImageFilter[type(transf_img), pixel_id].New()
         cast_filter.SetInput(transf_img)
         transf_img = cast_filter.GetOutput()
+        if all(np.equal(transf_img.shape, 0)):
+            # WORKAROUND: at least as of ITK v5.4rc3, CastImageFilter may
+            # give an empty Image object that gives a None array; cast
+            # directly to signed short, typically used for labels image
+            transf_img = transf_img_orig.astype(itk.SS)
     
     if preserve_idents:
         # map indices back to original values
         transf_inds = sitk_io.convert_img(transf_img)
         transf_inds = transf_inds.astype(int)
         bkgdi = np.nonzero(img_unique == 0)
         if len(bkgdi) > 0:
@@ -585,14 +593,17 @@
                 # set point files if both exist
                 metric = list(param_map["Metric"])
                 metric.append("CorrespondingPointsEuclideanDistanceMetric")
                 param_map["Metric"] = metric
                 #param_map["Metric2Weight"] = ["0.5"]
                 elastix_img_filter.SetFixedPointSetFileName(fix_pts_path)
                 elastix_img_filter.SetMovingPointSetFileName(move_pts_path)
+                msg = "{} image corresponding points loaded from: %s"
+                _logger.info(msg.format("Fixed"), fix_pts_path)
+                _logger.info(msg.format("Moving"), move_pts_path)
         
         if param_map_vector is not None:
             param_map_vector.append(param_map)
         elif reg_params is not None:
             reg_params.AddParameterMap(param_map)
     
     if is_sitk:
```

### Comparing `magellanmapper-1.6b3/magmap/atlas/transformer.py` & `magellanmapper-1.6b4/magmap/atlas/transformer.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/brain_globe/bg_controller.py` & `magellanmapper-1.6b4/magmap/brain_globe/bg_controller.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/brain_globe/bg_model.py` & `magellanmapper-1.6b4/magmap/brain_globe/bg_model.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cloud/aws.py` & `magellanmapper-1.6b4/magmap/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cloud/notify.py` & `magellanmapper-1.6b4/magmap/cloud/notify.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/chunking.py` & `magellanmapper-1.6b4/magmap/cv/chunking.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/classifier.py` & `magellanmapper-1.6b4/magmap/cv/classifier.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/colocalizer.py` & `magellanmapper-1.6b4/magmap/cv/colocalizer.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/cv_nd.py` & `magellanmapper-1.6b4/magmap/cv/cv_nd.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/detector.py` & `magellanmapper-1.6b4/magmap/cv/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1142,37 +1142,35 @@
 
 def get_blobs_in_roi(
         blobs: np.ndarray, offset: Sequence[int], size: Sequence[int],
         margin: Sequence[int] = (0, 0, 0), reverse: bool = True
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Get blobs within an ROI based on offset and size.
     
-    Note that dimensions are in x,y,z for natural ordering but may change for
-    consistency with z,y,x ordering used throughout MagellanMapper.
-    
     Args:
         blobs: The blobs to retrieve, given as 2D array of
             ``[n, [z, row, column, radius, ...]]``.
-        offset: Offset coordinates in ``x,y,z``.
-        size: Size of ROI in ``x,y,z``.
-        margin: Additional space outside the ROI to include in ``x,y,z``.
+        offset: Offset coordinates in ``z,y,x``.
+        size: Size of ROI in ``z,y,x``.
+        margin: Additional space outside the ROI to include in ``z,y,x``.
         reverse: True to reverse the order of ``offset`` and ``size``,
             assuming that they are in ``x,y,z`` rather than ``z,y,x`` order.
             Defaults to True for backward compatibility with the ROI
             convention used here.
     
     Returns:
         Tuple of:
         - ``segs_all`: Blobs within the ROI
         - ``mask``: the mask used to retrieve these blobs
     
     """
     if reverse:
         offset = offset[::-1]
         size = size[::-1]
+        margin = margin[::-1]
     mask = np.all([
         blobs[:, 0] >= offset[0] - margin[0],
         blobs[:, 0] < offset[0] + size[0] + margin[0],
         blobs[:, 1] >= offset[1] - margin[1],
         blobs[:, 1] < offset[1] + size[1] + margin[1],
         blobs[:, 2] >= offset[2] - margin[2],
         blobs[:, 2] < offset[2] + size[2] + margin[2]], axis=0)
```

### Comparing `magellanmapper-1.6b3/magmap/cv/segmenter.py` & `magellanmapper-1.6b4/magmap/cv/segmenter.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/stack_detect.py` & `magellanmapper-1.6b4/magmap/cv/stack_detect.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/cv/verifier.py` & `magellanmapper-1.6b4/magmap/cv/verifier.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/atlas_editor.py` & `magellanmapper-1.6b4/magmap/gui/atlas_editor.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/atlas_threads.py` & `magellanmapper-1.6b4/magmap/gui/atlas_threads.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/event_handlers.py` & `magellanmapper-1.6b4/magmap/gui/event_handlers.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/image_viewer.py` & `magellanmapper-1.6b4/magmap/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/import_threads.py` & `magellanmapper-1.6b4/magmap/gui/import_threads.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/pixel_display.py` & `magellanmapper-1.6b4/magmap/gui/pixel_display.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/plot_editor.py` & `magellanmapper-1.6b4/magmap/gui/plot_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Callable, List, Optional, Sequence, TYPE_CHECKING, Union
 
 from matplotlib import patches
 import numpy as np
 from skimage import draw
 
 from magmap.gui import image_viewer, pixel_display
-from magmap.io import libmag
+from magmap.io import libmag, np_io
 from magmap.settings import config
 from magmap.atlas import ontology
 from magmap.plot import plot_support
 
 if TYPE_CHECKING:
     from matplotlib import axes, colors, backend_bases, image
 
@@ -508,23 +508,25 @@
                 if artist in artists:
                     artists.remove(artist)
         
         # prep 2D image from main image, assumed to be an intensity image,
         # with settings for each channel within this main image
         imgs2d = [self._get_img2d(0, self.img3d, self.max_intens_proj)]
         self._channels = [config.channel]
-        cmaps = [config.cmaps]
+        cmaps = [config.cmaps]  # for all channels in image, even if not shown
+        # rest of settings are only for channels in config.channel
         alphas = list(self.alpha_img3d)
         alpha_is_default = True
         alpha_blends = [None]
         shapes = [self._img3d_shapes[0][1:3]]
         vmaxs = [None]
         vmins = [None]
         brightnesses = [None]
         contrasts = [None]
+        
         if self._plot_ax_imgs:
             # use vmin/vmax from norm values in previously displayed images
             # if available; None specifies auto-scaling
             vmaxs[0] = [p.vmax for p in self._plot_ax_imgs[0]]
             vmins[0] = [p.vmin for p in self._plot_ax_imgs[0]]
             
             # use opacity, brightness, anc contrast from prior images
@@ -581,21 +583,37 @@
                 self._channels.append([0])
                 cmaps.append(("Greys",))
                 alphas.append(0.4)
                 alpha_blends.append(None)
                 shapes.append(self._img3d_shapes[imgi][1:3])
                 vmaxs.append(None)
                 vmins.append(None)
-
+        
+        def make_abs_chls(vals):
+            # `overlay_images` requires channel-specific settings to be given
+            # for all channels of first (intensity) image in absolute rather
+            # than relative position
+            if libmag.is_seq(vals[0]):
+                # initialize for all channels and slot in channel-specific vals
+                vals_chls = [None] * nchls
+                for chl, v in zip(config.channel, vals[0]):
+                    vals_chls[chl] = v
+                vals = list(vals)
+                vals[0] = vals_chls
+            return vals
+        
         # overlay all images and set labels for footer value on mouseover;
         # if first time showing image, need to check for images with single
         # value since they fail to update on subsequent updates for unclear
         # reasons
+        nchls = np_io.get_num_channels(self.img3d, True)
         ax_imgs = self.overlayer.overlay_images(
-            imgs2d, self._channels, cmaps, alphas, vmins, vmaxs,
+            imgs2d, self._channels, cmaps,
+            # expand for all intensity channels
+            make_abs_chls(alphas), make_abs_chls(vmins), make_abs_chls(vmaxs),
             check_single=(self._ax_img_labels is None),
             alpha_blends=alpha_blends)
         
         # add or update colorbar
         colobar_prof = config.roi_profile["colorbar"]
         if self._colorbar:
             self._colorbar.update_normal(ax_imgs[0][0])
@@ -936,15 +954,21 @@
                     norm.vmax = norm.vmin
         if brightness is not None or contrast is not None:
             # adjust brightness and contrast together
             PlotEditor.change_brightness_contrast(
                 plot_ax_img, brightness, contrast)
         if alpha is not None:
             # adjust and store opacity
-            plot_ax_img.ax_img.set_alpha(alpha)
+            try:
+                plot_ax_img.ax_img.set_alpha(alpha)
+            except ValueError:
+                # WORKAROUND: matplotlib v3.8 give an error when stored alpha
+                #   is an array and new alpha is a scalar
+                plot_ax_img.ax_img._alpha = None
+                plot_ax_img.ax_img.set_alpha(alpha)
             plot_ax_img.alpha = alpha
         return plot_ax_img
 
     def update_alpha_blend(
             self, imgi: int, alpha_blend: float) -> List[PlotAxImg]:
         """Update alpha blending between two images.
```

### Comparing `magellanmapper-1.6b3/magmap/gui/roi_editor.py` & `magellanmapper-1.6b4/magmap/gui/roi_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1198,15 +1198,14 @@
             # "xz" planes
             size = libmag.swap_elements(size, 0, 1, image5d_shape_offset)
         elif plane == config.PLANE[2]:
             # "yz" planes
             size = libmag.swap_elements(size, 0, 2, image5d_shape_offset)
             size = libmag.swap_elements(size, 0, 1, image5d_shape_offset)
         z = offset[2]
-        ax.set_title("{}={}".format(plane_axis, z))
         if border is not None:
             # boundaries of border region, with xy point of corner in first
             # elements and [width, height] in 2nd, allowing flip for yz plane
             border_bounds = np.array([
                 border[0:2],
                 [roi_size[0] - 2 * border[0], roi_size[1] - 2 * border[1]]])
         
@@ -1256,15 +1255,17 @@
             overlaid = plot_support.ImageOverlayer(
                 ax, aspect, rgb=self.img5d.rgb,
                 additive_blend=self.additive_blend)
             plot_ed = plot_editor.PlotEditor(overlaid, roi[None])
             plot_ed.alpha_img3d = [alpha]
             plot_ed.coord = (0, 0, 0)
             plot_ed.show_overview()
-            #print("roi shape: {} for z_relative: {}".format(roi.shape, z_relative))
+            
+            # add title after showing overview, which cleared the axes
+            ax.set_title("{}={}".format(plane_axis, z))
 
             # show labels if provided and within ROI
             if labels is not None:
                 for i in range(len(labels)):
                     label = labels[i]
                     if 0 <= z_relative < label.shape[0]:
                         img = label[z_relative]
```

### Comparing `magellanmapper-1.6b3/magmap/gui/verifier_editor.py` & `magellanmapper-1.6b4/magmap/gui/verifier_editor.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/vis_3d.py` & `magellanmapper-1.6b4/magmap/gui/vis_3d.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/vis_handler.py` & `magellanmapper-1.6b4/magmap/gui/vis_handler.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/gui/visualizer.py` & `magellanmapper-1.6b4/magmap/gui/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,21 @@
     # scaling, eg 150%, which avoids excessive window size upscaling
     QtWidgets.QApplication.setHighDpiScaleFactorRoundingPolicy(
         QtCore.Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor)
 except AttributeError:
     pass
 
 # import PyFace components after HiDPI adjustment
+try:
+    # WORKAROUND: Mayavi as of v4.8.1 uses the older qt4 instead of qt
+    from traits.etsconfig.api import ETSConfig
+    ETSConfig.toolkit = "qt4"
+except AttributeError:
+    print("Could not set Traits ETSConfig")
+    pass
 from pyface import confirmation_dialog
 from pyface.api import DirectoryDialog, FileDialog, OK, YES, CANCEL
 from pyface.image_resource import ImageResource
 from traits.api import Any, Array, Bool, Button, Event, Float, Instance, \
     Int, List, observe, on_trait_change, Property, push_exception_handler, \
     Str, HasTraits
 from traitsui.api import ArrayEditor, BooleanEditor, CheckListEditor, \
@@ -79,14 +86,15 @@
 from magmap.io import cli, importer, libmag, load_env, naming, np_io, sitk_io, \
     sqlite
 from magmap.plot import colormaps, plot_2d, plot_3d
 from magmap.settings import config, prefs_prof, profiles
 
 if TYPE_CHECKING:
     from bg_atlasapi import BrainGlobeAtlas
+    from matplotlib import colors as mpl_colors
     from magmap.plot import plot_support
 
 # logging instance
 _logger = config.logger.getChild(__name__)
 
 
 def main():
@@ -425,14 +433,17 @@
 
     # Image adjustment panel
 
     _imgadj_names = Instance(TraitsList)
     _imgadj_name = Str
     _imgadj_chls_names = Instance(TraitsList)
     _imgadj_chls = Str
+    _imgadj_color_name = Str(
+        tooltip="Colormap for the channel. Start typing to search.")
+    _imgadj_color_names = Instance(TraitsList)
     _imgadj_min = Float
     _imgadj_min_low = Float(0)
     _imgadj_min_high = Float
     _imgadj_min_auto = Bool
     _imgadj_max = Float
     _imgadj_max_low = Float(0)
     _imgadj_max_high = Float
@@ -852,47 +863,53 @@
                  editor=CheckListEditor(
                      name="object._imgadj_names.selections")),
             # use EnumEditor for radio buttons
             Item("_imgadj_chls", label="Channel", style="custom",
                  editor=EnumEditor(
                      name="object._imgadj_chls_names.selections", cols=8)),
         ),
+        # channel colormap selector
+        Item("_imgadj_color_name", label="Color",
+             editor=EnumEditor(
+                 name="object._imgadj_color_names.selections",
+                 completion_mode="popup", evaluate=True)),
+        # use large range sliders to adjust min/max range and brightness
         HGroup(
-            Item("_imgadj_min", label="Minimum", editor=RangeEditor(
+            Item("_imgadj_min", label="Min", editor=RangeEditor(
                      low_name="_imgadj_min_low", high_name="_imgadj_min_high",
-                     mode="slider", format_str="%.4g")),
+                     mode="xslider", format_str="%.1g")),
             Item("_imgadj_min_auto", label="Auto", editor=BooleanEditor()),
         ),
         HGroup(
-            Item("_imgadj_max", label="Maximum", editor=RangeEditor(
+            Item("_imgadj_max", label="Max", editor=RangeEditor(
                      low_name="_imgadj_max_low", high_name="_imgadj_max_high",
-                     mode="slider", format_str="%.4g")),
+                     mode="xslider", format_str="%.1g")),
             Item("_imgadj_max_auto", label="Auto", editor=BooleanEditor()),
         ),
         HGroup(
             Item("_imgadj_brightness", label="Brightness", editor=RangeEditor(
                      low_name="_imgadj_brightness_low",
-                     high_name="_imgadj_brightness_high", mode="slider",
-                     format_str="%.4g"))
+                     high_name="_imgadj_brightness_high", mode="xslider",
+                     format_str="%.1g"))
         ),
         HGroup(
             Item("_imgadj_contrast", label="Contrast", editor=RangeEditor(
-                     low=0.0, high=2.0, mode="slider", format_str="%.3g")),
+                     low=0.0, high=2.0, mode="slider", format_str="%.1g")),
         ),
         HGroup(
             Item("_imgadj_alpha", label="Opacity", editor=RangeEditor(
-                 low=0.0, high=1.0, mode="slider", format_str="%.3g")),
+                 low=0.0, high=1.0, mode="slider", format_str="%.1g")),
         ),
         
         HGroup(
             # alpha blending controls
             Item("_imgadj_alpha_blend_check", label="Blend",
                  enabled_when="not _merge_chls"),
             Item("_imgadj_alpha_blend", show_label=False, editor=RangeEditor(
-                 low=0.0, high=1.0, mode="slider", format_str="%.3g"),
+                 low=0.0, high=1.0, mode="slider", format_str="%.1g"),
                  enabled_when="_imgadj_alpha_blend_check"),
         ),
         label="Adjust Image",
     )
     
     # import panel
     panel_import = VGroup(
@@ -1055,14 +1072,23 @@
             Vis3dOptions.RAW.value, Vis3dOptions.SURFACE.value]
         if (config.roi_profile["vis_3d"].lower()
                 == Vis3dOptions.SURFACE.value.lower()):
             # check "surface" if set in profile
             self._check_list_3d.append(Vis3dOptions.SURFACE.value)
         # self._structure_scale = self._structure_scale_high
         
+        # set up channel colormap selections
+        self._imgadj_color_names = TraitsList()
+        if not colormaps.CMAPS:
+            colormaps.setup_cmaps()
+        self._imgadj_colors: Dict[str, "mpl_colors.Colormap"] = {
+            k.value: v for k, v in colormaps.CMAPS.items()}
+        self._imgadj_colors.update(matplotlib.colormaps)
+        self._imgadj_color_names.selections = list(self._imgadj_colors.keys())
+        
         # set up atlas region names
         self._region_names = TraitsList()
         self._region_id_map = {}
         self._region_options_prev: Dict[Enum, bool] = {}
         self._region_options = [RegionOptions.INCL_CHILDREN.value]
         
         # set up blobs
@@ -1208,22 +1234,25 @@
                 str(n) for n in np.unique(detector.Blobs.get_blobs_channel(
                     config.blobs.blobs).astype(int))]
         else:
             # add detection channel selectors for all image channels
             self._segs_chls_names.selections = list(
                 self._channel_names.selections)
         
-        # pre-select channels for both main and profiles selector
+        # pre-select channels for both main and profiles selector; ignore
+        # channel handler to avoid redrawing the viewer
+        self._imgadj_ignore_update = True
         if not chls_pre and config.channel:
             # use config if all chls were unchecked, eg if setting for 1st time
             self._channel = sorted([
                 str(c) for i, c in enumerate(config.channel) if i < num_chls])
         else:
             # select all channels
             self._channel = self._channel_names.selections
+        self._imgadj_ignore_update = False
         
         # select detection and profile channels to match main channels
         self._segs_chls = list(self._channel)
         self._profiles_chls = self._channel
 
     def _init_imgadj(self):
         """Initialize image adjustment controls for the currently loaded images.
@@ -1277,32 +1306,42 @@
         self._imgadj_chls_names = TraitsList()
         self._imgadj_chls_names.selections = chls
         if self._imgadj_chls_names.selections:
             self._imgadj_chls = self._imgadj_chls_names.selections[0]
 
     @on_trait_change("_imgadj_name")
     def _update_imgadj_limits(self):
+        """Update image intensity limits."""
         img3d = self._img3ds.get(self._imgadj_name)
         if img3d is None: return
         info = libmag.get_dtype_info(img3d)
         self._setup_imgadj_channels()
 
-        # min/max based on near min/max pre-calculated from whole image
-        # including all channels, falling back to data type range; cannot
-        # used percentile or else need to load whole image from disk
+        # default to only include non-neg intensities
         min_inten = 0
         if config.near_min is not None:
+            # check for neg intensities from min/max pre-calculated from whole
+            # image for all channels; cannot used percentile or else need to
+            # load whole image from disk
             min_near_min = min(config.near_min)
             if min_near_min < 0:
-                # set min to 0 unless near min is < 0
-                min_inten = 2 * min_near_min
-        # default near max is an array of -1; assume that measured near
-        # max values are positive
-        max_near_max = -1 if config.near_max is None else max(config.near_max)
-        max_inten = info.max if max_near_max < 0 else max_near_max * 2
+                min_inten = info.min
+        
+        # default to max intensity based data type
+        max_inten = info.max
+        if config.near_max is not None:
+            max_near_max = max(config.near_max)
+            if -1 < max_near_max < 10:
+                # RangeEditor xslider does not scale below 10, which can make
+                # scrolling difficult for small values; workaround by using
+                # image max, still allowing higher values by the text field;
+                # ignore if default (-1)
+                max_inten = 2 * max_near_max
+        
+        # set min/max; slider has range adjustments
         self._imgadj_min_low = min_inten
         self._imgadj_min_high = max_inten
         self._imgadj_max_low = min_inten
         self._imgadj_max_high = max_inten
 
         # range brightness symmetrically to max limit
         self._imgadj_brightness_low = -max_inten
@@ -1336,34 +1375,35 @@
     
     @on_trait_change("_imgadj_chls")
     def update_imgadj_for_img(self):
         """Update image adjustment controls based on the currently selected
         viewer and channel.
 
         """
-        if not self.imgadj_chls:
-            # resetting image adjustment channel names triggers update as
-            # empty array
+        if not self.imgadj_chls or self._imgadj_ignore_update:
+            # initializations trigger imgadj_chls with empty value
             return
 
         # get currently displayed image
         plot_ax_img = self._get_curr_plot_ax_img()
         if plot_ax_img is None: return
         
         # ignore triggers
         self._imgadj_ignore_update = True
         
+        # populate channel colormap
+        cmap = colormaps.get_cmap(config.cmaps, int(self.imgadj_chls))
+        if cmap:
+            self._imgadj_color_name = cmap.name
+        
         # populate controls with intensity settings
         self._imgadj_brightness = plot_ax_img.brightness
         self._imgadj_contrast = plot_ax_img.contrast
         self._imgadj_alpha = plot_ax_img.alpha
 
-        # populate intensity limits, auto-scaling, and current val (if not auto)
-        self._adapt_imgadj_limits(plot_ax_img)
-        
         if plot_ax_img.vmin is None:
             self._imgadj_min_auto = True
         else:
             self._imgadj_min = plot_ax_img.ax_img.norm.vmin
             self._imgadj_min_auto = False
         
         if plot_ax_img.vmax is None:
@@ -1371,72 +1411,61 @@
         else:
             self._imgadj_max = plot_ax_img.ax_img.norm.vmax
             self._imgadj_max_auto = False
 
         # respond to triggers
         self._imgadj_ignore_update = False
     
-    def _adapt_imgadj_limits(self, plot_ax_img: "plot_editor.PlotAxImg"):
-        """Adapt image adjustment slider limits based on values in the
-        given plotted image.
+    def _restore_imgadj(self):
+        """Restore image adjustment settings."""
+        # populate with current settings
+        adj = dict(
+            brightness=self._imgadj_brightness,
+            contrast=self._imgadj_contrast,
+            alpha=self._imgadj_alpha,
+        )
         
-        Args:
-            plot_ax_img: Plotted image.
-
-        """
-        if plot_ax_img is None: return
-        norm = plot_ax_img.ax_img.norm
-        input_img = plot_ax_img.input_img
-        inten_lim = (np.amin(input_img), np.amax(input_img))
-
-        if inten_lim[0] < self._imgadj_max_low:
-            # ensure that lower limit is beyond current plane's lower limit;
-            # bottom out at 0 unless current low is < 0
-            low_thresh = inten_lim[0] if norm.vmin is None else min(
-                inten_lim[0], norm.vmin)
-            low = 2 * low_thresh if low_thresh < 0 else 0
-            self._imgadj_min_low = low
-            self._imgadj_max_low = low
-        
-        high = None
-        if inten_lim[1] > self._imgadj_max_high:
-            # ensure that upper limit is beyond current plane's limits;
-            # cap at 0 if current high is < 0 in case image is fully neg
-            high_thresh = inten_lim[1] if norm.vmax is None else max(
-                inten_lim[1], norm.vmax)
-            high = 2 * high_thresh if high_thresh > 0 else 0
-        elif (0 < inten_lim[1] < 0.1 * self._imgadj_max_high
-              and self._imgadj_max_high >= 0):
-            # reduce upper limit if current max is comparatively very small
-            high = 10 * inten_lim[1]
-        if high is not None:
-            # make brightness symmetric around upper limit
-            self._imgadj_min_high = high
-            self._imgadj_max_high = high
-            self._imgadj_brightness_low = -high
-            self._imgadj_brightness_high = high
+        # only add min/max if not auto
+        if not self._imgadj_min_auto:
+            adj["minimum"] = self._imgadj_min
+        
+        if not self._imgadj_max_auto:
+            adj["maximum"] = self._imgadj_max
+        
+        # update image
+        self._adjust_displayed_imgs(**adj)
     
     def _set_inten_min_to_curr(self, plot_ax_img):
         """Set min intensity to current image value."""
         if plot_ax_img is not None:
             vmin = plot_ax_img.ax_img.norm.vmin
-            self._adapt_imgadj_limits(plot_ax_img)
             if self._imgadj_min != vmin:
                 self._imgadj_min_ignore_update = True
                 self._imgadj_min = vmin
 
     def _set_inten_max_to_curr(self, plot_ax_img):
         """Set max intensity to current image value."""
         if plot_ax_img is not None:
             vmax = plot_ax_img.ax_img.norm.vmax
-            self._adapt_imgadj_limits(plot_ax_img)
             if self._imgadj_max != vmax:
                 self._imgadj_max_ignore_update = True
                 self._imgadj_max = vmax
 
+    @observe("_imgadj_color_name")
+    def _adjust_img_color(self, evt):
+        """Update the image colormap."""
+        if self._imgadj_ignore_update: return
+        # set colormap based on the selected name and refresh image
+        cmap = self._imgadj_colors[self._imgadj_color_name]
+        chl = int(self.imgadj_chls)
+        if chl < len(config.cmaps):
+            # config should have cmaps for all the image's channels
+            config.cmaps[chl] = cmap
+            self._adjust_displayed_imgs(True)
+
     @on_trait_change("_imgadj_min")
     def _adjust_img_min(self):
         if self._imgadj_min_ignore_update or self._imgadj_ignore_update:
             self._imgadj_min_ignore_update = False
             return
         self._imgadj_ignore_update = True
         self._imgadj_min_auto = False
@@ -1487,14 +1516,18 @@
         self._imgadj_ignore_update = True
         self._imgadj_max_auto = False
         self._imgadj_ignore_update = False
         plot_ax_img = self._adjust_displayed_imgs(maximum=self._imgadj_max)
         
         # # intensity min may have been adjusted to remain <= max
         # self._set_inten_min_to_curr(plot_ax_img)
+        
+        if self._imgadj_max > self._imgadj_max_high:
+            # expand range if increased above max, eg entered in text field
+            self._imgadj_max_high = self._imgadj_min_high = self._imgadj_max
 
     @on_trait_change("_imgadj_brightness")
     def _adjust_img_brightness(self):
         if self._imgadj_ignore_update: return
         # include contrast to restore its value while adjusting the original img
         self._adjust_displayed_imgs(
             brightness=self._imgadj_brightness, contrast=self._imgadj_contrast)
@@ -2206,19 +2239,23 @@
         else:
             # load the image in the empty current app window
             self.update_filename(filename)
     
     @observe("_filename_btn")
     def _filename_updated(self, evt):
         """Open a Pyface file dialog to set the main image path."""
-        open_dialog = FileDialog(
-            action="open", default_path=os.path.dirname(self._filename))
+        # get path from currently opened file or preferences
+        path = os.path.dirname(
+            self._filename) if self._filename else config.prefs.img_open_path
+        open_dialog = FileDialog(action="open", default_path=path)
+        
         if open_dialog.open() == OK:
-            # get user selected path
+            # get user selected path and save in preferences
             self._filename = open_dialog.path
+            config.prefs.img_open_path = self._filename
 
     @on_trait_change("_filename")
     def _image_path_updated(self):
         """Update the selected filename and load the corresponding image.
         
         Since an original (eg .czi) image can be processed in so many 
         different ways, assume that the user will select the Numpy image 
@@ -2248,16 +2285,17 @@
         if filename is not None:
             importer.parse_deconstructed_name(
                 filename, offset, size, reg_suffixes)
             np_io.setup_images(
                 config.filename, offset=offset, size=size, allow_import=False,
                 labels_ref_path=self._labels_ref_path)
             self._setup_for_image()
-            self.redraw_selected_viewer()
+            self.redraw_selected_viewer(restore_imgadj=False)
             self.update_imgadj_for_img()
+            config.prefs.img_open_path = self._filename
         else:
             print("Could not parse filename", self._filename)
         
         if config.image5d is None:
             # initiate import setup and direct user to import panel
             print("Could not open {}, directing to import panel"
                   .format(self._filename))
@@ -2300,36 +2338,42 @@
             action="open", default_path=os.path.dirname(self._filename))
         if open_dialog.open() == OK:
             # get user selected path
             self._labels_ref_path = open_dialog.path
     
     @on_trait_change("_channel")
     def update_channel(self):
-        """Update the selected channel and image adjustment controls.
+        """Update the selected channel and redraw the viewer.
         """
         if not self._channel:
             # resetting channel names triggers channel update as empty array
             return
+        
+        # update the configured channels
         config.channel = sorted([int(n) for n in self._channel])
-        self._setup_imgadj_channels()
-        print("Changed channel to {}".format(config.channel))
+        _logger.debug("Changed channel to %s", config.channel)
+        
+        if not self._imgadj_ignore_update:
+            # fully refresh the viewer with the channel update; need to ignore
+            # during channel control initialization
+            self.redraw_selected_viewer(restore_imgadj=False)
     
     @observe("_rgb", post_init=True)
     def _update_rgb(self, event):
         """Handle changes to the RGB button."""
         if config.img5d:
             # change image RGB setting, which editors reference
             config.img5d.rgb = self._rgb
             _logger.debug("Changed RGB to %s", config.img5d.rgb)
             
             # update image adjustment channel options
             self._update_imgadj_limits()
             
             # redraw viewer in selected RGB mode
-            self.redraw_selected_viewer()
+            self.redraw_selected_viewer(restore_imgadj=False)
 
     def reset_stale_viewers(self, val=vis_handler.StaleFlags.IMAGE):
         """Reset the stale viewer flags for all viewers.
         
         Args:
             val (:class:`vis_handler.StaleFlags`): Enumeration to set for all
                 viewers.
@@ -2491,19 +2535,21 @@
         self._open_help_docs(config.DocsURLs.DOCS_URL_VIEWER.value)
 
     @on_trait_change("_profiles_btn_help")
     def _help_profiles(self):
         """Respond to profiles panel help button presses."""
         self._open_help_docs(config.DocsURLs.DOCS_URL_SETTINGS.value)
     
-    def redraw_selected_viewer(self, clear=True):
+    def redraw_selected_viewer(
+            self, clear: bool = True, restore_imgadj: bool = True):
         """Redraw the selected viewer.
         
         Args:
-            clear (bool): True to clear the ROI and blobs; defaults to True.
+            clear: True to clear the ROI and blobs.
+            restore_imgadj: True to restore the current image settings.
         
         """
         def confirm(ed, fn):
             # prompt to save before redrawing if edited
             if ed.edited:
                 response = confirmation_dialog.confirm(
                     None, "Edits have not been saved. Save before redrawing?",
@@ -2531,14 +2577,19 @@
         self._drawn_offset = self._curr_offset()
         if clear:
             self.roi = None
             self._reset_segments()
             if self._rois_selections.selections:
                 self.rois_check_list = self._rois_selections.selections[0]
 
+        # relaunching an editor may trigger an image adjustment channel control
+        # event, populating settings with the current image instead of leaving
+        # them to be restored; set to ignore this trigger
+        self._imgadj_ignore_update = restore_imgadj
+        
         # redraw the currently selected viewer tab
         if self.selected_viewer_tab is vis_handler.ViewerTabs.ROI_ED:
             # disconnect existing ROI and Verifier Editors, which share the fig
             if self.roi_ed:
                 self.roi_ed.on_close()
             if self.verifier_ed:
                 self.verifier_ed.on_close()
@@ -2557,14 +2608,22 @@
             # launch Atlas Editor
             self.launch_atlas_editor()
         
         elif self.selected_viewer_tab is vis_handler.ViewerTabs.MAYAVI:
             # launch 3D Viewer
             self.show_3d()
             self._post_3d_display()
+        
+        if restore_imgadj:
+            # restore user image adjustment settings
+            self._restore_imgadj()
+            self._imgadj_ignore_update = False
+        else:
+            # synchronize adjustment controls with the redrawn image
+            self.update_imgadj_for_img()
     
     @on_trait_change("scene.activated")
     def orient_camera(self):
         """Provide a default camera orientation with orientation axes.
 
         """
         if self.scene is None: return
@@ -2996,20 +3055,24 @@
         curr_offset, curr_roi_size, feedback = self._check_roi_position()
         self._update_roi_feedback(" ".join(feedback))
 
         # update verify flag
         roi_editor.verify = self._DEFAULTS_2D[1] in self._check_list_2d
         roi = None
         if self._DEFAULTS_2D[0] in self._check_list_2d:
-            print("showing processed 2D images")
+            _logger.debug("Showing processed 2D images")
             # denoised ROI processed during 3D display
             roi = self.roi
             if config.roi_profile["thresholding"]:
                 # thresholds prior to blob detection
                 roi = plot_3d.threshold(roi)
+            
+            # scale ROI to original image since filtering it changes its range
+            roi = libmag.normalize(
+                roi, min(config.near_min), max(config.near_max))
         
         blobs_truth_roi = None
         if config.truth_db is not None:
             # collect truth blobs from the truth DB if available
             blobs_truth_roi, _ = detector.get_blobs_in_roi(
                 config.truth_db.blobs_truth, curr_offset, curr_roi_size, 
                 self._margin)
@@ -4206,15 +4269,15 @@
         config.filename = str(bg_atlas.root_dir)
         self.update_filename(config.filename, True)
         
         # display the atlas images
         np_io.setup_images(
             config.filename, allow_import=False, bg_atlas=bg_atlas)
         self._setup_for_image()
-        self.redraw_selected_viewer()
+        self.redraw_selected_viewer(restore_imgadj=False)
         self.update_imgadj_for_img()
     
     def _setup_brain_globe(self):
         """Set up the BrainGlobe controller."""
         panel = bg_controller.BrainGlobeCtrl(
             self._set_bg_atlases, self._set_bg_feedback, self._update_prog,
             self._bg_open_handler)
```

### Comparing `magellanmapper-1.6b3/magmap/io/cli.py` & `magellanmapper-1.6b4/magmap/io/cli.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/df_io.py` & `magellanmapper-1.6b4/magmap/io/df_io.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/export_regions.py` & `magellanmapper-1.6b4/magmap/io/export_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,65 +26,68 @@
 from magmap.plot import colormaps
 from magmap.settings import config, atlas_prof
 from magmap.stats import vols
 
 _logger = config.logger.getChild(__name__)
 
 
-def export_region_ids(labels_ref_lookup, path, level=None,
-                      drawn_labels_only=False):
-    """Export region IDs from annotation reference reverse mapped dictionary 
-    to CSV and Excel files.
-
-    Use a ``level`` of None to export labels only for the currently loaded
-    atlas. The RGB values used for the currently loaded atlas will also be
-    shown, with cell colors corresponding to these values in the Excel file.
+def export_region_ids(
+        labels_ref_lookup: Dict, path: str, level: Optional[int] = None,
+        drawn_labels_only: bool = False) -> pd.DataFrame:
+    """Export region IDs from annotation reference reverse mapped dictionary.
     
     Args:
-        labels_ref_lookup: The labels reference lookup, assumed to be an 
-            OrderedDict generated by :func:`ontology.create_reverse_lookup` 
-            to look up by ID while preserving key order to ensure that 
+        labels_ref_lookup: The labels reference lookup, assumed to be an
+            OrderedDict generated by :func:`ontology.create_reverse_lookup`
+            to look up by ID while preserving key order to ensure that
             parents of any child will be reached prior to the child.
-        path: Path to output CSV file; if does not end with ``.csv``, it will 
+        path: Path to output CSV file; if does not end with ``.csv``, it will
             be added.
-        level: Level at which to find parent for each label; defaults to None
-            to get the immediate parent.
-        drawn_labels_only (bool): True to export only the drawn labels for
+        level: Level at which to find parent for each label. If None, each
+            the immediate parent will be retrieved for each label.
+        drawn_labels_only: True to export only the drawn labels for
             atlas labels in the same folder as ``labels_ref_lookup``.
-            Defaults to False to use the full set of labels in
-            ``labels_ref_lookup``
+            The RGB values used for the currently loaded atlas will also be
+            shown in a corresponding Excel file (requires `openpyxl` and
+            `Jinja2` packages). If False, the full set of labels in
+            ``labels_ref_lookup`` is used.
     
     Returns:
         Pandas data frame of the region IDs and corresponding names.
+    
     """
     def color_cells(s):
         # convert RGB to hex values since Pandas Excel export only supports
         # named colors or hex (as of v0.22)
         css = ["background-color: #{:02x}{:02x}{:02x}".format(*c) for c in s]
         return css
 
     ext = ".csv"
     path_csv = path if path.endswith(ext) else path + ext
     
     # find ancestor for each label at the given level
     label_parents = ontology.labels_to_parent(
         labels_ref_lookup, level, allow_parent_same_level=True)
     
+    # load labels
     cols = [config.AtlasMetrics.REGION.value,
             config.AtlasMetrics.REGION_ABBR.value,
             config.AtlasMetrics.REGION_NAME.value,
             config.AtlasMetrics.LEVEL.value,
             config.AtlasMetrics.PARENT.value]
     data = OrderedDict()
     label_ids = sitk_io.find_atlas_labels(
         config.load_labels, drawn_labels_only, labels_ref_lookup)
     cm = colormaps.get_labels_discrete_colormap(None, 0, use_orig_labels=True)
+    
+    # prep RGB values for labels, only available if showing drawn labels
     rgbs = cm.cmap_labels
     if rgbs is not None:
         cols.append("RGB")
+    
     for i, key in enumerate(label_ids):
         # get label dict
         label = labels_ref_lookup.get(key)
         if label is None: continue
         
         # ID of parent at label_parents' level
         parent = label_parents[key]
@@ -92,23 +95,28 @@
                 label[ontology.NODE][config.ABAKeys.NAME.value],
                 label[ontology.NODE][config.ABAKeys.LEVEL.value], parent]
         if rgbs is not None:
             vals.append(rgbs[i, :3])
         for col, val in zip(cols, vals):
             data.setdefault(col, []).append(val)
     df = df_io.dict_to_data_frame(data, path_csv)
+    
     if rgbs is not None:
+        # color cells in RGB column
         df = df.style.apply(color_cells, subset="RGB")
+    
     path_xlsx = "{}.xlsx".format(os.path.splitext(path)[0])
     try:
+        # export Excel file, necessary for styling
         df.to_excel(path_xlsx)
         _logger.info("Exported regions to styled spreadsheet: %s", path_xlsx)
     except ModuleNotFoundError:
         raise ModuleNotFoundError(
             config.format_import_err("openpyxl", task="formatting Excel files"))
+    
     return df
 
 
 def export_region_network(labels_ref_lookup, path):
     """Export region network file showing relationships among regions 
     according to the SIF specification.
     
@@ -267,15 +275,15 @@
         # default to use labels image as the size of the output image
         if labels_img_sitk is None:
             labels_img_sitk = sitk_io.load_registered_img(
                 mod_path, config.RegNames.IMG_LABELS.value, get_sitk=True)
         labels_img = sitk_io.convert_img(labels_img_sitk)
         
         is_2d = labels_img.ndim == 2
-        labels_res = list(labels_img_sitk.GetSpacing()[::-1])
+        labels_res = list(labels_img_sitk.GetSpacing())[::-1]
         if is_2d:
             # temporarily convert 2D images to 3D
             labels_img = labels_img[None]
             labels_res.insert(0, 1)
         
         if blobs.resolutions is not None:
             # find scaling based on blob to labels image resolution ratio
```

### Comparing `magellanmapper-1.6b3/magmap/io/export_rois.py` & `magellanmapper-1.6b4/magmap/io/export_rois.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/export_stack.py` & `magellanmapper-1.6b4/magmap/io/export_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,48 +497,55 @@
     stacker.img_slice = img_sl
     
     return stacker
 
 
 def stack_to_img(paths, roi_offset, roi_size, series=None, subimg_offset=None,
                  subimg_size=None, animated=False, suffix=None):
-    """Build an image file from a stack of images in a directory or an 
-    array, exporting as an animated GIF or movie for multiple planes or 
+    """Build an image file from a stack of images in a directory or an
+    array, exporting as an animated GIF or movie for multiple planes or
     extracting a single plane to a standard image file format.
     
     Writes the file to the parent directory of path.
     
     Args:
-        paths (List[str]): Image paths, which can each be either an image 
-            directory or a base path to a single image, including 
-            volumetric images.
+        paths (List[str]): Image paths, which can each be either an image
+            directory or a base path to a single image, including
+            volumetric images. If more than one path is given, a collage of
+            images will be generated with the layout set by
+            :attr:`magmap.settings.config.plot_labels[config.PlotLabels.LAYOUT]`.
         roi_offset (Sequence[int]): Tuple of offset given in user order
             ``x,y,z``; defaults to None. Requires ``roi_size`` to not be None.
-        roi_size (Sequence[int]): Size of the region of interest in user order 
+        roi_size (Sequence[int]): Size of the region of interest in user order
             ``x,y,z``; defaults to None. Requires ``roi_offset`` to not be None.
         series (int): Image series number; defaults to None.
         subimg_offset (List[int]): Sub-image offset as (z,y,x) to load;
             defaults to None.
         subimg_size (List[int]): Sub-image size as (z,y,x) to load;
             defaults to None.
         animated (bool): True to export as an animated image; defaults to False.
-        suffix (str): String to append to output path before extension; 
+        suffix (str): String to append to output path before extension;
             defaults to None to ignore.
 
     """
     # set up figure layout for collages
     size = config.plot_labels[config.PlotLabels.LAYOUT]
     ncols, nrows = size if size else (1, 1)
     num_paths = len(paths)
     collage = num_paths > 1
     figs = {}
     
     path_base = paths[0]
     for i in range(nrows):
         for j in range(ncols):
+            # load image and display selected planes:
+            # - for collages, typically one plane of the image is shown as a
+            #   subplot of a single fig
+            # - for non-collages: one or more planes are shown, each in a
+            #   separate fig and axes except animations, which share one fig
             n = i * ncols + j
             if n >= num_paths: break
             
             # load an image and set up its image stacker
             path_sub = paths[n]
             axs = []
             # TODO: test directory of images
@@ -560,26 +567,29 @@
                 title = libmag.get_if_within(config.groups, n)
             elif num_paths > 1:
                 title = os.path.basename(path_sub)
             
             if not stacker.images: continue
             ax = None
             for k in range(len(stacker.images[0])):
-                # create or retrieve fig; animation has only 1 fig
+                # create or retrieve fig for the given images; animation and
+                # collage have only 1 fig, whereas stack of multiple planes
+                # has a separate fig for each plane
                 planei = 0 if animated else (
                         stacker.img_slice.start + k * stacker.img_slice.step)
                 fig_dict = figs.get(planei)
                 if not fig_dict:
-                    # set up new fig
+                    # set up new fig for each new plane unless animated
                     fig, gs = plot_support.setup_fig(
                         nrows, ncols, config.plot_labels[config.PlotLabels.SIZE])
                     fig_dict = {"fig": fig, "gs": gs, "imgs": []}
                     figs[planei] = fig_dict
-                if ax is None:
-                    # generate new axes for the gridspec position
+                if ax is None or not animated:
+                    # generate new axes for the gridspec position; share
+                    # axes for animation
                     ax = fig_dict["fig"].add_subplot(fig_dict["gs"][i, j])
                 if title:
                     ax.title.set_text(title)
                 axs.append(ax)
 
             # export planes
             plotted_imgs = stacker.build_stack(
```

### Comparing `magellanmapper-1.6b3/magmap/io/importer.py` & `magellanmapper-1.6b4/magmap/io/importer.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/libmag.py` & `magellanmapper-1.6b4/magmap/io/libmag.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/load_env.py` & `magellanmapper-1.6b4/magmap/io/load_env.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/naming.py` & `magellanmapper-1.6b4/magmap/io/naming.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/np_io.py` & `magellanmapper-1.6b4/magmap/io/np_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,23 +400,29 @@
     # main image is currently required since many parameters depend on it
     if fallback_main_img and atlas_suffix is None and config.image5d is None:
         # fallback to atlas if main image not already loaded
         atlas_suffix = config.RegNames.IMG_ATLAS.value
         _logger.info(
             "Main image is not set, falling back to registered image with "
             "suffix %s", atlas_suffix)
+    
     # use prefix to get images registered to a different image, eg a
     # downsampled version, or a different version of registered images
     path = config.prefix if config.prefix else path
     if path and atlas_suffix is not None:
         try:
             # will take the place of any previously loaded image5d
             config.img5d = sitk_io.read_sitk_files(
                 path, atlas_suffix, make_3d=True)
             config.image5d = config.img5d.img
+            
+            if config.img5d.img is not None:
+                # get near min/max across whole image
+                config.near_min, config.near_max = \
+                    importer.calc_intensity_bounds(config.img5d.img)
         except FileNotFoundError as e:
             print(e)
     
     # load metadata related to the labels image
     config.labels_metadata = labels_meta.LabelsMeta(
         f"{path}." if config.prefix else path).load()
     
@@ -514,17 +520,18 @@
             and not config.image5d_is_roi):
         # crop full image to bounds of sub-image
         config.image5d = plot_3d.prepare_subimg(
             config.image5d, offset, size)[None]
         config.img5d.img = config.image5d
         config.image5d_is_roi = True
 
-    # add any additional image5d thresholds for multichannel images, such 
+    # add any additional image5d thresholds for multichannel images, such
     # as those loaded without metadata for these settings
-    colormaps.setup_cmaps()
+    if not colormaps.CMAPS:
+        colormaps.setup_cmaps()
     num_channels = get_num_channels(config.image5d)
     config.near_max = libmag.pad_seq(config.near_max, num_channels, -1)
     config.near_min = libmag.pad_seq(config.near_min, num_channels, 0)
     config.vmax_overview = libmag.pad_seq(
         config.vmax_overview, num_channels)
     colormaps.setup_colormaps(num_channels)
     
@@ -541,26 +548,29 @@
         if not np.all(scaling == 1):
             _logger.debug("Scaling blobs to main image by factor: %s", scaling)
             blobs.blobs[:, :4] = ontology.scale_coords(
                 blobs.blobs[:, :4], scaling)
         blobs.scaling = scaling
 
 
-def get_num_channels(image5d):
-    """Get the number of channels in a 5D image.
+def get_num_channels(img: np.ndarray, is_3d: bool = False) -> int:
+    """Get the number of image channels based on expected dimensions.
 
     Args:
-        image5d (:obj:`np.ndarray`): Numpy arry in the order, `t,z,y,x[,c]`.
+        img: Numpy array.
+        is_3d: True if ``img` is a 3D+ array with ``z,y,x[,c]`` order.
+            Otherwise, assumes that the image is in 5D (4D+channel),
+            `t,z,y,x[,c]` order.
 
     Returns:
-        int: Number of channels inferred based on the presence and length
-        of the 5th dimension.
+        Inferred number of channels.
 
     """
-    return 1 if image5d is None or image5d.ndim <= 4 else image5d.shape[4]
+    chl_dim = 3 if is_3d else 4
+    return 1 if img is None or img.ndim <= chl_dim else img.shape[chl_dim]
 
 
 def write_raw_file(arr, path):
     """Write an array to a RAW data file.
     
     The array will be output directly to disk through a memmapped object.
```

### Comparing `magellanmapper-1.6b3/magmap/io/packaging.py` & `magellanmapper-1.6b4/magmap/io/packaging.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/sitk_io.py` & `magellanmapper-1.6b4/magmap/io/sitk_io.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/sqlite.py` & `magellanmapper-1.6b4/magmap/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/subproc_io.py` & `magellanmapper-1.6b4/magmap/io/subproc_io.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/io/yaml_io.py` & `magellanmapper-1.6b4/magmap/io/yaml_io.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/plot/colormaps.py` & `magellanmapper-1.6b4/magmap/plot/colormaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Colormaps for MagellanMapper
-# Author: David Young, 2018, 2020
+# Author: David Young, 2018, 2023
 """Custom colormaps for MagellanMapper.
 """
 
 from enum import Enum, auto
-from typing import Optional, Sequence, Tuple, Union
+from typing import Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from matplotlib import cm
 from matplotlib import colors
 
 from magmap.settings import config
 from magmap.io import libmag
 
 #: Dict[:class:`config.Cmaps`, :obj:`colors.LinearSegmentedColormap`]:
 # Default colormaps.
-CMAPS = {}
+CMAPS: Dict["config.Cmaps", colors.LinearSegmentedColormap] = {}
 
 _logger = config.logger.getChild(__name__)
 
 
 class DiscreteModes(Enum):
     """Discrete colormap generation modes."""
     RANDOMN = auto()
@@ -503,30 +503,32 @@
             symmetric_colors=config.atlas_labels[
                 config.AtlasLabels.SYMMETRIC_COLORS])
         args.update(kwargs)
         cmap_labels = get_labels_discrete_colormap(labels_img, 0, **args)
     return cmap_labels
 
 
-def get_cmap(cmap, n=None):
+def get_cmap(
+        cmap: Union[str, "config.Cmaps"], n: Optional[int] = None
+) -> Optional[colors.LinearSegmentedColormap]:
     """Get colormap from a list of colormaps, string, or enum.
     
-    If ``n`` is given, ``cmap`` is assumed to be a list from which a colormap 
-    will be retrieved. Colormaps that are strings will be converted to 
-    the associated standard `Colormap` object, while enums in 
-    :class:``config.Cmaps`` will be used to retrieve a `Colormap` object 
+    If ``n`` is given, ``cmap`` is assumed to be a list from which a colormap
+    will be retrieved. Colormaps that are strings will be converted to
+    the associated standard `Colormap` object, while enums in
+    :class:``config.Cmaps`` will be used to retrieve a `Colormap` object
     from :const:``CMAPS``, which is assumed to have been initialized.
     
     Args:
         cmap: Colormap given as a string of Enum or list of colormaps.
-        n: Index of `cmap` to retrieve a colormap, assuming that `cmap` 
+        n: Index of `cmap` to retrieve a colormap, assuming that `cmap`
             is a sequence. Defaults to None to use `cmap` directly.
     
     Returns:
-        The ``Colormap`` object, or None if no corresponding colormap 
+        The ``Colormap`` object, or None if no corresponding colormap
         is found.
     """
     if n is not None:
         # assume that cmap is a list
         cmap = config.cmaps[n] if n < len(cmap) else None
     if isinstance(cmap, str):
         # cmap given as a standard Matplotlib colormap name
```

### Comparing `magellanmapper-1.6b3/magmap/plot/plot_2d.py` & `magellanmapper-1.6b4/magmap/plot/plot_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1024,15 +1024,16 @@
         x_label: Optional[str] = None, y_label: Optional[str] = None,
         x_unit: Optional[str] = None, y_unit: Optional[str] = None,
         legend_names: Optional[Sequence[str]] = None,
         col_vspan: Optional[str] = None, vspan_fmt: Optional[str] = None,
         size: Optional[Sequence[float]] = None,
         ax: Optional["axes.Axes"] = None, rotation: Optional[float] = None,
         legend_title: Optional[str] = None,
-        kwargs_plot: Optional[Dict[str, Any]] = None, **kwargs) -> "axes.Axes":
+        kwargs_plot: Optional[Dict[str, Any]] = None, fn_plot: Callable = None,
+        **kwargs) -> "axes.Axes":
     """Generate a swarm/jitter plot in Seaborn.
     
     Supports x-axis scaling and vertical spans.
     
     Args:
         df: Data frame, assumed to be in melted format.
         x_cols: Column for x-values, typically categorical.
@@ -1046,35 +1047,40 @@
         x_unit: Unit for the x-axis; defaults to None.
         y_unit: Unit for the y-axis; defaults to None.
         legend_names: Legend names. Defaults to None to use those from
             ``group_col``
         col_vspan: Column for delineating vertical span groups. Groups
             are determined by contiguous values after reordering by ``x_order``.
             Defaults to None.
-        vspan_fmt: Vertical span label string format; defaulst to None.
+        vspan_fmt: Vertical span label string format.
         size: Figure size in ``width, height`` as inches; defaults to None.
         ax: Matplotlib axes; defaults to None.
         rotation: x-axis ttext angle rotation in degrees. Defaults to None,
             which will rotate by 45 degrees.
         legend_title: Legend title; defaults to None.
         kwargs_plot: Dictionary of arguments to :meth:`sns.swarmplot`; defaults
             to None.
+        fn_plot: Plotting function. If None (default), will use
+            :meth:`sns.swarmplot`. Typically, only similar Seaborn functions
+            are compatible.
         **kwargs: Additional arguments, passed to :meth:`decorate_plot`.
 
     Returns:
         Matplotlib axes with the plot.
     
     Raises:
         `ImportError` if Seaborn is not available.
 
     """
-    
-    if sns is None:
-        raise ImportError(
-            config.format_import_err("seaborn", task="swarm plots"))
+    if fn_plot is None:
+        # default to generating a swarm plot in Seaborn
+        if sns is None:
+            raise ImportError(
+                config.format_import_err("seaborn", task="swarm plots"))
+        fn_plot = sns.swarmplot
     
     if kwargs_plot is None:
         kwargs_plot = {}
     
     df_vspan = df
     if x_order is not None:
         # reorder so vals in x_cols match the order of vals in x_order;
@@ -1092,15 +1098,15 @@
         ax = fig.add_subplot(gs[0, 0])
     
     # convert to scientific notation if appropriate before plot since the
     # plot's formatter may otherwise be incompatible
     plot_support.set_scinot(ax, lbls=(y_label, x_label), units=(y_unit, x_unit))
     
     # plot in seaborn
-    ax = sns.swarmplot(
+    ax = fn_plot(
         x=x_cols, y=y_cols, hue=group_col, hue_order=legend_names,
         order=x_order, data=df, ax=ax, **kwargs_plot)
     
     # scale x-axis ticks and rotate labels
     if rotation is None:
         rotation = 45
     plot_support.scale_xticks(ax, rotation)
@@ -1110,14 +1116,16 @@
         # make legend translucent in case it overlaps points and remove
         # legend title
         legend.get_frame().set(alpha=0.5)
         legend.set_title(legend_title if legend_title else None)
 
     if col_vspan is not None:
         # add vertical spans
+        if x_order is None:
+            libmag.warn("Need to set `x_order` for vertical spans")
         vspans, vspan_lbls = plot_support.setup_vspans(
             df_vspan, col_vspan, vspan_fmt)
         plot_support.add_vspans(ax, vspans, vspan_lbls, 1, True)
     
     # add additional decorations
     ax = decorate_plot(
         ax, xlabel=x_label, ylabel=y_label, xunit=x_unit, yunit=y_unit,
```

### Comparing `magellanmapper-1.6b3/magmap/plot/plot_3d.py` & `magellanmapper-1.6b4/magmap/plot/plot_3d.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/plot/plot_support.py` & `magellanmapper-1.6b4/magmap/plot/plot_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         
         return img
     
     def overlay_images(
             self, imgs2d: Sequence[np.ndarray],
             channels: Optional[List[List[int]]],
             cmaps: Sequence[Union[
-                str, "colors.Colormap", colormaps.DiscreteColormap]],
+                str, "colors.Colormap", Sequence["colors.Colormap"]]],
             alphas: Optional[Union[
                 float, Sequence[Union[float, Sequence[float]]]]] = None,
             vmins: Optional[Union[
                 float, Sequence[Union[float, Sequence[float]]]]] = None,
             vmaxs: Optional[Union[
                 float, Sequence[Union[float, Sequence[float]]]]] = None,
             check_single: bool = False,
@@ -592,43 +592,50 @@
         for multiple channels. Subsequent images are typically label images,
         which may or may not have multple channels.
         
         Args:
             imgs2d: Sequence of 2D images to display,
                 where the first image may be 2D+channel.
             channels: A nested list of channels to display for
-                each image, or None to use :attr:``config.channel`` for the
+                each image, or None to use
+                :attr:``magmap.settings.config.channel`` for the
                 first image and 0 for all subsequent images.
-            cmaps: Either a single colormap for all images or a list of
-                colormaps corresponding to each image. Colormaps of type
-                :class:`colormaps.DiscreteColormap` will have their
-                normalization object applied as well. If a color is given for
-                :obj:`config.AtlasLabels.BINARY` in :attr:`config.atlas_labels`,
-                images with :class:`colormaps.DiscreteColormap` will be
+            cmaps: Either a single colormap for all images or a sequence of
+                colormaps corresponding to each image. If a sequence, the first
+                value should be another sequence corresponding to all channels,
+                including channels not included in ``channels``. Colormaps of
+                type :class:`magmap.plot.colormaps.DiscreteColormap` will have
+                their normalization object applied as well. If a color is
+                given for :obj:`magmap.settings.config.AtlasLabels.BINARY`
+                in :attr:`magmap.settings.config.atlas_labels`, images with
+                :class:`magmap.plot.colormaps.DiscreteColormap` will be
                 converted to NaN for foreground to use this color.
-            alphas: Either a single alpha for all images or a list of
-                alphas corresponding to each image. Defaults to None to use
-                :attr:`config.alphas`, filling with 0.9 for any additional
-                values required and :attr:`config.plot_labels` for the first value.
-            vmins: A list of vmins for each image; defaults to None to use
-                :attr:``config.vmins`` for the first image and None for all others.
-            vmaxs: A list of vmaxs for each image; defaults to None to use
-                :attr:``config.vmax_overview`` for the first image and None
-                for all others.
+            alphas: Image opacity, given in the same format as for ``cmaps``.
+                ``None`` to use :attr:`magmap.settings.config.alphas`,
+                filling with 0.9 for any additional values required and
+                :attr:`magmap.settings.config.plot_labels` for the first value.
+            vmins: Minimum intensities, given in the same format as for
+                ``cmaps``. ``None`` to use
+                :attr:``magmap.settings.config.vmins`` for the first
+                 image and None for all others.
+            vmaxs: Maximum intensities, given in the same format as for
+                ``cmaps``. ``None`` to use
+                :attr:``magmap.settings.config.vmax_overview`` for
+                the first image and None for all others.
             check_single: True to check for images with a single unique
-                value displayed with a :class:`colormaps.DiscreteColormap`, which
+                value displayed with a
+                :class:`magmap.plot.colormaps.DiscreteColormap`, which
                 will not update for unclear reasons. If found, the final value
                 will be incremented by one as a workaround to allow updates.
-                Defaults to False.
-            alpha_blends: Opacity blending values for each image in ``imgs2d``;
-                defaults to None.
+            alpha_blends: Opacity blending values for each image in ``imgs2d``.
         
         Returns:
-            Nested list containing a list of Matplotlib image objects 
+            Nested list containing a list of Matplotlib image objects
             corresponding to display of each ``imgs2d`` image.
+        
         """
         ax_imgs = []
         num_imgs2d = len(imgs2d)
         if num_imgs2d < 1: return None
     
         # fill default values for each set of 2D images
         img_norm_setting = config.roi_profile["norm"]
@@ -1304,15 +1311,15 @@
         # default to use existing labels
         x_labels = ax.get_xticklabels()
     
     font_size = plt.rcParams["axes.titlesize"]
     if libmag.is_number(font_size):
         # scale font size of x-axis labels by a sigmoid function to rapidly
         # decrease size for larger numbers of labels so they don't overlap
-        font_size *= (math.atan(len(x_labels) / 10 - 5) * -2 / math.pi + 1) / 2
+        font_size *= (math.atan(len(x_labels) / 30 - 5) * -2 / math.pi + 1) / 2
     font_dict = {"fontsize": font_size}
     
     # draw x-ticks based on number of bars per group and align to right
     # since center shifts the horiz middle of the label to the center;
     # rotation_mode in dict helps but still slightly off
     ax.set_xticklabels(
         x_labels, rotation=rotation, horizontalalignment="right",
@@ -1378,14 +1385,15 @@
     
     if vspans is not None:
         # show vertical spans alternating in white and black; assume
         # background is already white, so simply skip white shading
         for i, x in enumerate(xs):
             if i % 2 == 0: continue
             end = xs[i + 1] if i < num_xs - 1 else num_groups
+            ax.margins(x=0)  # otherwise axvspan increases x-margin
             ax.axvspan(x, end, facecolor="k", alpha=0.2, zorder=0)
 
     if vspan_lbls is not None:
         # show labels for vertical spans
         x_max = num_groups
         for i, x in enumerate(xs):
             # set x to middle of span
```

### Comparing `magellanmapper-1.6b3/magmap/settings/atlas_prof.py` & `magellanmapper-1.6b4/magmap/settings/atlas_prof.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/settings/config.py` & `magellanmapper-1.6b4/magmap/settings/config.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/settings/grid_search_prof.py` & `magellanmapper-1.6b4/magmap/settings/grid_search_prof.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/settings/logs.py` & `magellanmapper-1.6b4/magmap/settings/logs.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/settings/prefs_prof.py` & `magellanmapper-1.6b4/magmap/settings/prefs_prof.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     roi_styles: str = ""
     
     #: Figure save directory path.
     fig_save_dir: str = ""
 
     #: Import directory path.
     import_dir: str = ""
+    
+    #: Path to last opened image.
+    img_open_path: str = ""
 
     def __init__(self, *args, **kwargs):
         """Initialize a preferences profile dictionary.
         
         Args:
             *args: 
             **kwargs:
```

### Comparing `magellanmapper-1.6b3/magmap/settings/profiles.py` & `magellanmapper-1.6b4/magmap/settings/profiles.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/settings/roi_prof.py` & `magellanmapper-1.6b4/magmap/settings/roi_prof.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         "erosion_threshold",
         "adapt_hist_lim",
     )
     BLOCK_SIZES = (
         "segment_size",
         "denoise_size",
         "prune_tol_factor",
-        "verify_tol_factor",
         "sub_stack_max_pixels",
         "isotropic",
     )
 
     def __init__(self, *args, **kwargs):
         """Initialize an ROI profile dictionary.
```

### Comparing `magellanmapper-1.6b3/magmap/stats/atlas_stats.py` & `magellanmapper-1.6b4/magmap/stats/atlas_stats.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/stats/clustering.py` & `magellanmapper-1.6b4/magmap/stats/clustering.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/stats/mlearn.py` & `magellanmapper-1.6b4/magmap/stats/mlearn.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/stats/vols.py` & `magellanmapper-1.6b4/magmap/stats/vols.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_chunking.py` & `magellanmapper-1.6b4/magmap/tests/test_chunking.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_classifier.py` & `magellanmapper-1.6b4/magmap/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_cv_nd.py` & `magellanmapper-1.6b4/magmap/tests/test_cv_nd.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_detector.py` & `magellanmapper-1.6b4/magmap/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_img_equality.py` & `magellanmapper-1.6b4/magmap/tests/test_img_equality.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_libmag.py` & `magellanmapper-1.6b4/magmap/tests/test_libmag.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/test_visualizer.py` & `magellanmapper-1.6b4/magmap/tests/test_visualizer.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/magmap/tests/unit_testing.py` & `magellanmapper-1.6b4/magmap/tests/unit_testing.py`

 * *Files identical despite different names*

### Comparing `magellanmapper-1.6b3/setup.py` & `magellanmapper-1.6b4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,40 +43,45 @@
     # backend error with 5.15.8
     "PyQt5 != 5.15.8",
     "pyface",
     "traitsui",
 ]
 
 #: Optional dependencies for the 3D viewer.
-_EXTRAS_3D = ["mayavi"]
+_EXTRAS_3D = [
+    "mayavi",
+    # WORKAROUND: error in VTK 9.3.0 with Mayavi 4.8.1
+    "vtk < 9.3.0",
+]
 
 #: Optional pre-built SimpleITK with Elastix for image I/O and registration.
 _EXTRAS_SIMPLEITK = [
     "simpleitk==2.0.2rc2.dev785+g8ac4f ; python_version < '3.8'",
     "simpleitk==2.3.0.dev117+g0640d ; python_version >= '3.8'",
 ]
 
 #: Optional ITK and Elastix for image I/O and registration.
+#: `itk` not included since it does not load properly when installed with rest
+#: of dependencies. `itk-elastix` also installs a later `itk` version.
 _EXTRAS_ITK = [
-    "itk",
     "itk-elastix",
 ]
 
 
 # installation configuration
 config = {
     "name": "magellanmapper",
     "description": "3D atlas analysis and annotation",
     "long_description": open("README.md").read(),
     "long_description_content_type": "text/markdown",
     "author": "David Young",
     "url": "https://github.com/sanderslab/magellanmapper",
     "author_email": "david@textflex.com",
     "license": "BSD-3",
-    "version": "1.6b3",
+    "version": "1.6b4",
     "packages": setuptools.find_packages(),
     "scripts": [],
     "python_requires": ">=3.6",
     "entry_points": {
         # gui_scripts doesn't load because of TraitsUI issue #1032
         "console_scripts": ["mm = magmap.io.load_env:launch_magmap"],
     },
```

