# Comparing `tmp/bakabakabaka-0.8.7.tar.gz` & `tmp/bakabakabaka-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.8.7.tar", last modified: Thu Apr 11 21:00:36 2024, max compression
+gzip compressed data, was "bakabakabaka-0.8.8.tar", last modified: Sat Apr 13 05:22:11 2024, max compression
```

## Comparing `bakabakabaka-0.8.7.tar` & `bakabakabaka-0.8.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:36.203654 bakabakabaka-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 21:00:26.000000 bakabakabaka-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-11 21:00:36.203654 bakabakabaka-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-11 21:00:26.000000 bakabakabaka-0.8.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    33146 2024-04-11 21:00:26.000000 bakabakabaka-0.8.7/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:36.203654 bakabakabaka-0.8.7/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-11 21:00:36.000000 bakabakabaka-0.8.7/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 21:00:36.000000 bakabakabaka-0.8.7/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:00:36.000000 bakabakabaka-0.8.7/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 21:00:36.000000 bakabakabaka-0.8.7/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 21:00:36.000000 bakabakabaka-0.8.7/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:00:36.203654 bakabakabaka-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 21:00:26.000000 bakabakabaka-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:22:11.683558 bakabakabaka-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-13 05:22:11.679558 bakabakabaka-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33225 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:22:11.679558 bakabakabaka-0.8.8/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 05:22:11.000000 bakabakabaka-0.8.8/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:22:11.683558 bakabakabaka-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-13 05:22:03.000000 bakabakabaka-0.8.8/setup.py
```

### Comparing `bakabakabaka-0.8.7/LICENSE` & `bakabakabaka-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.7/PKG-INFO` & `bakabakabaka-0.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.7
+Version: 0.8.8
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.7/README.md` & `bakabakabaka-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.7/baka.py` & `bakabakabaka-0.8.8/baka.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import smtplib
 import socket
 import subprocess
 import sys
 import time
 import typing
 
-__version__: typing.Final[str] = "0.8.7"
+__version__: typing.Final[str] = "0.8.8"
 BASE_PATH: typing.Final[str] = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=__version__)
@@ -454,28 +454,28 @@
         cmds = [
             ["git", "add", "--ignore-errors", "--all"],
             ["git", "commit", "-m", f"baka pre-file {config.hostname}"]
         ]
         current_os = "windows" if os.name == "nt" else "linux"
         not_current_os_abbrev = "l" if current_os == "windows" else "w"
         copy_command = ["cp", "-f"] if current_os == "linux" else ["copy", "/Y"]
-        os.path.makedirs(os.path.join(BASE_PATH, config.hostname), exist_ok=True)
+        os.makedirs(os.path.join(BASE_PATH, config.hostname), exist_ok=True)
         for file in file_list:
             assert len(config.files[file]) == 1
             file_key = list(config.files[file].keys())[0]
             if not_current_os_abbrev in file_key.split("_"):
                 continue
             if args.file[0] in ["save", "s"]:
                 if "src" in file_key.split("_"):
-                    cmds.append([*copy_command, config.files[file][file_key], os.path.join(BASE_PATH, config.hostname, file)])
-                elif "cmd" in config.files[file]:
-                    cmds.append(["BAKA_DEST", os.path.join(BASE_PATH, config.hostname, file), *config.files[file]["cmd"]])
+                    cmds.append([*copy_command, os.path.expandvars(os.path.expanduser(config.files[file][file_key])), os.path.join(BASE_PATH, config.hostname, file)])
+                elif "cmd" in file_key.split("_"):
+                    cmds.append(["BAKA_DEST", os.path.join(BASE_PATH, config.hostname, file), *config.files[file][file_key]])
             elif args.file[0] in ["restore", "r"]:
                 if "src" in file_key.split("_"):
-                    cmds.append([*copy_command, os.path.join(BASE_PATH, config.hostname, file), config.files[file][file_key]])
+                    cmds.append([*copy_command, os.path.join(BASE_PATH, config.hostname, file), os.path.expandvars(os.path.expanduser(config.files[file][file_key]))])
         cmds.append(["git", "add", "--ignore-errors", "--all"])
         cmds.append(["git", "commit", "-m", f"baka file {config.hostname}"])
     elif args.job:
         if args.interactive:
             config.jobs[args.job]["interactive"] = True
         cmds = config.jobs[args.job]["commands"]
     elif args.list:
```

### Comparing `bakabakabaka-0.8.7/bakabakabaka.egg-info/PKG-INFO` & `bakabakabaka-0.8.8/bakabakabaka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.7
+Version: 0.8.8
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.7/setup.py` & `bakabakabaka-0.8.8/setup.py`

 * *Files identical despite different names*

