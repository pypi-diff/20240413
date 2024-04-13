# Comparing `tmp/reinforced-lib-1.1.0.tar.gz` & `tmp/reinforced_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reinforced-lib-1.1.0.tar", last modified: Sun Feb 11 14:55:23 2024, max compression
+gzip compressed data, was "reinforced_lib-1.1.1.tar", last modified: Sat Apr 13 17:30:43 2024, max compression
```

## Comparing `reinforced-lib-1.1.0.tar` & `reinforced_lib-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.853649 reinforced-lib-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27538 2024-02-11 14:55:23.853649 reinforced-lib-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.841649 reinforced-lib-1.1.0/reinforced_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.845649 reinforced-lib-1.1.0/reinforced_lib/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.845649 reinforced-lib-1.1.0/reinforced_lib/agents/deep/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/deep/ddpg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/deep/ddqn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14286 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/deep/dqn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/deep/expected_sarsa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.845649 reinforced-lib-1.1.0/reinforced_lib/agents/mab/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/e_greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/exp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/lognormal_thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/normal_thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/thompson_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/agents/mab/ucb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.849649 reinforced-lib-1.1.0/reinforced_lib/exts/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/exts/base_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/exts/basic_mab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/exts/gymnasium.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/exts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.849649 reinforced-lib-1.1.0/reinforced_lib/logs/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/logs_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/plots_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/stdout_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/tb_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/logs/wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    23361 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/rlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.849649 reinforced-lib-1.1.0/reinforced_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/utils/experience_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/reinforced_lib/utils/particle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.849649 reinforced-lib-1.1.0/reinforced_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27538 2024-02-11 14:55:23.000000 reinforced-lib-1.1.0/reinforced_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-11 14:55:23.000000 reinforced-lib-1.1.0/reinforced_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 14:55:23.000000 reinforced-lib-1.1.0/reinforced_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-11 14:55:23.000000 reinforced-lib-1.1.0/reinforced_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-11 14:55:23.000000 reinforced-lib-1.1.0/reinforced_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 14:55:23.853649 reinforced-lib-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 14:55:23.849649 reinforced-lib-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/test/test_rlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/test/test_rlib_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-11 14:55:16.000000 reinforced-lib-1.1.0/test/test_rlib_to_tflite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.764809 reinforced_lib-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28211 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.752809 reinforced_lib-1.1.1/reinforced_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.756809 reinforced_lib-1.1.1/reinforced_lib/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.756809 reinforced_lib-1.1.1/reinforced_lib/agents/deep/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/deep/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/deep/ddqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14286 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/deep/dqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/deep/expected_sarsa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.756809 reinforced_lib-1.1.1/reinforced_lib/agents/mab/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/e_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/exp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/lognormal_thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/normal_thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/thompson_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/agents/mab/ucb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/reinforced_lib/exts/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/exts/base_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/exts/basic_mab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/exts/gymnasium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/exts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/reinforced_lib/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/logs_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/plots_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/stdout_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/tb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/logs/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/rlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/reinforced_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/utils/experience_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/reinforced_lib/utils/particle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/reinforced_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28211 2024-04-13 17:30:43.000000 reinforced_lib-1.1.1/reinforced_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-13 17:30:43.000000 reinforced_lib-1.1.1/reinforced_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:30:43.000000 reinforced_lib-1.1.1/reinforced_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-13 17:30:43.000000 reinforced_lib-1.1.1/reinforced_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 17:30:43.000000 reinforced_lib-1.1.1/reinforced_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:30:43.764809 reinforced_lib-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:30:43.760809 reinforced_lib-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/test/test_rlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/test/test_rlib_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-04-13 17:30:39.000000 reinforced_lib-1.1.1/test/test_rlib_to_tflite.py
```

### Comparing `reinforced-lib-1.1.0/LICENSE` & `reinforced_lib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/PKG-INFO` & `reinforced_lib-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reinforced-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Reinforcement learning library
 Author-email: Maksymilian Wojnar <mwojnar@agh.edu.pl>, Wojciech Ciężobka <wciezobka@agh.edu.pl>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -389,25 +389,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: chex~=0.1.85
+Requires-Dist: chex~=0.1.86
 Requires-Dist: cloudpickle~=3.0.0
-Requires-Dist: flax~=0.8.1
+Requires-Dist: flax~=0.8.2
 Requires-Dist: gymnasium~=0.29.1
-Requires-Dist: jax~=0.4.24
-Requires-Dist: jaxlib~=0.4.24
+Requires-Dist: jax~=0.4.26
+Requires-Dist: jaxlib~=0.4.26
 Requires-Dist: lz4~=4.3.3
-Requires-Dist: matplotlib~=3.8.2
-Requires-Dist: optax~=0.1.9
+Requires-Dist: matplotlib~=3.8.4
+Requires-Dist: optax~=0.2.2
 Requires-Dist: tensorboardX~=2.6.2.2
-Requires-Dist: wandb~=0.16.3
+Requires-Dist: wandb~=0.16.6
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
 Provides-Extra: full
 Requires-Dist: joblib~=1.3.2; extra == "full"
 Requires-Dist: pygame~=2.5.2; extra == "full"
 Requires-Dist: seaborn~=0.13.2; extra == "full"
@@ -415,29 +415,30 @@
 
 # Reinforced-lib: Reinforcement learning library
 
 [![PyPI version][pypi-badge]][pypi]
 [![License: MPL 2.0][license-badge]][license]
 [![build and test][tests-badge]][github-actions]
 [![Documentation Status][rtd-badge]][documentation]
+[![DOI](https://img.shields.io/badge/DOI-10.1016/j.softx.2024.101706-blue.svg)](https://doi.org/10.1016/j.softx.2024.101706)
 
 [pypi-badge]: https://img.shields.io/pypi/v/reinforced-lib
 [pypi]: https://pypi.org/project/reinforced-lib/
 [license-badge]: https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg
 [license]: https://opensource.org/licenses/MPL-2.0
 [tests-badge]: https://github.com/m-wojnar/reinforced-lib/actions/workflows/python-package.yml/badge.svg
 [github-actions]: https://github.com/m-wojnar/reinforced-lib/actions
 [rtd-badge]: https://readthedocs.org/projects/reinforced-lib/badge/?version=latest
 [documentation]: https://reinforced-lib.readthedocs.io/en/latest/
 
-**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of RL solutions. It is open-source, 
-prioritizes ease of use, provides comprehensive documentation, and offers both deep reinforcement learning 
-(DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), it facilitates exporting 
-trained models to embedded devices, and makes it great for research and prototyping with RL algorithms. Access to JAX's 
-just-in-time (JIT) compilation ensures high-performance results.
+**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of reinforcement-learning (RL) 
+solutions. It is open-source, prioritizes ease of use, provides comprehensive documentation, and offers both deep 
+reinforcement learning (DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), 
+it facilitates exporting trained models to embedded devices, and makes it great for research and prototyping with RL 
+algorithms. Access to JAX's just-in-time (JIT) compilation ensures high-performance results.
 
 ## Installation
 
 You can install the latest version of Reinforced-lib from PyPI:
 
 ```bash
 pip install reinforced-lib
@@ -452,47 +453,50 @@
 pip install .
 ```
 
 In the spirit of making Reinforced-lib a lightweight solution, we include only the necessary dependencies in the base 
 requirements. To fully benefit from Reinforced-lib's conveniences, such as TF Lite export, install with the "full" suffix:
 
 ```bash
-pip3 install ".[full]"
+pip install ".[full]"
 ```
 
 ## Key components
 
 Reinforced-lib facilitates seamless interaction between RL agents and the environment. Here are the key components 
 within of the library, represented in the API as different modules.
 
 - **RLib** - The core module which provides a simple and intuitive interface to manage agents, use extensions, 
-  and configure the logging system. Even if you're not a reinforcement learning (RL) expert, *RLib* makes it easy to 
-  implement the agent-environment interaction loop.
+  and configure the logging system. Even if you're not an RL expert, *RLib* makes it easy to  implement the 
+  agent-environment interaction loop.
 
 - **Agents** - Choose from a variety of RL agents available in the *Agents* module. These agents are designed to be 
   versatile and work with any environment. If needed, you can even create your own agents using our documented recipes.
 
 - **Extensions** - Enhance agent observations with domain-specific knowledge by adding a suitable extension from the 
   *Extensions* module. This module enables seamless agent switching and parameter tuning without extensive reconfiguration.
 
-- **Logging** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
+- **Loggers** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
   specific needs, capturing training metrics, internal agent state, or environment observations. The library includes 
   various loggers for creating plots and output files, simplifying visualization and data processing.
 
 The figure below provides a visual representation of Reinforced-lib and the data-flow between its modules.
 
 <img src="docs/resources/data-flow.png" width="600">
 
 ## JAX Backend
 
 Our library is built on top of JAX, a high-performance numerical computing library. JAX makes it easy to implement 
-RL algorithms efficiently. It provides powerful transformations, including JIT compilation,  automatic differentiation, 
+RL algorithms efficiently. It provides powerful transformations, including JIT compilation, automatic differentiation, 
 vectorization, and parallelization. Our library is fully compatible with DeepMind's JAX ecosystem, granting access to 
 state-of-the-art RL models and helper libraries. JIT compilation significantly accelerates execution and ensures 
-portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications.
+portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications. 
+JAX offers another benefit through its robust pseudorandom number generator system, employed in our library to 
+guarantee result reproducibility. This critical aspect of scientific research is frequently underestimated but 
+remains highly significant.
 
 ## Edge Device Export
 
 Reinforced-lib is designed to work seamlessly on wireless, low-powered devices, where resources are limited. It's the 
 perfect solution for energy-constrained environments that may struggle with other ML frameworks. You can export your 
 trained models to [TensorFlow Lite](https://www.tensorflow.org/lite) with ease, reducing runtime overhead and 
 optimizing performance. This means you can deploy RL agents on resource-limited devices efficiently.
@@ -544,17 +548,22 @@
             env_state = env.step(action.item())
             action = rl.sample(*env_state)
             terminal = env_state[2] or env_state[3]
 ```
 
 ## Citing Reinforced-lib
 
-To cite this repository:
+To cite this repository, please use the following BibTeX entry for the Reinforced-lib paper:
 
-```
-@software{reinforcedlib2022,
-  author = {Maksymilian Wojnar and Wojciech Ciężobka},
-  title = {{R}einforced-lib: {R}einforcement learning library},
-  url = {http://github.com/m-wojnar/reinforced-lib},
-  year = {2022},
+```bibtex
+@article{reinforcedlib2022,
+  author = {Maksymilian Wojnar and Szymon Szott and Krzysztof Rusek and Wojciech Ciezobka},
+  title = {{R}einforced-lib: {R}apid prototyping of reinforcement learning solutions},
+  journal = {SoftwareX},
+  volume = {26},
+  pages = {101706},
+  year = {2024},
+  issn = {2352-7110},
+  doi = {https://doi.org/10.1016/j.softx.2024.101706},
+  url = {https://www.sciencedirect.com/science/article/pii/S2352711024000773}
 }
 ```
```

### Comparing `reinforced-lib-1.1.0/README.md` & `reinforced_lib-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Reinforced-lib: Reinforcement learning library
 
 [![PyPI version][pypi-badge]][pypi]
 [![License: MPL 2.0][license-badge]][license]
 [![build and test][tests-badge]][github-actions]
 [![Documentation Status][rtd-badge]][documentation]
+[![DOI](https://img.shields.io/badge/DOI-10.1016/j.softx.2024.101706-blue.svg)](https://doi.org/10.1016/j.softx.2024.101706)
 
 [pypi-badge]: https://img.shields.io/pypi/v/reinforced-lib
 [pypi]: https://pypi.org/project/reinforced-lib/
 [license-badge]: https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg
 [license]: https://opensource.org/licenses/MPL-2.0
 [tests-badge]: https://github.com/m-wojnar/reinforced-lib/actions/workflows/python-package.yml/badge.svg
 [github-actions]: https://github.com/m-wojnar/reinforced-lib/actions
 [rtd-badge]: https://readthedocs.org/projects/reinforced-lib/badge/?version=latest
 [documentation]: https://reinforced-lib.readthedocs.io/en/latest/
 
-**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of RL solutions. It is open-source, 
-prioritizes ease of use, provides comprehensive documentation, and offers both deep reinforcement learning 
-(DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), it facilitates exporting 
-trained models to embedded devices, and makes it great for research and prototyping with RL algorithms. Access to JAX's 
-just-in-time (JIT) compilation ensures high-performance results.
+**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of reinforcement-learning (RL) 
+solutions. It is open-source, prioritizes ease of use, provides comprehensive documentation, and offers both deep 
+reinforcement learning (DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), 
+it facilitates exporting trained models to embedded devices, and makes it great for research and prototyping with RL 
+algorithms. Access to JAX's just-in-time (JIT) compilation ensures high-performance results.
 
 ## Installation
 
 You can install the latest version of Reinforced-lib from PyPI:
 
 ```bash
 pip install reinforced-lib
@@ -37,47 +38,50 @@
 pip install .
 ```
 
 In the spirit of making Reinforced-lib a lightweight solution, we include only the necessary dependencies in the base 
 requirements. To fully benefit from Reinforced-lib's conveniences, such as TF Lite export, install with the "full" suffix:
 
 ```bash
-pip3 install ".[full]"
+pip install ".[full]"
 ```
 
 ## Key components
 
 Reinforced-lib facilitates seamless interaction between RL agents and the environment. Here are the key components 
 within of the library, represented in the API as different modules.
 
 - **RLib** - The core module which provides a simple and intuitive interface to manage agents, use extensions, 
-  and configure the logging system. Even if you're not a reinforcement learning (RL) expert, *RLib* makes it easy to 
-  implement the agent-environment interaction loop.
+  and configure the logging system. Even if you're not an RL expert, *RLib* makes it easy to  implement the 
+  agent-environment interaction loop.
 
 - **Agents** - Choose from a variety of RL agents available in the *Agents* module. These agents are designed to be 
   versatile and work with any environment. If needed, you can even create your own agents using our documented recipes.
 
 - **Extensions** - Enhance agent observations with domain-specific knowledge by adding a suitable extension from the 
   *Extensions* module. This module enables seamless agent switching and parameter tuning without extensive reconfiguration.
 
-- **Logging** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
+- **Loggers** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
   specific needs, capturing training metrics, internal agent state, or environment observations. The library includes 
   various loggers for creating plots and output files, simplifying visualization and data processing.
 
 The figure below provides a visual representation of Reinforced-lib and the data-flow between its modules.
 
 <img src="docs/resources/data-flow.png" width="600">
 
 ## JAX Backend
 
 Our library is built on top of JAX, a high-performance numerical computing library. JAX makes it easy to implement 
-RL algorithms efficiently. It provides powerful transformations, including JIT compilation,  automatic differentiation, 
+RL algorithms efficiently. It provides powerful transformations, including JIT compilation, automatic differentiation, 
 vectorization, and parallelization. Our library is fully compatible with DeepMind's JAX ecosystem, granting access to 
 state-of-the-art RL models and helper libraries. JIT compilation significantly accelerates execution and ensures 
-portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications.
+portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications. 
+JAX offers another benefit through its robust pseudorandom number generator system, employed in our library to 
+guarantee result reproducibility. This critical aspect of scientific research is frequently underestimated but 
+remains highly significant.
 
 ## Edge Device Export
 
 Reinforced-lib is designed to work seamlessly on wireless, low-powered devices, where resources are limited. It's the 
 perfect solution for energy-constrained environments that may struggle with other ML frameworks. You can export your 
 trained models to [TensorFlow Lite](https://www.tensorflow.org/lite) with ease, reducing runtime overhead and 
 optimizing performance. This means you can deploy RL agents on resource-limited devices efficiently.
@@ -129,17 +133,22 @@
             env_state = env.step(action.item())
             action = rl.sample(*env_state)
             terminal = env_state[2] or env_state[3]
 ```
 
 ## Citing Reinforced-lib
 
-To cite this repository:
+To cite this repository, please use the following BibTeX entry for the Reinforced-lib paper:
 
-```
-@software{reinforcedlib2022,
-  author = {Maksymilian Wojnar and Wojciech Ciężobka},
-  title = {{R}einforced-lib: {R}einforcement learning library},
-  url = {http://github.com/m-wojnar/reinforced-lib},
-  year = {2022},
+```bibtex
+@article{reinforcedlib2022,
+  author = {Maksymilian Wojnar and Szymon Szott and Krzysztof Rusek and Wojciech Ciezobka},
+  title = {{R}einforced-lib: {R}apid prototyping of reinforcement learning solutions},
+  journal = {SoftwareX},
+  volume = {26},
+  pages = {101706},
+  year = {2024},
+  issn = {2352-7110},
+  doi = {https://doi.org/10.1016/j.softx.2024.101706},
+  url = {https://www.sciencedirect.com/science/article/pii/S2352711024000773}
 }
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `reinforced-lib-1.1.0/pyproject.toml` & `reinforced_lib-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reinforced-lib"
-version = "1.1.0"
+version = "1.1.1"
 requires-python = ">=3.9, <4"
 
 description = "Reinforcement learning library"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["deep-reinforcement-learning", "jax", "library", "machine-learning", "reinforcement-learning"]
 
@@ -29,25 +29,25 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Typing :: Typed"
 ]
 
 dependencies = [
-    "chex~=0.1.85",
+    "chex~=0.1.86",
     "cloudpickle~=3.0.0",
-    "flax~=0.8.1",
+    "flax~=0.8.2",
     "gymnasium~=0.29.1",
-    "jax~=0.4.24",
-    "jaxlib~=0.4.24",
+    "jax~=0.4.26",
+    "jaxlib~=0.4.26",
     "lz4~=4.3.3",
-    "matplotlib~=3.8.2",
-    "optax~=0.1.9",
+    "matplotlib~=3.8.4",
+    "optax~=0.2.2",
     "tensorboardX~=2.6.2.2",
-    "wandb~=0.16.3"
+    "wandb~=0.16.6"
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx~=7.2.6",
     "sphinx-rtd-theme~=2.0.0"
 ]
```

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/base_agent.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/base_agent.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/deep/ddpg.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/deep/ddpg.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/deep/ddqn.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/deep/ddqn.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/deep/dqn.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/deep/dqn.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/deep/expected_sarsa.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/deep/expected_sarsa.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/e_greedy.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/e_greedy.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/exp3.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/exp3.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/lognormal_thompson_sampling.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/lognormal_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/normal_thompson_sampling.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/normal_thompson_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             alpha: Scalar,
             beta: Scalar,
             lam: Scalar,
             mu: Scalar
     ) -> None:
         assert alpha > 0
         assert beta > 0
-        assert lam > 0
+        assert lam >= 0
 
         self.n_arms = n_arms
 
         self.init = jax.jit(partial(self.init, n_arms=self.n_arms, alpha=alpha, beta=beta, lam=lam, mu=mu))
         self.update = jax.jit(self.update)
         self.sample = jax.jit(self.sample)
```

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/softmax.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/softmax.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/thompson_sampling.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/thompson_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
     of successful and failed attempts. Higher values of the parameters decrease the entropy of the distribution while
     changing the ratio of the parameters shifts the expected value.
 
     Parameters
     ----------
     n_arms : int
         Number of bandit arms. :math:`N \in \mathbb{N}_{+}`.
-    decay : float, default=1.0
+    decay : float, default=0.0
         Decay rate. If equal to zero, smoothing is not applied. :math:`w \geq 0`.
 
     References
     ----------
     .. [7] Alexander Krotov, Anton Kiryanov and Evgeny Khorov. 2020. Rate Control With Spatial Reuse
        for Wi-Fi 6 Dense Deployments. IEEE Access. 8. 168898-168909.
     """
 
-    def __init__(self, n_arms: int, decay: Scalar = 1.0) -> None:
+    def __init__(self, n_arms: int, decay: Scalar = 0.0) -> None:
         assert decay >= 0
 
         self.n_arms = n_arms
 
         self.init = jax.jit(partial(self.init, n_arms=self.n_arms))
         self.update = jax.jit(partial(self.update, decay=decay))
         self.sample = jax.jit(self.sample)
@@ -97,16 +97,16 @@
         Returns
         -------
         ThompsonSamplingState
             Initial state of the Thompson sampling agent.
         """
 
         return ThompsonSamplingState(
-            alpha=jnp.zeros((n_arms,1)),
-            beta=jnp.zeros((n_arms,1))
+            alpha=jnp.zeros((n_arms, 1)),
+            beta=jnp.zeros((n_arms, 1))
         )
 
     @staticmethod
     def update(
             state: ThompsonSamplingState,
             key: PRNGKey,
             action: int,
```

### Comparing `reinforced-lib-1.1.0/reinforced_lib/agents/mab/ucb.py` & `reinforced_lib-1.1.1/reinforced_lib/agents/mab/ucb.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/exts/base_ext.py` & `reinforced_lib-1.1.1/reinforced_lib/exts/base_ext.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/exts/basic_mab.py` & `reinforced_lib-1.1.1/reinforced_lib/exts/basic_mab.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/exts/gymnasium.py` & `reinforced_lib-1.1.1/reinforced_lib/exts/gymnasium.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/exts/utils.py` & `reinforced_lib-1.1.1/reinforced_lib/exts/utils.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/base_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/base_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/csv_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/csv_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/logs_observer.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/logs_observer.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/plots_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/plots_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/stdout_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/tb_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/tb_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/logs/wandb_logger.py` & `reinforced_lib-1.1.1/reinforced_lib/logs/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/rlib.py` & `reinforced_lib-1.1.1/reinforced_lib/rlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     agent_params : dict, optional
         Parameters of the selected agent.
     ext_type : type, optional
         Type of the selected extension. Must inherit from the ``BaseExt`` class.
     ext_params : dict, optional
         Parameters of the selected extension.
     logger_types : type or list[type], optional
-        Types of the selected logging modules. Must inherit from the ``BaseLogger`` class.
+        Types of the selected loggers. Must inherit from the ``BaseLogger`` class.
     logger_sources : Source or list[Source], optional
         Sources to log.
     logger_params : dict, optional
         Parameters of the selected loggers.
     no_ext_mode : bool, default=False
         Pass observations directly to the agent (do not use the extensions).
     auto_checkpoint : int, optional
@@ -210,19 +210,19 @@
         to log. A source can be a name (e.g., "action") or tuple containing the name and the ``SourceType`` (e.g.,
         ``("action", SourceType.OBSERVATION)``). If the name itself is inconclusive (e.g., it occurs as a metric and
         as an observation), the behavior depends on the implementation of the logger.
 
         Parameters
         ----------
         logger_types : type or list[type]
-            Types of the selected logging modules.
+            Types of the selected loggers.
         logger_sources : Source or list[Source], optional
             Sources to log.
         logger_params : dict, optional
-            Parameters of the selected logging modules.
+            Parameters of the selected loggers.
         """
 
         if not self._init_loggers:
             raise ForbiddenLoggerSetError()
 
         self._logger_types = deepcopy(logger_types)
         self._logger_sources = deepcopy(logger_sources)
@@ -498,15 +498,15 @@
         path : str
             Path to the checkpoint file.
         agent_params : dict[str, any], optional
             Dictionary of altered agent parameters with their new values, by default None.
         ext_params : dict[str, any], optional
             Dictionary of altered extension parameters with their new values, by default None.
         logger_types : type or list[type], optional
-            Types of the selected logging modules. Must inherit from the ``BaseLogger`` class.
+            Types of the selected loggers. Must inherit from the ``BaseLogger`` class.
         logger_sources : Source or list[Source], optional
             Sources to log.
         logger_params : dict, optional
             Parameters of the selected loggers.
         """
 
         with lz4.frame.open(path, 'rb') as f:
```

### Comparing `reinforced-lib-1.1.0/reinforced_lib/utils/__init__.py` & `reinforced_lib-1.1.1/reinforced_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/utils/exceptions.py` & `reinforced_lib-1.1.1/reinforced_lib/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/utils/experience_replay.py` & `reinforced_lib-1.1.1/reinforced_lib/utils/experience_replay.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/utils/jax_utils.py` & `reinforced_lib-1.1.1/reinforced_lib/utils/jax_utils.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib/utils/particle_filter.py` & `reinforced_lib-1.1.1/reinforced_lib/utils/particle_filter.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/reinforced_lib.egg-info/PKG-INFO` & `reinforced_lib-1.1.1/reinforced_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reinforced-lib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Reinforcement learning library
 Author-email: Maksymilian Wojnar <mwojnar@agh.edu.pl>, Wojciech Ciężobka <wciezobka@agh.edu.pl>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -389,25 +389,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: chex~=0.1.85
+Requires-Dist: chex~=0.1.86
 Requires-Dist: cloudpickle~=3.0.0
-Requires-Dist: flax~=0.8.1
+Requires-Dist: flax~=0.8.2
 Requires-Dist: gymnasium~=0.29.1
-Requires-Dist: jax~=0.4.24
-Requires-Dist: jaxlib~=0.4.24
+Requires-Dist: jax~=0.4.26
+Requires-Dist: jaxlib~=0.4.26
 Requires-Dist: lz4~=4.3.3
-Requires-Dist: matplotlib~=3.8.2
-Requires-Dist: optax~=0.1.9
+Requires-Dist: matplotlib~=3.8.4
+Requires-Dist: optax~=0.2.2
 Requires-Dist: tensorboardX~=2.6.2.2
-Requires-Dist: wandb~=0.16.3
+Requires-Dist: wandb~=0.16.6
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0.0; extra == "docs"
 Provides-Extra: full
 Requires-Dist: joblib~=1.3.2; extra == "full"
 Requires-Dist: pygame~=2.5.2; extra == "full"
 Requires-Dist: seaborn~=0.13.2; extra == "full"
@@ -415,29 +415,30 @@
 
 # Reinforced-lib: Reinforcement learning library
 
 [![PyPI version][pypi-badge]][pypi]
 [![License: MPL 2.0][license-badge]][license]
 [![build and test][tests-badge]][github-actions]
 [![Documentation Status][rtd-badge]][documentation]
+[![DOI](https://img.shields.io/badge/DOI-10.1016/j.softx.2024.101706-blue.svg)](https://doi.org/10.1016/j.softx.2024.101706)
 
 [pypi-badge]: https://img.shields.io/pypi/v/reinforced-lib
 [pypi]: https://pypi.org/project/reinforced-lib/
 [license-badge]: https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg
 [license]: https://opensource.org/licenses/MPL-2.0
 [tests-badge]: https://github.com/m-wojnar/reinforced-lib/actions/workflows/python-package.yml/badge.svg
 [github-actions]: https://github.com/m-wojnar/reinforced-lib/actions
 [rtd-badge]: https://readthedocs.org/projects/reinforced-lib/badge/?version=latest
 [documentation]: https://reinforced-lib.readthedocs.io/en/latest/
 
-**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of RL solutions. It is open-source, 
-prioritizes ease of use, provides comprehensive documentation, and offers both deep reinforcement learning 
-(DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), it facilitates exporting 
-trained models to embedded devices, and makes it great for research and prototyping with RL algorithms. Access to JAX's 
-just-in-time (JIT) compilation ensures high-performance results.
+**Introducing Reinforced-lib:** a lightweight Python library for the rapid development of reinforcement-learning (RL) 
+solutions. It is open-source, prioritizes ease of use, provides comprehensive documentation, and offers both deep 
+reinforcement learning (DRL) and classic non-neural agents. Built on [JAX](https://jax.readthedocs.io/en/latest/), 
+it facilitates exporting trained models to embedded devices, and makes it great for research and prototyping with RL 
+algorithms. Access to JAX's just-in-time (JIT) compilation ensures high-performance results.
 
 ## Installation
 
 You can install the latest version of Reinforced-lib from PyPI:
 
 ```bash
 pip install reinforced-lib
@@ -452,47 +453,50 @@
 pip install .
 ```
 
 In the spirit of making Reinforced-lib a lightweight solution, we include only the necessary dependencies in the base 
 requirements. To fully benefit from Reinforced-lib's conveniences, such as TF Lite export, install with the "full" suffix:
 
 ```bash
-pip3 install ".[full]"
+pip install ".[full]"
 ```
 
 ## Key components
 
 Reinforced-lib facilitates seamless interaction between RL agents and the environment. Here are the key components 
 within of the library, represented in the API as different modules.
 
 - **RLib** - The core module which provides a simple and intuitive interface to manage agents, use extensions, 
-  and configure the logging system. Even if you're not a reinforcement learning (RL) expert, *RLib* makes it easy to 
-  implement the agent-environment interaction loop.
+  and configure the logging system. Even if you're not an RL expert, *RLib* makes it easy to  implement the 
+  agent-environment interaction loop.
 
 - **Agents** - Choose from a variety of RL agents available in the *Agents* module. These agents are designed to be 
   versatile and work with any environment. If needed, you can even create your own agents using our documented recipes.
 
 - **Extensions** - Enhance agent observations with domain-specific knowledge by adding a suitable extension from the 
   *Extensions* module. This module enables seamless agent switching and parameter tuning without extensive reconfiguration.
 
-- **Logging** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
+- **Loggers** - This module allows you to monitor agent-environment interactions. Customize and adapt logging to your 
   specific needs, capturing training metrics, internal agent state, or environment observations. The library includes 
   various loggers for creating plots and output files, simplifying visualization and data processing.
 
 The figure below provides a visual representation of Reinforced-lib and the data-flow between its modules.
 
 <img src="docs/resources/data-flow.png" width="600">
 
 ## JAX Backend
 
 Our library is built on top of JAX, a high-performance numerical computing library. JAX makes it easy to implement 
-RL algorithms efficiently. It provides powerful transformations, including JIT compilation,  automatic differentiation, 
+RL algorithms efficiently. It provides powerful transformations, including JIT compilation, automatic differentiation, 
 vectorization, and parallelization. Our library is fully compatible with DeepMind's JAX ecosystem, granting access to 
 state-of-the-art RL models and helper libraries. JIT compilation significantly accelerates execution and ensures 
-portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications.
+portability across different architectures (CPUs, GPUs, TPUs) without requiring code modifications. 
+JAX offers another benefit through its robust pseudorandom number generator system, employed in our library to 
+guarantee result reproducibility. This critical aspect of scientific research is frequently underestimated but 
+remains highly significant.
 
 ## Edge Device Export
 
 Reinforced-lib is designed to work seamlessly on wireless, low-powered devices, where resources are limited. It's the 
 perfect solution for energy-constrained environments that may struggle with other ML frameworks. You can export your 
 trained models to [TensorFlow Lite](https://www.tensorflow.org/lite) with ease, reducing runtime overhead and 
 optimizing performance. This means you can deploy RL agents on resource-limited devices efficiently.
@@ -544,17 +548,22 @@
             env_state = env.step(action.item())
             action = rl.sample(*env_state)
             terminal = env_state[2] or env_state[3]
 ```
 
 ## Citing Reinforced-lib
 
-To cite this repository:
+To cite this repository, please use the following BibTeX entry for the Reinforced-lib paper:
 
-```
-@software{reinforcedlib2022,
-  author = {Maksymilian Wojnar and Wojciech Ciężobka},
-  title = {{R}einforced-lib: {R}einforcement learning library},
-  url = {http://github.com/m-wojnar/reinforced-lib},
-  year = {2022},
+```bibtex
+@article{reinforcedlib2022,
+  author = {Maksymilian Wojnar and Szymon Szott and Krzysztof Rusek and Wojciech Ciezobka},
+  title = {{R}einforced-lib: {R}apid prototyping of reinforcement learning solutions},
+  journal = {SoftwareX},
+  volume = {26},
+  pages = {101706},
+  year = {2024},
+  issn = {2352-7110},
+  doi = {https://doi.org/10.1016/j.softx.2024.101706},
+  url = {https://www.sciencedirect.com/science/article/pii/S2352711024000773}
 }
 ```
```

### Comparing `reinforced-lib-1.1.0/reinforced_lib.egg-info/SOURCES.txt` & `reinforced_lib-1.1.1/reinforced_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/test/test_rlib.py` & `reinforced_lib-1.1.1/test/test_rlib.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/test/test_rlib_serialization.py` & `reinforced_lib-1.1.1/test/test_rlib_serialization.py`

 * *Files identical despite different names*

### Comparing `reinforced-lib-1.1.0/test/test_rlib_to_tflite.py` & `reinforced_lib-1.1.1/test/test_rlib_to_tflite.py`

 * *Files identical despite different names*

