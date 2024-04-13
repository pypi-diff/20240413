# Comparing `tmp/rclip-1.8.5.tar.gz` & `tmp/rclip-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.8.5.tar", max compression
+gzip compressed data, was "rclip-1.8.6.tar", max compression
```

## Comparing `rclip-1.8.5.tar` & `rclip-1.8.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-09 09:42:49.584924 rclip-1.8.5/LICENSE
--rw-r--r--   0        0        0     7269 2024-04-09 09:42:49.584924 rclip-1.8.5/README.md
--rw-r--r--   0        0        0     1747 2024-04-09 09:42:49.584924 rclip-1.8.5/pyproject.toml
--rw-r--r--   0        0        0      158 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/const.py
--rw-r--r--   0        0        0     3830 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/db.py
--rw-r--r--   0        0        0      993 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/fs.py
--rw-r--r--   0        0        0     7002 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/model.py
--rw-r--r--   0        0        0     7043 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1169 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-04-09 09:42:49.588924 rclip-1.8.5/rclip/utils/snap.py
--rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-13 15:03:08.622929 rclip-1.8.6/LICENSE
+-rw-r--r--   0        0        0     7269 2024-04-13 15:03:08.622929 rclip-1.8.6/README.md
+-rw-r--r--   0        0        0     1747 2024-04-13 15:03:08.622929 rclip-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/const.py
+-rw-r--r--   0        0        0     3830 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/fs.py
+-rw-r--r--   0        0        0     7002 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/model.py
+-rw-r--r--   0        0        0     7230 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1169 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-04-13 15:03:08.622929 rclip-1.8.6/rclip/utils/snap.py
+-rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.6/PKG-INFO
```

### Comparing `rclip-1.8.5/LICENSE` & `rclip-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/README.md` & `rclip-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/pyproject.toml` & `rclip-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.8.5"
+version = "1.8.6"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.8.5/rclip/db.py` & `rclip-1.8.6/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/rclip/fs.py` & `rclip-1.8.6/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/rclip/main.py` & `rclip-1.8.6/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/rclip/model.py` & `rclip-1.8.6/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/rclip/utils/helpers.py` & `rclip-1.8.6/rclip/utils/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from rclip.const import IS_LINUX, IS_MACOS, IS_WINDOWS
 
 
 MAX_DOWNLOAD_SIZE_BYTES = 50_000_000
 DOWNLOAD_TIMEOUT_SECONDS = 60
 WIN_ABSOLUTE_FILE_PATH_REGEX = re.compile(r'^[a-z]:\\', re.I)
+DEFAULT_TERMINAL_TEXT_WIDTH = 100
 
 
 def __get_system_datadir() -> pathlib.Path:
   '''
   Returns a parent directory path
   where persistent application data can be stored.
 
@@ -53,17 +54,20 @@
   if arg_int < 1:
     raise argparse.ArgumentTypeError('should be >0')
   return arg_int
 
 
 def get_terminal_text_width() -> int:
   try:
-    return min(100, os.get_terminal_size().columns - 2)
+    computed_width = min(DEFAULT_TERMINAL_TEXT_WIDTH, os.get_terminal_size().columns - 2)
+    if computed_width < 20:
+      return DEFAULT_TERMINAL_TEXT_WIDTH
+    return computed_width
   except OSError:
-    return 100
+    return DEFAULT_TERMINAL_TEXT_WIDTH
 
 
 class HelpFormatter(argparse.RawDescriptionHelpFormatter):
   def __init__(self, prog: str, indent_increment: int = 2, max_help_position: int = 24) -> None:
     text_width = get_terminal_text_width()
     super().__init__(prog, indent_increment, max_help_position, width=text_width)
```

### Comparing `rclip-1.8.5/rclip/utils/preview.py` & `rclip-1.8.6/rclip/utils/preview.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/rclip/utils/snap.py` & `rclip-1.8.6/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.5/PKG-INFO` & `rclip-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.8.5
+Version: 1.8.6
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.9,<3.13
```

