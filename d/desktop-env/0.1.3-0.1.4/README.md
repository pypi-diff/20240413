# Comparing `tmp/desktop_env-0.1.3.tar.gz` & `tmp/desktop_env-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop_env-0.1.3.tar", last modified: Sun Apr  7 09:07:54 2024, max compression
+gzip compressed data, was "desktop_env-0.1.4.tar", last modified: Sat Apr 13 15:41:57 2024, max compression
```

## Comparing `desktop_env-0.1.3.tar` & `desktop_env-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/
--rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     7626 2024-04-07 09:07:54.652974 desktop_env-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5745 2024-04-07 09:02:51.000000 desktop_env-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.621513 desktop_env-0.1.3/desktop_env/
--rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.3/desktop_env/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/controllers/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.3/desktop_env/controllers/__init__.py
--rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.3/desktop_env/controllers/python.py
--rw-rw-rw-   0        0        0    29803 2024-03-07 09:50:37.000000 desktop_env-0.1.3/desktop_env/controllers/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/envs/
--rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.3/desktop_env/envs/__init__.py
--rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.3/desktop_env/envs/actions.py
--rw-rw-rw-   0        0        0    15658 2024-03-21 14:27:50.000000 desktop_env-0.1.3/desktop_env/envs/desktop_env.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.637219 desktop_env-0.1.3/desktop_env/evaluators/
--rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.3/desktop_env/evaluators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.642458 desktop_env-0.1.3/desktop_env/evaluators/getters/
--rw-rw-rw-   0        0        0     1502 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/__init__.py
--rw-rw-rw-   0        0        0      539 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/calc.py
--rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/chrome.py
--rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/file.py
--rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/general.py
--rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/gimp.py
--rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/impress.py
--rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/info.py
--rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/misc.py
--rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/replay.py
--rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/vlc.py
--rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.3/desktop_env/evaluators/getters/vscode.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/desktop_env/evaluators/metrics/
--rw-rw-rw-   0        0        0     4081 2024-03-20 14:11:55.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/__init__.py
--rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/basic_os.py
--rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/chrome.py
--rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/docs.py
--rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/general.py
--rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/gimp.py
--rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/libreoffice.py
--rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/others.py
--rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/pdf.py
--rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/slides.py
--rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/table.py
--rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/thunderbird.py
--rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/utils.py
--rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/vlc.py
--rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.3/desktop_env/evaluators/metrics/vscode.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:07:54.652974 desktop_env-0.1.3/desktop_env.egg-info/
--rw-rw-rw-   0        0        0     7626 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1552 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      567 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 09:07:54.000000 desktop_env-0.1.3/desktop_env.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 09:07:54.652974 desktop_env-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2752 2024-04-07 09:04:50.000000 desktop_env-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.725081 desktop_env-0.1.4/
+-rw-rw-rw-   0        0        0    11358 2024-02-24 15:43:05.000000 desktop_env-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7626 2024-04-13 15:41:57.724022 desktop_env-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5745 2024-04-07 09:02:51.000000 desktop_env-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.692194 desktop_env-0.1.4/desktop_env/
+-rw-rw-rw-   0        0        0        2 2023-12-24 03:12:41.000000 desktop_env-0.1.4/desktop_env/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.706202 desktop_env-0.1.4/desktop_env/controllers/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.4/desktop_env/controllers/__init__.py
+-rw-rw-rw-   0        0        0    15393 2024-03-21 03:16:56.000000 desktop_env-0.1.4/desktop_env/controllers/python.py
+-rw-rw-rw-   0        0        0    29975 2024-04-13 14:40:47.000000 desktop_env-0.1.4/desktop_env/controllers/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.707250 desktop_env-0.1.4/desktop_env/envs/
+-rw-rw-rw-   0        0        0        0 2023-11-21 09:05:29.000000 desktop_env-0.1.4/desktop_env/envs/__init__.py
+-rw-rw-rw-   0        0        0     7377 2024-01-14 13:22:15.000000 desktop_env-0.1.4/desktop_env/envs/actions.py
+-rw-rw-rw-   0        0        0    14755 2024-04-13 14:40:47.000000 desktop_env-0.1.4/desktop_env/envs/desktop_env.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.708268 desktop_env-0.1.4/desktop_env/evaluators/
+-rw-rw-rw-   0        0        0      113 2023-12-24 05:57:07.000000 desktop_env-0.1.4/desktop_env/evaluators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.714828 desktop_env-0.1.4/desktop_env/evaluators/getters/
+-rw-rw-rw-   0        0        0     1504 2024-04-13 14:50:54.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/__init__.py
+-rw-rw-rw-   0        0        0      537 2024-04-13 14:50:54.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/calc.py
+-rw-rw-rw-   0        0        0    62483 2024-04-01 11:46:38.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/chrome.py
+-rw-rw-rw-   0        0        0     4746 2024-03-10 07:16:40.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/file.py
+-rw-rw-rw-   0        0        0     1269 2024-03-08 12:39:20.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/general.py
+-rw-rw-rw-   0        0        0     1144 2024-01-30 18:56:45.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/gimp.py
+-rw-rw-rw-   0        0        0     7156 2024-03-08 11:36:11.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/impress.py
+-rw-rw-rw-   0        0        0      660 2024-01-26 05:22:46.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/info.py
+-rw-rw-rw-   0        0        0     7985 2024-03-08 12:47:17.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/misc.py
+-rw-rw-rw-   0        0        0      729 2024-01-13 16:57:53.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/replay.py
+-rw-rw-rw-   0        0        0     3768 2024-01-30 07:42:11.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/vlc.py
+-rw-rw-rw-   0        0        0     1113 2024-01-30 07:42:11.000000 desktop_env-0.1.4/desktop_env/evaluators/getters/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.722968 desktop_env-0.1.4/desktop_env/evaluators/metrics/
+-rw-rw-rw-   0        0        0     4083 2024-04-13 14:50:54.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1877 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/basic_os.py
+-rw-rw-rw-   0        0        0    13473 2024-03-10 16:02:05.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/chrome.py
+-rw-rw-rw-   0        0        0    28929 2024-04-02 06:37:07.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/docs.py
+-rw-rw-rw-   0        0        0    17228 2024-04-01 06:53:32.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/general.py
+-rw-rw-rw-   0        0        0    20366 2024-03-19 10:44:27.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/gimp.py
+-rw-rw-rw-   0        0        0     1242 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/libreoffice.py
+-rw-rw-rw-   0        0        0     3316 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/others.py
+-rw-rw-rw-   0        0        0      832 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/pdf.py
+-rw-rw-rw-   0        0        0    22385 2024-03-21 14:05:41.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/slides.py
+-rw-rw-rw-   0        0        0    23931 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/table.py
+-rw-rw-rw-   0        0        0     6801 2024-03-14 04:54:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/thunderbird.py
+-rw-rw-rw-   0        0        0    29419 2024-03-08 12:47:17.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/utils.py
+-rw-rw-rw-   0        0        0    14582 2024-01-25 04:36:46.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/vlc.py
+-rw-rw-rw-   0        0        0     8034 2024-03-18 12:33:10.000000 desktop_env-0.1.4/desktop_env/evaluators/metrics/vscode.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:41:57.724022 desktop_env-0.1.4/desktop_env.egg-info/
+-rw-rw-rw-   0        0        0     7626 2024-04-13 15:41:57.000000 desktop_env-0.1.4/desktop_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1552 2024-04-13 15:41:57.000000 desktop_env-0.1.4/desktop_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:41:57.000000 desktop_env-0.1.4/desktop_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      567 2024-04-13 15:41:57.000000 desktop_env-0.1.4/desktop_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 15:41:57.000000 desktop_env-0.1.4/desktop_env.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:41:57.725081 desktop_env-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2752 2024-04-13 15:40:17.000000 desktop_env-0.1.4/setup.py
```

### Comparing `desktop_env-0.1.3/LICENSE` & `desktop_env-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/PKG-INFO` & `desktop_env-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.3
+Version: 0.1.4
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
 Author: Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.3 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.4 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
 Danyang Zhang, Toh Jing Hua, etc. Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: numpy~=1.24.3 Requires-Dist:
```

### Comparing `desktop_env-0.1.3/README.md` & `desktop_env-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/controllers/python.py` & `desktop_env-0.1.4/desktop_env/controllers/python.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/controllers/setup.py` & `desktop_env-0.1.4/desktop_env/controllers/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import json
 import logging
 import os
 import os.path
+import shutil
 import sqlite3
 import tempfile
 import time
 import traceback
 import uuid
 from datetime import datetime, timedelta
 from typing import Any, Union, Optional
 from typing import Dict, List
 
-import shutil
 import requests
 from playwright.sync_api import sync_playwright, TimeoutError
 from pydrive.auth import GoogleAuth
 from pydrive.drive import GoogleDrive, GoogleDriveFile, GoogleDriveFileList
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from desktop_env.controllers.python import PythonController
 from desktop_env.evaluators.metrics.utils import compare_urls
 
 logger = logging.getLogger("desktopenv.setup")
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 
+
 class SetupController:
     def __init__(self, vm_ip: str, cache_dir: str):
         self.vm_ip: str = vm_ip
         self.http_server: str = f"http://{vm_ip}:5000"
         self.http_server_setup_root: str = f"http://{vm_ip}:5000/setup"
         self.cache_dir: str = cache_dir
 
@@ -56,47 +57,14 @@
             # protocol
             setup_function: str = "_{:}_setup".format(config_type)
             assert hasattr(self, setup_function), f'Setup controller cannot find init function {setup_function}'
             getattr(self, setup_function)(**parameters)
 
             logger.info("SETUP: %s(%s)", setup_function, str(parameters))
 
-        # self._download_setup(config)
-        # self._change_wallpaper(config)
-        # self._tidy_desktop(config) todo: implement this
-        # self._open_setup(config)
-        # can add other setup steps
-
-    # ZDY_COMMENT: merged with launch
-    # def _command_setup(self, command: str):
-    # """
-    # Directly send a command into the virtual machine os for setting up.
-    # """
-    # payload = json.dumps({"command": command})
-    # headers = {
-    # 'Content-Type': 'application/json'
-    # }
-    # timeout = 5
-    # timout_whitelist = ["vlc"]
-    #
-    # try:
-    #
-    # response = requests.post(self.http_server + "/execute", headers=headers, data=payload, timeout=timeout)
-    # if response.status_code == 200:
-    # print("Command executed successfully:", response.text)
-    # else:
-    # print("Failed to execute command. Status code:", response.status_code)
-    # except requests.exceptions.Timeout as e:
-    # if command in timout_whitelist:
-    # print("Command executed successfully:", command)
-    # else:
-    # print("An error occurred while trying to execute the command:", e)
-    # except requests.exceptions.RequestException as e:
-    # print("An error occurred while trying to execute the command:", e)
-
     def _download_setup(self, files: List[Dict[str, str]]):
         """
         Args:
             files (List[Dict[str, str]]): files to download. lisf of dict like
               {
                 "url": str, the url to download
                 "path": str, the path on the VM to store the downloaded file
@@ -136,19 +104,14 @@
 
                     except requests.RequestException as e:
                         logger.error(
                             f"Failed to download {url} caused by {e}. Retrying... ({max_retries - i - 1} attempts left)")
                 if not downloaded:
                     raise requests.RequestException(f"Failed to download {url}. No retries left. Error: {e}")
 
-            # payload = json.dumps({"url": url, "path": path})
-            # headers = {
-            # 'Content-Type': 'application/json'
-            # }
-
             form = MultipartEncoder({
                 "file_path": path,
                 "file_data": (os.path.basename(path), open(cache_path, "rb"))
             })
             headers = {"Content-Type": form.content_type}
             logger.debug(form.content_type)
 
@@ -159,14 +122,49 @@
                 if response.status_code == 200:
                     logger.info("Command executed successfully: %s", response.text)
                 else:
                     logger.error("Failed to upload file. Status code: %s", response.text)
             except requests.exceptions.RequestException as e:
                 logger.error("An error occurred while trying to send the request: %s", e)
 
+    def _upload_file_setup(self, files: List[Dict[str, str]]):
+        """
+        Args:
+            files (List[Dict[str, str]]): files to download. lisf of dict like
+              {
+                "local_path": str, the local path to the file to upload
+                "path": str, the path on the VM to store the downloaded file
+              }
+        """
+        for f in files:
+            local_path: str = f["local_path"]
+            path: str = f["path"]
+
+            if not os.path.exists(local_path):
+                logger.error(f"Setup Upload - Invalid local path ({local_path}).")
+                return
+
+            form = MultipartEncoder({
+                "file_path": path,
+                "file_data": (os.path.basename(path), open(local_path, "rb"))
+            })
+            headers = {"Content-Type": form.content_type}
+            logger.debug(form.content_type)
+
+            # send request to server to upload file
+            try:
+                logger.debug("REQUEST ADDRESS: %s", self.http_server + "/setup" + "/upload")
+                response = requests.post(self.http_server + "/setup" + "/upload", headers=headers, data=form)
+                if response.status_code == 200:
+                    logger.info("Command executed successfully: %s", response.text)
+                else:
+                    logger.error("Failed to upload file. Status code: %s", response.text)
+            except requests.exceptions.RequestException as e:
+                logger.error("An error occurred while trying to send the request: %s", e)
+
     def _change_wallpaper_setup(self, path: str):
         # if not config:
         # return
         # if not 'wallpaper' in config:
         # return
 
         # path = config['wallpaper']
@@ -555,15 +553,15 @@
 
             if platform == 'googledrive':
                 url = 'https://drive.google.com/drive/my-drive'
                 page = context.new_page()  # Create a new page (tab) within the existing context
                 try:
                     page.goto(url, timeout=60000)
                 except:
-                    logger.warning("Opening %s exceeds time limit", url) # only for human test
+                    logger.warning("Opening %s exceeds time limit", url)  # only for human test
                 logger.info(f"Opened new page: {url}")
                 settings = json.load(open(config['settings_file']))
                 email, password = settings['email'], settings['password']
 
                 try:
                     page.wait_for_selector('input[type="email"]', state="visible", timeout=3000)
                     page.fill('input[type="email"]', email)
```

### Comparing `desktop_env-0.1.3/desktop_env/envs/actions.py` & `desktop_env-0.1.4/desktop_env/envs/actions.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/envs/desktop_env.py` & `desktop_env-0.1.4/desktop_env/envs/desktop_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from __future__ import annotations
 
 import logging
 import os
 import subprocess
-import tempfile
 import time
 from typing import Callable, Any, Optional, Tuple
-# import uuid
-# import platform
 from typing import List, Dict, Union
 
 import gymnasium as gym
 
 from desktop_env.controllers.python import PythonController
 from desktop_env.controllers.setup import SetupController
-# from desktop_env.evaluators import eval_funcs
 from desktop_env.evaluators import metrics, getters
 
-# import requests
-
 logger = logging.getLogger("desktopenv.env")
 
 Metric = Callable[[Any, Any], float]
 Getter = Callable[[gym.Env, Dict[str, Any]], Any]
 
 
 def _execute_command(command: List[str]) -> None:
@@ -42,68 +36,68 @@
         if result.returncode != 0:
             raise Exception("\033[91m" + result.stdout + result.stderr + "\033[0m")
         return result.stdout
 
 
 class DesktopEnv(gym.Env):
     """
-    DesktopEnv with OpenAI Gym interface.
-    Fixme: refactor the logic when implementing the multi-process version
+    DesktopEnv with OpenAI Gym interface. It provides a desktop environment for setting and evaluating desktop automation tasks.
     """
 
     def __init__(
             self,
             path_to_vm: str,
             snapshot_name: str = "init_state",
             action_space: str = "computer_13",
-            tmp_dir: str = "tmp",
             cache_dir: str = "cache",
             screen_size: Tuple[int] = (1920, 1080),
             headless: bool = False,
             require_a11y_tree: bool = True,
+            require_terminal: bool = False,
     ):
         """
         Args:
             path_to_vm (str): path to .vmx file
+            snapshot_name (str): snapshot name to revert to, default to "init_state"
             action_space (str): "computer_13" | "pyautogui"
-            tmp_dir (str): temporary directory to store trajectory stuffs like
-              the extracted screenshots
             cache_dir (str): cache directory to cache task-related stuffs like
               reference file for evaluation
+            screen_size (Tuple[int]): screen size of the VM
+            headless (bool): whether to run the VM in headless mode
+            require_a11y_tree (bool): whether to require accessibility tree
+            require_terminal (bool): whether to require terminal output
         """
 
         # Initialize environment variables
         self.path_to_vm = os.path.abspath(os.path.expandvars(os.path.expanduser(path_to_vm)))
         self.snapshot_name = snapshot_name
-        self.tmp_dir_base: str = tmp_dir
         self.cache_dir_base: str = cache_dir
         self.vm_screen_size = screen_size  # todo: add the logic to get the screen size from the VM
         self.headless = headless
         self.require_a11y_tree = require_a11y_tree
-
-        os.makedirs(self.tmp_dir_base, exist_ok=True)
+        self.require_terminal = require_terminal
 
         # Initialize emulator and controller
         logger.info("Initializing...")
         self._start_emulator()
         self.vm_ip = self._get_vm_ip()
         self.controller = PythonController(vm_ip=self.vm_ip)
         self.setup_controller = SetupController(vm_ip=self.vm_ip, cache_dir=self.cache_dir_base)
 
-        # Meta info of the VM, move to the reset() function
-        self.vm_platform: str = ""  # self.controller.get_vm_platform()
+        # Meta info of the VM
+        self.vm_platform: str = self.controller.get_vm_platform()
+        self.vm_screen_size = self.controller.get_vm_screen_size()
 
         # mode: human or machine
+        self.instruction = None
         assert action_space in ["computer_13", "pyautogui"]
         self.action_space = action_space
-        # todo: define the action space and the observation space as gym did, or extend theirs
 
-        # episodic stuffs, like tmp dir and counters, will be updated or reset
+        # episodic stuffs, like counters, will be updated or reset
         # when calling self.reset()
-        self.tmp_dir: str = self.tmp_dir_base  # just an init value, updated during reset
         self._traj_no: int = -1
         self._step_no: int = 0
         self.action_history: List[Dict[str, any]] = []
 
     def _start_emulator(self):
         while True:
             try:
@@ -136,35 +130,35 @@
                 logger.info("Retrying...")
         raise Exception("Failed to get VM IP address!")
 
     def _save_state(self):
         _execute_command(["vmrun", "-T", "ws" "snapshot", self.path_to_vm, self.snapshot_name])
 
     def _get_screenshot(self):
-        # random_uuid = str(uuid.uuid4())
-        # os.makedirs(os.path.join("tmp", random_uuid), exist_ok=True)
-        # image_path = os.path.join("tmp", random_uuid, "screenshot.png")
-        image_path: str = os.path.join(self.tmp_dir, "screenshots", "{:d}.png".format(self._step_no))
-
+        screenshot = None
         # Get the screenshot and save to the image_path
         max_retries = 20
         for _ in range(max_retries):
             screenshot = self.controller.get_screenshot()
             if screenshot is not None:
                 break
             time.sleep(1)
 
-        with open(image_path, "wb") as f:
-            f.write(screenshot)
+        if screenshot is None:
+            logger.error("Failed to get screenshot!")
 
-        return image_path
+        return screenshot
 
     def _get_obs(self):
-        screenshot_image_path = self._get_screenshot()
-        return screenshot_image_path
+        return {
+            "screenshot": self._get_screenshot(),
+            "accessibility_tree": self.controller.get_accessibility_tree() if self.require_a11y_tree else None,
+            "terminal": self.controller.get_terminal_output() if self.require_terminal else None,
+            "instruction": self.instruction
+        }
 
     def _set_task_info(self, task_config: Dict[str, Any]):
         self.task_id: str = task_config["id"]
         self.cache_dir: str = os.path.join(self.cache_dir_base, self.task_id)
         os.makedirs(self.cache_dir, exist_ok=True)
         self.instruction = task_config["instruction"]
         self.config = task_config["config"] if "config" in task_config else []
@@ -178,25 +172,25 @@
         # if func is a str list, then result, expected (if exists), options (if exists) should also be lists of the same length
         # even if one of the metrics does not need expected or options field, it should be included in the list with None
         self.evaluator = task_config["evaluator"]
         self.metric: Metric = [getattr(metrics, func) for func in self.evaluator["func"]] \
             if isinstance(self.evaluator["func"], list) \
             else getattr(metrics, self.evaluator["func"])
         self.metric_conj: str = self.evaluator.get("conj", "and")  # take conjunction of multiple metrics
-        if "result" in self.evaluator and len(self.evaluator["result"])>0:
+        if "result" in self.evaluator and len(self.evaluator["result"]) > 0:
             self.result_getter: Getter = [getattr(getters, "get_{:}".format(res["type"])) for res in
                                           self.evaluator["result"]] \
                 if isinstance(self.evaluator["result"], list) \
                 else getattr(getters, "get_{:}".format(self.evaluator["result"]["type"]))
         else:
             self.result_getter = [None] * len(self.metric) \
                 if isinstance(self.metric, list) \
                 else None
 
-        if "expected" in self.evaluator and len(self.evaluator["expected"])>0:
+        if "expected" in self.evaluator and len(self.evaluator["expected"]) > 0:
             self.expected_getter: Getter = [getattr(getters, "get_{:}".format(exp["type"])) if exp else None for exp in
                                             self.evaluator["expected"]] \
                 if isinstance(self.evaluator["expected"], list) \
                 else getattr(getters, "get_{:}".format(self.evaluator["expected"]["type"]))
         else:
             self.expected_getter = [None] * len(self.metric) \
                 if isinstance(self.metric, list) \
@@ -223,45 +217,33 @@
             self.setup_controller.reset_cache_dir(self.cache_dir)
 
         logger.info("Setting counters...")
         self._traj_no += 1
         self._step_no = 0
         self.action_history.clear()
 
-        logger.info("Setup new temp dir...")
-        self.tmp_dir = tempfile.mkdtemp(
-            prefix="{:d}.{:}.".format(self._traj_no, self.task_id),
-            dir=self.tmp_dir_base
-        )
-        os.makedirs(os.path.join(self.tmp_dir, "screenshots"))
-
         logger.info("Reverting to snapshot to {}...".format(self.snapshot_name))
         _execute_command(["vmrun", "-T", "ws", "revertToSnapshot", self.path_to_vm, self.snapshot_name])
         time.sleep(5)
 
-        print(self.vm_screen_size)
         logger.info("Starting emulator...")
         self._start_emulator()
         logger.info("Emulator started.")
 
         logger.info("Get meta info of the VM...")
         self.vm_platform = self.controller.get_vm_platform()
         self.vm_screen_size = self.controller.get_vm_screen_size()
-        print(self.vm_screen_size)
 
         logger.info("Setting up environment...")
         self.setup_controller.setup(self.config)
 
         time.sleep(5)
         logger.info("Environment setup complete.")
 
-        observation = {
-            "screenshot": self._get_obs(),
-            "accessibility_tree": self.controller.get_accessibility_tree() if self.require_a11y_tree else None,
-        }
+        observation = self._get_obs()
         return observation
 
     def step(self, action, pause=0.5):
         self._step_no += 1
         self.action_history.append(action)
 
         reward = 0  # todo: Define reward calculation for each example
@@ -275,31 +257,25 @@
             elif action == 'FAIL':
                 done = True
                 info = {"fail": True}
             elif action == 'DONE':
                 done = True
                 info = {"done": True}
 
-        # fixme: add reminding logic here, decide if the action is valid for the current action_space
         if self.action_space == "computer_13":
             # the set of all possible actions defined in the action representation
             self.controller.execute_action(action)
         elif self.action_space == "pyautogui":
             if action in ['WAIT', 'FAIL', 'DONE']:
                 self.controller.execute_action(action)
             else:
                 # the set of all possible python commands insides `pyautogui`
                 self.controller.execute_python_command(action)
 
-        observation = {
-            "screenshot": self._get_obs(),
-            "accessibility_tree": self.controller.get_accessibility_tree() if self.require_a11y_tree else None,
-            # "terminal": self.controller.get_terminal_output(),
-            "instruction": self.instruction
-        }
+        observation = self._get_obs()
 
         return observation, reward, done, info
 
     def evaluate(self):
         """
         Evaluate whether the task is successfully completed.
         """
@@ -354,13 +330,13 @@
                                         **self.metric_options) if expected_state is not None \
                 else self.metric(result_state, **self.metric_options)
 
         return metric
 
     def render(self, mode='rgb_array'):
         if mode == 'rgb_array':
-            return self._get_obs()
+            return self._get_screenshot()
         else:
             raise ValueError('Unsupported render mode: {}'.format(mode))
 
     def close(self):
         _execute_command(["vmrun", "stop", self.path_to_vm])
```

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/__init__.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 from .gimp import get_gimp_config_file
 from .impress import get_audio_in_slide, get_background_image_in_slide
 from .info import get_vm_screen_size, get_vm_window_size, get_vm_wallpaper, get_list_directory
 from .misc import get_rule, get_accessibility_tree, get_rule_relativeTime, get_time_diff_range
 from .replay import get_replay
 from .vlc import get_vlc_playing_info, get_vlc_config, get_default_video_player
 from .vscode import get_vscode_config
-from .calc import get_conference_city_in_order
+from .calc import get_conference_city_in_order
```

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/calc.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
 
+
 # I want to write a function, reads a csv file, and get all the contents in the third column in the order of rows
 def get_conference_city_in_order(env, config):
     # read the csv file
     csv_path = config['csv_path']
     print(f"Reading csv file from {csv_path}")
     with open(csv_path, 'r') as f:
         reader = csv.reader(f)
     # skip the header row
     next(reader)
     # get the third column in the order of rows
     conference_city_list = [row[2] for row in reader]
     return conference_city_list
-
```

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/chrome.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/file.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/file.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/general.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/gimp.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/impress.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/impress.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/info.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/info.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/misc.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/misc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/replay.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/replay.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/vlc.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/getters/vscode.py` & `desktop_env-0.1.4/desktop_env/evaluators/getters/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/__init__.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     decrease_brightness,
     check_file_exists,
     compare_triangle_positions,
     check_sharper,
     check_image_file_size
 )
 from .libreoffice import check_libre_locale
+from .others import compare_epub, check_mp3_meta
 from .pdf import check_pdf_pages
 from .slides import (
     check_presenter_console_disable,
     check_image_stretch_and_center,
     check_slide_numbers_color,
     compare_pptx_files,
     check_strikethrough,
@@ -146,11 +147,11 @@
     check_json_settings,
     check_json_keybindings,
     check_python_file_by_test_suite,
     check_python_file_by_gold_file,
     check_html_background_image,
     compare_zip_files
 )
-from .others import compare_epub, check_mp3_meta
+
 
 def infeasible():
     pass
```

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/basic_os.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/basic_os.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/chrome.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/chrome.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/docs.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/docs.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/general.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/general.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/gimp.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/gimp.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/libreoffice.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/libreoffice.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/others.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/others.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/pdf.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/pdf.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/slides.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/slides.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/table.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/table.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/thunderbird.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/thunderbird.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/utils.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/vlc.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/vlc.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env/evaluators/metrics/vscode.py` & `desktop_env-0.1.4/desktop_env/evaluators/metrics/vscode.py`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env.egg-info/PKG-INFO` & `desktop_env-0.1.4/desktop_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop_env
-Version: 0.1.3
+Version: 0.1.4
 Summary: The package provides a desktop environment for setting and evaluating desktop automation tasks.
 Home-page: https://github.com/xlang-ai/desktop_env
 Author: Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.
 Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: desktop_env Version: 0.1.3 Summary: The package
+Metadata-Version: 2.1 Name: desktop_env Version: 0.1.4 Summary: The package
 provides a desktop environment for setting and evaluating desktop automation
 tasks. Home-page: https://github.com/xlang-ai/desktop_env Author: Tianbao Xie,
 Danyang Zhang, Toh Jing Hua, etc. Author-email: tianbaoxiexxx@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: numpy~=1.24.3 Requires-Dist:
```

### Comparing `desktop_env-0.1.3/desktop_env.egg-info/SOURCES.txt` & `desktop_env-0.1.4/desktop_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/desktop_env.egg-info/requires.txt` & `desktop_env-0.1.4/desktop_env.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `desktop_env-0.1.3/setup.py` & `desktop_env-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         except subprocess.CalledProcessError as e:
             print("Failed to run 'playwright install'. Please run 'playwright install' manually.")
             print(e)
 
 
 setup(
     name="desktop_env",
-    version="0.1.3",
+    version="0.1.4",
     author="Tianbao Xie, Danyang Zhang, Toh Jing Hua, etc.",
     author_email="tianbaoxiexxx@gmail.com",
     description="The package provides a desktop environment for setting and evaluating desktop automation tasks.",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/xlang-ai/desktop_env",
     packages=find_packages(),
```

