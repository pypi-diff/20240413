# Comparing `tmp/autogluon.timeseries-1.1.0b20240411.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.0b20240411.tar", last modified: Thu Apr 11 09:05:01 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240412.tar", last modified: Fri Apr 12 09:05:37 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.0b20240411.tar` & `autogluon.timeseries-1.1.0b20240412.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.210771 autogluon.timeseries-1.1.0b20240411/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.210771 autogluon.timeseries-1.1.0b20240411/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45593 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31299 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34031 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.858183 autogluon.timeseries-1.1.0b20240412/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.858183 autogluon.timeseries-1.1.0b20240412/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.862183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.862183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.862183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31299 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33055 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.866183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81219 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.870183 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-12 09:04:11.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:37.862183 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:05:37.000000 autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.0b20240411/PKG-INFO` & `autogluon.timeseries-1.1.0b20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240411
+Version: 1.1.0b20240412
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240411/setup.py` & `autogluon.timeseries-1.1.0b20240412/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "pandas",  # version range defined in `core/_setup_utils.py`
     "torch",  # version range defined in `core/_setup_utils.py`
     "lightning",  # version range defined in `core/_setup_utils.py`
     "pytorch_lightning",  # version range defined in `core/_setup_utils.py`
     "transformers[sentencepiece]",  # version range defined in `core/_setup_utils.py`
     "accelerate",  # version range defined in `core/_setup_utils.py`
     "statsmodels>=0.13.0,<0.15",
-    "gluonts>=0.14.0,<0.15",
+    "gluonts>=0.14.0,<0.14.4",  # 0.14.4 caps pandas<2.2
     "networkx",  # version range defined in `core/_setup_utils.py`
     # TODO: update statsforecast to v1.5.0 - resolve antlr4-python3-runtime dependency clash with multimodal
     "statsforecast>=1.4.0,<1.5",
     "mlforecast>=0.10.0,<0.10.1",
     "utilsforecast>=0.0.10,<0.0.11",
     "tqdm",  # version range defined in `core/_setup_utils.py`
     "orjson~=3.9",  # use faster JSON implementation in GluonTS
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         Number of CPU cores used to process the iterable dataset in parallel. Set to -1 to use all cores. This argument
         is only used when constructing a TimeSeriesDataFrame using format 4 (iterable dataset).
 
     Attributes
     ----------
     freq : str
         A pandas-compatible string describing the frequency of the time series. For example ``"D"`` for daily data,
-        ``"H"`` for hourly data, etc. This attribute is determined automatically based on the timestamps. For the full
+        ``"h"`` for hourly data, etc. This attribute is determined automatically based on the timestamps. For the full
         list of possible values, see `pandas documentation <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases>`_.
     num_items : int
         Number of items (time series) in the data set.
     item_ids : pd.Index
         List of unique time series IDs contained in the data set.
     """
 
@@ -957,20 +957,20 @@
                 2020-06-30     2.0
                 2020-09-30     3.0
                 2020-12-31     4.0
                 2021-03-31     5.0
                 2021-06-30     6.0
                 2021-09-30     7.0
                 2021-12-31     8.0
-        >>> ts_df.convert_frequency("Y")
+        >>> ts_df.convert_frequency("YE")
                             target
         item_id timestamp
         0       2020-12-31     2.5
                 2021-12-31     6.5
-        >>> ts_df.convert_frequency("Y", agg_numeric="sum")
+        >>> ts_df.convert_frequency("YE", agg_numeric="sum")
                             target
         item_id timestamp
         0       2020-12-31    10.0
                 2021-12-31    26.0
         """
         offset = pd.tseries.frequencies.to_offset(freq)
         if self.freq == offset.freqstr:
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,16 @@
                     "No features provided to compute feature importance. At least some valid features should be provided."
                 )
             for fn in features:
                 if fn not in self.feature_generator.covariate_metadata.all_features and fn not in unused_features:
                     raise ValueError(f"Feature {fn} not found in covariate metadata or the dataset.")
 
         if len(set(features)) < len(features):
-            logger.warning(
-                "Duplicate feature names provided to compute feature importance. This will lead to unexpected behavior. "
+            raise ValueError(
+                "Duplicate feature names provided to compute feature importance. "
                 "Please provide unique feature names across both static features and covariates."
             )
 
         data = self.feature_generator.transform(data)
 
         importance_df = trainer.get_feature_importance(
             data=data,
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Parameters
     ----------
     path : str, default = None
         Directory location to store all outputs.
         If None, a new unique time-stamped directory is chosen.
     freq: str
         Frequency string (cf. gluonts frequency strings) describing the frequency
-        of the time series data. For example, "H" for hourly or "D" for daily data.
+        of the time series data. For example, "h" for hourly or "D" for daily data.
     prediction_length: int
         Length of the prediction horizon, i.e., the number of time steps the model
         is fit to forecast.
     name : str, default = None
         Name of the subdirectory inside path where model will be saved.
         The final model directory will be os.path.join(path, name)
         If None, defaults to the model's class name: self.__class__.__name__
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,46 +11,42 @@
 import pandas as pd
 from gluonts.core.component import from_hyperparameters
 from gluonts.dataset.common import Dataset as GluonTSDataset
 from gluonts.dataset.field_names import FieldName
 from gluonts.model.estimator import Estimator as GluonTSEstimator
 from gluonts.model.forecast import Forecast, QuantileForecast, SampleForecast
 from gluonts.model.predictor import Predictor as GluonTSPredictor
-from pandas.tseries.frequencies import to_offset
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import QuantileTransformer, StandardScaler
 
 from autogluon.common.loaders import load_pkl
 from autogluon.core.hpo.constants import RAY_BACKEND
 from autogluon.tabular.models.tabular_nn.utils.categorical_encoders import (
     OneHotMergeRaresHandleUnknownEncoder as OneHotEncoder,
 )
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
-from autogluon.timeseries.utils.datetime import norm_freq_str
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 from autogluon.timeseries.utils.warning_filters import disable_root_logger, warning_filter
 
 # NOTE: We avoid imports for torch and lightning.pytorch at the top level and hide them inside class methods.
 # This is done to skip these imports during multiprocessing (which may cause bugs)
 
 logger = logging.getLogger(__name__)
 gts_logger = logging.getLogger(gluonts.__name__)
 
 
-GLUONTS_SUPPORTED_OFFSETS = ["Y", "Q", "M", "W", "D", "B", "H", "T", "min", "S"]
-
-
 class SimpleGluonTSDataset(GluonTSDataset):
     """Wrapper for TimeSeriesDataFrame that is compatible with the GluonTS Dataset API."""
 
+    _dummy_gluonts_freq = "D"
+
     def __init__(
         self,
         target_df: TimeSeriesDataFrame,
-        freq: str,
         target_column: str = "target",
         feat_static_cat: Optional[np.ndarray] = None,
         feat_static_real: Optional[np.ndarray] = None,
         feat_dynamic_cat: Optional[np.ndarray] = None,
         feat_dynamic_real: Optional[np.ndarray] = None,
         past_feat_dynamic_cat: Optional[np.ndarray] = None,
         past_feat_dynamic_real: Optional[np.ndarray] = None,
@@ -62,15 +58,14 @@
         self.target_array = target_df[target_column].to_numpy(np.float32)
         self.feat_static_cat = self._astype(feat_static_cat, dtype=np.int64)
         self.feat_static_real = self._astype(feat_static_real, dtype=np.float32)
         self.feat_dynamic_cat = self._astype(feat_dynamic_cat, dtype=np.int64)
         self.feat_dynamic_real = self._astype(feat_dynamic_real, dtype=np.float32)
         self.past_feat_dynamic_cat = self._astype(past_feat_dynamic_cat, dtype=np.int64)
         self.past_feat_dynamic_real = self._astype(past_feat_dynamic_real, dtype=np.float32)
-        self.freq = self._to_gluonts_freq(freq)
 
         # Necessary to compute indptr for known_covariates at prediction time
         self.includes_future = includes_future
         self.prediction_length = prediction_length
 
         # Replace inefficient groupby ITEMID with indptr that stores start:end of each time series
         item_id_index = target_df.index.get_level_values(ITEMID)
@@ -84,40 +79,25 @@
     @staticmethod
     def _astype(array: Optional[np.ndarray], dtype: np.dtype) -> Optional[np.ndarray]:
         if array is None:
             return None
         else:
             return array.astype(dtype)
 
-    @staticmethod
-    def _to_gluonts_freq(freq: str) -> str:
-        # FIXME: GluonTS expects a frequency string, but only supports a limited number of such strings
-        # for feature generation. If the frequency string doesn't match or is not provided, it raises an exception.
-        # Here we bypass this by issuing a default "yearly" frequency, tricking it into not producing
-        # any lags or features.
-        pd_offset = to_offset(freq)
-
-        # normalize freq str to handle peculiarities such as W-SUN
-        offset_base_alias = norm_freq_str(pd_offset)
-        if offset_base_alias not in GLUONTS_SUPPORTED_OFFSETS:
-            return "A"
-        else:
-            return f"{pd_offset.n}{offset_base_alias}"
-
     def __len__(self):
         return len(self.indptr) - 1  # noqa
 
     def __iter__(self) -> Iterator[Dict[str, Any]]:
         for j in range(len(self.indptr) - 1):
             start_idx = self.indptr[j]
             end_idx = self.indptr[j + 1]
             # GluonTS expects item_id to be a string
             ts = {
                 FieldName.ITEM_ID: str(self.item_ids[j]),
-                FieldName.START: pd.Period(self.start_timestamps.iloc[j], freq=self.freq),
+                FieldName.START: pd.Period(self.start_timestamps.iloc[j], freq=self._dummy_gluonts_freq),
                 FieldName.TARGET: self.target_array[start_idx:end_idx],
             }
             if self.feat_static_cat is not None:
                 ts[FieldName.FEAT_STATIC_CAT] = self.feat_static_cat[j]
             if self.feat_static_real is not None:
                 ts[FieldName.FEAT_STATIC_REAL] = self.feat_static_real[j]
             if self.past_feat_dynamic_cat is not None:
@@ -491,15 +471,14 @@
                         [past_feat_dynamic_real, past_feat_dynamic_cat_ohe], axis=1
                     )
             else:
                 past_feat_dynamic_real = None
 
             return SimpleGluonTSDataset(
                 target_df=time_series_df[[self.target]],
-                freq=self.freq,
                 target_column=self.target,
                 feat_static_cat=feat_static_cat,
                 feat_static_real=feat_static_real,
                 feat_dynamic_cat=feat_dynamic_cat,
                 feat_dynamic_real=feat_dynamic_real,
                 past_feat_dynamic_cat=past_feat_dynamic_cat,
                 past_feat_dynamic_real=past_feat_dynamic_real,
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,9 +420,9 @@
         init_kwargs["cardinality"] = [1] if self.num_feat_static_cat == 0 else self.feat_static_cat_cardinality
         init_kwargs["num_feat_dynamic_real"] = self.num_feat_dynamic_real
         init_kwargs.setdefault("negative_data", self.negative_data)
         init_kwargs.setdefault("seasonality", get_seasonality(self.freq))
         init_kwargs.setdefault("time_features", get_time_features_for_frequency(self.freq))
         init_kwargs.setdefault("num_parallel_samples", self.default_num_samples)
         # WaveNet model fails if an unsupported frequency such as "SM" is provided. We provide a dummy freq instead
-        init_kwargs["freq"] = "H"
+        init_kwargs["freq"] = "D"
         return init_kwargs
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         Name of column that contains the target values to forecast (i.e., numeric observations of the time series).
     prediction_length : int, default = 1
         The forecast horizon, i.e., How many time steps into the future the models should be trained to predict.
         For example, if time series contain daily observations, setting ``prediction_length = 3`` will train
         models that predict up to 3 days into the future from the most recent observation.
     freq : str, optional
         Frequency of the time series data (see `pandas documentation <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases>`_
-        for available frequencies). For example, ``"D"`` for daily data or ``"H"`` for hourly data.
+        for available frequencies). For example, ``"D"`` for daily data or ``"h"`` for hourly data.
 
         By default, the predictor will attempt to automatically infer the frequency from the data. This argument should
         only be set in two cases:
 
         1. The time series data has irregular timestamps, so frequency cannot be inferred automatically.
         2. You would like to resample the original data at a different frequency (for example, convert hourly measurements into daily measurements).
 
@@ -191,15 +191,15 @@
         self.known_covariates_names = list(known_covariates_names)
 
         self.prediction_length = prediction_length
         # For each validation fold, all time series in training set must have length >= _min_train_length
         self._min_train_length = max(self.prediction_length + 1, 5)
         self.freq = freq
         if self.freq is not None:
-            # Standardize frequency string (e.g., "min" -> "T", "Y" -> "A-DEC")
+            # Standardize frequency string (e.g., "T" -> "min", "Y" -> "YE")
             std_freq = pd.tseries.frequencies.to_offset(self.freq).freqstr
             if std_freq != str(self.freq):
                 logger.info(f"Frequency '{self.freq}' stored as '{std_freq}'")
             self.freq = std_freq
         self.eval_metric = check_get_evaluation_metric(eval_metric)
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         if quantile_levels is None:
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 import pandas as pd
 
 TO_MAJOR_FREQ = {
-    "min": "T",
-    "ms": "L",
-    "us": "U",
+    # sub-daily
+    "H": "h",
+    "BH": "bh",
+    "cbh": "bh",
+    "CBH": "bh",
+    "T": "min",
+    "S": "s",
+    "L": "ms",
+    "U": "us",
+    "N": "ns",
     # business day
     "C": "B",
     # month
-    "BM": "M",
-    "CBM": "M",
-    "MS": "M",
-    "BMS": "M",
-    "CBMS": "M",
+    "M": "ME",
+    "BM": "ME",
+    "BME": "ME",
+    "CBM": "ME",
+    "CBME": "ME",
+    "MS": "ME",
+    "BMS": "ME",
+    "CBMS": "ME",
     # semi-month
-    "SMS": "SM",
+    "SM": "SME",
+    "SMS": "SME",
     # quarter
-    "BQ": "Q",
-    "QS": "Q",
-    "BQS": "Q",
+    "Q": "QE",
+    "BQ": "QE",
+    "BQE": "QE",
+    "QS": "QE",
+    "BQS": "QE",
     # annual
-    "Y": "A",
-    "BA": "A",
-    "BY": "A",
-    "AS": "A",
-    "YS": "A",
-    "BAS": "A",
-    "BYS": "A",
+    "A": "YE",
+    "Y": "YE",
+    "BA": "YE",
+    "BY": "YE",
+    "BYE": "YE",
+    "AS": "YE",
+    "YS": "YE",
+    "BAS": "YE",
+    "BYS": "YE",
 }
 
 
 def norm_freq_str(offset: pd.DateOffset) -> str:
     """Obtain frequency string from a pandas.DateOffset object.
 
     "Non-standard" frequencies are converted to their "standard" counterparts. For example, MS (month start) is mapped
-    to M (month) since both correspond to the same seasonality, lags and time features.
+    to ME (month end) since both correspond to the same seasonality, lags and time features.
+
+    The frequencies are always mapped to the new non-deprecated aliases (pandas>=2.2), e.g., "H" is mapped to "h". The
+    downstream functions like `get_seasonality` handle the new aliases even if older version of pandas is used.
     """
     base_freq = offset.name.split("-")[0]
     return TO_MAJOR_FREQ.get(base_freq, base_freq)
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Generate lag indices based on frequency string. Adapted from gluonts.time_feature.lag.
 """
+
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 
 from .base import norm_freq_str
 
@@ -92,75 +93,75 @@
     num_default_lags
         The number of default lags; by default it is 7.
     """
 
     offset = pd.tseries.frequencies.to_offset(freq)
     offset_name = norm_freq_str(offset)
 
-    if offset_name == "A":
+    if offset_name == "YE":
         lags = []
-    elif offset_name == "Q":
+    elif offset_name == "QE":
         lags = _make_lags_for_quarter(offset.n)
-    elif offset_name == "M":
+    elif offset_name == "ME":
         lags = _make_lags_for_month(offset.n)
-    elif offset_name == "SM":
+    elif offset_name == "SME":
         lags = _make_lags_for_semi_month(offset.n)
     elif offset_name == "W":
         lags = _make_lags_for_week(offset.n)
     elif offset_name == "D":
         lags = _make_lags_for_day(offset.n) + _make_lags_for_week(offset.n / 7.0)
     elif offset_name == "B":
         lags = _make_lags_for_day(offset.n, days_in_week=5, days_in_month=22) + _make_lags_for_week(offset.n / 5.0)
-    elif offset_name == "H":
+    elif offset_name == "h":
         lags = (
             _make_lags_for_hour(offset.n)
             + _make_lags_for_day(offset.n / 24)
             + _make_lags_for_week(offset.n / (24 * 7))
         )
     # business hour
-    elif offset_name == "BH":
+    elif offset_name == "bh":
         lags = (
             _make_lags_for_business_hour(offset.n)
             + _make_lags_for_day(offset.n / 9)
             + _make_lags_for_week(offset.n / (9 * 7))
         )
     # minutes
-    elif offset_name == "T":
+    elif offset_name == "min":
         lags = (
             _make_lags_for_minute(offset.n)
             + _make_lags_for_hour(offset.n / 60)
             + _make_lags_for_day(offset.n / (60 * 24))
             + _make_lags_for_week(offset.n / (60 * 24 * 7))
         )
     # second
-    elif offset_name == "S":
+    elif offset_name == "s":
         lags = (
             _make_lags_for_second(offset.n)
             + _make_lags_for_minute(offset.n / 60)
             + _make_lags_for_hour(offset.n / (60 * 60))
         )
-    elif offset_name == "L":
+    elif offset_name == "ms":
         lags = (
             _make_lags_for_second(offset.n / 1e3)
             + _make_lags_for_minute(offset.n / (60 * 1e3))
             + _make_lags_for_hour(offset.n / (60 * 60 * 1e3))
         )
-    elif offset_name == "U":
+    elif offset_name == "us":
         lags = (
             _make_lags_for_second(offset.n / 1e6)
             + _make_lags_for_minute(offset.n / (60 * 1e6))
             + _make_lags_for_hour(offset.n / (60 * 60 * 1e6))
         )
-    elif offset_name == "N":
+    elif offset_name == "ns":
         lags = (
             _make_lags_for_second(offset.n / 1e9)
             + _make_lags_for_minute(offset.n / (60 * 1e9))
             + _make_lags_for_hour(offset.n / (60 * 60 * 1e9))
         )
     else:
-        raise Exception(f"invalid frequency {freq}")
+        raise Exception(f"Cannot get lags for unsupported frequency {freq}")
 
     # flatten lags list and filter
     lags = [int(lag) for sub_list in lags for lag in sub_list if 7 < lag <= lag_ub]
     lags = list(range(1, num_default_lags + 1)) + sorted(list(set(lags)))
 
     return sorted(set(lags))[:num_lags]
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Union
 
 import pandas as pd
 
 from .base import norm_freq_str
 
 DEFAULT_SEASONALITIES = {
-    "A": 1,
-    "Q": 4,
-    "M": 12,
-    "SM": 24,
+    "YE": 1,
+    "QE": 4,
+    "ME": 12,
+    "SME": 24,
     "W": 1,
     "D": 7,
     "B": 5,
-    "BH": 9,
-    "H": 24,
-    "T": 60 * 24,
-    "S": 1,
-    "L": 1,
-    "U": 1,
-    "N": 1,
+    "bh": 9,
+    "h": 24,
+    "min": 60 * 24,
+    "s": 1,
+    "ms": 1,
+    "us": 1,
+    "ns": 1,
 }
 
 
 def get_seasonality(freq: Union[str, None]) -> int:
     """Return the seasonality of a given frequency. Adapted from ``gluonts.time_feature.seasonality``."""
     if freq is None:
         return 1
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Generate time features based on frequency string. Adapted from gluonts.time_feature.time_feature.
 """
+
 from typing import Callable, List
 
 import numpy as np
 import pandas as pd
 
 from .base import norm_freq_str
 
@@ -53,25 +54,25 @@
 
 def second_of_minute(index: pd.DatetimeIndex) -> np.ndarray:
     return _normalize(index.second, num=60)
 
 
 def get_time_features_for_frequency(freq) -> List[Callable]:
     features_by_offset_name = {
-        "A": [],
-        "Q": [quarter_of_year],
-        "M": [month_of_year],
-        "SM": [day_of_month, month_of_year],
+        "YE": [],
+        "QE": [quarter_of_year],
+        "ME": [month_of_year],
+        "SME": [day_of_month, month_of_year],
         "W": [day_of_month, week_of_year],
         "D": [day_of_week, day_of_month, day_of_year],
         "B": [day_of_week, day_of_month, day_of_year],
-        "BH": [hour_of_day, day_of_week, day_of_month, day_of_year],
-        "H": [hour_of_day, day_of_week, day_of_month, day_of_year],
-        "T": [minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
-        "S": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
-        "L": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
-        "U": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
-        "N": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
+        "bh": [hour_of_day, day_of_week, day_of_month, day_of_year],
+        "h": [hour_of_day, day_of_week, day_of_month, day_of_year],
+        "min": [minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
+        "s": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
+        "ms": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
+        "us": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
+        "ns": [second_of_minute, minute_of_hour, hour_of_day, day_of_week, day_of_month, day_of_year],
     }
     offset = pd.tseries.frequencies.to_offset(freq)
     offset_name = norm_freq_str(offset)
     return features_by_offset_name[offset_name]
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from autogluon.features.generators import (
     AsTypeFeatureGenerator,
     CategoryFeatureGenerator,
     IdentityFeatureGenerator,
     PipelineFeatureGenerator,
 )
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
+from autogluon.timeseries.utils.warning_filters import warning_filter
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CovariateMetadata:
     """Provides mapping from different covariate types to columns in the dataset."""
@@ -331,15 +332,17 @@
 
         is_categorical = feature_name in self.covariate_metadata.cat_features
 
         if feature_name in self.covariate_metadata.past_covariates:
             # we'll have to work on the history of the data alone
             data[feature_name] = data[feature_name].copy()
             feature_data = data[feature_name].groupby(level=ITEMID, sort=False).head(-self.prediction_length)
-            data[feature_name].update(self._transform_series(feature_data, is_categorical=is_categorical))
+            # Silence spurious FutureWarning raised by DataFrame.update https://github.com/pandas-dev/pandas/issues/57124
+            with warning_filter():
+                data[feature_name].update(self._transform_series(feature_data, is_categorical=is_categorical))
         elif feature_name in self.covariate_metadata.static_features:
             feature_data = data.static_features[feature_name].copy()
             feature_data.reset_index(drop=True, inplace=True)
             data.static_features[feature_name] = self._transform_static_series(
                 feature_data, is_categorical=is_categorical
             )
         else:  # known covariates
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240412/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240411
+Version: 1.1.0b20240412
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240412/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 joblib<2,>=1.1
 numpy<1.29,>=1.21
 scipy<1.13,>=1.5.4
-pandas<2.2.0,>=2.0.0
+pandas<2.3.0,>=2.0.0
 torch<2.2,>=2.1
 lightning<2.2,>=2.1
 pytorch_lightning<2.2,>=2.1
 transformers[sentencepiece]<4.39.0,>=4.38.0
 accelerate<0.22.0,>=0.21.0
 statsmodels<0.15,>=0.13.0
-gluonts<0.15,>=0.14.0
+gluonts<0.14.4,>=0.14.0
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.0b20240411
-autogluon.common==1.1.0b20240411
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240411
+autogluon.core[raytune]==1.1.0b20240412
+autogluon.common==1.1.0b20240412
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240412
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

