# Comparing `tmp/faster-coco-eval-1.4.3.tar.gz` & `tmp/faster_coco_eval-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-coco-eval-1.4.3.tar", last modified: Mon Mar  4 22:44:48 2024, max compression
+gzip compressed data, was "faster_coco_eval-1.5.1.tar", last modified: Sat Apr 13 21:04:00 2024, max compression
```

## Comparing `faster-coco-eval-1.4.3.tar` & `faster_coco_eval-1.5.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.600897 faster-coco-eval-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-04 22:44:48.600897 faster-coco-eval-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.592897 faster-coco-eval-1.4.3/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/csrc/faster_eval_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/csrc/faster_eval_api/coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/faster_eval_api/coco_eval/cocoeval.h
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/faster_eval_api/faster_eval_api.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.592897 faster-coco-eval-1.4.3/csrc/mask/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/csrc/mask/common/
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/mask/common/maskApi.c
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/mask/common/maskApi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/csrc/mask/pycocotools/
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/csrc/mask/pycocotools/_mask.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/faster_coco_eval/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/faster_coco_eval/core/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/core/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    21634 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/core/cocoeval.py
--rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/core/faster_eval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/core/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/faster_coco_eval/extra/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/extra/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/extra/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/extra/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/faster_coco_eval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.600897 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-04 22:44:48.000000 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-04 22:44:48.000000 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:44:48.000000 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-04 22:44:48.000000 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 22:44:48.000000 faster-coco-eval-1.4.3/faster_coco_eval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:44:48.596897 faster-coco-eval-1.4.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-04 22:44:48.600897 faster-coco-eval-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-03-04 22:44:42.000000 faster-coco-eval-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/faster_eval_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/faster_eval_api/faster_eval_api.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/common/maskApi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/common/maskApi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/csrc/mask/pycocotools/
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/csrc/mask/pycocotools/_mask.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.228935 faster_coco_eval-1.5.1/faster_coco_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16881 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/cocoeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/faster_eval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/core/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/extra/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/faster_coco_eval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 21:04:00.000000 faster_coco_eval-1.5.1/faster_coco_eval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 21:04:00.232935 faster_coco_eval-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-13 21:03:53.000000 faster_coco_eval-1.5.1/setup.py
```

### Comparing `faster-coco-eval-1.4.3/LICENSE` & `faster_coco_eval-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/PKG-INFO` & `faster_coco_eval-1.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.4.3
+Version: 1.5.1
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,21 @@
 Requires-Dist: numpy
 Requires-Dist: plotly
 Requires-Dist: pandas
 Requires-Dist: Pillow
 
 # Faster-COCO-Eval
 
+[![PyPI](https://img.shields.io/pypi/v/faster-coco-eval)](https://pypi.org/project/faster-coco-eval)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/faster-coco-eval.svg?label=PyPI%20downloads)](
+https://pypi.org/project/faster-coco-eval/)
+
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://github.com/MiXaiLL76/faster_coco_eval/wiki)
+[![license](https://img.shields.io/github/license/MiXaiLL76/faster_coco_eval.svg)](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/LICENSE)
+
 ## Disclaimer
 
 I often use this project, but I saw it abandoned and without a public repository on github.
 Also, part of the project remained unfinished for a long time. I implemented some of the author's ideas and decided to make the results publicly available.
 
 ## Faster-COCO-Eval base
 
@@ -38,21 +45,30 @@
 for coco's AP metrics, especially when dealing with a high number of instances in an image.
 
 ## Comparison
 
 For our use case with a test dataset of 5000 images from the coco val dataset.
 Testing was carried out using the mmdetection framework and the eval_metric.py script. The indicators are presented below.
 
-Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/comparison.ipynb)
+Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/mmdet/comparison.ipynb)
 Tested with yolo3 model (bbox eval) and yoloact model (segm eval)
 
-| Type | COCOeval    | COCOeval_faster | Profit      |
-| ---- | ----------- | --------------- | ----------- |
-| bbox | 18.477 sec. | 7.345 sec.      | 2.5x faster |
-| segm | 29.819 sec. | 15.840 sec.     | 2x faster   |
+### Summary for 5000 imgs
+
+| Type | COCOeval    | COCOeval_faster | Profit       |
+| ---- | ----------- | --------------- | ------------ |
+| bbox | 18.477 sec. | 7.345 sec.      | ~2.5x faster |
+| segm | 29.819 sec. | 15.840 sec.     | ~1.7x faster |
+
+## Summary for 500 imgs
+
+| Type | COCOeval  | COCOeval_faster | Profit       |
+| ---- | --------- | --------------- | ------------ |
+| bbox | 3.57 sec. | 2.03 sec.       | ~1.7x faster |
+| segm | 4.16 sec. | 2.41 sec.       | ~1.7x faster |
 
 ## Feautures
 
 This library provides not only validation functions, but also error visualization functions. Including visualization of errors in the image.  
 You can study in more detail in the [examples](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples) and [Wiki](https://github.com/MiXaiLL76/faster_coco_eval/wiki).
 
 ## Usage
@@ -63,7 +79,19 @@
 
 Available via link [history.md](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/history.md)
 
 ## License
 
 The original module was licensed with apache 2, I will continue with the same license.
 Distributed under the apache version 2.0 license, see [license](LICENSE) for more information.
+
+## Citation
+
+If you use this benchmark in your research, please cite this project.
+
+```
+@article{faster-coco-eval,
+  title   = {{Faster-COCO-Eval}: Faster interpretation of the original COCOEval},
+  author  = {MiXaiLL76},
+  year    = {2024}
+}
+```
```

### Comparing `faster-coco-eval-1.4.3/README.md` & `faster_coco_eval-1.5.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Faster-COCO-Eval
 
+[![PyPI](https://img.shields.io/pypi/v/faster-coco-eval)](https://pypi.org/project/faster-coco-eval)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/faster-coco-eval.svg?label=PyPI%20downloads)](
+https://pypi.org/project/faster-coco-eval/)
+
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://github.com/MiXaiLL76/faster_coco_eval/wiki)
+[![license](https://img.shields.io/github/license/MiXaiLL76/faster_coco_eval.svg)](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/LICENSE)
+
 ## Disclaimer
 
 I often use this project, but I saw it abandoned and without a public repository on github.
 Also, part of the project remained unfinished for a long time. I implemented some of the author's ideas and decided to make the results publicly available.
 
 ## Faster-COCO-Eval base
 
@@ -13,21 +20,30 @@
 for coco's AP metrics, especially when dealing with a high number of instances in an image.
 
 ## Comparison
 
 For our use case with a test dataset of 5000 images from the coco val dataset.
 Testing was carried out using the mmdetection framework and the eval_metric.py script. The indicators are presented below.
 
-Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/comparison.ipynb)
+Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/mmdet/comparison.ipynb)
 Tested with yolo3 model (bbox eval) and yoloact model (segm eval)
 
-| Type | COCOeval    | COCOeval_faster | Profit      |
-| ---- | ----------- | --------------- | ----------- |
-| bbox | 18.477 sec. | 7.345 sec.      | 2.5x faster |
-| segm | 29.819 sec. | 15.840 sec.     | 2x faster   |
+### Summary for 5000 imgs
+
+| Type | COCOeval    | COCOeval_faster | Profit       |
+| ---- | ----------- | --------------- | ------------ |
+| bbox | 18.477 sec. | 7.345 sec.      | ~2.5x faster |
+| segm | 29.819 sec. | 15.840 sec.     | ~1.7x faster |
+
+## Summary for 500 imgs
+
+| Type | COCOeval  | COCOeval_faster | Profit       |
+| ---- | --------- | --------------- | ------------ |
+| bbox | 3.57 sec. | 2.03 sec.       | ~1.7x faster |
+| segm | 4.16 sec. | 2.41 sec.       | ~1.7x faster |
 
 ## Feautures
 
 This library provides not only validation functions, but also error visualization functions. Including visualization of errors in the image.  
 You can study in more detail in the [examples](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples) and [Wiki](https://github.com/MiXaiLL76/faster_coco_eval/wiki).
 
 ## Usage
@@ -38,7 +54,19 @@
 
 Available via link [history.md](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/history.md)
 
 ## License
 
 The original module was licensed with apache 2, I will continue with the same license.
 Distributed under the apache version 2.0 license, see [license](LICENSE) for more information.
+
+## Citation
+
+If you use this benchmark in your research, please cite this project.
+
+```
+@article{faster-coco-eval,
+  title   = {{Faster-COCO-Eval}: Faster interpretation of the original COCOEval},
+  author  = {MiXaiLL76},
+  year    = {2024}
+}
+```
```

### Comparing `faster-coco-eval-1.4.3/csrc/faster_eval_api/coco_eval/cocoeval.cpp` & `faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.cpp`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/csrc/faster_eval_api/coco_eval/cocoeval.h` & `faster_coco_eval-1.5.1/csrc/faster_eval_api/coco_eval/cocoeval.h`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/csrc/faster_eval_api/faster_eval_api.cpp` & `faster_coco_eval-1.5.1/csrc/faster_eval_api/faster_eval_api.cpp`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/csrc/mask/common/maskApi.c` & `faster_coco_eval-1.5.1/csrc/mask/common/maskApi.c`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/csrc/mask/common/maskApi.h` & `faster_coco_eval-1.5.1/csrc/mask/common/maskApi.h`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/csrc/mask/pycocotools/_mask.pyx` & `faster_coco_eval-1.5.1/csrc/mask/pycocotools/_mask.pyx`

 * *Files identical despite different names*

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/core/coco.py` & `faster_coco_eval-1.5.1/faster_coco_eval/core/coco.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 # Microsoft COCO is a large image dataset designed for object detection,
 # segmentation, and caption generation. pycocotools is a Python API that
 # assists in loading, parsing and visualizing the annotations in COCO.
 # Please visit http://mscoco.org/ for more information on COCO, including
 # for the data, paper, and tutorials. The exact format of the annotations
 # is also described on the COCO website. For example usage of the pycocotools
-# please see pycocotools_demo.ipynb. In addition to this API, please download both
+# please see pycocotools_demo.ipynb. In addition to this API, please download both # noqa: E501
 # the COCO images and annotations in order to run the demo.
 
 # An alternative to using the API is to load the annotations directly
 # into Python dictionary
 # Using the API provides additional utility functions. Note that this API
 # supports both *instance* and *caption* annotations. In the case of
 # captions not all functions are defined (e.g. categories are undefined).
 
 # The following API functions are defined:
-#  COCO       - COCO api class that loads COCO annotation file and prepare data structures.
+#  COCO       - COCO api class that loads COCO annotation file and prepare data structures. # noqa: E501
 #  decodeMask - Decode binary mask M encoded via run-length encoding.
 #  encodeMask - Encode binary mask M using run-length encoding.
 #  getAnnIds  - Get ann ids that satisfy given filter conditions.
 #  getCatIds  - Get cat ids that satisfy given filter conditions.
 #  getImgIds  - Get img ids that satisfy given filter conditions.
 #  loadAnns   - Load anns with the specified ids.
 #  loadCats   - Load cats with the specified ids.
@@ -44,35 +44,39 @@
 # Code written by Piotr Dollar and Tsung-Yi Lin, 2014.
 # Licensed under the Simplified BSD License [see bsd.txt]
 
 import copy
 import itertools
 import json
 import logging
-import numpy as np
 import time
 import warnings
 from collections import defaultdict
 
+import numpy as np
+
 from . import mask as maskUtils
 
 logger = logging.getLogger(__name__)
 
 
 def _isArrayLike(obj):
     return hasattr(obj, "__iter__") and hasattr(obj, "__len__")
 
 
 class COCO:
     def __init__(self, annotation_file=None):
-        """
-        Constructor of Microsoft COCO helper class for reading and visualizing annotations.
+        """Constructor of Microsoft COCO helper class for reading and
+        visualizing annotations.
+
         :param annotation_file (str): location of annotation file
-        :param image_folder (str): location to the folder that hosts images.
+        :param image_folder (str): location to the folder that hosts
+            images.
         :return:
+
         """
         # load dataset
         self.dataset, self.anns, self.cats, self.imgs = (
             dict(),
             dict(),
             dict(),
             dict(),
@@ -80,16 +84,15 @@
         self.imgToAnns, self.catToImgs = defaultdict(list), defaultdict(list)
         self.score_tresh: float = 0.0
 
         if annotation_file is not None:
             logger.debug("loading annotations into memory...")
             tic = time.time()
             if type(annotation_file) is str:
-                with open(annotation_file, "r") as f:
-                    self.dataset = json.load(f)
+                self.dataset = self.load_json(annotation_file)
             elif type(annotation_file) is dict:
                 self.dataset = annotation_file
             else:
                 self.dataset = None
 
             assert (
                 type(self.dataset) is dict
@@ -132,29 +135,34 @@
         self.anns = anns
         self.imgToAnns = imgToAnns
         self.catToImgs = catToImgs
         self.imgs = imgs
         self.cats = cats
 
     def info(self):
-        """
-        Print information about the annotation file.
+        """Print information about the annotation file.
+
         :return:
+
         """
         for key, value in self.dataset["info"].items():
             logger.debug("{}: {}".format(key, value))
 
     def getAnnIds(self, imgIds=[], catIds=[], areaRng=[], iscrowd=None):
-        """
-        Get ann ids that satisfy given filter conditions. default skips that filter
-        :param imgIds  (int array)     : get anns for given imgs
-               catIds  (int array)     : get anns for given cats
-               areaRng (float array)   : get anns for given area range (e.g. [0 inf])
-               iscrowd (boolean)       : get anns for given crowd label (False or True)
+        """Get ann ids that satisfy given filter conditions.
+
+        default skips that filter
+        :param imgIds (int array) : get anns for given imgs :param
+            catIds (int array) : get anns for given cats
+        :param areaRng (float array) : get anns for given area range
+            (e.g. [0 inf])
+        :param iscrowd (boolean) : get anns for given crowd label (False
+            or True)
         :return: ids (int array)       : integer array of ann ids
+
         """
         imgIds = imgIds if _isArrayLike(imgIds) else [imgIds]
         catIds = catIds if _isArrayLike(catIds) else [catIds]
 
         if len(imgIds) == len(catIds) == len(areaRng) == 0:
             anns = self.dataset["annotations"]
         else:
@@ -184,20 +192,23 @@
         if iscrowd is not None:
             ids = [ann["id"] for ann in anns if ann["iscrowd"] == iscrowd]
         else:
             ids = [ann["id"] for ann in anns]
         return ids
 
     def getCatIds(self, catNms=[], supNms=[], catIds=[]):
-        """
-        filtering parameters. default skips that filter.
+        """Filtering parameters.
+
+        default skips that filter.
         :param catNms (str array)  : get cats for given cat names
-        :param supNms (str array)  : get cats for given supercategory names
+        :param supNms (str array) : get cats for given supercategory
+            names
         :param catIds (int array)  : get cats for given cat ids
         :return: ids (int array)   : integer array of cat ids
+
         """
         catNms = catNms if _isArrayLike(catNms) else [catNms]
         supNms = supNms if _isArrayLike(supNms) else [supNms]
         catIds = catIds if _isArrayLike(catIds) else [catIds]
 
         if len(catNms) == len(supNms) == len(catIds) == 0:
             cats = self.dataset["categories"]
@@ -218,19 +229,20 @@
                 if len(catIds) == 0
                 else [cat for cat in cats if cat["id"] in catIds]
             )
         ids = [cat["id"] for cat in cats]
         return ids
 
     def getImgIds(self, imgIds=[], catIds=[]):
-        """
-        Get img ids that satisfy given filter conditions.
+        """Get img ids that satisfy given filter conditions.
+
         :param imgIds (int array) : get imgs for given ids
         :param catIds (int array) : get imgs with all given cats
         :return: ids (int array)  : integer array of img ids
+
         """
         imgIds = imgIds if _isArrayLike(imgIds) else [imgIds]
         catIds = catIds if _isArrayLike(catIds) else [catIds]
 
         if len(imgIds) == len(catIds) == 0:
             ids = self.imgs.keys()
         else:
@@ -239,60 +251,70 @@
                 if i == 0 and len(ids) == 0:
                     ids = set(self.catToImgs[catId])
                 else:
                     ids &= set(self.catToImgs[catId])
         return list(ids)
 
     def loadAnns(self, ids=[]):
-        """
-        Load anns with the specified ids.
+        """Load anns with the specified ids.
+
         :param ids (int array)       : integer ids specifying anns
         :return: anns (object array) : loaded ann objects
+
         """
         if _isArrayLike(ids):
             return [self.anns[id] for id in ids]
         elif type(ids) is int:
             return [self.anns[ids]]
 
     def loadCats(self, ids=[]):
-        """
-        Load cats with the specified ids.
+        """Load cats with the specified ids.
+
         :param ids (int array)       : integer ids specifying cats
         :return: cats (object array) : loaded cat objects
+
         """
         if _isArrayLike(ids):
             return [self.cats[id] for id in ids]
         elif type(ids) is int:
             return [self.cats[ids]]
 
     def loadImgs(self, ids=[]):
-        """
-        Load anns with the specified ids.
+        """Load anns with the specified ids.
+
         :param ids (int array)       : integer ids specifying img
         :return: imgs (object array) : loaded img objects
+
         """
         if _isArrayLike(ids):
             return [self.imgs[id] for id in ids]
         elif type(ids) is int:
             return [self.imgs[ids]]
 
+    @staticmethod
+    def load_json(json_file):
+        with open(json_file) as io:
+            _data = json.load(io)
+        return _data
+
     def loadRes(self, resFile, min_score=0):
-        """
-        Load result file and return a result api object.
+        """Load result file and return a result api object.
+
         :param   resFile (str)     : file name of result file
         :return: res (obj)         : result api object
+
         """
         self.score_tresh = min_score
         res = COCO()
         res.dataset["images"] = [img for img in self.dataset["images"]]
 
         logger.debug("Loading and preparing results...")
         tic = time.time()
         if type(resFile) is str:
-            anns = json.load(open(resFile))
+            anns = self.load_json(resFile)
         elif type(resFile) is np.ndarray:
             anns = self.loadNumpyAnnotations(resFile)
         else:
             anns = resFile
         assert type(anns) is list, "results in not an array of objects"
 
         anns = [ann for ann in anns if ann.get("score", 1) >= self.score_tresh]
@@ -357,19 +379,22 @@
     def showAnns(self, anns, draw_bbox=False):
         warnings.warn("showAnns deprecated in 1.3.0", DeprecationWarning)
 
     def download(self, tarDir=None, imgIds=[]):
         warnings.warn("download deprecated in 1.3.0", DeprecationWarning)
 
     def loadNumpyAnnotations(self, data):
-        """
-        Convert result data from a numpy array [Nx7] where each row contains {imageID,x1,y1,w,h,score,class}
-        :param  data (numpy.ndarray)
+        """Convert result data from array to anns.
+
+        :param data (numpy.ndarray): array [Nx7] where each row contains
+            [imageID,x1,y1,w,h,score,class]
         :return: annotations (python nested list)
+
         """
+
         logger.debug("Converting ndarray to lists...")
         assert type(data) is np.ndarray
         logger.debug(data.shape)
         assert data.shape[1] == 7
         N = data.shape[0]
         ann = []
         for i in range(N):
@@ -382,17 +407,18 @@
                     "score": data[i, 5],
                     "category_id": int(data[i, 6]),
                 }
             ]
         return ann
 
     def annToRLE(self, ann):
-        """
-        Convert annotation which can be polygons, uncompressed RLE to RLE.
+        """Convert annotation which can be polygons, uncompressed RLE to RLE.
+
         :return: binary mask (numpy 2D array)
+
         """
         t = self.imgs[ann["image_id"]]
         h, w = t["height"], t["width"]
         segm = ann["segmentation"]
         if type(segm) is list:
             # polygon -- a single object might consist of multiple parts
             # we merge all parts into one mask rle code
@@ -403,14 +429,42 @@
             rle = maskUtils.frPyObjects(segm, h, w)
         else:
             # rle
             rle = ann["segmentation"]
         return rle
 
     def annToMask(self, ann):
-        """
-        Convert annotation which can be polygons, uncompressed RLE, or RLE to binary mask.
+        """Convert annotation which can be polygons, uncompressed RLE, or RLE
+        to binary mask.
+
         :return: binary mask (numpy 2D array)
+
         """
         rle = self.annToRLE(ann)
         m = maskUtils.decode(rle)
         return m
+
+    def get_ann_ids(self, img_ids=[], cat_ids=[], area_rng=[], iscrowd=None):
+        return self.getAnnIds(img_ids, cat_ids, area_rng, iscrowd)
+
+    def get_cat_ids(self, cat_names=[], sup_names=[], cat_ids=[]):
+        return self.getCatIds(cat_names, sup_names, cat_ids)
+
+    def get_img_ids(self, img_ids=[], cat_ids=[]):
+        return self.getImgIds(img_ids, cat_ids)
+
+    def load_anns(self, ids):
+        return self.loadAnns(ids)
+
+    def load_cats(self, ids):
+        return self.loadCats(ids)
+
+    def load_imgs(self, ids):
+        return self.loadImgs(ids)
+
+    @property
+    def img_ann_map(self):
+        return self.imgToAnns
+
+    @property
+    def cat_img_map(self):
+        return self.catToImgs
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/core/cocoeval.py` & `faster_coco_eval-1.5.1/faster_coco_eval/core/cocoeval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __author__ = "tsungyi"
 
 import copy
 import logging
-import numpy as np
 import time
 from collections import defaultdict
 
+import numpy as np
+
 from . import mask as maskUtils
 from .coco import COCO
 
 logger = logging.getLogger(__name__)
 
 
 class COCOeval:
@@ -66,19 +67,20 @@
         self,
         cocoGt=None,
         cocoDt=None,
         iouType="segm",
         print_function=logger.debug,
         extra_calc=False,
     ):
-        """
-        Initialize CocoEval using coco APIs for gt and dt
-        :param cocoGt: coco object with ground truth annotations
+        """Initialize CocoEval using coco APIs for gt and dt :param cocoGt:
+
+        coco object with ground truth annotations
         :param cocoDt: coco object with detection results
-        :return: None
+        :return: None.
+
         """
         if not iouType:
             logger.warning("iouType not specified. use default iouType segm")
 
         self.cocoGt: COCO = cocoGt  # ground truth COCO API
         self.cocoDt: COCO = cocoDt  # detections COCO API
         # per-image per-category evaluation results [KxAxI] elements
@@ -97,17 +99,18 @@
         if cocoGt is not None:
             self.params.imgIds = sorted(cocoGt.getImgIds())
             self.params.catIds = sorted(cocoGt.getCatIds())
 
         self.print_function = print_function  # output print function
 
     def _prepare(self):
-        """
-        Prepare ._gts and ._dts for evaluation based on params
+        """Prepare ._gts and ._dts for evaluation based on params.
+
         :return: None
+
         """
 
         def _toMask(anns, coco):
             # modify ann['segmentation'] by reference
             for ann in anns:
                 rle = coco.annToRLE(ann)
                 ann["rle"] = rle
@@ -141,28 +144,29 @@
         for dt in dts:
             self._dts[dt["image_id"], dt["category_id"]].append(dt)
         # per-image per-category evaluation results
         self.evalImgs = defaultdict(list)
         self.eval = {}  # accumulated evaluation results
 
     def evaluate(self):
-        """
-        Run per image evaluation on given images and store results (a list of dict) in self.evalImgs
+        """Run per image evaluation on given images and store results (a list
+        of dict) in self.evalImgs.
+
         :return: None
+
         """
         tic = time.time()
         self.print_function("Running per image evaluation...")
         p = self.params
         # add backward compatibility if useSegm is specified in params
         if p.useSegm is not None:
             p.iouType = "segm" if p.useSegm == 1 else "bbox"
             logger.warning(
-                "useSegm (deprecated) is not None. Running {} evaluation".format(
-                    p.iouType
-                )
+                "useSegm (deprecated) is not None. Running {} evaluation"
+                .format(p.iouType)
             )
         self.print_function("Evaluate annotation type *{}*".format(p.iouType))
         p.imgIds = list(np.unique(p.imgIds))
         if p.useCats:
             p.catIds = list(np.unique(p.catIds))
         p.maxDets = sorted(p.maxDets)
         self.params = p
@@ -271,17 +275,18 @@
                 e = (dx**2 + dy**2) / vars / (gt["area"] + np.spacing(1)) / 2
                 if k1 > 0:
                     e = e[vg > 0]
                 ious[i, j] = np.sum(np.exp(-e)) / e.shape[0]
         return ious
 
     def evaluateImg(self, imgId, catId, aRng, maxDet):
-        """
-        perform evaluation for single category and image
+        """Perform evaluation for single category and image.
+
         :return: dict (single image results)
+
         """
         p = self.params
         if p.useCats:
             gt = self._gts[imgId, catId]
             dt = self._dts[imgId, catId]
         else:
             gt = [_ for cId in p.catIds for _ in self._gts[imgId, cId]]
@@ -327,15 +332,15 @@
                             continue
                         # if dt matched to reg gt, and on ignore gt, stop
                         if m > -1 and gtIg[m] == 0 and gtIg[gind] == 1:
                             break
                         # continue to next gt unless better match made
                         if ious[dind, gind] < iou:
                             continue
-                        # if match successful and best so far, store appropriately
+                        # if match successful and best so far, store appropriately # noqa: E501
                         iou = ious[dind, gind]
                         m = gind
                     # if match made store id of match for both dt and gt
                     if m == -1:
                         continue
                     dtIg[tind, dind] = gtIg[m]
                     dtm[tind, dind] = gt[m]["id"]
@@ -360,22 +365,27 @@
             "dtIgnore": dtIg,
         }
 
     def accumulate(self, p=None):
         raise DeprecationWarning("deprecated")
 
     def summarize(self):
-        """
-        Compute and display summary metrics for evaluation results.
-        Note this functin can *only* be applied on the default parameter setting
+        """Compute and display summary metrics for evaluation results.
+
+        Note this functin can *only* be applied on the default parameter
+        setting
+
         """
 
         def _summarize(ap=1, iouThr=None, areaRng="all", maxDets=100):
             p = self.params
-            iStr = " {:<18} {} @[ IoU={:<9} | area={:>6s} | maxDets={:>3d} ] = {:0.3f}"
+            iStr = (
+                " {:<18} {} @[ IoU={:<9} | area={:>6s} | maxDets={:>3d} ] ="
+                " {:0.3f}"
+            )
             titleStr = "Average Precision" if ap == 1 else "Average Recall"
             typeStr = "(AP)" if ap == 1 else "(AR)"
             iouStr = (
                 "{:0.2f}:{:0.2f}".format(p.iouThrs[0], p.iouThrs[-1])
                 if iouThr is None
                 else "{:0.2f}".format(iouThr)
             )
@@ -480,22 +490,20 @@
         self.stats = self.all_stats[:12]
 
     def __str__(self):
         self.summarize()
 
 
 class Params:
-    """
-    Params for coco evaluation api
-    """
+    """Params for coco evaluation api."""
 
     def setDetParams(self):
         self.imgIds = []
         self.catIds = []
-        # np.arange causes trouble.  the data point on arange is slightly larger than the true value
+        # np.arange causes trouble.  the data point on arange is slightly larger than the true value # noqa: E501
         self.iouThrs = np.linspace(
             0.5, 0.95, int(np.round((0.95 - 0.5) / 0.05)) + 1, endpoint=True
         )
         self.recThrs = np.linspace(
             0.0, 1.00, int(np.round((1.00 - 0.0) / 0.01)) + 1, endpoint=True
         )
         self.maxDets = [1, 10, 100]
@@ -507,15 +515,15 @@
         ]
         self.areaRngLbl = ["all", "small", "medium", "large"]
         self.useCats = 1
 
     def setKpParams(self):
         self.imgIds = []
         self.catIds = []
-        # np.arange causes trouble.  the data point on arange is slightly larger than the true value
+        # np.arange causes trouble.  the data point on arange is slightly larger than the true value # noqa: E501
         self.iouThrs = np.linspace(
             0.5, 0.95, int(np.round((0.95 - 0.5) / 0.05)) + 1, endpoint=True
         )
         self.recThrs = np.linspace(
             0.0, 1.00, int(np.round((1.00 - 0.0) / 0.01)) + 1, endpoint=True
         )
         self.maxDets = [20]
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/core/faster_eval_api.py` & `faster_coco_eval-1.5.1/faster_coco_eval/core/faster_eval_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # Original work Copyright (c) Facebook, Inc. and its affiliates.
 # Modified work Copyright (c) 2021 Sartorius AG
 
 import copy
 import logging
-import numpy as np
 import time
 
+import numpy as np
+
 import faster_coco_eval.faster_eval_api_cpp as _C
+
 from . import mask as maskUtils
 from .cocoeval import COCOeval
 
 logger = logging.getLogger(__name__)
 
 
 class COCOeval_faster(COCOeval):
-    """
-    This is a slightly modified version of the original COCO API, where the functions evaluateImg()
-    and accumulate() are implemented in C++ to speedup evaluation
-    """
+    """This is a slightly modified version of the original COCO API, where the
+    functions evaluateImg() and accumulate() are implemented in C++ to speedup
+    evaluation."""
 
     def evaluate(self):
-        """
-        Run per image evaluation on given images and store results in self.evalImgs_cpp, a
-        datastructure that isn't readable from Python but is used by a c++ implementation of
-        accumulate().  Unlike the original COCO PythonAPI, we don't populate the datastructure
-        self.evalImgs because this datastructure is a computational bottleneck.
+        """Run per image evaluation on given images and store results in
+        self.evalImgs_cpp, a datastructure that isn't readable from Python but
+        is used by a c++ implementation of accumulate().
+
+        Unlike the original COCO PythonAPI, we don't populate the
+        datastructure self.evalImgs because this datastructure is a
+        computational bottleneck.
         :return: None
+
         """
         tic = time.time()
 
         p = self.params
         # add backward compatibility if useSegm is specified in params
         if p.useSegm is not None:
             p.iouType = "segm" if p.useSegm == 1 else "bbox"
@@ -57,29 +61,29 @@
             for catId in catIds
         }  # bottleneck
 
         maxDet = p.maxDets[-1]
 
         # <<<< Beginning of code differences with original COCO API
         def convert_instances_to_cpp(instances, is_det=False):
-            # Convert annotations for a list of instances in an image to a format that's fast
+            # Convert annotations for a list of instances in an image to a format that's fast # noqa: E501
             # to access in C++
             instances_cpp = []
             for instance in instances:
                 instance_cpp = _C.InstanceAnnotation(
                     int(instance["id"]),
                     instance["score"] if is_det else instance.get("score", 0.0),
                     instance["area"],
                     bool(instance.get("iscrowd", 0)),
                     bool(instance.get("ignore", 0)),
                 )
                 instances_cpp.append(instance_cpp)
             return instances_cpp
 
-        # Convert GT annotations, detections, and IOUs to a format that's fast to access in C++
+        # Convert GT annotations, detections, and IOUs to a format that's fast to access in C++ # noqa: E501
         ground_truth_instances = [
             [
                 convert_instances_to_cpp(self._gts[imgId, catId])
                 for catId in p.catIds
             ]
             for imgId in p.imgIds
         ]
@@ -118,33 +122,35 @@
 
         toc = time.time()
 
         self.print_function("COCOeval_opt.evaluate() finished...")
         self.print_function("DONE (t={:0.2f}s).".format(toc - tic))
 
     def accumulate(self):
-        """
-        Accumulate per image evaluation results and store the result in self.eval.  Does not
-        support changing parameter settings from those used by self.evaluate()
+        """Accumulate per image evaluation results and store the result in
+        self.eval.
+
+        Does not support changing parameter settings from those used by
+        self.evaluate()
+
         """
         self.print_function("Accumulating evaluation results...")
         tic = time.time()
         assert hasattr(
             self, "_evalImgs_cpp"
         ), "evaluate() must be called before accmulate() is called."
 
         self.eval = _C.COCOevalAccumulate(self._paramsEval, self._evalImgs_cpp)
 
-        # recall is num_iou_thresholds X num_categories X num_area_ranges X num_max_detections
+        # recall is num_iou_thresholds X num_categories X num_area_ranges X num_max_detections # noqa: E501
         self.eval["recall"] = np.array(self.eval["recall"]).reshape(
             self.eval["counts"][:1] + self.eval["counts"][2:]
         )
 
-        # precision and scores are num_iou_thresholds X num_recall_thresholds X num_categories X
-        # num_area_ranges X num_max_detections
+        # precision and scores are num_iou_thresholds X num_recall_thresholds X num_categories X num_area_ranges X num_max_detections # noqa: E501
         self.eval["precision"] = np.array(self.eval["precision"]).reshape(
             self.eval["counts"]
         )
         self.eval["scores"] = np.array(self.eval["scores"]).reshape(
             self.eval["counts"]
         )
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/core/mask.py` & `faster_coco_eval-1.5.1/faster_coco_eval/core/mask.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 # The following API functions are defined:
 #  encode         - Encode binary masks using RLE.
 #  decode         - Decode binary masks encoded via RLE.
 #  merge          - Compute union or intersection of encoded masks.
 #  iou            - Compute intersection over union between masks.
 #  area           - Compute area of encoded masks.
 #  toBbox         - Get bounding boxes surrounding encoded masks.
-#  frPyObjects    - Convert polygon, bbox, and uncompressed RLE to encoded RLE mask.
+#  frPyObjects    - Convert polygon, bbox, and uncompressed RLE to encoded RLE mask. # noqa: E501
 #
 # Usage:
 #  Rs     = encode( masks )
 #  masks  = decode( Rs )
 #  R      = merge( Rs, intersect=false )
 #  o      = iou( dt, gt, iscrowd )
 #  a      = area( Rs )
 #  bbs    = toBbox( Rs )
 #  Rs     = frPyObjects( [pyObjects], h, w )
 #
 # In the API the following formats are used:
 #  Rs      - [dict] Run-length encoding of binary masks
 #  R       - dict Run-length encoding of binary mask
-#  masks   - [hxwxn] Binary mask(s) (must have type np.ndarray(dtype=uint8) in column-major order)
-#  iscrowd - [nx1] list of np.ndarray. 1 indicates corresponding gt image has crowd region to ignore
+#  masks   - [hxwxn] Binary mask(s) (must have type np.ndarray(dtype=uint8) in column-major order) # noqa: E501
+#  iscrowd - [nx1] list of np.ndarray. 1 indicates corresponding gt image has crowd region to ignore # noqa: E501
 #  bbs     - [nx4] Bounding box(es) stored as [x y w h]
 #  poly    - Polygon stored as [[x1 y1 x2 y2...],[x1 y1 ...],...] (2D list)
 #  dt,gt   - May be either bounding boxes or encoded masks
 # Both poly and bbs are 0-indexed (bbox=[0 0 1 1] encloses first pixel).
 #
 # Finally, a note about the intersection over union (iou) computation.
 # The standard iou of a ground truth (gt) and detected (dt) object is
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/extra/display.py` & `faster_coco_eval-1.5.1/faster_coco_eval/extra/draw.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,330 +1,376 @@
 import logging
-import numpy as np
 import os.path as osp
+from typing import Optional
+
+import numpy as np
 import plotly.express as px
 import plotly.graph_objs as go
 from PIL import Image
 
-from .extra import ExtraEval
+from ..core import COCO
 
 logger = logging.getLogger(__name__)
 
+A = 0.1
+DT_COLOR = (238, 130, 238, A)
 
-class PreviewResults(ExtraEval):
-    A = 0.1
-    DT_COLOR = (238, 130, 238, A)
-
-    GT_COLOR = (0, 255, 0, A)
-    FN_COLOR = (0, 0, 255, A)
-    FP_COLOR = (255, 0, 0, A)
-
-    def get_ann_poly(self, ann, color, text=None, legendgroup=None):
-        all_x = []
-        all_y = []
-
-        if self.iouType == "bbox":
-            x1, y1, w, h = ann["bbox"]
-            all_x = [x1, x1 + w, x1 + w, x1, x1, None]
-            all_y = [y1, y1, y1 + h, y1 + h, y1, None]
-        else:
-            for poly in ann["segmentation"]:
-                if len(poly) > 3:
-                    poly += poly[:2]
-                    poly = np.array(poly).reshape(-1, 2)
-                    all_x += poly[:, 0].tolist() + [None]
-                    all_y += poly[:, 1].tolist() + [None]
-
-        return go.Scatter(
-            x=all_x,
-            y=all_y,
-            name="",
-            text=text,
-            hovertemplate="{text}<extra></extra>",
-            mode="lines",
-            legendgroup=legendgroup,
-            legendgrouptitle_text=legendgroup,
-            showlegend=False,
-            fill="toself",
-            fillcolor="rgba{}".format(color),
-            line=dict(color="rgb{}".format(color[:3])),
+GT_COLOR = (0, 255, 0, A)
+FN_COLOR = (0, 0, 255, A)
+FP_COLOR = (255, 0, 0, A)
+
+
+def generate_ann_polygon(
+    ann: dict,
+    color: tuple,
+    iouType: str = "bbox",
+    text: Optional[str] = None,
+    legendgroup: Optional[str] = None,
+):
+    all_x = []
+    all_y = []
+
+    if iouType == "bbox":
+        x1, y1, w, h = ann["bbox"]
+        all_x = [x1, x1 + w, x1 + w, x1, x1, None]
+        all_y = [y1, y1, y1 + h, y1 + h, y1, None]
+    else:
+        for poly in ann["segmentation"]:
+            if len(poly) > 3:
+                poly += poly[:2]
+                poly = np.array(poly).reshape(-1, 2)
+                all_x += poly[:, 0].tolist() + [None]
+                all_y += poly[:, 1].tolist() + [None]
+
+    return go.Scatter(
+        x=all_x,
+        y=all_y,
+        name="",
+        text=text,
+        hovertemplate="{text}<extra></extra>",
+        mode="lines",
+        legendgroup=legendgroup,
+        legendgrouptitle_text=legendgroup,
+        showlegend=False,
+        fill="toself",
+        fillcolor="rgba{}".format(color),
+        line=dict(color="rgb{}".format(color[:3])),
+    )
+
+
+def display_image(
+    cocoGt: COCO,
+    cocoDt: Optional[COCO] = None,
+    image_id: int = 1,
+    iouType: Optional[str] = "bbox",
+    display_fp: bool = True,
+    display_fn: bool = True,
+    display_tp: bool = True,
+    display_gt: bool = True,
+    data_folder: Optional[str] = None,
+    categories: Optional[list] = None,
+    return_fig: bool = False,
+):
+    polygons = []
+
+    image = cocoGt.imgs[image_id]
+    gt_anns = {ann["id"]: ann for ann in cocoGt.imgToAnns[image_id]}
+
+    if cocoDt is not None:
+        dt_anns = {ann["id"]: ann for ann in cocoDt.imgToAnns[image_id]}
+    else:
+        dt_anns = {}
+
+    image_fn = image["file_name"]
+    if data_folder is not None:
+        image_load_path = osp.join(data_folder, image["file_name"])
+    else:
+        image_load_path = image["file_name"]
+
+    if osp.exists(image_load_path):
+        im = Image.open(image_load_path).convert("RGB")
+    else:
+        logger.warning(
+            "[{}] not found!\nLoading default empty image".format(
+                image_load_path
+            )
         )
 
-    def display_image(
-        self,
-        image_id=1,
-        display_fp=True,
-        display_fn=True,
-        display_tp=True,
-        display_gt=True,
-        data_folder=None,
-        categories=None,
-        return_fig: bool = False,
-    ):
-        polygons = []
-
-        image = self.cocoGt.imgs[image_id]
-        gt_anns = {ann["id"]: ann for ann in self.cocoGt.imgToAnns[image_id]}
-
-        if self.cocoDt is not None:
-            dt_anns = {
-                ann["id"]: ann for ann in self.cocoDt.imgToAnns[image_id]
-            }
-        else:
-            dt_anns = {}
-
-        image_fn = image["file_name"]
-        if data_folder is not None:
-            image_load_path = osp.join(data_folder, image["file_name"])
-        else:
-            image_load_path = image["file_name"]
-
-        if osp.exists(image_load_path):
-            im = Image.open(image_load_path).convert("RGB")
-        else:
-            logger.warning(
-                "[{}] not found!\nLoading default empty image".format(
-                    image_load_path
-                )
+        im = Image.new("RGB", (image["width"], image["height"]))
+
+    categories_labels = {
+        category["id"]: category["name"] for _, category in cocoGt.cats.items()
+    }
+
+    if len(gt_anns) > 0:
+        for ann in gt_anns.values():
+            if categories is None or ann["category_id"] in categories:
+                if ann.get("fn", False):
+                    if display_fn:
+                        poly = generate_ann_polygon(
+                            ann,
+                            color=FN_COLOR,
+                            iouType=iouType,
+                            text="<b>FN</b><br>id={}<br>category={}".format(
+                                ann["id"],
+                                categories_labels[ann["category_id"]],
+                            ),
+                            legendgroup="fn",
+                        )
+                        polygons.append(poly)
+                else:
+                    if display_gt:
+                        poly = generate_ann_polygon(
+                            ann,
+                            color=GT_COLOR,
+                            iouType=iouType,
+                            text="<b>GT</b><br>id={}<br>category={}".format(
+                                ann["id"],
+                                categories_labels[ann["category_id"]],
+                            ),
+                            legendgroup="gt",
+                        )
+                        polygons.append(poly)
+
+    if len(dt_anns) > 0:
+        for ann in dt_anns.values():
+            if categories is None or ann["category_id"] in categories:
+                if ann.get("tp", False):
+                    if display_tp:
+                        poly = generate_ann_polygon(
+                            ann,
+                            color=DT_COLOR,
+                            iouType=iouType,
+                            text=(
+                                "<b>DT</b><br>"
+                                "id={}<br>"
+                                "category={}<br>"
+                                "score={:.2f}<br>"
+                                "IoU={:.2f}"
+                            ).format(
+                                ann["id"],
+                                categories_labels[ann["category_id"]],
+                                ann["score"],
+                                ann["iou"],
+                            ),
+                            legendgroup="tp",
+                        )
+                        polygons.append(poly)
+                else:
+                    if display_fp:
+                        poly = generate_ann_polygon(
+                            ann,
+                            color=FP_COLOR,
+                            iouType=iouType,
+                            text=(
+                                "<b>FP</b><br>"
+                                "id={}<br>"
+                                "category={}<br>"
+                                "score={:.2f}"
+                            ).format(
+                                ann["id"],
+                                categories_labels[ann["category_id"]],
+                                ann["score"],
+                            ),
+                            legendgroup="fp",
+                        )
+                        polygons.append(poly)
+
+    fig = px.imshow(
+        im,
+        binary_compression_level=5,
+        binary_format="jpg",
+        aspect="auto",
+        labels=dict(animation_frame="shown picture"),
+    )
+
+    legends = {}
+    for poly in polygons:
+        if legends.get(poly.legendgroup) is None:
+            poly.showlegend = True
+            legends[poly.legendgroup] = True
+
+        fig.add_trace(poly)
+
+    layout = {
+        "title": "image_id={}<br>image_fn={}".format(image_id, image_fn),
+        "autosize": True,
+        "height": 700,
+        "width": 900,
+    }
+
+    fig.update_layout(layout)
+    fig.update_xaxes(range=[0, image["width"]])
+    fig.update_yaxes(range=[image["height"], 0])
+
+    if return_fig:
+        return fig
+
+    fig.show()
+
+
+def display_matrix(
+    conf_matrix: np.ndarray,
+    labels: list,
+    normalize: bool = False,
+    return_fig: bool = False,
+):
+    _labels = labels + ["fp", "fn"]
+
+    if normalize:
+        conf_matrix /= conf_matrix.sum(axis=1).reshape(-1, 1)
+        conf_matrix *= 100
+
+    hovertemplate = "Real: %{y}<br>Predict: %{x}<br>"
+
+    if normalize:
+        hovertemplate += "Percent: %{z:.0f}<extra></extra>"
+    else:
+        hovertemplate += "Count: %{z:.0f}<extra></extra>"
+
+    heatmap = go.Heatmap(
+        z=conf_matrix,
+        x=_labels,
+        y=_labels[:-2],
+        colorscale="Blues",
+        hovertemplate=hovertemplate,
+    )
+
+    annotations = []
+    for j, row in enumerate(conf_matrix):
+        for i, value in enumerate(row):
+            text_value = "{:.0f}".format(value)
+            if normalize:
+                text_value += "%"
+
+            annotations.append(
+                {
+                    "x": _labels[i],
+                    "y": _labels[j],
+                    "font": {"color": "white"},
+                    "text": text_value,
+                    "xref": "x1",
+                    "yref": "y1",
+                    "showarrow": False,
+                }
             )
 
-            im = Image.new("RGB", (image["width"], image["height"]))
+    title = "Confusion Matrix"
+    if normalize:
+        title = "Normalized " + title
+
+    layout = {
+        "title": title,
+        "xaxis": {"title": "Predicted value"},
+        "yaxis": {"title": "Real value"},
+        "annotations": annotations,
+    }
+
+    fig = go.Figure(data=[heatmap], layout=layout)
+    fig.update_traces(showscale=False)
+    fig.update_layout(height=700, width=900)
+
+    if return_fig:
+        return fig
+
+    fig.show()
+
+
+def plot_pre_rec(curves, return_fig: bool = False):
+    fig = go.Figure()
+
+    for _curve in curves:
+        recall_list = _curve["recall_list"]
+        precision_list = _curve["precision_list"]
+        scores = _curve["scores"]
+        name = _curve["name"]
+
+        fig.add_trace(
+            go.Scatter(
+                x=recall_list,
+                y=precision_list,
+                name=name,
+                text=scores,
+                hovertemplate="Pre: %{y:.3f}<br>"
+                + "Rec: %{x:.3f}<br>"
+                + "Score: %{text:.3f}<extra></extra>",
+                showlegend=True,
+                mode="lines",
+            )
+        )
 
-        categories_labels = {
-            category["id"]: category["name"]
-            for _, category in self.cocoGt.cats.items()
-        }
-
-        if len(gt_anns) > 0:
-            for ann in gt_anns.values():
-                if categories is None or ann["category_id"] in categories:
-                    if ann.get("fn", False):
-                        if display_fn:
-                            poly = self.get_ann_poly(
-                                ann,
-                                color=self.FN_COLOR,
-                                text="<b>FN</b><br>id={}<br>category={}".format(
-                                    ann["id"],
-                                    categories_labels[ann["category_id"]],
-                                ),
-                                legendgroup="fn",
-                            )
-                            polygons.append(poly)
-                    else:
-                        if display_gt:
-                            poly = self.get_ann_poly(
-                                ann,
-                                color=self.GT_COLOR,
-                                text="<b>GT</b><br>id={}<br>category={}".format(
-                                    ann["id"],
-                                    categories_labels[ann["category_id"]],
-                                ),
-                                legendgroup="gt",
-                            )
-                            polygons.append(poly)
-
-        if len(dt_anns) > 0:
-            for ann in dt_anns.values():
-                if categories is None or ann["category_id"] in categories:
-                    if ann.get("tp", False):
-                        if display_tp:
-                            poly = self.get_ann_poly(
-                                ann,
-                                color=self.DT_COLOR,
-                                text="<b>DT</b><br>id={}<br>category={}<br>score={:.2f}<br>IoU={:.2f}".format(
-                                    ann["id"],
-                                    categories_labels[ann["category_id"]],
-                                    ann["score"],
-                                    ann["iou"],
-                                ),
-                                legendgroup="tp",
-                            )
-                            polygons.append(poly)
-                    else:
-                        if display_fp:
-                            poly = self.get_ann_poly(
-                                ann,
-                                color=self.FP_COLOR,
-                                text="<b>FP</b><br>id={}<br>category={}<br>score={:.2f}".format(
-                                    ann["id"],
-                                    categories_labels[ann["category_id"]],
-                                    ann["score"],
-                                ),
-                                legendgroup="fp",
-                            )
-                            polygons.append(poly)
-
-        fig = px.imshow(
-            im,
-            binary_compression_level=5,
-            binary_format="jpg",
-            aspect="auto",
-            labels=dict(animation_frame="shown picture"),
+    margin = 0.01
+    fig.layout.yaxis.range = [0 - margin, 1 + margin]
+    fig.layout.xaxis.range = [0 - margin, 1 + margin]
+
+    fig.layout.yaxis.title = "Precision"
+    fig.layout.xaxis.title = "Recall"
+
+    fig.update_xaxes(showspikes=True)
+    fig.update_yaxes(showspikes=True)
+
+    layout = {
+        "title": "Precision-Recall",
+        "autosize": True,
+        "height": 600,
+        "width": 1200,
+    }
+
+    fig.update_layout(layout)
+
+    if return_fig:
+        return fig
+
+    fig.show()
+
+
+def plot_f1_confidence(curves, return_fig: bool = False):
+    fig = go.Figure()
+    eps = 1e-16
+    for _curve in curves:
+        recall_list = _curve["recall_list"]
+        precision_list = _curve["precision_list"]
+        scores = _curve["scores"]
+        f1_curve = (
+            2
+            * precision_list
+            * recall_list
+            / (precision_list + recall_list + eps)
         )
 
-        legends = {}
-        for poly in polygons:
-            if legends.get(poly.legendgroup) is None:
-                poly.showlegend = True
-                legends[poly.legendgroup] = True
-
-            fig.add_trace(poly)
-
-        layout = {
-            "title": "image_id={}<br>image_fn={}".format(image_id, image_fn),
-            "autosize": True,
-            "height": 700,
-            "width": 900,
-        }
-
-        fig.update_layout(layout)
-        fig.update_xaxes(range=[0, image["width"]])
-        fig.update_yaxes(range=[image["height"], 0])
-
-        if return_fig:
-            return fig
-
-        fig.show()
-
-    def display_tp_fp_fn(
-        self,
-        image_ids=["all"],
-        display_fp=True,
-        display_fn=True,
-        display_tp=True,
-        display_gt=False,
-        data_folder=None,
-        categories=None,
-    ):
-        for image_id, _ in self.cocoGt.imgToAnns.items():
-            if (image_id in image_ids) or "all" in image_ids:
-                self.display_image(
-                    image_id,
-                    display_fp=display_fp,
-                    display_fn=display_fn,
-                    display_tp=display_tp,
-                    display_gt=display_gt,
-                    data_folder=data_folder,
-                    categories=categories,
-                )
-
-    def _compute_confusion_matrix(self, y_true, y_pred, fp={}, fn={}):
-        """
-        return classes*(classes + fp col + fn col)
-        """
-        categories_real_ids = list(self.cocoGt.cats)
-        categories_enum_ids = {
-            category_id: _i
-            for _i, category_id in enumerate(categories_real_ids)
-        }
-        K = len(categories_enum_ids)
-
-        cm = np.zeros((K, K + 2), dtype=np.float32)
-        for a, p in zip(y_true, y_pred):
-            cm[categories_enum_ids[a]][categories_enum_ids[p]] += 1
-
-        for enum_id, category_id in enumerate(categories_real_ids):
-            cm[enum_id][-2] = fp.get(category_id, 0)
-            cm[enum_id][-1] = fn.get(category_id, 0)
-
-        return cm
-
-    def compute_confusion_matrix(self):
-        assert self.eval is not None, "Run first self.evaluate()"
-
-        if self.useCats:
-            logger.warning(
-                "The calculation may not be accurate. No intersection of classes. useCats={}".format(
-                    self.useCats
-                )
+        name = _curve["label"] if len(_curve["label"]) > 0 else "F1-Confidence"
+
+        fig.add_trace(
+            go.Scatter(
+                x=scores,
+                y=f1_curve,
+                name=name,
+                hovertemplate="F1: %{y:.3f}<br>"
+                + "Confidence: %{x:.3f}<br><extra></extra>",
+                showlegend=True,
+                mode="lines",
             )
+        )
 
-        y_true = []
-        y_pred = []
+    margin = 0.01
+    fig.layout.yaxis.range = [0 - margin, 1 + margin]
+    fig.layout.xaxis.range = [0 - margin, 1 + margin]
 
-        fn = {}
-        fp = {}
+    fig.layout.yaxis.title = "F1"
+    fig.layout.xaxis.title = "Confidence"
 
-        for ann_id, ann in self.cocoGt.anns.items():
-            if ann.get("dt_id") is not None:
-                dt_ann = self.cocoDt.anns[ann["dt_id"]]
-
-                y_true.append(ann["category_id"])
-                y_pred.append(dt_ann["category_id"])
-
-            else:
-                if fn.get(ann["category_id"]) is None:
-                    fn[ann["category_id"]] = 0
-                fn[ann["category_id"]] += 1
-
-        for ann_id, ann in self.cocoDt.anns.items():
-            if ann.get("gt_id") is None:
-                if fp.get(ann["category_id"]) is None:
-                    fp[ann["category_id"]] = 0
-                fp[ann["category_id"]] += 1
-
-        # classes fp fn
-        cm = self._compute_confusion_matrix(y_true, y_pred, fp=fp, fn=fn)
-        return cm
-
-    def display_matrix(
-        self, in_percent=False, conf_matrix=None, return_fig: bool = False
-    ):
-        if conf_matrix is None:
-            conf_matrix = self.compute_confusion_matrix()
-
-        labels = [category["name"] for _, category in self.cocoGt.cats.items()]
-        labels += ["fp", "fn"]
-
-        if in_percent:
-            conf_matrix /= conf_matrix.sum(axis=1).reshape(-1, 1)
-            conf_matrix *= 100
-
-        hovertemplate = "Real: %{y}<br>" "Predict: %{x}<br>"
-
-        if in_percent:
-            hovertemplate += "Percent: %{z:.0f}<extra></extra>"
-        else:
-            hovertemplate += "Count: %{z:.0f}<extra></extra>"
-
-        heatmap = go.Heatmap(
-            z=conf_matrix,
-            x=labels,
-            y=labels[:-2],
-            colorscale="Blues",
-            hovertemplate=hovertemplate,
-        )
+    fig.update_xaxes(showspikes=True)
+    fig.update_yaxes(showspikes=True)
+
+    layout = {
+        "title": "F1-Confidence",
+        "autosize": True,
+        "height": 600,
+        "width": 1200,
+    }
 
-        annotations = []
-        for j, row in enumerate(conf_matrix):
-            for i, value in enumerate(row):
-                text_value = "{:.0f}".format(value)
-                if in_percent:
-                    text_value += "%"
-
-                annotations.append(
-                    {
-                        "x": labels[i],
-                        "y": labels[j],
-                        "font": {"color": "white"},
-                        "text": text_value,
-                        "xref": "x1",
-                        "yref": "y1",
-                        "showarrow": False,
-                    }
-                )
-
-        layout = {
-            "title": "Confusion Matrix",
-            "xaxis": {"title": "Predicted value"},
-            "yaxis": {"title": "Real value"},
-            "annotations": annotations,
-        }
-
-        fig = go.Figure(data=[heatmap], layout=layout)
-        fig.update_traces(showscale=False)
-        fig.update_layout(height=700, width=900)
+    fig.update_layout(layout)
 
-        if return_fig:
-            return fig
+    if return_fig:
+        return fig
 
-        fig.show()
+    fig.show()
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval/extra/extra.py` & `faster_coco_eval-1.5.1/faster_coco_eval/extra/extra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import logging
+
 import numpy as np
 
 from ..core import COCO, COCOeval_faster
 
 logger = logging.getLogger(__name__)
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval.egg-info/PKG-INFO` & `faster_coco_eval-1.5.1/faster_coco_eval.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster-coco-eval
-Version: 1.4.3
+Version: 1.5.1
 Summary: Faster interpretation of the original COCOEval
 Home-page: https://github.com/MiXaiLL76/faster_coco_eval
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,21 @@
 Requires-Dist: numpy
 Requires-Dist: plotly
 Requires-Dist: pandas
 Requires-Dist: Pillow
 
 # Faster-COCO-Eval
 
+[![PyPI](https://img.shields.io/pypi/v/faster-coco-eval)](https://pypi.org/project/faster-coco-eval)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/faster-coco-eval.svg?label=PyPI%20downloads)](
+https://pypi.org/project/faster-coco-eval/)
+
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://github.com/MiXaiLL76/faster_coco_eval/wiki)
+[![license](https://img.shields.io/github/license/MiXaiLL76/faster_coco_eval.svg)](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/LICENSE)
+
 ## Disclaimer
 
 I often use this project, but I saw it abandoned and without a public repository on github.
 Also, part of the project remained unfinished for a long time. I implemented some of the author's ideas and decided to make the results publicly available.
 
 ## Faster-COCO-Eval base
 
@@ -38,21 +45,30 @@
 for coco's AP metrics, especially when dealing with a high number of instances in an image.
 
 ## Comparison
 
 For our use case with a test dataset of 5000 images from the coco val dataset.
 Testing was carried out using the mmdetection framework and the eval_metric.py script. The indicators are presented below.
 
-Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/comparison.ipynb)
+Visualization of testing **comparison.ipynb** available in directory [examples/comparison](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples/comparison/mmdet/comparison.ipynb)
 Tested with yolo3 model (bbox eval) and yoloact model (segm eval)
 
-| Type | COCOeval    | COCOeval_faster | Profit      |
-| ---- | ----------- | --------------- | ----------- |
-| bbox | 18.477 sec. | 7.345 sec.      | 2.5x faster |
-| segm | 29.819 sec. | 15.840 sec.     | 2x faster   |
+### Summary for 5000 imgs
+
+| Type | COCOeval    | COCOeval_faster | Profit       |
+| ---- | ----------- | --------------- | ------------ |
+| bbox | 18.477 sec. | 7.345 sec.      | ~2.5x faster |
+| segm | 29.819 sec. | 15.840 sec.     | ~1.7x faster |
+
+## Summary for 500 imgs
+
+| Type | COCOeval  | COCOeval_faster | Profit       |
+| ---- | --------- | --------------- | ------------ |
+| bbox | 3.57 sec. | 2.03 sec.       | ~1.7x faster |
+| segm | 4.16 sec. | 2.41 sec.       | ~1.7x faster |
 
 ## Feautures
 
 This library provides not only validation functions, but also error visualization functions. Including visualization of errors in the image.  
 You can study in more detail in the [examples](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/examples) and [Wiki](https://github.com/MiXaiLL76/faster_coco_eval/wiki).
 
 ## Usage
@@ -63,7 +79,19 @@
 
 Available via link [history.md](https://github.com/MiXaiLL76/faster_coco_eval/blob/main/history.md)
 
 ## License
 
 The original module was licensed with apache 2, I will continue with the same license.
 Distributed under the apache version 2.0 license, see [license](LICENSE) for more information.
+
+## Citation
+
+If you use this benchmark in your research, please cite this project.
+
+```
+@article{faster-coco-eval,
+  title   = {{Faster-COCO-Eval}: Faster interpretation of the original COCOEval},
+  author  = {MiXaiLL76},
+  year    = {2024}
+}
+```
```

### Comparing `faster-coco-eval-1.4.3/faster_coco_eval.egg-info/SOURCES.txt` & `faster_coco_eval-1.5.1/faster_coco_eval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 csrc/faster_eval_api/faster_eval_api.cpp
 csrc/faster_eval_api/coco_eval/cocoeval.cpp
 csrc/faster_eval_api/coco_eval/cocoeval.h
 csrc/mask/common/maskApi.c
 csrc/mask/common/maskApi.h
 csrc/mask/pycocotools/_mask.pyx
@@ -21,9 +20,10 @@
 faster_coco_eval/core/coco.py
 faster_coco_eval/core/cocoeval.py
 faster_coco_eval/core/faster_eval_api.py
 faster_coco_eval/core/mask.py
 faster_coco_eval/extra/__init__.py
 faster_coco_eval/extra/curves.py
 faster_coco_eval/extra/display.py
+faster_coco_eval/extra/draw.py
 faster_coco_eval/extra/extra.py
 requirements/runtime.txt
```

### Comparing `faster-coco-eval-1.4.3/setup.py` & `faster_coco_eval-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python3
 
-import setuptools
-from setuptools import Extension, setup
-
 import glob
-import numpy as np
 import platform
+
+import numpy as np
+import setuptools
 from pybind11.setup_helpers import Pybind11Extension, build_ext
+from setuptools import Extension, setup
 
 
 def readme():
     with open("README.md", encoding="utf-8") as f:
         content = f.read()
     return content
 
@@ -23,21 +23,23 @@
         exec(compile(f.read(), version_file, "exec"))
     return locals()["__version__"], locals()["__author__"]
 
 
 def parse_requirements(fname="requirements/runtime.txt", with_version=True):
     """Parse the package dependencies listed in a requirements file but strips
     specific versioning information.
+
     Args:
         fname (str): path to requirements file
         with_version (bool, default=False): if True include version specs
     Returns:
         List[str]: list of requirements items
     CommandLine:
         python -c "import setup; print(setup.parse_requirements())"
+
     """
     import re
     import sys
     from os.path import exists
 
     require_fpath = fname
 
@@ -63,15 +65,15 @@
                     op, rest = parts[1:]
                     if ";" in rest:
                         # Handle platform specific dependencies
                         # http://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-platform-specific-dependencies
                         version, platform_deps = map(str.strip, rest.split(";"))
                         info["platform_deps"] = platform_deps
                     else:
-                        version = rest  # NOQA
+                        version = rest
                     info["version"] = (op, version)
             yield info
 
     def parse_require_file(fpath):
         with open(fpath) as f:
             for line in f.readlines():
                 line = line.strip()
```

