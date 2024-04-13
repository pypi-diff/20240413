# Comparing `tmp/everywhereml-0.2.8.tar.gz` & `tmp/everywhereml-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/everywhereml-0.2.8.tar", last modified: Fri Nov 11 16:50:42 2022, max compression
+gzip compressed data, was "dist/everywhereml-0.2.9.tar", last modified: Mon Nov 14 15:38:24 2022, max compression
```

## Comparing `everywhereml-0.2.8.tar` & `everywhereml-0.2.9.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/
--rw-r--r--   0 simone     (501) staff       (20)      822 2022-11-11 16:50:42.000000 everywhereml-0.2.8/PKG-INFO
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-28 13:07:53.000000 everywhereml-0.2.8/everywhereml/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/arduino/
--rw-r--r--   0 simone     (501) staff       (20)     1676 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/BoardEntry.py
--rw-r--r--   0 simone     (501) staff       (20)     4501 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/Cli.py
--rw-r--r--   0 simone     (501) staff       (20)      378 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/H.py
--rw-r--r--   0 simone     (501) staff       (20)      307 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/Ino.py
--rw-r--r--   0 simone     (501) staff       (20)     1881 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/PortEntry.py
--rw-r--r--   0 simone     (501) staff       (20)      889 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/Selector.py
--rw-r--r--   0 simone     (501) staff       (20)     4210 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/Sketch.py
--rw-r--r--   0 simone     (501) staff       (20)      125 2022-09-06 13:44:04.000000 everywhereml-0.2.8/everywhereml/arduino/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/code_generators/
--rw-r--r--   0 simone     (501) staff       (20)     4997 2022-08-21 15:02:49.000000 everywhereml-0.2.8/everywhereml/code_generators/GeneratesCode.py
--rw-r--r--   0 simone     (501) staff       (20)       68 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/code_generators/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/
--rw-r--r--   0 simone     (501) staff       (20)      822 2022-05-02 08:03:44.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/Environment.py
--rw-r--r--   0 simone     (501) staff       (20)     2111 2022-11-05 16:58:21.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/FileSystemLoader.py
--rw-r--r--   0 simone     (501) staff       (20)     1981 2022-08-20 07:34:56.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/Jinja.py
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-28 14:47:54.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/
--rw-r--r--   0 simone     (501) staff       (20)      478 2022-08-20 07:19:01.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/__init__.py
--rw-r--r--   0 simone     (501) staff       (20)      326 2022-05-02 09:47:04.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/c_shape.py
--rw-r--r--   0 simone     (501) staff       (20)      545 2022-06-27 16:17:02.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_c_array.py
--rw-r--r--   0 simone     (501) staff       (20)      220 2022-05-02 09:58:24.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_c_comment.py
--rw-r--r--   0 simone     (501) staff       (20)      225 2022-08-20 07:12:51.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_py_comment.py
--rw-r--r--   0 simone     (501) staff       (20)      549 2022-08-20 07:21:27.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_py_list.py
--rw-r--r--   0 simone     (501) staff       (20)      205 2022-07-09 06:12:31.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_variable_name.py
--rw-r--r--   0 simone     (501) staff       (20)      209 2022-11-02 07:11:56.000000 everywhereml-0.2.8/everywhereml/code_generators/jinja/helpers.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/code_generators/prettifiers/
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-08-20 07:47:17.000000 everywhereml-0.2.8/everywhereml/code_generators/prettifiers/__init__.py
--rw-r--r--   0 simone     (501) staff       (20)      640 2022-08-20 07:54:43.000000 everywhereml-0.2.8/everywhereml/code_generators/prettifiers/basic_python_prettifier.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/code_generators/templates/
--rw-r--r--   0 simone     (501) staff       (20)     2017 2022-08-06 14:49:42.000000 everywhereml-0.2.8/everywhereml/code_generators/templates/TensorFlowPorter.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     1339 2022-08-04 16:40:11.000000 everywhereml-0.2.8/everywhereml/code_generators/tensorflow.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/data/
--rw-r--r--   0 simone     (501) staff       (20)     8784 2022-06-27 16:21:28.000000 everywhereml-0.2.8/everywhereml/data/Dataset.py
--rw-r--r--   0 simone     (501) staff       (20)    11540 2022-07-14 15:27:12.000000 everywhereml-0.2.8/everywhereml/data/ImageDataset.py
--rw-r--r--   0 simone     (501) staff       (20)      101 2022-06-21 12:02:31.000000 everywhereml-0.2.8/everywhereml/data/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/data/collect/
--rw-r--r--   0 simone     (501) staff       (20)      845 2022-06-25 12:30:46.000000 everywhereml-0.2.8/everywhereml/data/collect/BaseCollector.py
--rw-r--r--   0 simone     (501) staff       (20)     2066 2022-06-29 06:57:28.000000 everywhereml-0.2.8/everywhereml/data/collect/ByteStream.py
--rw-r--r--   0 simone     (501) staff       (20)     4105 2022-07-08 17:45:30.000000 everywhereml-0.2.8/everywhereml/data/collect/MjpegCollector.py
--rw-r--r--   0 simone     (501) staff       (20)     9142 2022-06-29 06:58:06.000000 everywhereml-0.2.8/everywhereml/data/collect/SerialCollector.py
--rw-r--r--   0 simone     (501) staff       (20)      138 2022-06-24 07:43:22.000000 everywhereml-0.2.8/everywhereml/data/collect/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/get_started/
--rw-r--r--   0 simone     (501) staff       (20)      277 2022-06-11 16:47:08.000000 everywhereml-0.2.8/everywhereml/get_started/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/plot/
--rw-r--r--   0 simone     (501) staff       (20)     2155 2022-07-02 15:42:28.000000 everywhereml-0.2.8/everywhereml/plot/DatasetPlotter.py
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-27 16:06:35.000000 everywhereml-0.2.8/everywhereml/plot/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/preprocessing/
--rw-r--r--   0 simone     (501) staff       (20)     1773 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/preprocessing/MinMaxScaler.py
--rw-r--r--   0 simone     (501) staff       (20)     3299 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/preprocessing/Pipeline.py
--rw-r--r--   0 simone     (501) staff       (20)     6164 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/preprocessing/SpectralFeatures.py
--rw-r--r--   0 simone     (501) staff       (20)     2276 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/preprocessing/Window.py
--rw-r--r--   0 simone     (501) staff       (20)      248 2022-06-08 11:41:34.000000 everywhereml-0.2.8/everywhereml/preprocessing/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/
--rw-r--r--   0 simone     (501) staff       (20)     4226 2022-07-12 18:02:19.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/HOG.py
--rw-r--r--   0 simone     (501) staff       (20)     5244 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/LBP.py
--rw-r--r--   0 simone     (501) staff       (20)      105 2022-07-04 16:33:14.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/
--rw-r--r--   0 simone     (501) staff       (20)     3312 2022-07-12 10:22:37.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/BaseObjectDetectionPipeline.py
--rw-r--r--   0 simone     (501) staff       (20)      588 2022-07-12 07:08:11.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/HogPipeline.py
--rw-r--r--   0 simone     (501) staff       (20)       85 2022-07-08 18:19:26.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/
--rw-r--r--   0 simone     (501) staff       (20)      734 2022-07-11 14:01:34.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/Grayscale.py
--rw-r--r--   0 simone     (501) staff       (20)     2242 2022-07-12 17:52:14.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/Resize.py
--rw-r--r--   0 simone     (501) staff       (20)      143 2022-07-11 14:27:30.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/templates/
--rw-r--r--   0 simone     (501) staff       (20)      507 2022-07-12 10:23:19.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/templates/Resize.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-07-11 14:15:37.000000 everywhereml-0.2.8/everywhereml/preprocessing/image/transform/templates/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/sklearn/
--rw-r--r--   0 simone     (501) staff       (20)     3887 2022-07-11 14:34:54.000000 everywhereml-0.2.8/everywhereml/sklearn/SklearnBaseClassifier.py
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-05-02 10:09:00.000000 everywhereml-0.2.8/everywhereml/sklearn/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/sklearn/ensemble/
--rw-r--r--   0 simone     (501) staff       (20)      728 2022-05-02 10:22:33.000000 everywhereml-0.2.8/everywhereml/sklearn/ensemble/RandomForestClassifier.py
--rw-r--r--   0 simone     (501) staff       (20)       88 2022-05-02 10:12:45.000000 everywhereml-0.2.8/everywhereml/sklearn/ensemble/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/sklearn/tree/
--rw-r--r--   0 simone     (501) staff       (20)      655 2022-05-29 14:27:52.000000 everywhereml-0.2.8/everywhereml/sklearn/tree/DecisionTreeClassifier.py
--rw-r--r--   0 simone     (501) staff       (20)       83 2022-05-29 14:27:20.000000 everywhereml-0.2.8/everywhereml/sklearn/tree/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-05-02 10:27:53.000000 everywhereml-0.2.8/everywhereml/templates/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/cpp/
--rw-r--r--   0 simone     (501) staff       (20)     1082 2022-08-20 11:19:26.000000 everywhereml-0.2.8/everywhereml/templates/cpp/BaseClassifier.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      599 2022-06-24 15:12:05.000000 everywhereml-0.2.8/everywhereml/templates/cpp/class_map.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      175 2022-06-09 17:50:33.000000 everywhereml-0.2.8/everywhereml/templates/cpp/latency.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      254 2022-05-05 13:41:13.000000 everywhereml-0.2.8/everywhereml/templates/cpp/vote.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/
--rw-r--r--   0 simone     (501) staff       (20)      479 2022-09-06 13:48:30.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/MinMaxScaler.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     2044 2022-09-06 13:48:04.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Pipeline.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     4642 2022-09-06 13:48:30.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/SpectralFeatures.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      520 2022-06-24 14:34:36.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Step.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      768 2022-09-06 13:48:30.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Window.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/
--rw-r--r--   0 simone     (501) staff       (20)      555 2022-07-09 06:23:39.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     3338 2022-07-12 10:45:10.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/HOG.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     1902 2022-07-02 14:55:52.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/LBP.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/object_detection/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/object_detection/cpp/
--rw-r--r--   0 simone     (501) staff       (20)     2106 2022-11-11 16:50:04.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)       45 2022-07-09 05:56:05.000000 everywhereml-0.2.8/everywhereml/templates/preprocessing/image/object_detection/cpp/HogPipeline.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/py/
--rw-r--r--   0 simone     (501) staff       (20)     1078 2022-08-21 13:41:04.000000 everywhereml-0.2.8/everywhereml/templates/py/BaseClassifier.py.jinja
--rw-r--r--   0 simone     (501) staff       (20)      534 2022-08-20 06:42:13.000000 everywhereml-0.2.8/everywhereml/templates/py/class_map.py.jinja
--rw-r--r--   0 simone     (501) staff       (20)      195 2022-08-20 07:23:09.000000 everywhereml-0.2.8/everywhereml/templates/py/latency.py.jinja
--rw-r--r--   0 simone     (501) staff       (20)      130 2022-08-20 11:53:20.000000 everywhereml-0.2.8/everywhereml/templates/py/vote.py.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/cpp/
--rw-r--r--   0 simone     (501) staff       (20)      871 2022-08-20 11:20:28.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      421 2022-08-20 11:19:26.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/cpp/tree.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/py/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/py/micro/
--rw-r--r--   0 simone     (501) staff       (20)      795 2022-08-20 11:40:26.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja
--rw-r--r--   0 simone     (501) staff       (20)      355 2022-08-20 07:36:52.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/py/micro/tree.py.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/tree/
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/tree/cpp/
--rw-r--r--   0 simone     (501) staff       (20)       91 2022-08-20 11:16:42.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/tree/cpp/DecisionTreeClassifier.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      350 2022-08-20 11:19:26.000000 everywhereml-0.2.8/everywhereml/templates/sklearn/tree/cpp/tree.cpp.jinja
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/
--rw-r--r--   0 simone     (501) staff       (20)     2054 2022-07-04 18:02:57.000000 everywhereml-0.2.8/everywhereml/tests/BaseTestCase.py
--rw-r--r--   0 simone     (501) staff       (20)       88 2022-06-27 16:00:39.000000 everywhereml-0.2.8/everywhereml/tests/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/data/
--rw-r--r--   0 simone     (501) staff       (20)        0 2022-06-25 14:59:45.000000 everywhereml-0.2.8/everywhereml/tests/data/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/
--rw-r--r--   0 simone     (501) staff       (20)      613 2022-06-27 16:08:08.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/BasePreprocessingTestCase.py
--rw-r--r--   0 simone     (501) staff       (20)      719 2022-06-27 16:37:48.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/MinMaxScalerTest.py
--rw-r--r--   0 simone     (501) staff       (20)      117 2022-07-02 14:56:18.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/image/
--rw-r--r--   0 simone     (501) staff       (20)      627 2022-07-04 17:54:37.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/image/HOGTest.py
--rw-r--r--   0 simone     (501) staff       (20)      733 2022-06-27 16:37:18.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/image/LBPTest.py
--rw-r--r--   0 simone     (501) staff       (20)      122 2022-07-04 17:51:13.000000 everywhereml-0.2.8/everywhereml/tests/preprocessing/image/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/runtime/
--rw-r--r--   0 simone     (501) staff       (20)     2523 2022-06-27 16:02:41.000000 everywhereml-0.2.8/everywhereml/tests/runtime/BaseRuntime.py
--rw-r--r--   0 simone     (501) staff       (20)      483 2022-06-27 16:00:39.000000 everywhereml-0.2.8/everywhereml/tests/runtime/CppRuntime.py
--rw-r--r--   0 simone     (501) staff       (20)      183 2021-07-29 16:09:46.000000 everywhereml-0.2.8/everywhereml/tests/runtime/JsRuntime.py
--rw-r--r--   0 simone     (501) staff       (20)      185 2021-07-28 15:29:17.000000 everywhereml-0.2.8/everywhereml/tests/runtime/PHPRuntime.py
--rw-r--r--   0 simone     (501) staff       (20)        0 2021-07-25 05:59:04.000000 everywhereml-0.2.8/everywhereml/tests/runtime/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/sklearn/
--rw-r--r--   0 simone     (501) staff       (20)       49 2022-06-25 16:05:58.000000 everywhereml-0.2.8/everywhereml/tests/sklearn/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/sklearn/ensemble/
--rw-r--r--   0 simone     (501) staff       (20)     1582 2022-06-25 16:12:07.000000 everywhereml-0.2.8/everywhereml/tests/sklearn/ensemble/RandomForestClassifierTest.py
--rw-r--r--   0 simone     (501) staff       (20)       78 2022-07-02 14:56:18.000000 everywhereml-0.2.8/everywhereml/tests/sklearn/ensemble/__init__.py
-drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-11 16:50:42.000000 everywhereml-0.2.8/everywhereml/tests/templates/
--rw-r--r--   0 simone     (501) staff       (20)      319 2022-06-25 16:05:58.000000 everywhereml-0.2.8/everywhereml/tests/templates/classifier.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)      591 2022-06-25 15:20:26.000000 everywhereml-0.2.8/everywhereml/tests/templates/pipeline.cpp.jinja
--rw-r--r--   0 simone     (501) staff       (20)     4250 2022-11-11 16:50:36.000000 everywhereml-0.2.8/setup.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/
+-rw-r--r--   0 simone     (501) staff       (20)      822 2022-11-14 15:38:24.000000 everywhereml-0.2.9/PKG-INFO
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-28 13:07:53.000000 everywhereml-0.2.9/everywhereml/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/arduino/
+-rw-r--r--   0 simone     (501) staff       (20)     1676 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/BoardEntry.py
+-rw-r--r--   0 simone     (501) staff       (20)     4501 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/Cli.py
+-rw-r--r--   0 simone     (501) staff       (20)      378 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/H.py
+-rw-r--r--   0 simone     (501) staff       (20)      307 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/Ino.py
+-rw-r--r--   0 simone     (501) staff       (20)     1881 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/PortEntry.py
+-rw-r--r--   0 simone     (501) staff       (20)      889 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/Selector.py
+-rw-r--r--   0 simone     (501) staff       (20)     4210 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/Sketch.py
+-rw-r--r--   0 simone     (501) staff       (20)      125 2022-09-06 13:44:04.000000 everywhereml-0.2.9/everywhereml/arduino/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/code_generators/
+-rw-r--r--   0 simone     (501) staff       (20)     4997 2022-08-21 15:02:49.000000 everywhereml-0.2.9/everywhereml/code_generators/GeneratesCode.py
+-rw-r--r--   0 simone     (501) staff       (20)       68 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/code_generators/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/
+-rw-r--r--   0 simone     (501) staff       (20)      822 2022-05-02 08:03:44.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/Environment.py
+-rw-r--r--   0 simone     (501) staff       (20)     2111 2022-11-05 16:58:21.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/FileSystemLoader.py
+-rw-r--r--   0 simone     (501) staff       (20)     1981 2022-08-20 07:34:56.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/Jinja.py
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-28 14:47:54.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/
+-rw-r--r--   0 simone     (501) staff       (20)      478 2022-08-20 07:19:01.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/__init__.py
+-rw-r--r--   0 simone     (501) staff       (20)      326 2022-05-02 09:47:04.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/c_shape.py
+-rw-r--r--   0 simone     (501) staff       (20)      545 2022-06-27 16:17:02.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_c_array.py
+-rw-r--r--   0 simone     (501) staff       (20)      220 2022-05-02 09:58:24.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_c_comment.py
+-rw-r--r--   0 simone     (501) staff       (20)      225 2022-08-20 07:12:51.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_py_comment.py
+-rw-r--r--   0 simone     (501) staff       (20)      549 2022-08-20 07:21:27.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_py_list.py
+-rw-r--r--   0 simone     (501) staff       (20)      205 2022-07-09 06:12:31.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_variable_name.py
+-rw-r--r--   0 simone     (501) staff       (20)      209 2022-11-02 07:11:56.000000 everywhereml-0.2.9/everywhereml/code_generators/jinja/helpers.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/code_generators/prettifiers/
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-08-20 07:47:17.000000 everywhereml-0.2.9/everywhereml/code_generators/prettifiers/__init__.py
+-rw-r--r--   0 simone     (501) staff       (20)      640 2022-08-20 07:54:43.000000 everywhereml-0.2.9/everywhereml/code_generators/prettifiers/basic_python_prettifier.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/code_generators/templates/
+-rw-r--r--   0 simone     (501) staff       (20)     2017 2022-08-06 14:49:42.000000 everywhereml-0.2.9/everywhereml/code_generators/templates/TensorFlowPorter.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     1339 2022-08-04 16:40:11.000000 everywhereml-0.2.9/everywhereml/code_generators/tensorflow.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/data/
+-rw-r--r--   0 simone     (501) staff       (20)     8804 2022-11-14 15:35:49.000000 everywhereml-0.2.9/everywhereml/data/Dataset.py
+-rw-r--r--   0 simone     (501) staff       (20)    11540 2022-07-14 15:27:12.000000 everywhereml-0.2.9/everywhereml/data/ImageDataset.py
+-rw-r--r--   0 simone     (501) staff       (20)      101 2022-06-21 12:02:31.000000 everywhereml-0.2.9/everywhereml/data/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/data/collect/
+-rw-r--r--   0 simone     (501) staff       (20)      845 2022-06-25 12:30:46.000000 everywhereml-0.2.9/everywhereml/data/collect/BaseCollector.py
+-rw-r--r--   0 simone     (501) staff       (20)     2066 2022-06-29 06:57:28.000000 everywhereml-0.2.9/everywhereml/data/collect/ByteStream.py
+-rw-r--r--   0 simone     (501) staff       (20)     4105 2022-07-08 17:45:30.000000 everywhereml-0.2.9/everywhereml/data/collect/MjpegCollector.py
+-rw-r--r--   0 simone     (501) staff       (20)     9142 2022-06-29 06:58:06.000000 everywhereml-0.2.9/everywhereml/data/collect/SerialCollector.py
+-rw-r--r--   0 simone     (501) staff       (20)      138 2022-06-24 07:43:22.000000 everywhereml-0.2.9/everywhereml/data/collect/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/get_started/
+-rw-r--r--   0 simone     (501) staff       (20)      277 2022-06-11 16:47:08.000000 everywhereml-0.2.9/everywhereml/get_started/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/plot/
+-rw-r--r--   0 simone     (501) staff       (20)     2155 2022-07-02 15:42:28.000000 everywhereml-0.2.9/everywhereml/plot/DatasetPlotter.py
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-04-27 16:06:35.000000 everywhereml-0.2.9/everywhereml/plot/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/preprocessing/
+-rw-r--r--   0 simone     (501) staff       (20)     1773 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/preprocessing/MinMaxScaler.py
+-rw-r--r--   0 simone     (501) staff       (20)     3299 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/preprocessing/Pipeline.py
+-rw-r--r--   0 simone     (501) staff       (20)     6164 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/preprocessing/SpectralFeatures.py
+-rw-r--r--   0 simone     (501) staff       (20)     2276 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/preprocessing/Window.py
+-rw-r--r--   0 simone     (501) staff       (20)      248 2022-06-08 11:41:34.000000 everywhereml-0.2.9/everywhereml/preprocessing/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/
+-rw-r--r--   0 simone     (501) staff       (20)     4226 2022-07-12 18:02:19.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/HOG.py
+-rw-r--r--   0 simone     (501) staff       (20)     5244 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/LBP.py
+-rw-r--r--   0 simone     (501) staff       (20)      105 2022-07-04 16:33:14.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/
+-rw-r--r--   0 simone     (501) staff       (20)     3312 2022-07-12 10:22:37.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/BaseObjectDetectionPipeline.py
+-rw-r--r--   0 simone     (501) staff       (20)      588 2022-07-12 07:08:11.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/HogPipeline.py
+-rw-r--r--   0 simone     (501) staff       (20)       85 2022-07-08 18:19:26.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/transform/
+-rw-r--r--   0 simone     (501) staff       (20)      734 2022-07-11 14:01:34.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/transform/Grayscale.py
+-rw-r--r--   0 simone     (501) staff       (20)     2242 2022-07-12 17:52:14.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/transform/Resize.py
+-rw-r--r--   0 simone     (501) staff       (20)      143 2022-07-11 14:27:30.000000 everywhereml-0.2.9/everywhereml/preprocessing/image/transform/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/sklearn/
+-rw-r--r--   0 simone     (501) staff       (20)     3887 2022-07-11 14:34:54.000000 everywhereml-0.2.9/everywhereml/sklearn/SklearnBaseClassifier.py
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-05-02 10:09:00.000000 everywhereml-0.2.9/everywhereml/sklearn/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/sklearn/ensemble/
+-rw-r--r--   0 simone     (501) staff       (20)      728 2022-05-02 10:22:33.000000 everywhereml-0.2.9/everywhereml/sklearn/ensemble/RandomForestClassifier.py
+-rw-r--r--   0 simone     (501) staff       (20)       88 2022-05-02 10:12:45.000000 everywhereml-0.2.9/everywhereml/sklearn/ensemble/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/sklearn/tree/
+-rw-r--r--   0 simone     (501) staff       (20)      655 2022-05-29 14:27:52.000000 everywhereml-0.2.9/everywhereml/sklearn/tree/DecisionTreeClassifier.py
+-rw-r--r--   0 simone     (501) staff       (20)       83 2022-05-29 14:27:20.000000 everywhereml-0.2.9/everywhereml/sklearn/tree/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-05-02 10:27:53.000000 everywhereml-0.2.9/everywhereml/templates/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)     1082 2022-08-20 11:19:26.000000 everywhereml-0.2.9/everywhereml/templates/cpp/BaseClassifier.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      599 2022-06-24 15:12:05.000000 everywhereml-0.2.9/everywhereml/templates/cpp/class_map.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      175 2022-06-09 17:50:33.000000 everywhereml-0.2.9/everywhereml/templates/cpp/latency.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      254 2022-05-05 13:41:13.000000 everywhereml-0.2.9/everywhereml/templates/cpp/vote.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)      479 2022-09-06 13:48:30.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/MinMaxScaler.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     2044 2022-09-06 13:48:04.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Pipeline.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     4642 2022-09-06 13:48:30.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/SpectralFeatures.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      520 2022-06-24 14:34:36.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Step.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      768 2022-09-06 13:48:30.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Window.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)      555 2022-07-09 06:23:39.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     3338 2022-07-12 10:45:10.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/HOG.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     1902 2022-07-02 14:55:52.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/LBP.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/object_detection/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/object_detection/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)     2106 2022-11-11 16:50:04.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)       45 2022-07-09 05:56:05.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/object_detection/cpp/HogPipeline.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/transform/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/transform/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)      507 2022-07-12 10:23:19.000000 everywhereml-0.2.9/everywhereml/templates/preprocessing/image/transform/cpp/Resize.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/py/
+-rw-r--r--   0 simone     (501) staff       (20)     1078 2022-08-21 13:41:04.000000 everywhereml-0.2.9/everywhereml/templates/py/BaseClassifier.py.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      534 2022-08-20 06:42:13.000000 everywhereml-0.2.9/everywhereml/templates/py/class_map.py.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      195 2022-08-20 07:23:09.000000 everywhereml-0.2.9/everywhereml/templates/py/latency.py.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      130 2022-08-20 11:53:20.000000 everywhereml-0.2.9/everywhereml/templates/py/vote.py.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)      871 2022-08-20 11:20:28.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      421 2022-08-20 11:19:26.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/cpp/tree.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/py/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/py/micro/
+-rw-r--r--   0 simone     (501) staff       (20)      795 2022-08-20 11:40:26.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      355 2022-08-20 07:36:52.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/py/micro/tree.py.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/tree/
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/tree/cpp/
+-rw-r--r--   0 simone     (501) staff       (20)       91 2022-08-20 11:16:42.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/tree/cpp/DecisionTreeClassifier.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      350 2022-08-20 11:19:26.000000 everywhereml-0.2.9/everywhereml/templates/sklearn/tree/cpp/tree.cpp.jinja
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/
+-rw-r--r--   0 simone     (501) staff       (20)     2054 2022-07-04 18:02:57.000000 everywhereml-0.2.9/everywhereml/tests/BaseTestCase.py
+-rw-r--r--   0 simone     (501) staff       (20)       88 2022-06-27 16:00:39.000000 everywhereml-0.2.9/everywhereml/tests/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/data/
+-rw-r--r--   0 simone     (501) staff       (20)        0 2022-06-25 14:59:45.000000 everywhereml-0.2.9/everywhereml/tests/data/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/
+-rw-r--r--   0 simone     (501) staff       (20)      613 2022-06-27 16:08:08.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/BasePreprocessingTestCase.py
+-rw-r--r--   0 simone     (501) staff       (20)      719 2022-06-27 16:37:48.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/MinMaxScalerTest.py
+-rw-r--r--   0 simone     (501) staff       (20)      117 2022-07-02 14:56:18.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/image/
+-rw-r--r--   0 simone     (501) staff       (20)      627 2022-07-04 17:54:37.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/image/HOGTest.py
+-rw-r--r--   0 simone     (501) staff       (20)      733 2022-06-27 16:37:18.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/image/LBPTest.py
+-rw-r--r--   0 simone     (501) staff       (20)      122 2022-07-04 17:51:13.000000 everywhereml-0.2.9/everywhereml/tests/preprocessing/image/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/runtime/
+-rw-r--r--   0 simone     (501) staff       (20)     2523 2022-06-27 16:02:41.000000 everywhereml-0.2.9/everywhereml/tests/runtime/BaseRuntime.py
+-rw-r--r--   0 simone     (501) staff       (20)      483 2022-06-27 16:00:39.000000 everywhereml-0.2.9/everywhereml/tests/runtime/CppRuntime.py
+-rw-r--r--   0 simone     (501) staff       (20)      183 2021-07-29 16:09:46.000000 everywhereml-0.2.9/everywhereml/tests/runtime/JsRuntime.py
+-rw-r--r--   0 simone     (501) staff       (20)      185 2021-07-28 15:29:17.000000 everywhereml-0.2.9/everywhereml/tests/runtime/PHPRuntime.py
+-rw-r--r--   0 simone     (501) staff       (20)        0 2021-07-25 05:59:04.000000 everywhereml-0.2.9/everywhereml/tests/runtime/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/sklearn/
+-rw-r--r--   0 simone     (501) staff       (20)       49 2022-06-25 16:05:58.000000 everywhereml-0.2.9/everywhereml/tests/sklearn/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/sklearn/ensemble/
+-rw-r--r--   0 simone     (501) staff       (20)     1582 2022-06-25 16:12:07.000000 everywhereml-0.2.9/everywhereml/tests/sklearn/ensemble/RandomForestClassifierTest.py
+-rw-r--r--   0 simone     (501) staff       (20)       78 2022-07-02 14:56:18.000000 everywhereml-0.2.9/everywhereml/tests/sklearn/ensemble/__init__.py
+drwxr-xr-x   0 simone     (501) staff       (20)        0 2022-11-14 15:38:24.000000 everywhereml-0.2.9/everywhereml/tests/templates/
+-rw-r--r--   0 simone     (501) staff       (20)      319 2022-06-25 16:05:58.000000 everywhereml-0.2.9/everywhereml/tests/templates/classifier.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)      591 2022-06-25 15:20:26.000000 everywhereml-0.2.9/everywhereml/tests/templates/pipeline.cpp.jinja
+-rw-r--r--   0 simone     (501) staff       (20)     4314 2022-11-14 15:38:15.000000 everywhereml-0.2.9/setup.py
```

### Comparing `everywhereml-0.2.8/PKG-INFO` & `everywhereml-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: everywhereml
-Version: 0.2.8
+Version: 0.2.9
 Summary: Train ML in Python, run everywhere
 Home-page: https://github.com/eloquentarduino/everywhereml
 Author: Simone Salerno
 Author-email: support@eloquentarduino.com
 License: MIT
-Download-URL: https://github.com/eloquentarduino/everywhereml/blob/master/dist/everywhereml-0.2.8.tar.gz?raw=true
+Download-URL: https://github.com/eloquentarduino/everywhereml/blob/master/dist/everywhereml-0.2.9.tar.gz?raw=true
 Description: UNKNOWN
 Keywords: ML,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `everywhereml-0.2.8/everywhereml/arduino/BoardEntry.py` & `everywhereml-0.2.9/everywhereml/arduino/BoardEntry.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/arduino/Cli.py` & `everywhereml-0.2.9/everywhereml/arduino/Cli.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/arduino/PortEntry.py` & `everywhereml-0.2.9/everywhereml/arduino/PortEntry.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/arduino/Selector.py` & `everywhereml-0.2.9/everywhereml/arduino/Selector.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/arduino/Sketch.py` & `everywhereml-0.2.9/everywhereml/arduino/Sketch.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/GeneratesCode.py` & `everywhereml-0.2.9/everywhereml/code_generators/GeneratesCode.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/jinja/Environment.py` & `everywhereml-0.2.9/everywhereml/code_generators/jinja/Environment.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/jinja/FileSystemLoader.py` & `everywhereml-0.2.9/everywhereml/code_generators/jinja/FileSystemLoader.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/jinja/Jinja.py` & `everywhereml-0.2.9/everywhereml/code_generators/jinja/Jinja.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_c_array.py` & `everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_c_array.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/jinja/filters/to_py_list.py` & `everywhereml-0.2.9/everywhereml/code_generators/jinja/filters/to_py_list.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/prettifiers/basic_python_prettifier.py` & `everywhereml-0.2.9/everywhereml/code_generators/prettifiers/basic_python_prettifier.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/templates/TensorFlowPorter.cpp.jinja` & `everywhereml-0.2.9/everywhereml/code_generators/templates/TensorFlowPorter.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/code_generators/tensorflow.py` & `everywhereml-0.2.9/everywhereml/code_generators/tensorflow.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/data/Dataset.py` & `everywhereml-0.2.9/everywhereml/data/Dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,24 +257,24 @@
         :param pipeline:
         :return:
         """
         dataset = pipeline.fit_transform(self)
 
         return self.replace(**dataset.__dict__)
 
-    def split(self, train_size=None, test_size=None):
+    def split(self, train_size=None, test_size=None, **kwargs):
         """
         Split into train/test
         :param train_size:
         :param test_size:
         :return:
         """
         assert (train_size is None or 0 < train_size < 1) or (test_size is None or 0 < test_size < 1), 'train or test size MUST be in the range [0, 1] exclusive'
 
-        X_train, X_test, y_train, y_test = train_test_split(self.X, self.y, train_size=train_size, test_size=test_size)
+        X_train, X_test, y_train, y_test = train_test_split(self.X, self.y, train_size=train_size, test_size=test_size, **kwargs)
 
         return (
             self.clone(name='%s Train' % self.name, X=X_train, y=y_train),
             self.clone(name='%s Test' % self.name, X=X_test, y=y_test)
         )
 
     def _update_df(self):
```

### Comparing `everywhereml-0.2.8/everywhereml/data/ImageDataset.py` & `everywhereml-0.2.9/everywhereml/data/ImageDataset.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/data/collect/BaseCollector.py` & `everywhereml-0.2.9/everywhereml/data/collect/BaseCollector.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/data/collect/ByteStream.py` & `everywhereml-0.2.9/everywhereml/data/collect/ByteStream.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/data/collect/MjpegCollector.py` & `everywhereml-0.2.9/everywhereml/data/collect/MjpegCollector.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/data/collect/SerialCollector.py` & `everywhereml-0.2.9/everywhereml/data/collect/SerialCollector.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/plot/DatasetPlotter.py` & `everywhereml-0.2.9/everywhereml/plot/DatasetPlotter.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/MinMaxScaler.py` & `everywhereml-0.2.9/everywhereml/preprocessing/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/Pipeline.py` & `everywhereml-0.2.9/everywhereml/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/SpectralFeatures.py` & `everywhereml-0.2.9/everywhereml/preprocessing/SpectralFeatures.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/Window.py` & `everywhereml-0.2.9/everywhereml/preprocessing/Window.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/HOG.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/HOG.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/LBP.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/LBP.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/BaseObjectDetectionPipeline.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/BaseObjectDetectionPipeline.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/object_detection/HogPipeline.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/object_detection/HogPipeline.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/transform/Grayscale.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/transform/Grayscale.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/preprocessing/image/transform/Resize.py` & `everywhereml-0.2.9/everywhereml/preprocessing/image/transform/Resize.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/sklearn/SklearnBaseClassifier.py` & `everywhereml-0.2.9/everywhereml/sklearn/SklearnBaseClassifier.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/sklearn/ensemble/RandomForestClassifier.py` & `everywhereml-0.2.9/everywhereml/sklearn/ensemble/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/sklearn/tree/DecisionTreeClassifier.py` & `everywhereml-0.2.9/everywhereml/sklearn/tree/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/cpp/BaseClassifier.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/cpp/BaseClassifier.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/cpp/class_map.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/cpp/class_map.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Pipeline.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Pipeline.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/SpectralFeatures.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/SpectralFeatures.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Step.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Step.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/cpp/Window.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/cpp/Window.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/HOG.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/HOG.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/image/cpp/LBP.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/image/cpp/LBP.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/py/BaseClassifier.py.jinja` & `everywhereml-0.2.9/everywhereml/templates/py/BaseClassifier.py.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/py/class_map.py.jinja` & `everywhereml-0.2.9/everywhereml/templates/py/class_map.py.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja` & `everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja` & `everywhereml-0.2.9/everywhereml/templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/BaseTestCase.py` & `everywhereml-0.2.9/everywhereml/tests/BaseTestCase.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/preprocessing/BasePreprocessingTestCase.py` & `everywhereml-0.2.9/everywhereml/tests/preprocessing/BasePreprocessingTestCase.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/preprocessing/MinMaxScalerTest.py` & `everywhereml-0.2.9/everywhereml/tests/preprocessing/MinMaxScalerTest.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/preprocessing/image/HOGTest.py` & `everywhereml-0.2.9/everywhereml/tests/preprocessing/image/HOGTest.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/preprocessing/image/LBPTest.py` & `everywhereml-0.2.9/everywhereml/tests/preprocessing/image/LBPTest.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/runtime/BaseRuntime.py` & `everywhereml-0.2.9/everywhereml/tests/runtime/BaseRuntime.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/sklearn/ensemble/RandomForestClassifierTest.py` & `everywhereml-0.2.9/everywhereml/tests/sklearn/ensemble/RandomForestClassifierTest.py`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/everywhereml/tests/templates/pipeline.cpp.jinja` & `everywhereml-0.2.9/everywhereml/tests/templates/pipeline.cpp.jinja`

 * *Files identical despite different names*

### Comparing `everywhereml-0.2.8/setup.py` & `everywhereml-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from distutils.core import setup
 
-packages=["everywhereml", "everywhereml.plot", "everywhereml.tests", "everywhereml.tests.runtime", "everywhereml.tests.sklearn", "everywhereml.tests.sklearn.ensemble", "everywhereml.tests.templates", "everywhereml.tests.preprocessing", "everywhereml.tests.preprocessing.image", "everywhereml.tests.data", "everywhereml.arduino", "everywhereml.sklearn", "everywhereml.sklearn.tree", "everywhereml.sklearn.ensemble", "everywhereml.get_started", "everywhereml.code_generators", "everywhereml.code_generators.jinja", "everywhereml.code_generators.jinja.filters", "everywhereml.code_generators.prettifiers", "everywhereml.code_generators.templates", "everywhereml.templates", "everywhereml.templates.py", "everywhereml.templates.sklearn", "everywhereml.templates.sklearn.tree", "everywhereml.templates.sklearn.tree.cpp", "everywhereml.templates.sklearn.ensemble", "everywhereml.templates.sklearn.ensemble.py", "everywhereml.templates.sklearn.ensemble.py.micro", "everywhereml.templates.sklearn.ensemble.cpp", "everywhereml.templates.cpp", "everywhereml.templates.preprocessing", "everywhereml.templates.preprocessing.image", "everywhereml.templates.preprocessing.image.cpp", "everywhereml.templates.preprocessing.image.object_detection", "everywhereml.templates.preprocessing.image.object_detection.cpp", "everywhereml.templates.preprocessing.cpp", "everywhereml.preprocessing", "everywhereml.preprocessing.image", "everywhereml.preprocessing.image.object_detection", "everywhereml.preprocessing.image.transform", "everywhereml.preprocessing.image.transform.templates", "everywhereml.data", "everywhereml.data.collect"]
-data=["tests/templates/pipeline.cpp.jinja", "tests/templates/classifier.cpp.jinja", "code_generators/templates/TensorFlowPorter.cpp.jinja", "templates/py/vote.py.jinja", "templates/py/latency.py.jinja", "templates/py/class_map.py.jinja", "templates/py/BaseClassifier.py.jinja", "templates/sklearn/tree/cpp/tree.cpp.jinja", "templates/sklearn/tree/cpp/DecisionTreeClassifier.cpp.jinja", "templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja", "templates/sklearn/ensemble/py/micro/tree.py.jinja", "templates/sklearn/ensemble/cpp/tree.cpp.jinja", "templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja", "templates/cpp/latency.cpp.jinja", "templates/cpp/vote.cpp.jinja", "templates/cpp/class_map.cpp.jinja", "templates/cpp/BaseClassifier.cpp.jinja", "templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja", "templates/preprocessing/image/cpp/HOG.cpp.jinja", "templates/preprocessing/image/cpp/LBP.cpp.jinja", "templates/preprocessing/image/object_detection/cpp/HogPipeline.cpp.jinja", "templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja", "templates/preprocessing/cpp/Step.cpp.jinja", "templates/preprocessing/cpp/Pipeline.cpp.jinja", "templates/preprocessing/cpp/SpectralFeatures.cpp.jinja", "templates/preprocessing/cpp/Window.cpp.jinja", "templates/preprocessing/cpp/MinMaxScaler.cpp.jinja", "preprocessing/image/transform/templates/Resize.cpp.jinja"]
+packages=["everywhereml", "everywhereml.plot", "everywhereml.tests", "everywhereml.tests.runtime", "everywhereml.tests.sklearn", "everywhereml.tests.sklearn.ensemble", "everywhereml.tests.templates", "everywhereml.tests.preprocessing", "everywhereml.tests.preprocessing.image", "everywhereml.tests.data", "everywhereml.arduino", "everywhereml.sklearn", "everywhereml.sklearn.tree", "everywhereml.sklearn.ensemble", "everywhereml.get_started", "everywhereml.code_generators", "everywhereml.code_generators.jinja", "everywhereml.code_generators.jinja.filters", "everywhereml.code_generators.prettifiers", "everywhereml.code_generators.templates", "everywhereml.templates", "everywhereml.templates.py", "everywhereml.templates.sklearn", "everywhereml.templates.sklearn.tree", "everywhereml.templates.sklearn.tree.cpp", "everywhereml.templates.sklearn.ensemble", "everywhereml.templates.sklearn.ensemble.py", "everywhereml.templates.sklearn.ensemble.py.micro", "everywhereml.templates.sklearn.ensemble.cpp", "everywhereml.templates.cpp", "everywhereml.templates.preprocessing", "everywhereml.templates.preprocessing.image", "everywhereml.templates.preprocessing.image.cpp", "everywhereml.templates.preprocessing.image.object_detection", "everywhereml.templates.preprocessing.image.object_detection.cpp", "everywhereml.templates.preprocessing.image.transform", "everywhereml.templates.preprocessing.image.transform.cpp", "everywhereml.templates.preprocessing.cpp", "everywhereml.preprocessing", "everywhereml.preprocessing.image", "everywhereml.preprocessing.image.object_detection", "everywhereml.preprocessing.image.transform", "everywhereml.data", "everywhereml.data.collect"]
+data=["tests/templates/pipeline.cpp.jinja", "tests/templates/classifier.cpp.jinja", "code_generators/templates/TensorFlowPorter.cpp.jinja", "templates/py/vote.py.jinja", "templates/py/latency.py.jinja", "templates/py/class_map.py.jinja", "templates/py/BaseClassifier.py.jinja", "templates/sklearn/tree/cpp/tree.cpp.jinja", "templates/sklearn/tree/cpp/DecisionTreeClassifier.cpp.jinja", "templates/sklearn/ensemble/py/micro/RandomForestClassifier.py.micro.jinja", "templates/sklearn/ensemble/py/micro/tree.py.jinja", "templates/sklearn/ensemble/cpp/tree.cpp.jinja", "templates/sklearn/ensemble/cpp/RandomForestClassifier.cpp.jinja", "templates/cpp/latency.cpp.jinja", "templates/cpp/vote.cpp.jinja", "templates/cpp/class_map.cpp.jinja", "templates/cpp/BaseClassifier.cpp.jinja", "templates/preprocessing/image/cpp/BaseImageStep.cpp.jinja", "templates/preprocessing/image/cpp/HOG.cpp.jinja", "templates/preprocessing/image/cpp/LBP.cpp.jinja", "templates/preprocessing/image/object_detection/cpp/HogPipeline.cpp.jinja", "templates/preprocessing/image/object_detection/cpp/BaseObjectDetectionPipeline.cpp.jinja", "templates/preprocessing/image/transform/cpp/Resize.cpp.jinja", "templates/preprocessing/cpp/Step.cpp.jinja", "templates/preprocessing/cpp/Pipeline.cpp.jinja", "templates/preprocessing/cpp/SpectralFeatures.cpp.jinja", "templates/preprocessing/cpp/Window.cpp.jinja", "templates/preprocessing/cpp/MinMaxScaler.cpp.jinja"]
 
 setup(
   name='everywhereml',
   packages=packages,
-  version='0.2.8',
+  version='0.2.9',
   license='MIT',
   description='Train ML in Python, run everywhere',
   author='Simone Salerno',
   author_email='support@eloquentarduino.com',
   url='https://github.com/eloquentarduino/everywhereml',
-  download_url='https://github.com/eloquentarduino/everywhereml/blob/master/dist/everywhereml-0.2.8.tar.gz?raw=true',
+  download_url='https://github.com/eloquentarduino/everywhereml/blob/master/dist/everywhereml-0.2.9.tar.gz?raw=true',
   keywords=[
     'ML',
     'machine learning'
   ],
   install_requires=[
     'numpy',
     'pandas',
```

