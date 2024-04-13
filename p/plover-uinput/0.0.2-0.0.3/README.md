# Comparing `tmp/plover-uinput-0.0.2.tar.gz` & `tmp/plover-uinput-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-uinput-0.0.2.tar", last modified: Fri Apr 12 13:11:29 2024, max compression
+gzip compressed data, was "plover-uinput-0.0.3.tar", last modified: Sat Apr 13 13:56:26 2024, max compression
```

## Comparing `plover-uinput-0.0.2.tar` & `plover-uinput-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-12 13:11:29.682291 plover-uinput-0.0.2/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-04-11 16:08:24.000000 plover-uinput-0.0.2/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-12 13:11:29.682291 plover-uinput-0.0.2/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-12 13:11:29.682291 plover-uinput-0.0.2/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9261 2024-04-12 13:11:03.000000 plover-uinput-0.0.2/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-04-09 10:35:53.000000 plover-uinput-0.0.2/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-04-09 10:31:51.000000 plover-uinput-0.0.2/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-04-11 13:38:12.000000 plover-uinput-0.0.2/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-12 13:11:29.682291 plover-uinput-0.0.2/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-04-12 13:11:29.000000 plover-uinput-0.0.2/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-04-11 16:18:33.000000 plover-uinput-0.0.2/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      625 2024-04-11 16:10:12.000000 plover-uinput-0.0.2/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-04-12 13:11:29.683291 plover-uinput-0.0.2/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-04-09 17:27:40.000000 plover-uinput-0.0.2/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-04-11 16:08:24.000000 plover-uinput-0.0.3/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.686653 plover-uinput-0.0.3/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9283 2024-04-13 13:54:59.000000 plover-uinput-0.0.3/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-04-09 10:35:53.000000 plover-uinput-0.0.3/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-04-09 10:31:51.000000 plover-uinput-0.0.3/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     2019 2024-04-11 13:38:12.000000 plover-uinput-0.0.3/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2090 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-04-13 13:56:26.000000 plover-uinput-0.0.3/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-04-11 16:18:33.000000 plover-uinput-0.0.3/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      625 2024-04-11 16:10:12.000000 plover-uinput-0.0.3/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      670 2024-04-13 13:56:26.687653 plover-uinput-0.0.3/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-04-09 17:27:40.000000 plover-uinput-0.0.3/setup.py
```

### Comparing `plover-uinput-0.0.2/LICENSE` & `plover-uinput-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.2/PKG-INFO` & `plover-uinput-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover-uinput-0.0.2/plover_uinput/__init__.py` & `plover-uinput-0.0.3/plover_uinput/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,16 @@
         self._press_key(modifiers["control_l"], True)
         self._press_key(modifiers["shift_l"], False)
         self._send_key(keys["u"])
         self._press_key(modifiers["control_l"], False)
         self._press_key(modifiers["shift_l"], False)
         self._ui.syn()
         self._send_string(hex)
-        self._press_key(keys["\n"])
+        self._send_key(keys["\n"])
+        self._ui.syn()
 
     def _send_char(self, char):
         # === Key can be sent with a key combination ===
         if char in self._symbols:
             (base, mods) = self._symbols[char]
             for mod in mods.split():
                 self._press_key(modifiers[mods], True)
```

### Comparing `plover-uinput-0.0.2/plover_uinput/keys.py` & `plover-uinput-0.0.3/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.2/plover_uinput/symbols.py` & `plover-uinput-0.0.3/plover_uinput/symbols.py`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.2/plover_uinput.egg-info/PKG-INFO` & `plover-uinput-0.0.3/plover_uinput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `plover-uinput-0.0.2/readme.md` & `plover-uinput-0.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `plover-uinput-0.0.2/setup.cfg` & `plover-uinput-0.0.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.2
+version = 0.0.3
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
```

