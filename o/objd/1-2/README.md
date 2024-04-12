# Comparing `tmp/objd-1.tar.gz` & `tmp/objd-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objd-1.tar", last modified: Fri Apr 12 14:50:42 2024, max compression
+gzip compressed data, was "objd-2.tar", last modified: Fri Apr 12 22:46:09 2024, max compression
```

## Comparing `objd-1.tar` & `objd-2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:50:42.492107 objd-1/
--rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 14:50:42.492107 objd-1/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3192 2024-04-12 14:50:21.000000 objd-1/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:50:42.492107 objd-1/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1000)     4014 2024-04-12 14:30:42.000000 objd-1/bin/objd
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:50:42.492107 objd-1/objd/
--rw-r--r--   0 bart      (1000) bart      (1000)      768 2024-04-12 14:31:22.000000 objd-1/objd/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1414 2024-04-12 14:26:34.000000 objd-1/objd/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)      206 2024-04-12 14:26:34.000000 objd-1/objd/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      377 2024-04-12 14:26:34.000000 objd-1/objd/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      388 2024-04-12 14:26:34.000000 objd-1/objd/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      746 2024-04-12 14:26:34.000000 objd-1/objd/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17463 2024-04-12 14:26:34.000000 objd-1/objd/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      681 2024-04-12 14:26:34.000000 objd-1/objd/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)      235 2024-04-12 14:26:34.000000 objd-1/objd/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-12 14:26:34.000000 objd-1/objd/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9730 2024-04-12 14:26:34.000000 objd-1/objd/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1090 2024-04-12 14:26:34.000000 objd-1/objd/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1030 2024-04-12 14:26:34.000000 objd-1/objd/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4980 2024-04-12 14:26:34.000000 objd-1/objd/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-12 14:26:34.000000 objd-1/objd/utils.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:50:42.492107 objd-1/objd.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      395 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       10 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:50:42.000000 objd-1/objd.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      773 2024-04-12 14:27:33.000000 objd-1/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 14:50:42.492107 objd-1/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-12 14:25:38.000000 objd-1/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 22:46:09.371814 objd-2/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3192 2024-04-12 22:29:33.000000 objd-2/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.367814 objd-2/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4014 2024-04-12 14:30:42.000000 objd-2/bin/objd
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/objd/
+-rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-04-12 15:45:57.000000 objd-2/objd/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1414 2024-04-12 14:26:34.000000 objd-2/objd/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      206 2024-04-12 14:26:34.000000 objd-2/objd/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      377 2024-04-12 14:26:34.000000 objd-2/objd/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      388 2024-04-12 14:26:34.000000 objd-2/objd/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      746 2024-04-12 14:26:34.000000 objd-2/objd/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17463 2024-04-12 21:59:34.000000 objd-2/objd/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      681 2024-04-12 14:26:34.000000 objd-2/objd/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      235 2024-04-12 14:26:34.000000 objd-2/objd/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-12 14:26:34.000000 objd-2/objd/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     9730 2024-04-12 14:26:34.000000 objd-2/objd/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1090 2024-04-12 14:26:34.000000 objd-2/objd/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1030 2024-04-12 14:26:34.000000 objd-2/objd/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4980 2024-04-12 14:26:34.000000 objd-2/objd/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1235 2024-04-12 14:26:34.000000 objd-2/objd/utils.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 22:46:09.371814 objd-2/objd.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3715 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      395 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       10 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 22:46:09.000000 objd-2/objd.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      775 2024-04-12 15:36:27.000000 objd-2/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 22:46:09.371814 objd-2/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-12 14:25:38.000000 objd-2/setup.py
```

### Comparing `objd-1/PKG-INFO` & `objd-2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: objd
-Version: 1
-Summary: objects daemon
-Author-email: xobjects <objx@proton.me>
+Version: 2
+Summary: object daemon
+Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objd
 Project-URL: bugs, https://github.com/xobjectz/objd/issues
 Project-URL: source, https://github.com/xobjectz/objd
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
@@ -153,15 +153,15 @@
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.objd
-    ExecStart=/home/<user>/.local/pipx/venvs/zbot/bin/objd
+    ExecStart=/home/<user>/.local/pipx/venvs/objd/bin/objd
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `objd-1/README.rst` & `objd-2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.objd
-    ExecStart=/home/<user>/.local/pipx/venvs/zbot/bin/objd
+    ExecStart=/home/<user>/.local/pipx/venvs/objd/bin/objd
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `objd-1/bin/objd` & `objd-2/bin/objd`

 * *Files identical despite different names*

### Comparing `objd-1/objd/broker.py` & `objd-2/objd/broker.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/fnd.py` & `objd-2/objd/fnd.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/irc.py` & `objd-2/objd/irc.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from objx import Default, Object, edit, fmt, keys, last, sync, whitelist
 from objr import Client, Command, Event, command, later, launch
 
 
 from .broker import broker
 
 
-NAME       = __file__.split(os.sep)[-3]
+NAME       = __file__.split(os.sep)[-2]
 filterlist = ["PING", "PONG", "PRIVMSG"]
 saylock    = _thread.allocate_lock()
 
 
 myirc = None
```

### Comparing `objd-1/objd/log.py` & `objd-2/objd/log.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/req.py` & `objd-2/objd/req.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/rss.py` & `objd-2/objd/rss.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/tdo.py` & `objd-2/objd/tdo.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/thr.py` & `objd-2/objd/thr.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/tmr.py` & `objd-2/objd/tmr.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd/utils.py` & `objd-2/objd/utils.py`

 * *Files identical despite different names*

### Comparing `objd-1/objd.egg-info/PKG-INFO` & `objd-2/objd.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: objd
-Version: 1
-Summary: objects daemon
-Author-email: xobjects <objx@proton.me>
+Version: 2
+Summary: object daemon
+Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objd
 Project-URL: bugs, https://github.com/xobjectz/objd/issues
 Project-URL: source, https://github.com/xobjectz/objd
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
@@ -153,15 +153,15 @@
     After=network-online.target
 
     [Service]
     Type=simple
     User=<user>
     Group=<user>
     WorkingDirectory=/home/<user>/.objd
-    ExecStart=/home/<user>/.local/pipx/venvs/zbot/bin/objd
+    ExecStart=/home/<user>/.local/pipx/venvs/objd/bin/objd
     RemainAfterExit=yes
 
     [Install]
     WantedBy=default.target
 
     then run this
```

### Comparing `objd-1/pyproject.toml` & `objd-2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objd"
-description = "objects daemon"
-version = "1"
+description = "object daemon"
+version = "2"
 authors = [
-    {name = "xobjects",email = "objx@proton.me"},
+    {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 dependencies = [
     'objx',
     'objr'
 ]
@@ -34,8 +34,10 @@
 [tool.setuptools]
 script-files = [
     'bin/objd',
 ]
 packages = [
     "objd",
 ]
+
+
 zip-safe=true
```

