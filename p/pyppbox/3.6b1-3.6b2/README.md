# Comparing `tmp/pyppbox-3.6b1.tar.gz` & `tmp/pyppbox-3.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-3.6b1.tar", last modified: Wed Apr 10 20:09:22 2024, max compression
+gzip compressed data, was "pyppbox-3.6b2.tar", last modified: Sat Apr 13 13:49:14 2024, max compression
```

## Comparing `pyppbox-3.6b1.tar` & `pyppbox-3.6b2.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-10 20:09:15.000000 pyppbox-3.6b1/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 20:09:15.000000 pyppbox-3.6b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-10 20:09:15.000000 pyppbox-3.6b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-10 20:09:22.893230 pyppbox-3.6b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-10 20:09:15.000000 pyppbox-3.6b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-10 20:09:15.000000 pyppbox-3.6b1/RELEASENOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/cfg.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/detectors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/reiders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/cfg/trackers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/configtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/myconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/config/unifiedstrings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.873230 pyppbox-3.6b1/pyppbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.877230 pyppbox-3.6b1/pyppbox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/modules/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/data/res/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/res/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/data/res/idmap.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.881230 pyppbox-3.6b1/pyppbox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/TReID.png
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guidemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guihub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/guitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/gui/tmp/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/tmp/input.tmp
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/tmp/ui.tmp
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_facenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_torchreid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_yolocls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/gui/ui_yoloult.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/detect_face.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/facenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.885230 pyppbox-3.6b1/pyppbox/modules/trackers/centroid/
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/centroid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/sort/
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.889230 pyppbox-3.6b1/pyppbox/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/standalone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52132 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/standalone/mt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/pyppbox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/evatools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/gttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/mot2pyppbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/persontools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/restools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyppbox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/pyppbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 20:09:22.000000 pyppbox-3.6b1/pyppbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 20:09:15.000000 pyppbox-3.6b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:09:22.893230 pyppbox-3.6b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-10 20:09:15.000000 pyppbox-3.6b1/requirements/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:09:22.893230 pyppbox-3.6b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-10 20:09:15.000000 pyppbox-3.6b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-10 20:09:15.000000 pyppbox-3.6b1/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.237316 pyppbox-3.6b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-13 13:49:08.000000 pyppbox-3.6b2/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 13:49:08.000000 pyppbox-3.6b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-13 13:49:08.000000 pyppbox-3.6b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-13 13:49:14.233316 pyppbox-3.6b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-13 13:49:08.000000 pyppbox-3.6b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-04-13 13:49:08.000000 pyppbox-3.6b2/RELEASENOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.213316 pyppbox-3.6b2/pyppbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/cfg.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/detectors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/reiders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/cfg/trackers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/configtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65155 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/myconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/config/unifiedstrings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.209315 pyppbox-3.6b2/pyppbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.217316 pyppbox-3.6b2/pyppbox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/modules/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/data/res/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/res/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/data/res/idmap.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.221315 pyppbox-3.6b2/pyppbox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   833181 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/TReID.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guidemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guihub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/guitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/gui/tmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/tmp/input.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/tmp/ui.tmp
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_facenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23388 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_torchreid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_yolocls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13885 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/gui/ui_yoloult.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/
+-rw-r--r--   0 runner    (1001) docker     (127)    13251 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.225316 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31858 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/detect_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/facenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/centroid/
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/centroid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.229316 pyppbox-3.6b2/pyppbox/modules/trackers/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/ppb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/ppb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52182 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/ppb/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/standalone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/evatools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13446 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/gttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/mot2pyppbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/persontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/restools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyppbox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/pyppbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 13:49:14.000000 pyppbox-3.6b2/pyppbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 13:49:08.000000 pyppbox-3.6b2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:49:14.233316 pyppbox-3.6b2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-13 13:49:08.000000 pyppbox-3.6b2/requirements/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:49:14.237316 pyppbox-3.6b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-13 13:49:08.000000 pyppbox-3.6b2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-13 13:49:08.000000 pyppbox-3.6b2/setup_extra.yaml
```

### Comparing `pyppbox-3.6b1/GETSTARTED.md` & `pyppbox-3.6b2/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/LICENSE` & `pyppbox-3.6b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/PKG-INFO` & `pyppbox-3.6b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.6b1
+Version: 3.6b2
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.6b1/README.md` & `pyppbox-3.6b2/README.md`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/RELEASENOTES.md` & `pyppbox-3.6b2/RELEASENOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 # Release Notes 
 
+## **pyppbox V4 - Even Smaller**
+
+* `pyppbox` v4.0b1 (COMING SOON 🚀)
+
+  - `pyppbox` will leverage [`vsensebox`](https://github.com/rathaumons/vsensebox) for detection and tracking
+  - `pyppbox.utils.persontools` will change to adapt [`vsensebox`](https://github.com/rathaumons/vsensebox)
+  - `pyppbox.ppb` will replace `pyppbox.standalone`
+  - All configuration files will also change
+  - More changes will be added here! Stay tuned!
+
 ## **pyppbox V3 - Make Simpler and Faster**
 
-* `pyppbox` [v3.6b1](https://github.com/rathaumons/pyppbox/tree/v3.5b2)
+* `pyppbox` [v3.6b2](https://github.com/rathaumons/pyppbox/tree/v3.6b2)
+
+  - Add a warning for the changes in the coming major version 4
+  - Update documentations
+  - **Known issue/limitation**:
+    - You tell me :)
+
+* `pyppbox` [v3.6b1](https://github.com/rathaumons/pyppbox/tree/v3.6b1)
 
   - Replace `pyunpack` & `patool` with `shutil`
   - Improve Example 9 - example_09_eva_offline.py
   - Add `pyppbox.gui.guitools` to the documentations
   - Fix `useInternalConfigDir()` in `pyppbox.gui.guitools`
   - Fix sphinx-build warning for utils.rst
   - Fix and improve documentations
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyppbox-3.6b1/pyppbox/__init__.py` & `pyppbox-3.6b2/pyppbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     useInternalConfigDir, 
     useThisConfigDir,
     resetInternalConfig,
     generateConfig
 )
 
 
-__version__ = '3.6b1'
+__version__ = '3.6b2'
 __author__ = 'Ratha SIV'
 __description__ = 'Toolbox for people detecting, tracking, and re-identifying.'
 __homepage__ = 'https://rathaumons.github.io/pyppbox'
 __url__ = 'https://github.com/rathaumons/pyppbox.git'
```

### Comparing `pyppbox-3.6b1/pyppbox/config/__init__.py` & `pyppbox-3.6b2/pyppbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/cfg/cfg.zip` & `pyppbox-3.6b2/pyppbox/config/cfg/cfg.zip`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/cfg/detectors.yaml` & `pyppbox-3.6b2/pyppbox/config/cfg/detectors.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/cfg/reiders.yaml` & `pyppbox-3.6b2/pyppbox/config/cfg/reiders.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/cfg/trackers.yaml` & `pyppbox-3.6b2/pyppbox/config/cfg/trackers.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/configtools.py` & `pyppbox-3.6b2/pyppbox/config/configtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/myconfig.py` & `pyppbox-3.6b2/pyppbox/config/myconfig.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/config/unifiedstrings.py` & `pyppbox-3.6b2/pyppbox/config/unifiedstrings.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/__init__.py` & `pyppbox-3.6b2/pyppbox/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/assets/TReID.png` & `pyppbox-3.6b2/pyppbox/gui/assets/TReID.png`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/assets/icon.ico` & `pyppbox-3.6b2/pyppbox/gui/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/assets/settings.ico` & `pyppbox-3.6b2/pyppbox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/guidemo.py` & `pyppbox-3.6b2/pyppbox/gui/guidemo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/guihub.py` & `pyppbox-3.6b2/pyppbox/gui/guihub.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/guitools.py` & `pyppbox-3.6b2/pyppbox/gui/guitools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_centroid.py` & `pyppbox-3.6b2/pyppbox/gui/ui_centroid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_deepsort.py` & `pyppbox-3.6b2/pyppbox/gui/ui_deepsort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_facenet.py` & `pyppbox-3.6b2/pyppbox/gui/ui_facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_gt.py` & `pyppbox-3.6b2/pyppbox/gui/ui_gt.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_launcher.py` & `pyppbox-3.6b2/pyppbox/gui/ui_launcher.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_sort.py` & `pyppbox-3.6b2/pyppbox/gui/ui_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_torchreid.py` & `pyppbox-3.6b2/pyppbox/gui/ui_torchreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_yolocls.py` & `pyppbox-3.6b2/pyppbox/gui/ui_yolocls.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/gui/ui_yoloult.py` & `pyppbox-3.6b2/pyppbox/gui/ui_yoloult.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/detectors/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/detectors/yolocls/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/detectors/yolocls/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,33 +52,33 @@
         self.cfg = cfg
         net = cv2.dnn.readNet(cfg.model_weights, cfg.model_cfg_file)
         net.setPreferableBackend(cv2.dnn.DNN_BACKEND_CUDA)
         net.setPreferableTarget(cv2.dnn.DNN_TARGET_CUDA)
         self.model = cv2.dnn_DetectionModel(net)
         self.model.setInputParams(size=cfg.model_resolution, scale=1/255.0)
 
-    def detect(self, img, visual=True, class_filter=0, min_width_filter=35):
+    def detect(self, img, visual=True, class_filter=[0], min_width_filter=35):
         """Detect general object with object's class filter :obj:`class_filter` in a 
-        given cv :obj:`Mat` image.
+        given :obj:`Mat` like image.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         visual : bool, default=True
             An indication of whether to visualize the detected objects.
-        class_filter : int, defualt=0
-            Object's class filter, 0 means person only
+        class_filter : list[int, ...], defualt=0
+            Object's class filter, [0] = Person only.
         min_width_filter : int, default=35
             Mininum width filter of a detected object.
 
         Returns
         -------
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         list[ndarray[int, int, int, int], ...]
             A list of bounding box :code:`ndarray[x, y, width, height]`.
         list[ndarray[int, int, int, int], ...]
             A list of bounding box :code:`ndarray[x1, y1, x2, y2]`.
         list[tuple(int, int)]
             A lsit of represented 2D point :code:`(x, y)` of every detected object.
         float
@@ -89,15 +89,15 @@
         repspoints = []
         confs = []
         classes, confidences, boxes = self.model.detect(img, 
                                                         confThreshold=float(self.cfg.conf), 
                                                         nmsThreshold=float(self.cfg.nms))
         if len(classes) > 0:
             for class_id, conf, box_xywh in zip(classes.flatten(), confidences, boxes):
-                if class_id == class_filter and box_xywh[2] >= min_width_filter:
+                if class_id in class_filter and box_xywh[2] >= min_width_filter:
                     box_xywh = box_xywh.astype(int)
                     pboxes_xywh.append(box_xywh)
                     box_xyxy = to_xyxy(box_xywh)
                     pboxes_xyxy.append(box_xyxy)
                     repspoint = findRepspoint(box_xyxy, self.cfg.repspoint_calibration)
                     repspoints.append(repspoint)
                     confs.append(float(conf))
@@ -105,35 +105,35 @@
                         cv2.circle(img, (repspoint[0], repspoint[1]), radius=5, 
                                    color=(0, 0, 255), thickness=-1)
                         cv2.rectangle(img, (box_xyxy[0], box_xyxy[1]), 
                                       (box_xyxy[2], box_xyxy[3]), (255, 255, 0), 2)
         return img, pboxes_xywh, pboxes_xyxy, repspoints, confs
 
     def detectPeople(self, img, visual=True, min_width_filter=35, alt_repspoint=False, alt_repspoint_top=True):
-        """Detect person(s) in a given cv :obj:`Mat` image.
+        """Detect person(s) in a given :obj:`Mat` like image.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         visual : bool, default=True
             An indication of whether to visualize the detected people.
         min_width_filter : int, default=35
             Mininum width filter of a detected person.
         alt_repspoint : bool, default=False
             An indication of whether to use the alternative :meth:`findRepspointBB`.
         alt_repspoint_top : bool, default=True
             A parameter passed to :obj:`prefer_top` of :meth:`findRepspointBB`.
 
         Returns
         -------
         list[Person, ...]
             A list of detected :class:`Person` object.
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         """
         people = []
         classes, confidences, boxes = self.model.detect(
             img, 
             confThreshold=float(self.cfg.conf), 
             nmsThreshold=float(self.cfg.nms)
         )
```

### Comparing `pyppbox-3.6b1/pyppbox/modules/detectors/yoloult/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/detectors/yoloult/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,31 +113,31 @@
                     pos2[0] < 0 or pos2[1] < 0):
                     continue
                 cv2.line(img, pos1, pos2, [int(x) for x in limb_color[i]], 
                          thickness=2, lineType=cv2.LINE_AA)
 
     def detect(self, img, visual=True, classes=0, min_width_filter=35):
         """Detect general object with object's class filter :obj:`class_filter` 
-        in a given cv :obj:`Mat` image.
+        in a given :obj:`Mat` like image.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         visual : bool, default=True
             An indication of whether to visualize the detected objects.
         classes : int, defualt=0
             Object's class filter, 0 means person only
         min_width_filter : int, default=35
             Mininum width filter of a detected object.
 
         Returns
         -------
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         list[ndarray[int, int, int, int], ...]
             A list of bounding box :code:`ndarray[x, y, width, height]`.
         list[ndarray[int, int, int, int], ...]
             A list of bounding box :code:`ndarray[x1, y1, x2, y2]`.
         list[tuple(int, int)]
             A lsit of represented 2D point :code:`(x, y)` of every detected object.
         list[ndarray[int, ...], ...]
@@ -201,35 +201,35 @@
                         cv2.circle(img, (repspoint[0], repspoint[1]), 
                                    radius=5, color=(0, 0, 255), thickness=-1)
                         cv2.rectangle(img, (box_xyxy[0], box_xyxy[1]), 
                                       (box_xyxy[2], box_xyxy[3]), (255, 255, 0), 2)
         return img, pboxes_xywh, pboxes_xyxy, repspoints, keypoints, confs
 
     def detectPeople(self, img, visual=True, min_width_filter=35, alt_repspoint=False, alt_repspoint_top=True):
-        """Detect person(s) in a given cv :obj:`Mat` image.
+        """Detect person(s) in a given :obj:`Mat` like image.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         visual : bool, default=True
             An indication of whether to visualize the detected people.
         min_width_filter : int, default=35
             Mininum width filter of a detected person.
         alt_repspoint : bool, default=False
             An indication of whether to use the alternative :meth:`findRepspointBB`.
         alt_repspoint_top : bool, default=True
             A parameter passed to :obj:`prefer_top` of :meth:`findRepspointBB`.
 
         Returns
         -------
         list[Person, ...]
             A list of detected :class:`Person` object.
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         """
         numpy_dets = []
         people = []
         dets = self.model.predict(
             img,
             imgsz=int(self.cfg.imgsz),
             conf=float(self.cfg.conf),
```

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     def recognize(self, img, is_bgr=True):
         """Recognize or re-identify a person in the given :obj:`img`.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         is_bgr : bool, default=True
             An indication of whether the color channel of given :obj:`img` is BGR.
 
         Returns
         -------
         str
             A class name.
```

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/align_dataset_mtcnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/detect_face.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/detect_face.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/facenet/origin/facenet.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/facenet/origin/facenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def recognize(self, img, is_bgr=True):
         """Recognize or re-identify a person in the given :obj:`img`.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         is_bgr : bool, default=True
             An indication of whether the color channel of given :obj:`img` is BGR.
 
         Returns
         -------
         str
             A class name.
```

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/model_dict.yaml` & `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/model_dict.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/reiders/torchreid/utils.py` & `pyppbox-3.6b2/pyppbox/modules/reiders/torchreid/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/centroid/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         """Update the tracker and return the updated list of :class:`Person`.
 
         Parameters
         ----------
         person_list : list[Person, ...]
             A list of :class:`Person` object which stores the detected people in the given :obj:`img`.
         img : any, default=None
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         max_spread : int, default=5
             Max spread or max margin used to decide whether 2 bounding boxes are the same by comparing 
             the differences between the elements in the bounding box given by the embedded SORT and the 
             coressponding elements of a person's bounding box in the :obj:`person_list`.
 
         Returns
         -------
```

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/generate_detections.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/generate_detections.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/iou_matching.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/iou_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/nn_matching.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/nn_matching.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/preprocessing.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/track.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/track.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/deepsort/origin/tracker.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/deepsort/origin/tracker.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/sort/__init__.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/modules/trackers/sort/origin/sort.py` & `pyppbox-3.6b2/pyppbox/modules/trackers/sort/origin/sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/standalone/__init__.py` & `pyppbox-3.6b2/pyppbox/ppb/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 """
 Standalone is designed for easy detect, track, and reid people in a single thread 
 enviroment or in command line. 
 
-For multithreading application, see :py:class:`pyppbox.standalone.mt.MT`.
+For multithreading application, see :py:class:`pyppbox.ppb.mt.MT`.
 
 Example:
 
 >>> import cv2
 >>> from pyppbox.standalone import (setMainDetector, detectPeople, 
 >>>                                 setMainReIDer, reidPeople)
 >>> from pyppbox.utils.visualizetools import visualizePeople
@@ -65,70 +65,70 @@
 >>> 
 
 """
 
 
 from .mt import MT
 
-__stdmt__ = MT()
+_mt = MT()
 
 def setConfigDir(config_dir=None, load_all=False):
-    """See :func:`pyppbox.standalone.mt.MT.setConfigDir`"""
-    __stdmt__.setConfigDir(config_dir=config_dir, load_all=load_all)
+    """See :func:`pyppbox.ppb.mt.MT.setConfigDir`"""
+    _mt.setConfigDir(config_dir=config_dir, load_all=load_all)
 
 def setMainModules(main_yaml=None, load_all=True):
-    """See :func:`pyppbox.standalone.mt.MT.setMainModules`"""
-    __stdmt__.setMainModules(main_yaml=main_yaml, load_all=load_all)
+    """See :func:`pyppbox.ppb.mt.MT.setMainModules`"""
+    _mt.setMainModules(main_yaml=main_yaml, load_all=load_all)
 
 def getConfig():
-    """See :func:`pyppbox.standalone.mt.MT.getConfig`"""
-    return __stdmt__.getConfig()
+    """See :func:`pyppbox.ppb.mt.MT.getConfig`"""
+    return _mt.getConfig()
 
 def forceFullGTMode():
-    """See :func:`pyppbox.standalone.mt.MT.forceFullGTMode`"""
-    __stdmt__.forceFullGTMode()
+    """See :func:`pyppbox.ppb.mt.MT.forceFullGTMode`"""
+    _mt.forceFullGTMode()
 
 def setMainDetector(detector=""):
-    """See :func:`pyppbox.standalone.mt.MT.setMainDetector`"""
-    __stdmt__.setMainDetector(detector=detector)
+    """See :func:`pyppbox.ppb.mt.MT.setMainDetector`"""
+    _mt.setMainDetector(detector=detector)
 
 def detectPeople(img, 
                  img_is_mat=False, 
                  visual=False, 
                  save=False, 
                  save_file="", 
                  min_width_filter=35, 
                  alt_repspoint=False, 
                  alt_repspoint_top=True):
-    """See :func:`pyppbox.standalone.mt.MT.detectPeople`"""
-    return __stdmt__.detectPeople(img, 
+    """See :func:`pyppbox.ppb.mt.MT.detectPeople`"""
+    return _mt.detectPeople(img, 
                                   img_is_mat=img_is_mat, 
                                   visual=visual, 
                                   save=save, 
                                   save_file=save_file, 
                                   min_width_filter=min_width_filter, 
                                   alt_repspoint=alt_repspoint, 
                                   alt_repspoint_top=alt_repspoint_top)
 
 def setMainTracker(tracker=""):
-    """See :func:`pyppbox.standalone.mt.MT.setMainTracker`"""
-    __stdmt__.setMainTracker(tracker=tracker)
+    """See :func:`pyppbox.ppb.mt.MT.setMainTracker`"""
+    _mt.setMainTracker(tracker=tracker)
 
 def trackPeople(img, people, img_is_mat=False):
-    """See :func:`pyppbox.standalone.mt.MT.trackPeople`"""
-    return __stdmt__.trackPeople(img, people, img_is_mat=img_is_mat)
+    """See :func:`pyppbox.ppb.mt.MT.trackPeople`"""
+    return _mt.trackPeople(img, people, img_is_mat=img_is_mat)
 
 def setMainReIDer(reider="", auto_load=True):
-    """See :func:`pyppbox.standalone.mt.MT.setMainReIDer`"""
-    __stdmt__.setMainReIDer(reider=reider, auto_load=auto_load)
+    """See :func:`pyppbox.ppb.mt.MT.setMainReIDer`"""
+    _mt.setMainReIDer(reider=reider, auto_load=auto_load)
 
 def reidPeople(img, people, deduplicate=True, img_is_mat=False):
-    """See :func:`pyppbox.standalone.mt.MT.reidPeople`"""
-    return __stdmt__.reidPeople(img, people, deduplicate=deduplicate, img_is_mat=img_is_mat)
+    """See :func:`pyppbox.ppb.mt.MT.reidPeople`"""
+    return _mt.reidPeople(img, people, deduplicate=deduplicate, img_is_mat=img_is_mat)
 
 def trainReIDClassifier(reider="Default", train_data="", classifier_pkl=""):
-    """See :func:`pyppbox.standalone.mt.MT.trainReIDClassifier`"""
-    __stdmt__.trainReIDClassifier(reider=reider, train_data=train_data, classifier_pkl=classifier_pkl)
+    """See :func:`pyppbox.ppb.mt.MT.trainReIDClassifier`"""
+    _mt.trainReIDClassifier(reider=reider, train_data=train_data, classifier_pkl=classifier_pkl)
 
 __all__ = ['setConfigDir', 'setMainModules', 'getConfig', 'forceFullGTMode', 
            'setMainDetector', 'detectPeople', 'setMainTracker', 'trackPeople', 
            'setMainReIDer', 'reidPeople', 'trainReIDClassifier', 'MT']
```

### Comparing `pyppbox-3.6b1/pyppbox/standalone/mt.py` & `pyppbox-3.6b2/pyppbox/ppb/mt.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,17 +420,17 @@
                      alt_repspoint_top=True): 
         """Detect people by giving an image. :func:`setConfigDir()` or :func:`setMainDetector()` must 
         be called in advance.
 
         Parameters
         ----------
         img : str or Mat
-            Set an image file or a cv :obj:`Mat`.
+            Set an image file or a :obj:`Mat` like image.
         img_is_mat : bool, default=False
-            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+            Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like image.
         visual : bool, default=False
             Decide whether to visualize like drawing bounding boxes and keypoints to the 
             return :obj:`img`.
         save : bool, default=False
             Decide whether to save the return :obj:`img` to a JPG file.
         save_file : str, default=""
             Indicate a path of where to save the processed image.
@@ -442,15 +442,15 @@
             A parameter passed to :obj:`prefer_top` of :meth:`findRepspointBB`.
         
         Returns
         -------
         list[Person, ...]
             A  list of :class:`Person` object.
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         """ 
         people = []
         if self.__dt_is_set__: 
             if not isinstance(self.__dt__, NothingDetecter):
                 if not img_is_mat: img = getCVMat(img)
                 if (self.__dt_cfg__.dt_name.lower() == self.__unistrings__.yolo_cls or 
                     self.__dt_cfg__.dt_name.lower() == self.__unistrings__.yolo_ult):
@@ -615,19 +615,19 @@
     def trackPeople(self, img, people, img_is_mat=False):
         """Track people by giving an image and a list of detected people. :func:`setConfigDir()` 
         or :func:`setMainTracker()` must be called in advance.
 
         Parameters
         ----------
         img : str or Mat
-            Set an image file or a cv :obj:`Mat`.
+            Set an image file or a :obj:`Mat` like image.
         people : list[Person, ...]
             Set a list of :class:`Person` object which stores the detected people in the input :obj:`img`.
         img_is_mat : bool, default=False
-            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+            Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like image.
         
         Returns
         -------
         list[Person, ...]
             A list of :class:`Person` object which stores people with updated IDs.
         """
         res = []
@@ -787,22 +787,22 @@
     def reidPeople(self, img, people, deduplicate=True, img_is_mat=False):
         """Re-identify people by giving an image and a list of detected or tracked people. 
         :func:`setConfigDir()` or :func:`setMainReIDer()` must be called in advance.
 
         Parameters
         ----------
         img : str or Mat
-            Set an image file or a cv :obj:`Mat`.
+            Set an image file or a :obj:`Mat` like image.
         people : list[Person, ...]
             Set a list of :class:`Person` object which stores the detected or tracked people in 
             the input :obj:`img`.
         deduplicate : bool, default=True
             Indicate whether to re-reid people who have the same face ids or deep ids.
         img_is_mat : bool, default=False
-            Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+            Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like image.
         
         Returns
         -------
         list[Person, ...]
             A list of :class:`Person` object which stores people with the updated IDs.
         tuple(int, int)
             A tuple of (ReID count, ReID deduplicate count).
```

### Comparing `pyppbox-3.6b1/pyppbox/utils/__init__.py` & `pyppbox-3.6b2/pyppbox/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/commontools.py` & `pyppbox-3.6b2/pyppbox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/evatools.py` & `pyppbox-3.6b2/pyppbox/utils/evatools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/gttools.py` & `pyppbox-3.6b2/pyppbox/utils/gttools.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,24 +269,24 @@
     def getPeople(self, img, visual=False):
         """Return a :code:`list[Person, ...]` and a cv :obj:`Mat`, similar to function 
         :func:`detectPeople()` in :py:mod:`pyppbox.standalone`.
 
         Parameters
         ----------
         img : Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         visual : 
             An indication of whether to draw bounding boxes on the return :obj:`img`.
 
         Returns
         -------
         list[Person, ...]
             A list of :class:`Person` object.
         Mat
-            A cv :obj:`Mat` image.
+            A :obj:`Mat` like image.
         """
         people = []
         tmp_id = 0
         for gt in self.findGTFrame(self.current_frame):
             box_xywh = convertStringToNPL(gt[3])
             box_xyxy = convertStringToNPL(gt[4])
             if self.detect_only:
```

### Comparing `pyppbox-3.6b1/pyppbox/utils/logtools.py` & `pyppbox-3.6b2/pyppbox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/mot2pyppbox.py` & `pyppbox-3.6b2/pyppbox/utils/mot2pyppbox.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/persontools.py` & `pyppbox-3.6b2/pyppbox/utils/persontools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/restools.py` & `pyppbox-3.6b2/pyppbox/utils/restools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/pyppbox/utils/visualizetools.py` & `pyppbox-3.6b2/pyppbox/utils/visualizetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 def visualizePeople(img, people, show_box=True, show_skl=(True,True,5), show_ids=(True,True,True), 
                     show_reid=(0,0), show_repspoint=True, img_is_mat=True):
     """Visualize people in the image by the given people. 
 
     Parameters
     ----------
     img : str or Mat
-        An image file or a cv :obj:`Mat`.
+        An image file or a :obj:`Mat` like image.
     people : list[Person, ...]
         Set a list of :class:`Person` object found in the input :obj:`img`.
     show_box : bool, default=True
         Indicate whether to visualize bounding boxes.
     show_skl : tuple(bool, bool, int), default=(True,True,5)
         Set how to visualize the keypoints and skeletons. 
         Set the first element to :code:`True` to visualize the keypoints.
@@ -124,20 +124,20 @@
         Set the third element to :code:`True` to visualize the deepid.
     show_reid : tuple(int, int), default=(0,0)
         :obj:`show_reid` is corresponding to :obj:`reid_count` in :func:`reidPeople()`
         Tuple of (ReID count, ReID deduplicate count)
     show_repspoint : bool, default=True
         Indicate whether to show the :obj:`repspoint` of :class:`Person` object.
     img_is_mat : bool, default=True
-        Speed up the function by telling whether the :obj:`img` is cv :obj:`Mat`.
+        Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like image.
     
     Returns
     -------
     Mat
-        A visualized cv :obj:`Mat`.
+        A visualized :obj:`Mat` like image.
     """
     # Overwrite `img_is_mat` to False when `img` is a file.
     if img_is_mat and isinstance(img, str): img_is_mat = False
     if not img_is_mat: img = getCVMat(img)
     if isinstance(people, list):
         if len(people) > 0:
             if isinstance(people[0], Person):
```

### Comparing `pyppbox-3.6b1/pyppbox.egg-info/PKG-INFO` & `pyppbox-3.6b2/pyppbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox
-Version: 3.6b1
+Version: 3.6b2
 Summary: Toolbox for people detecting, tracking, and re-identifying.
 Home-page: https://github.com/rathaumons/pyppbox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,People Detecting,People Tracking,People Re-Identification
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyppbox-3.6b1/pyppbox.egg-info/SOURCES.txt` & `pyppbox-3.6b2/pyppbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,17 @@
 pyppbox/modules/trackers/deepsort/origin/nn_matching.py
 pyppbox/modules/trackers/deepsort/origin/preprocessing.py
 pyppbox/modules/trackers/deepsort/origin/track.py
 pyppbox/modules/trackers/deepsort/origin/tracker.py
 pyppbox/modules/trackers/deepsort/origin/voc_classes.txt
 pyppbox/modules/trackers/sort/__init__.py
 pyppbox/modules/trackers/sort/origin/sort.py
+pyppbox/ppb/__init__.py
+pyppbox/ppb/mt.py
 pyppbox/standalone/__init__.py
-pyppbox/standalone/mt.py
 pyppbox/utils/__init__.py
 pyppbox/utils/commontools.py
 pyppbox/utils/evatools.py
 pyppbox/utils/gttools.py
 pyppbox/utils/logtools.py
 pyppbox/utils/mot2pyppbox.py
 pyppbox/utils/persontools.py
```

### Comparing `pyppbox-3.6b1/requirements/requirements.txt` & `pyppbox-3.6b2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/requirements/test_gpu.py` & `pyppbox-3.6b2/requirements/test_gpu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/setup.py` & `pyppbox-3.6b2/setup.py`

 * *Files identical despite different names*

### Comparing `pyppbox-3.6b1/setup_extra.yaml` & `pyppbox-3.6b2/setup_extra.yaml`

 * *Files identical despite different names*

