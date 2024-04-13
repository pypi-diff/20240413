# Comparing `tmp/ez_pyload-1.0.0.tar.gz` & `tmp/ez_pyload-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_pyload-1.0.0.tar", max compression
+gzip compressed data, was "ez_pyload-1.0.1.tar", max compression
```

## Comparing `ez_pyload-1.0.0.tar` & `ez_pyload-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      907 2024-03-21 01:13:49.381467 ez_pyload-1.0.0/README.md
--rw-r--r--   0        0        0       39 2024-03-21 01:13:49.381467 ez_pyload-1.0.0/ez_pyload/__init__.py
--rw-r--r--   0        0        0      613 2024-03-21 01:13:49.381467 ez_pyload-1.0.0/ez_pyload/__main__.py
--rw-r--r--   0        0        0     3111 2024-03-21 01:13:49.381467 ez_pyload-1.0.0/ez_pyload/download.py
--rw-r--r--   0        0        0      451 2024-03-21 01:13:49.381467 ez_pyload-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 ez_pyload-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1356 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/README.md
+-rw-r--r--   0        0        0       39 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/__main__.py
+-rw-r--r--   0        0        0     3128 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/download.py
+-rw-r--r--   0        0        0      451 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ez_pyload-1.0.1/PKG-INFO
```

### Comparing `ez_pyload-1.0.0/README.md` & `ez_pyload-1.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # ez-pyload
 
-Wrapper for [pyLoad](https://github.com/pyload/pyload) so it can be used in your Python projects without too much overhead (it won't start a webserver like pyLoad normally does).
+Wrapper for [pyLoad](https://github.com/pyload/pyload) so it can be used in your Python projects without starting a webserver like pyLoad normally does.
+
+## Why?
+I've been trying to find a library or CLI app which is able to download from many different filehosting sites for a long while now. The only free downloaders I have been able to find with support for many filehosting sites are jDownloader2 and pyLoad, neither of which seem to have a CLI interface or developer friendly API/documentation, and both of which seem to run a webserver just to be able to download some files. This library (hopefully) fixes this problem.
 
 ## Installation
 
 `$ python3 -m pip install ez-pyload`
 
 ## Using as a library
```

### Comparing `ez_pyload-1.0.0/ez_pyload/__main__.py` & `ez_pyload-1.0.1/ez_pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.0/ez_pyload/download.py` & `ez_pyload-1.0.1/ez_pyload/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import glob
 import logging
 import os
-from pathlib import Path
 import shutil
 import sys
+from pathlib import Path
 
 cwd = os.getcwd() # pyload messes with cwd
+
 from pyload.core import Core
-from pyload.core.log_factory import LogFactory
-from pyload.core.datatypes.enums import Destination
 from pyload.core.datatypes.pyfile import PyFile
-from pyload.core.datatypes.pypackage import PyPackage
+from pyload.core.log_factory import LogFactory
 from pyload.core.threads.download_thread import DownloadThread
+
 os.chdir(cwd)
 
 logger = logging.getLogger("pyload")
 consoleform = logging.Formatter(
     LogFactory.LINEFORMAT, LogFactory.DATEFORMAT, LogFactory.LINESTYLE
 )
 consolehdlr = logging.StreamHandler(sys.stdout)
@@ -23,20 +22,21 @@
 logger.addHandler(consolehdlr)
 def new_get_logger(self, name: str):
     return logger
 LogFactory.get_logger = new_get_logger
 
 import tempfile
 
+
 def _download(pyload: Core, url: str, pkg_name: str = "unknown", pkg_dir: str = "unknown") -> bool:
     urls = [url]
     data = pyload.plugin_manager.parse_urls(urls)
     url, plugin = data[0]
-    PyPackage(pyload.file_manager, 0, pkg_name, pkg_dir, None, None, Destination.QUEUE, None)
-    pyfile = PyFile(pyload.files, -1, url, url, 0, 0, "", plugin, 0, -1)
+    pkg_id = pyload.files.add_package(pkg_name, pkg_dir)
+    pyfile = PyFile(pyload.files, -1, url, url, 0, 0, "", plugin, pkg_id, -1)
     pyfile.init_plugin()
     if pyfile.plugin.__type__ == "downloader":
         thread = DownloadThread(pyload.thread_manager)
         pyload.addon_manager.download_preparing(pyfile)
         pyfile.plugin.preprocessing(thread)
         pyfile.release()
         return False
@@ -48,15 +48,17 @@
             pass
         pyfile.plugin._initialize()
         pyfile.plugin._setup()
         pyload.addon_manager.download_preparing(pyfile)
         pyfile.plugin.process(pyfile)
         for folder, urls, name in pyfile.plugin.packages:
             for url in urls:
-                _download(pyload, url, name, pkg_dir + "/" + folder)
+                _download(
+                    pyload, url, name, pkg_dir + os.sep + folder
+                )  # pyload uses os.sep instead of / so this is necessary
         return True
 
 def download(url: str, download_dir: str | Path, loglevel: int = logging.INFO) -> Path:
     """Download the file or folder at the given URL
 
     Args:
         url (str): URL to file or folder hosted on a supported site
@@ -66,21 +68,23 @@
 
     Returns:
         Path: Path to downloaded file/folder
     """
     download_dir = Path(download_dir)
     debug = loglevel == logging.DEBUG
     logger.setLevel(loglevel)
-    with tempfile.TemporaryDirectory(".ez-pyload") as tmp:
+    tmp = "."
+    with tempfile.TemporaryDirectory(".ez-pyload", ignore_cleanup_errors=True) as tmp:
         pyload = Core(tmp, "tmpdir", "storage", debug)
         is_dir = _download(pyload, url)
         src_path = next((Path(tmp) / "data" / "storage" / "unknown").glob("*"))
         name = src_path.name
         dst_path = download_dir / name
         # pyload messes with cwd again
         os.chdir(cwd)
         if is_dir:
             shutil.copytree(src_path, dst_path)
         else:
             shutil.copy(src_path, dst_path)
-        pyload.terminate()
-        return dst_path
+        pyload.stop()
+        pyload.db.shutdown()
+        return dst_path
```

### Comparing `ez_pyload-1.0.0/PKG-INFO` & `ez_pyload-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-pyload
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper for pyLoad to allow downloading files through Python (no webserver). Includes CLI
 License: MIT
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyload-ng (>=0.5.0b3.dev81,<0.6.0)
 Description-Content-Type: text/markdown
 
 # ez-pyload
 
-Wrapper for [pyLoad](https://github.com/pyload/pyload) so it can be used in your Python projects without too much overhead (it won't start a webserver like pyLoad normally does).
+Wrapper for [pyLoad](https://github.com/pyload/pyload) so it can be used in your Python projects without starting a webserver like pyLoad normally does.
+
+## Why?
+I've been trying to find a library or CLI app which is able to download from many different filehosting sites for a long while now. The only free downloaders I have been able to find with support for many filehosting sites are jDownloader2 and pyLoad, neither of which seem to have a CLI interface or developer friendly API/documentation, and both of which seem to run a webserver just to be able to download some files. This library (hopefully) fixes this problem.
 
 ## Installation
 
 `$ python3 -m pip install ez-pyload`
 
 ## Using as a library
```

