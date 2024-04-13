# Comparing `tmp/yt-queue-0.8.0.tar.gz` & `tmp/yt_queue-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-queue-0.8.0.tar", last modified: Sun Mar 17 08:37:02 2024, max compression
+gzip compressed data, was "yt_queue-0.9.1.tar", last modified: Sat Apr 13 17:57:22 2024, max compression
```

## Comparing `yt-queue-0.8.0.tar` & `yt_queue-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.130171 yt-queue-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-17 08:36:53.000000 yt-queue-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-17 08:37:02.130171 yt-queue-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-17 08:36:53.000000 yt-queue-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-17 08:36:53.000000 yt-queue-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-17 08:36:53.000000 yt-queue-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-17 08:36:53.000000 yt-queue-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 08:37:02.130171 yt-queue-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-17 08:36:53.000000 yt-queue-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.126171 yt-queue-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.126171 yt-queue-0.8.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/cli/test_cli_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/cli/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/cli/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_cli_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_compatability.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_time_is_stale.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_video_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-17 08:36:53.000000 yt-queue-0.8.0/tests/test_videos_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.126171 yt-queue-0.8.0/yt_queue/
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.126171 yt-queue-0.8.0/yt_queue/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/internal/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/internal/yt_dlp_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.130171 yt-queue-0.8.0/yt_queue/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/utils/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-17 08:36:53.000000 yt-queue-0.8.0/yt_queue/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 08:37:02.130171 yt-queue-0.8.0/yt_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-17 08:37:02.000000 yt-queue-0.8.0/yt_queue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.858437 yt_queue-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 17:57:13.000000 yt_queue-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-13 17:57:22.858437 yt_queue-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-13 17:57:13.000000 yt_queue-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-13 17:57:13.000000 yt_queue-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 17:57:13.000000 yt_queue-0.9.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 17:57:13.000000 yt_queue-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:57:22.858437 yt_queue-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 17:57:13.000000 yt_queue-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.854437 yt_queue-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.854437 yt_queue-0.9.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/cli/test_cli_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/cli/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/cli/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_cli_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_compatability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_time_is_stale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_video_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-13 17:57:13.000000 yt_queue-0.9.1/tests/test_videos_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.858437 yt_queue-0.9.1/yt_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.858437 yt_queue-0.9.1/yt_queue/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/internal/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/internal/yt_dlp_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.858437 yt_queue-0.9.1/yt_queue/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/utils/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 17:57:13.000000 yt_queue-0.9.1/yt_queue/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:57:22.858437 yt_queue-0.9.1/yt_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 17:57:22.000000 yt_queue-0.9.1/yt_queue.egg-info/top_level.txt
```

### Comparing `yt-queue-0.8.0/LICENSE` & `yt_queue-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/PKG-INFO` & `yt_queue-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-queue
-Version: 0.8.0
+Version: 0.9.1
 Summary: CLI to keep track of videos in Youtube playlists
 Author-email: Hendri Pretorius <pretorh@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hendri Pretorius
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Keywords: yt-dlp,YouTube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yt-dlp==2024.03.10
+Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: pylint==3.0.2; extra == "dev"
 Requires-Dist: pytest==7.4.3; extra == "dev"
 
 # yt-queue
 CLI to keep track of videos in Youtube playlists
```

### Comparing `yt-queue-0.8.0/README.md` & `yt_queue-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/pyproject.toml` & `yt_queue-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/cli/test_cli_arguments.py` & `yt_queue-0.9.1/tests/cli/test_cli_arguments.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/cli/test_filter.py` & `yt_queue-0.9.1/tests/cli/test_filter.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/cli/test_refresh.py` & `yt_queue-0.9.1/tests/cli/test_refresh.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/mocks.py` & `yt_queue-0.9.1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_cli_functions.py` & `yt_queue-0.9.1/tests/test_cli_functions.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_compatability.py` & `yt_queue-0.9.1/tests/test_compatability.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_filters.py` & `yt_queue-0.9.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_refresh.py` & `yt_queue-0.9.1/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_time_is_stale.py` & `yt_queue-0.9.1/tests/test_time_is_stale.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_video_mapping.py` & `yt_queue-0.9.1/tests/test_video_mapping.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/tests/test_videos_list.py` & `yt_queue-0.9.1/tests/test_videos_list.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/__init__.py` & `yt_queue-0.9.1/yt_queue/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from . import file
 from .cli import argument_parser
 from .internal import mapper, yt_dlp_wrapper
 from .filters import filter_videos
 from .utils.loggers import StdLogger
 from .utils.time import is_stale
 
-VERSION = '0.8.0'
+VERSION = '0.9.1'
 _fullname = f"yt-queue {VERSION}"
 
 # utils
 
 def read(filename):
     return file.read(filename)
```

### Comparing `yt-queue-0.8.0/yt_queue/cli.py` & `yt_queue-0.9.1/yt_queue/cli.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/filters.py` & `yt_queue-0.9.1/yt_queue/filters.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/internal/mapper.py` & `yt_queue-0.9.1/yt_queue/internal/mapper.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/internal/yt_dlp_wrapper.py` & `yt_queue-0.9.1/yt_queue/internal/yt_dlp_wrapper.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/utils/loggers.py` & `yt_queue-0.9.1/yt_queue/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue/utils/time.py` & `yt_queue-0.9.1/yt_queue/utils/time.py`

 * *Files identical despite different names*

### Comparing `yt-queue-0.8.0/yt_queue.egg-info/PKG-INFO` & `yt_queue-0.9.1/yt_queue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-queue
-Version: 0.8.0
+Version: 0.9.1
 Summary: CLI to keep track of videos in Youtube playlists
 Author-email: Hendri Pretorius <pretorh@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hendri Pretorius
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,15 @@
 Keywords: yt-dlp,YouTube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yt-dlp==2024.03.10
+Requires-Dist: yt-dlp==2024.4.9
 Provides-Extra: dev
 Requires-Dist: pylint==3.0.2; extra == "dev"
 Requires-Dist: pytest==7.4.3; extra == "dev"
 
 # yt-queue
 CLI to keep track of videos in Youtube playlists
```

### Comparing `yt-queue-0.8.0/yt_queue.egg-info/SOURCES.txt` & `yt_queue-0.9.1/yt_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

