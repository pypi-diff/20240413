# Comparing `tmp/autogluon.core-1.1.0b20240411.tar.gz` & `tmp/autogluon.core-1.1.0b20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.1.0b20240411.tar", last modified: Thu Apr 11 09:04:00 2024, max compression
+gzip compressed data, was "autogluon.core-1.1.0b20240412.tar", last modified: Fri Apr 12 09:04:37 2024, max compression
```

## Comparing `autogluon.core-1.1.0b20240411.tar` & `autogluon.core-1.1.0b20240412.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.094239 autogluon.core-1.1.0b20240411/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.094239 autogluon.core-1.1.0b20240411/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.098240 autogluon.core-1.1.0b20240411/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.098240 autogluon.core-1.1.0b20240411/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.098240 autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.098240 autogluon.core-1.1.0b20240411/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    99982 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.102239 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66393 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/stacked_overfitting/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/stacked_overfitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.106239 autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   198790 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.110240 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 09:03:38.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 09:03:59.000000 autogluon.core-1.1.0b20240411/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:04:00.098240 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:04:00.000000 autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.613931 autogluon.core-1.1.0b20240412/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.613931 autogluon.core-1.1.0b20240412/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.621931 autogluon.core-1.1.0b20240412/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.621931 autogluon.core-1.1.0b20240412/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.621931 autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.621931 autogluon.core-1.1.0b20240412/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.621931 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29424 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100159 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.625931 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66570 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/stacked_overfitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/stacked_overfitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.629931 autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198790 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.633931 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-12 09:04:11.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:37.617931 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:04:37.000000 autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-1.1.0b20240411/PKG-INFO` & `autogluon.core-1.1.0b20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-1.1.0b20240411/setup.py` & `autogluon.core-1.1.0b20240412/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/_setup_utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/_setup_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 PYTHON_REQUIRES = ">=3.8, <3.12"
 
 
 # Only put packages here that would otherwise appear multiple times across different module's setup.py files.
 DEPENDENT_PACKAGES = {
     "boto3": ">=1.10,<2",  # <2 because unlikely to introduce breaking changes in minor releases. >=1.10 because 1.10 is 3 years old, no need to support older
     "numpy": ">=1.21,<1.29",  # "<{N+3}" upper cap, where N is the latest released minor version, assuming no warnings using N
-    "pandas": ">=2.0.0,<2.2.0",  # "<{N+1}" upper cap
+    "pandas": ">=2.0.0,<2.3.0",  # "<{N+3}" upper cap
     "scikit-learn": ">=1.3.0,<1.4.1",  # "<{N+1}" upper cap, capping to micro version as AutoMM HPO tests fail on upgrading to higher version
     "scipy": ">=1.5.4,<1.13",  # "<{N+2}" upper cap
     "psutil": ">=5.7.3,<6",  # Major version cap
     "s3fs": ">=2023.1,<2025",  # Yearly cap
     "networkx": ">=3.0,<4",  # Major version cap
     "tqdm": ">=4.38,<5",  # Major version cap
     "Pillow": ">=10.0.1,<11",  # Major version cap
```

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/constants.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/data/cleaner.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/dataset.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/executors.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,17 +392,17 @@
             Type of adapter used by ray hpo experiment.
             Adapters are used to provide custom info or behavior that's module specific to the ray hpo experiment.
             For more info, please refer to `autogluon/core/hpo/ray_hpo`
             Valid values are ['tabular', 'timeseries', 'automm']
         trainable_is_parallel
             Whether the trainable itself will use ray to run parallel job or not.
         tune_config_kwargs
-            Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
+            Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/tune/api/doc/ray.tune.TuneConfig.html#ray-tune-tuneconfig
         run_config_kwargs
-            Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
+            Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/train/api/doc/ray.train.RunConfig.html#ray.train.RunConfig
         """
         from .ray_hpo import RayTuneAdapterFactory, run
 
         # Disable tensorboard logging to avoid layer warning
         # TODO: remove this when ray tune fix ray tune pass tuple to hyperopt issue
         os.environ["TUNE_DISABLE_AUTO_CALLBACK_LOGGERS"] = "1"
         analysis = run(
```

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,17 +202,17 @@
         Provide optional estimate of the model memory usage.
         Calculation of the resources_per_trial might use this info to better distribute resources
     time_budget_s
         Time limit for the HPO.
     verbose
         0 = silent, 1 = only status updates, 2 = status and brief trial results, 3 = status and detailed trial results.
     tune_config_kwargs
-        Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
+        Additional args being passed to tune.TuneConfig  https://docs.ray.io/en/latest/tune/api/doc/ray.tune.TuneConfig.html#ray-tune-tuneconfig
     run_config_kwargs
-        Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
+        Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/train/api/doc/ray.train.RunConfig.html#ray.train.RunConfig
     """
     assert mode in [MIN, MAX], f"mode {mode} is not a valid option. Options are {[MIN, MAX]}"
     if isinstance(hyperparameter_tune_kwargs, str):
         assert (
             hyperparameter_tune_kwargs in ray_tune_adapter.presets
         ), f"{hyperparameter_tune_kwargs} is not a valid option. Options are {ray_tune_adapter.presets.keys()}"
         hyperparameter_tune_kwargs = ray_tune_adapter.presets.get(hyperparameter_tune_kwargs)
```

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/__init__.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/_utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1526,23 +1526,26 @@
             val_path=val_path,
             hpo_executor=hpo_executor,
         )
         model_estimate_memory_usage = None
         if self.estimate_memory_usage is not None:
             model_estimate_memory_usage = self.estimate_memory_usage(X=X, **kwargs)
         minimum_resources = self.get_minimum_resources(is_gpu_available=(hpo_executor.resources.get("num_gpus", 0) > 0))
+        # This explicitly tells ray.Tune to not change the working directory
+        # to the trial directory, giving access to paths relative to
+        # the original working directory.
+        os.environ["RAY_CHDIR_TO_TRIAL_DIR"] = "0"
         hpo_executor.execute(
             model_trial=model_trial,
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
             minimum_cpu_per_trial=minimum_resources.get("num_cpus", 1),
             minimum_gpu_per_trial=minimum_resources.get("num_gpus", 0),
             model_estimate_memory_usage=model_estimate_memory_usage,
             adapter_type="tabular",
-            tune_config_kwargs={"chdir_to_trial_dir": False},
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
```

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1377,24 +1377,27 @@
             is_bagged_model=True,
         )
 
         minimum_resources_per_fold = self.get_minimum_resources(is_gpu_available=(hpo_executor.resources.get("num_gpus", 0) > 0))
         minimum_cpu_per_fold = minimum_resources_per_fold.get("num_cpus", 1)
         minimum_gpu_per_fold = minimum_resources_per_fold.get("num_gpus", 0)
 
+        # This explicitly tells ray.Tune to not change the working directory
+        # to the trial directory, giving access to paths relative to
+        # the original working directory.
+        os.environ["RAY_CHDIR_TO_TRIAL_DIR"] = "0"
         hpo_executor.execute(
             model_trial=model_trial,
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
             minimum_cpu_per_trial=minimum_cpu_per_fold,
             minimum_gpu_per_trial=minimum_gpu_per_fold,
             model_estimate_memory_usage=None,  # Not needed as we've already calculated it above
             adapter_type="tabular",
             trainable_is_parallel=True,
-            tune_config_kwargs={"chdir_to_trial_dir": False},
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
```

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/problem_type.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/stacked_overfitting/utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/stacked_overfitting/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/trainer/utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/decorators.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/files.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/plots.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/time.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon/core/utils/version_utils.py` & `autogluon.core-1.1.0b20240412/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
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

### Comparing `autogluon.core-1.1.0b20240411/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-1.1.0b20240412/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

