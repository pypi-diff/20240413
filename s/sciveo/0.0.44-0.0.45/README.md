# Comparing `tmp/sciveo-0.0.44.tar.gz` & `tmp/sciveo-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.44.tar", last modified: Wed Apr 10 19:57:00 2024, max compression
+gzip compressed data, was "sciveo-0.0.45.tar", last modified: Sat Apr 13 06:54:38 2024, max compression
```

## Comparing `sciveo-0.0.44.tar` & `sciveo-0.0.45.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.638592 sciveo-0.0.44/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 19:57:00.638370 sciveo-0.0.44/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5712 2024-03-17 11:37:08.000000 sciveo-0.0.44/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.616259 sciveo-0.0.44/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1360 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.629045 sciveo-0.0.44/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.44/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.44/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.630873 sciveo-0.0.44/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.44/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.44/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.633405 sciveo-0.0.44/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.44/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2023-12-12 14:35:14.000000 sciveo-0.0.44/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.44/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1552 2024-04-08 15:42:14.000000 sciveo-0.0.44/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.44/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.44/sciveo/common/tools/synchronized.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.635310 sciveo-0.0.44/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.44/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.44/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.44/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.635895 sciveo-0.0.44/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.44/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3650 2024-04-10 19:31:28.000000 sciveo-0.0.44/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-10 19:29:12.000000 sciveo-0.0.44/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.627963 sciveo-0.0.44/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5825 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      879 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-10 19:57:00.000000 sciveo-0.0.44/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-10 19:57:00.638719 sciveo-0.0.44/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.44/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-10 19:57:00.637551 sciveo-0.0.44/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.44/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.44/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.44/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.44/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.931099 sciveo-0.0.45/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-13 06:54:38.930920 sciveo-0.0.45/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.45/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.902453 sciveo-0.0.45/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1297 2024-04-13 06:50:59.000000 sciveo-0.0.45/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.913643 sciveo-0.0.45/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.45/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.45/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.916382 sciveo-0.0.45/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.45/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.45/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.920070 sciveo-0.0.45/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.45/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1416 2024-04-13 06:51:43.000000 sciveo-0.0.45/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.45/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1552 2024-04-08 15:42:14.000000 sciveo-0.0.45/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.45/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1102 2023-12-10 07:08:19.000000 sciveo-0.0.45/sciveo/common/tools/synchronized.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.926544 sciveo-0.0.45/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.45/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.45/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.45/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.928869 sciveo-0.0.45/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.45/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3684 2024-04-13 06:01:12.000000 sciveo-0.0.45/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1440 2024-04-13 06:48:20.000000 sciveo-0.0.45/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-13 05:14:12.000000 sciveo-0.0.45/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.912673 sciveo-0.0.45/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6168 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      906 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       50 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-13 06:54:38.000000 sciveo-0.0.45/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-13 06:54:38.931153 sciveo-0.0.45/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      418 2024-04-07 18:52:23.000000 sciveo-0.0.45/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-13 06:54:38.930564 sciveo-0.0.45/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.45/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.45/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.45/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.45/test/test_sampling.py
```

### Comparing `sciveo-0.0.44/PKG-INFO` & `sciveo-0.0.45/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-Metadata-Version: 2.1
-Name: sciveo
-Version: 0.0.44
-Description-Content-Type: text/markdown
-Provides-Extra: mon
-
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+
+
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
 
 ## Installation
 
+ - main sciveo
 pip install sciveo
 
+ - optional for sciveo monitoring
+pip install sciveo[mon]
+
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 
+When using sciveo monitoring just run, using suitable python environment
+python -c "import sciveo; sciveo.monitor(period=120)"
+
+When using sciveo experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
 
@@ -135,8 +140,8 @@
 
 
 
 
 ### Who do I talk to? ###
 
 * Pavlin Georgiev
-* pavlin@softel.bg
+* pavlin@softel.bg
```

### Comparing `sciveo-0.0.44/README.md` & `sciveo-0.0.45/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,50 @@
+Metadata-Version: 2.1
+Name: sciveo
+Version: 0.0.45
+Description-Content-Type: text/markdown
+Provides-Extra: mon
+
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+
+
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
 
 ## Installation
 
+ - main sciveo
 pip install sciveo
 
+ - optional for sciveo monitoring
+pip install sciveo[mon]
+
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 
+When using sciveo monitoring just run, using suitable python environment
+python -c "import sciveo; sciveo.monitor(period=120)"
+
+When using sciveo experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
 
@@ -129,8 +146,8 @@
 
 
 
 
 ### Who do I talk to? ###
 
 * Pavlin Georgiev
-* pavlin@softel.bg
+* pavlin@softel.bg
```

### Comparing `sciveo-0.0.44/sciveo/__init__.py` & `sciveo-0.0.45/sciveo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,39 +16,36 @@
   import os
   import time
 
   from sciveo.common.tools.logger import *
   from sciveo.common.tools.daemon import TasksDaemon, __upload_content__
   from sciveo.content.runner import ProjectRunner
   from sciveo.content.dataset import Dataset
-  from sciveo.monitoring.monitor import BaseMonitor
+  from sciveo.monitoring.start import MonitorStart
   from sciveo.version import __version__
 
 
   TasksDaemon.current = TasksDaemon(num_threads=int(os.environ.get("SCIVEO_TASKS_NUM_THREADS", 1)))
-  TasksDaemon.current.start()
 
 
   # New Experiment
   def open():
     if ProjectRunner.current is not None:
       return ProjectRunner.current.project
     else:
       error("there is no started project")
 
   def start(project, function, configuration={}, **kwargs):
+    TasksDaemon.current.start()
     ProjectRunner.current = ProjectRunner(project=project, function=function, configuration=configuration, **kwargs)
     ProjectRunner.current.run()
 
   # Dataset info
   def dataset(info={}):
     return Dataset.get(info)
 
   # Monitoring start
-  def monitor(period=120):
-    mon = BaseMonitor(period=period)
-    mon.start()
-    while(True):
-      time.sleep(60)
+  def monitor(**kwargs):
+    MonitorStart(**kwargs)()
 
 except ImportError as e:
   pass
```

### Comparing `sciveo-0.0.44/sciveo/api/base.py` & `sciveo-0.0.45/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/api/upload.py` & `sciveo-0.0.45/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/configuration.py` & `sciveo-0.0.45/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/model.py` & `sciveo-0.0.45/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/optimizers.py` & `sciveo-0.0.45/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/sampling.py` & `sciveo-0.0.45/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/tools/daemon.py` & `sciveo-0.0.45/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/tools/formating.py` & `sciveo-0.0.45/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/tools/hardware.py` & `sciveo-0.0.45/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/tools/logger.py` & `sciveo-0.0.45/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/common/tools/synchronized.py` & `sciveo-0.0.45/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/content/dataset.py` & `sciveo-0.0.45/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/content/experiment.py` & `sciveo-0.0.45/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/content/project.py` & `sciveo-0.0.45/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/content/runner.py` & `sciveo-0.0.45/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/sciveo/monitoring/monitor.py` & `sciveo-0.0.45/sciveo/monitoring/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # Warmup the psutil cpu usage
     psutil.cpu_percent(interval=0.3, percpu=True)
     initial_cpu_usage = psutil.cpu_percent(interval=None, percpu=True)
     time.sleep(1)
 
     machine_serial = self.getserial()
 
-    debug(type(self).__name__, "init", machine_serial, "initial_cpu_usage", initial_cpu_usage)
+    debug(type(self).__name__, f"init monitor with period={period}", machine_serial, "initial_cpu_usage", initial_cpu_usage)
 
   def __call__(self):
     return self.data
 
   def loop(self):
     self.get_cpu_usage()
     self.get_memory()
@@ -83,15 +83,15 @@
     machine_serial = None
     try:
       machine_serial = f"{socket.gethostname()}-{uuid.getnode()}"
     except Exception:
       pass
     if machine_serial is None:
       try:
-        machine_serial = socket.gethostname()
+        machine_serial = f"UUID-{uuid.getnode()}"
       except Exception:
         pass
     if machine_serial is None:
       machine_serial = f"RND-{random_token(8)}"
     self.data["serial"] = machine_serial
     return machine_serial
```

### Comparing `sciveo-0.0.44/sciveo.egg-info/PKG-INFO` & `sciveo-0.0.45/sciveo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.44
+Version: 0.0.45
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 
 # SCIVEO - ML/Scientific Experiments Management Client
 
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+
+
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
 
 ## Installation
 
+ - main sciveo
 pip install sciveo
 
+ - optional for sciveo monitoring
+pip install sciveo[mon]
+
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
 
+When using sciveo monitoring just run, using suitable python environment
+python -c "import sciveo; sciveo.monitor(period=120)"
+
+When using sciveo experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
```

### Comparing `sciveo-0.0.44/sciveo.egg-info/SOURCES.txt` & `sciveo-0.0.45/sciveo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,12 @@
 sciveo/content/__init__.py
 sciveo/content/dataset.py
 sciveo/content/experiment.py
 sciveo/content/project.py
 sciveo/content/runner.py
 sciveo/monitoring/__init__.py
 sciveo/monitoring/monitor.py
+sciveo/monitoring/start.py
 test/test_configuration.py
 test/test_monitoring.py
 test/test_runner.py
 test/test_sampling.py
```

### Comparing `sciveo-0.0.44/test/test_configuration.py` & `sciveo-0.0.45/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/test/test_monitoring.py` & `sciveo-0.0.45/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/test/test_runner.py` & `sciveo-0.0.45/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.44/test/test_sampling.py` & `sciveo-0.0.45/test/test_sampling.py`

 * *Files identical despite different names*

