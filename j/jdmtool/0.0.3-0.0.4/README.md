# Comparing `tmp/jdmtool-0.0.3.tar.gz` & `tmp/jdmtool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdmtool-0.0.3.tar", last modified: Sun Mar 24 07:08:02 2024, max compression
+gzip compressed data, was "/home/dima/src/jdmtool/dist/.tmp-6qbvcsxc/jdmtool-0.0.4.tar", last modified: Sat Apr 13 00:32:55 2024, max compression
```

## Comparing `jdmtool-0.0.3.tar` & `jdmtool-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-03-24 07:08:02.619440 jdmtool-0.0.3/
--rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.0.3/LICENSE
--rw-r--r--   0 dima      (1000) dima      (1000)     7099 2024-03-24 07:08:02.619440 jdmtool-0.0.3/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     6415 2023-04-14 02:01:35.000000 jdmtool-0.0.3/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)      825 2024-03-24 07:03:07.000000 jdmtool-0.0.3/pyproject.toml
--rw-r--r--   0 dima      (1000) dima      (1000)       38 2024-03-24 07:08:02.619440 jdmtool-0.0.3/setup.cfg
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-03-24 07:08:02.614440 jdmtool-0.0.3/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-03-24 07:08:02.616440 jdmtool-0.0.3/src/jdmtool/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.0.3/src/jdmtool/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     2780 2024-03-03 07:11:25.000000 jdmtool-0.0.3/src/jdmtool/chartview.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3700 2023-04-12 13:42:28.000000 jdmtool-0.0.3/src/jdmtool/device.py
--rw-r--r--   0 dima      (1000) dima      (1000)     8468 2024-03-24 06:58:42.000000 jdmtool-0.0.3/src/jdmtool/downloader.py
--rw-r--r--   0 dima      (1000) dima      (1000)    15242 2024-03-03 06:35:29.000000 jdmtool-0.0.3/src/jdmtool/main.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-03-24 07:08:02.618440 jdmtool-0.0.3/src/jdmtool.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)     7099 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)      361 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       81 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/entry_points.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       64 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2024-03-24 07:08:02.000000 jdmtool-0.0.3/src/jdmtool.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/
+-rw-r--r--   0 dima      (1000) dima      (1000)    11357 2023-03-28 17:09:03.000000 jdmtool-0.0.4/LICENSE
+-rw-r--r--   0 dima      (1000) dima      (1000)     6975 2024-04-13 00:32:55.000000 jdmtool-0.0.4/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     6415 2023-04-14 02:01:35.000000 jdmtool-0.0.4/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      825 2024-04-13 00:31:22.000000 jdmtool-0.0.4/pyproject.toml
+-rw-r--r--   0 dima      (1000) dima      (1000)       38 2024-04-13 00:32:55.000000 jdmtool-0.0.4/setup.cfg
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-03-28 16:55:30.000000 jdmtool-0.0.4/src/jdmtool/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     2780 2024-04-13 00:27:00.000000 jdmtool-0.0.4/src/jdmtool/chartview.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3700 2023-04-12 13:42:28.000000 jdmtool-0.0.4/src/jdmtool/device.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     8477 2024-04-13 00:29:55.000000 jdmtool-0.0.4/src/jdmtool/downloader.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    15242 2024-04-13 00:27:00.000000 jdmtool-0.0.4/src/jdmtool/main.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)     6975 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)      361 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       81 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/entry_points.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       64 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2024-04-13 00:32:55.000000 jdmtool-0.0.4/src/jdmtool.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `jdmtool-0.0.3/LICENSE` & `jdmtool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.3/PKG-INFO` & `jdmtool-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libusb1>=2.0.1
-Requires-Dist: platformdirs>=2.6.2
-Requires-Dist: requests>=2.26.0
-Requires-Dist: tqdm>=4.1.0
 
 # JdmTool
 
 A command-line tool for downloading Jeppesen databases and programming Garmin aviation data cards aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
 
 It requires:
 - Jeppesen subscription
```

### Comparing `jdmtool-0.0.3/README.md` & `jdmtool-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.3/pyproject.toml` & `jdmtool-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jdmtool"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Dima Ryazanov", email="dima@gmail.com" },
 ]
 description = "Tool for downloading Jeppesen databases and programming Garmin aviation data cards"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jdmtool-0.0.3/src/jdmtool/chartview.py` & `jdmtool-0.0.4/src/jdmtool/chartview.py`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.3/src/jdmtool/device.py` & `jdmtool-0.0.4/src/jdmtool/device.py`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.3/src/jdmtool/downloader.py` & `jdmtool-0.0.4/src/jdmtool/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def get_downloads_dir(cls) -> pathlib.Path:
         path = cls.get_data_dir() / 'downloads'
         path.mkdir(parents=True, exist_ok=True)
         return path
 
     @classmethod
     def get_cov_check(cls) -> T.Tuple[str, str]:
-        now = datetime.datetime.now(datetime.UTC)
+        now = datetime.datetime.now(datetime.timezone.utc)
         date_str = now.strftime('%a %b %d %H:%M:%S %Y')
         cov_check = hashlib.md5((date_str + cls.COV_CHECK_MAGIC).encode()).hexdigest()
         return date_str, cov_check
 
     @classmethod
     def get_common_headers_params(cls) -> T.Tuple[T.Dict[str, str], T.Dict[str, str]]:
         date_str, cov_check = cls.get_cov_check()
```

### Comparing `jdmtool-0.0.3/src/jdmtool/main.py` & `jdmtool-0.0.4/src/jdmtool/main.py`

 * *Files identical despite different names*

### Comparing `jdmtool-0.0.3/src/jdmtool.egg-info/PKG-INFO` & `jdmtool-0.0.4/src/jdmtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: jdmtool
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool for downloading Jeppesen databases and programming Garmin aviation data cards
 Author-email: Dima Ryazanov <dima@gmail.com>
 Project-URL: Homepage, https://github.com/dimaryaz/jdmtool
 Project-URL: Bug Tracker, https://github.com/dimaryaz/jdmtool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libusb1>=2.0.1
-Requires-Dist: platformdirs>=2.6.2
-Requires-Dist: requests>=2.26.0
-Requires-Dist: tqdm>=4.1.0
 
 # JdmTool
 
 A command-line tool for downloading Jeppesen databases and programming Garmin aviation data cards aiming to be compatible with [Jeppesen Distribution Manager](https://ww2.jeppesen.com/data-solutions/jeppesen-distribution-manager/).
 
 It requires:
 - Jeppesen subscription
```

