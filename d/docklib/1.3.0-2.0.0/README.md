# Comparing `tmp/docklib-1.3.0.tar.gz` & `tmp/docklib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docklib-1.3.0.tar", last modified: Tue Jun  1 04:55:21 2021, max compression
+gzip compressed data, was "docklib-2.0.0.tar", last modified: Sat Apr 13 18:30:11 2024, max compression
```

## Comparing `docklib-1.3.0.tar` & `docklib-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 elliotj    (501) staff       (20)        0 2021-06-01 04:55:21.651068 docklib-1.3.0/
--rw-r--r--   0 elliotj    (501) staff       (20)      530 2020-12-03 06:36:55.000000 docklib-1.3.0/LICENSE.md
--rw-r--r--   0 elliotj    (501) staff       (20)     6835 2021-06-01 04:55:21.650830 docklib-1.3.0/PKG-INFO
--rw-r--r--   0 elliotj    (501) staff       (20)     6027 2021-06-01 04:53:55.000000 docklib-1.3.0/README.md
-drwxr-xr-x   0 elliotj    (501) staff       (20)        0 2021-06-01 04:55:21.648873 docklib-1.3.0/docklib/
--rwxr-xr-x   0 elliotj    (501) staff       (20)       46 2021-05-23 05:57:46.000000 docklib-1.3.0/docklib/__init__.py
--rwxr-xr-x   0 elliotj    (501) staff       (20)    12471 2021-05-31 00:08:37.000000 docklib-1.3.0/docklib/docklib.py
-drwxr-xr-x   0 elliotj    (501) staff       (20)        0 2021-06-01 04:55:21.650449 docklib-1.3.0/docklib.egg-info/
--rw-r--r--   0 elliotj    (501) staff       (20)     6835 2021-06-01 04:55:21.000000 docklib-1.3.0/docklib.egg-info/PKG-INFO
--rw-r--r--   0 elliotj    (501) staff       (20)      192 2021-06-01 04:55:21.000000 docklib-1.3.0/docklib.egg-info/SOURCES.txt
--rw-r--r--   0 elliotj    (501) staff       (20)        1 2021-06-01 04:55:21.000000 docklib-1.3.0/docklib.egg-info/dependency_links.txt
--rw-r--r--   0 elliotj    (501) staff       (20)        8 2021-06-01 04:55:21.000000 docklib-1.3.0/docklib.egg-info/top_level.txt
--rw-r--r--   0 elliotj    (501) staff       (20)       38 2021-06-01 04:55:21.651156 docklib-1.3.0/setup.cfg
--rw-r--r--   0 elliotj    (501) staff       (20)     1571 2020-12-03 06:36:55.000000 docklib-1.3.0/setup.py
+drwxr-xr-x   0 elliot     (501) staff       (20)        0 2024-04-13 18:30:11.320909 docklib-2.0.0/
+-rw-r--r--   0 elliot     (501) staff       (20)      530 2019-06-04 05:53:14.000000 docklib-2.0.0/LICENSE.md
+-rw-r--r--   0 elliot     (501) staff       (20)     8359 2024-04-13 18:30:11.320626 docklib-2.0.0/PKG-INFO
+-rw-r--r--   0 elliot     (501) staff       (20)     7571 2024-04-13 18:26:27.000000 docklib-2.0.0/README.md
+drwxr-xr-x   0 elliot     (501) staff       (20)        0 2024-04-13 18:30:11.319409 docklib-2.0.0/docklib/
+-rwxr-xr-x   0 elliot     (501) staff       (20)       46 2024-04-13 18:26:27.000000 docklib-2.0.0/docklib/__init__.py
+-rwxr-xr-x   0 elliot     (501) staff       (20)    11982 2024-04-13 18:26:27.000000 docklib-2.0.0/docklib/docklib.py
+drwxr-xr-x   0 elliot     (501) staff       (20)        0 2024-04-13 18:30:11.320358 docklib-2.0.0/docklib.egg-info/
+-rw-r--r--   0 elliot     (501) staff       (20)     8359 2024-04-13 18:30:11.000000 docklib-2.0.0/docklib.egg-info/PKG-INFO
+-rw-r--r--   0 elliot     (501) staff       (20)      192 2024-04-13 18:30:11.000000 docklib-2.0.0/docklib.egg-info/SOURCES.txt
+-rw-r--r--   0 elliot     (501) staff       (20)        1 2024-04-13 18:30:11.000000 docklib-2.0.0/docklib.egg-info/dependency_links.txt
+-rw-r--r--   0 elliot     (501) staff       (20)        8 2024-04-13 18:30:11.000000 docklib-2.0.0/docklib.egg-info/top_level.txt
+-rw-r--r--   0 elliot     (501) staff       (20)       38 2024-04-13 18:30:11.320978 docklib-2.0.0/setup.cfg
+-rwxr-xr-x   0 elliot     (501) staff       (20)     1571 2023-10-08 21:15:35.000000 docklib-2.0.0/setup.py
```

### Comparing `docklib-1.3.0/LICENSE.md` & `docklib-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `docklib-1.3.0/PKG-INFO` & `docklib-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: docklib
-Version: 1.3.0
-Summary: Python module intended to assist IT administrators with manipulation of the macOS Dock.
-Home-page: https://github.com/homebysix/docklib
-Author: Elliot Jordan
-Author-email: elliot@elliotjordan.com
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: MacOS X
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # docklib
 
 This is a Python module intended to assist IT administrators with manipulation of the macOS Dock.
 
 Originally created as a [Gist](https://gist.github.com/gregneagle/5c422d709c93615341a21009f800222e) by @gregneagle, this fork has been modified to include support for some additional Dock features, and has been packaged for multiple distribution options.
 
+## docklib or dockutil?
+
+The very capable [dockutil](https://github.com/kcrawford/dockutil) tool serves a similar function to docklib. Why would Mac admins choose one over the other?
+
+The primary benefit of **docklib** is that it allows the Dock to be manipulated in a "Pythonic" way. By parsing the Dock configuration into an object with attributes and data structures that can be modified using familiar functions like `.append()` and `.insert()`, docklib aims to make Python scripters feel at home.
+
+In contrast, **dockutil** behaves more like a shell command-line utility and is written in Swift. This makes dockutil a good choice if you don't have a 'management python' or you're more comfortable writing user setup scripts in bash or zsh. Dockutil also has an `--allhomes` argument that allows Dock configuration for all users to be modified at the same time. Docklib isn't designed for this, instead focusing on configuring the Dock for the user that is currently logged in (for example, via an [outset](https://github.com/macadmins/outset) `login-once` or `login-every` script). [Here's](https://appleshare.it/posts/use-dockutil-in-a-script/) a great article to get you started with dockutil, if that sounds like what you're after.
+
 ## Installation
 
 There are multiple methods of installing docklib, depending on how you plan to use it.
 
 ### Package installer
 
 You can use the included __build_pkg.sh__ script to build a macOS installer .pkg file. You can use this package to install docklib on your own Mac, or deploy the package using a tool like Jamf or Munki to install docklib on managed devices.
@@ -107,15 +94,15 @@
 
 ### Display the current orientation of the Dock
 
 ```python
 from docklib import Dock
 
 dock = Dock()
-print dock.orientation
+print(dock.orientation)
 ```
 
 ### Make the Dock display on the left, and enable autohide
 
 ```python
 from docklib import Dock
 
@@ -202,8 +189,13 @@
 dock = Dock()
 dock.items["persistent-apps"] = [
     dock.makeDockAppEntry(item) for item in tech_dock if os.path.exists(item)
 ]
 dock.save()
 ```
 
+## More information
+
+For more examples and tips for creating your docklib script, see my guides on:
 
+- [Writing Resilient Docklib Scripts](https://www.elliotjordan.com/posts/resilient-docklib/)
+- [Deploying and running docklib scripts using Outset](https://www.elliotjordan.com/posts/docklib-outset/)
```

### Comparing `docklib-1.3.0/docklib/docklib.py` & `docklib-2.0.0/docklib/docklib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-# -*- coding: utf-8 -*-
-
 # pylint: disable=C0103
 
 """Python module intended to assist IT administrators with manipulation of the macOS Dock.
 
 See project details on GitHub: https://github.com/homebysix/docklib
 """
 
 import os
 import subprocess
-from distutils.version import LooseVersion
-from platform import mac_ver
-
-try:
-    # Python 3
-    from urllib.parse import unquote, urlparse
-except ImportError:
-    # Python 2
-    from urllib import unquote
-
-    from urlparse import urlparse
-
+from urllib.parse import unquote, urlparse
 
 # pylint: disable=E0611
 from Foundation import (
     NSURL,
     CFPreferencesAppSynchronize,
     CFPreferencesCopyAppValue,
     CFPreferencesSetAppValue,
@@ -46,46 +33,41 @@
     _DOCK_PLIST = os.path.expanduser("~/Library/Preferences/com.apple.dock.plist")
     _DOCK_LAUNCHAGENT_ID = "com.apple.Dock.agent"
     _DOCK_LAUNCHAGENT_FILE = "/System/Library/LaunchAgents/com.apple.Dock.plist"
     # TODO: static-apps and static-others
     _SECTIONS = ["persistent-apps", "persistent-others"]
     _MUTABLE_KEYS = [
         "autohide",
-        "orientation",
-        "tilesize",
-        "largesize",
-        "orientation-immutable",
-        "position-immutable",
         "autohide-immutable",
+        "contents-immutable",
+        "dblclickbehavior",
+        "largesize",
+        "launchanim",
+        "launchanim-immutable",
         "magnification",
         "magnification-immutable",
         "magsize-immutable",
-        "show-progress-indicators",
-        "contents-immutable",
-        "size-immutable",
         "mineffect",
         "mineffect-immutable",
-        "size-immutable",
         "minimize-to-application",
         "minimize-to-application-immutable",
+        "orientation",
+        "orientation-immutable",
+        "position-immutable",
+        "tilesize",
         "show-process-indicators",
-        "launchanim",
-        "launchanim-immutable",
+        "show-progress-indicators",
+        "show-recents",
+        "show-recents-immutable",
+        "size-immutable",
+        "windowtabbing",
+        "AllowDockFixupOverride",
     ]
 
-    _IMMUTABLE_KEYS = ["mod-count", "trash-full"]
-    if LooseVersion(mac_ver()[0]) >= LooseVersion("10.12"):
-        _MUTABLE_KEYS.append("AllowDockFixupOverride")
-    if LooseVersion(mac_ver()[0]) >= LooseVersion("10.14"):
-        _MUTABLE_KEYS.append("show-recents")
-        _IMMUTABLE_KEYS.append("recent-apps")
-    if LooseVersion(mac_ver()[0]) >= LooseVersion("10.15"):
-        _MUTABLE_KEYS.extend(
-            ["dblclickbehavior", "show-recents-immutable", "windowtabbing"]
-        )
+    _IMMUTABLE_KEYS = ["mod-count", "recent-apps", "trash-full"]
 
     items = {}
 
     def __init__(self):
         for key in self._SECTIONS:
             try:
                 section = CFPreferencesCopyAppValue(key, self._DOMAIN)
@@ -103,28 +85,28 @@
         """Saves our (modified) Dock preferences."""
         # unload Dock launchd job so we can make our changes unmolested
         subprocess.call(["/bin/launchctl", "unload", self._DOCK_LAUNCHAGENT_FILE])
 
         for key in self._SECTIONS:
             try:
                 CFPreferencesSetAppValue(key, self.items[key], self._DOMAIN)
-            except Exception:
-                raise DockError
+            except Exception as exc:
+                raise DockError from exc
         for key in self._MUTABLE_KEYS:
             # Python doesn't support hyphens in attribute names, so convert
             # to/from underscores as needed.
             if getattr(self, key.replace("-", "_")) is not None:
                 try:
                     CFPreferencesSetAppValue(
                         key.replace("_", "-"),
                         getattr(self, key.replace("-", "_")),
                         self._DOMAIN,
                     )
-                except Exception:
-                    raise DockError
+                except Exception as exc:
+                    raise DockError from exc
         if not CFPreferencesAppSynchronize(self._DOMAIN):
             raise DockError
 
         # restart the Dock
         subprocess.call(["/bin/launchctl", "load", self._DOCK_LAUNCHAGENT_FILE])
         subprocess.call(["/bin/launchctl", "start", self._DOCK_LAUNCHAGENT_ID])
 
@@ -249,20 +231,20 @@
             match_str = os.path.splitext(os.path.basename(newpath))[0]
         found_index = self.findExistingEntry(
             match_str, match_on=match_on, section=section
         )
         if found_index > -1:
             self.items[section][found_index] = newitem
 
-    def makeDockAppSpacer(self, type="spacer-tile"):
+    def makeDockAppSpacer(self, tile_type="spacer-tile"):
         """Makes an empty space in the Dock."""
-        if type not in ["spacer-tile", "small-spacer-tile"]:
-            msg = "{0}: invalid makeDockAppSpacer type.".format(type)
+        if tile_type not in ["spacer-tile", "small-spacer-tile"]:
+            msg = f"{tile_type}: invalid makeDockAppSpacer type."
             raise ValueError(msg)
-        result = {"tile-data": {}, "tile-type": type}
+        result = {"tile-data": {}, "tile-type": tile_type}
 
         return result
 
     def makeDockAppEntry(self, thePath, label_name=None):
         """Returns a dictionary corresponding to a Dock application item."""
         if not label_name:
             label_name = os.path.splitext(os.path.basename(thePath))[0]
```

### Comparing `docklib-1.3.0/docklib.egg-info/PKG-INFO` & `docklib-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: docklib
-Version: 1.3.0
+Version: 2.0.0
 Summary: Python module intended to assist IT administrators with manipulation of the macOS Dock.
 Home-page: https://github.com/homebysix/docklib
 Author: Elliot Jordan
 Author-email: elliot@elliotjordan.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +20,22 @@
 
 # docklib
 
 This is a Python module intended to assist IT administrators with manipulation of the macOS Dock.
 
 Originally created as a [Gist](https://gist.github.com/gregneagle/5c422d709c93615341a21009f800222e) by @gregneagle, this fork has been modified to include support for some additional Dock features, and has been packaged for multiple distribution options.
 
+## docklib or dockutil?
+
+The very capable [dockutil](https://github.com/kcrawford/dockutil) tool serves a similar function to docklib. Why would Mac admins choose one over the other?
+
+The primary benefit of **docklib** is that it allows the Dock to be manipulated in a "Pythonic" way. By parsing the Dock configuration into an object with attributes and data structures that can be modified using familiar functions like `.append()` and `.insert()`, docklib aims to make Python scripters feel at home.
+
+In contrast, **dockutil** behaves more like a shell command-line utility and is written in Swift. This makes dockutil a good choice if you don't have a 'management python' or you're more comfortable writing user setup scripts in bash or zsh. Dockutil also has an `--allhomes` argument that allows Dock configuration for all users to be modified at the same time. Docklib isn't designed for this, instead focusing on configuring the Dock for the user that is currently logged in (for example, via an [outset](https://github.com/macadmins/outset) `login-once` or `login-every` script). [Here's](https://appleshare.it/posts/use-dockutil-in-a-script/) a great article to get you started with dockutil, if that sounds like what you're after.
+
 ## Installation
 
 There are multiple methods of installing docklib, depending on how you plan to use it.
 
 ### Package installer
 
 You can use the included __build_pkg.sh__ script to build a macOS installer .pkg file. You can use this package to install docklib on your own Mac, or deploy the package using a tool like Jamf or Munki to install docklib on managed devices.
@@ -107,15 +114,15 @@
 
 ### Display the current orientation of the Dock
 
 ```python
 from docklib import Dock
 
 dock = Dock()
-print dock.orientation
+print(dock.orientation)
 ```
 
 ### Make the Dock display on the left, and enable autohide
 
 ```python
 from docklib import Dock
 
@@ -202,8 +209,13 @@
 dock = Dock()
 dock.items["persistent-apps"] = [
     dock.makeDockAppEntry(item) for item in tech_dock if os.path.exists(item)
 ]
 dock.save()
 ```
 
+## More information
+
+For more examples and tips for creating your docklib script, see my guides on:
 
+- [Writing Resilient Docklib Scripts](https://www.elliotjordan.com/posts/resilient-docklib/)
+- [Deploying and running docklib scripts using Outset](https://www.elliotjordan.com/posts/docklib-outset/)
```

### Comparing `docklib-1.3.0/setup.py` & `docklib-2.0.0/setup.py`

 * *Files identical despite different names*

