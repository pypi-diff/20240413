# Comparing `tmp/syllogistic-0.0.44.tar.gz` & `tmp/syllogistic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syllogistic-0.0.44.tar", last modified: Tue Apr  9 01:19:46 2024, max compression
+gzip compressed data, was "syllogistic-0.1.1.tar", last modified: Sat Apr 13 06:39:00 2024, max compression
```

## Comparing `syllogistic-0.0.44.tar` & `syllogistic-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 01:19:46.991561 syllogistic-0.0.44/
--rw-rw-rw-   0        0        0      244 2024-04-07 00:34:25.000000 syllogistic-0.0.44/LICENSE
--rw-rw-rw-   0        0        0     1625 2024-04-09 01:19:46.991561 syllogistic-0.0.44/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-07 05:50:31.000000 syllogistic-0.0.44/README
--rw-rw-rw-   0        0        0     1164 2024-04-09 01:16:23.000000 syllogistic-0.0.44/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 01:19:46.991561 syllogistic-0.0.44/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 01:19:46.977559 syllogistic-0.0.44/syllogistic/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:32:08.000000 syllogistic-0.0.44/syllogistic/__init__.py
--rw-rw-rw-   0        0        0       45 2024-04-07 00:44:25.000000 syllogistic-0.0.44/syllogistic/__main__.py
--rw-rw-rw-   0        0        0     1422 2024-04-07 04:42:08.000000 syllogistic-0.0.44/syllogistic/main.py
--rw-rw-rw-   0        0        0     9829 2024-04-09 01:15:58.000000 syllogistic-0.0.44/syllogistic/processor.py
--rw-rw-rw-   0        0        0     3647 2024-04-08 21:43:32.000000 syllogistic-0.0.44/syllogistic/watcher.py
-drwxrwxrwx   0        0        0        0 2024-04-09 01:19:46.990558 syllogistic-0.0.44/syllogistic.egg-info/
--rw-rw-rw-   0        0        0     1625 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 01:19:46.000000 syllogistic-0.0.44/syllogistic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 01:19:46.989558 syllogistic-0.0.44/tests/
--rw-rw-rw-   0        0        0     6806 2024-04-09 01:15:07.000000 syllogistic-0.0.44/tests/test_include.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:39:00.875358 syllogistic-0.1.1/
+-rw-rw-rw-   0        0        0      244 2024-04-07 00:34:25.000000 syllogistic-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1899 2024-04-13 06:39:00.874358 syllogistic-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-04-09 17:32:59.000000 syllogistic-0.1.1/README
+-rw-rw-rw-   0        0        0     1163 2024-04-13 05:36:24.000000 syllogistic-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 06:39:00.875358 syllogistic-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 06:39:00.853358 syllogistic-0.1.1/syllogistic/
+-rw-rw-rw-   0        0        0        0 2024-04-07 00:32:08.000000 syllogistic-0.1.1/syllogistic/__init__.py
+-rw-rw-rw-   0        0        0       45 2024-04-07 00:44:25.000000 syllogistic-0.1.1/syllogistic/__main__.py
+-rw-rw-rw-   0        0        0     1582 2024-04-10 05:21:06.000000 syllogistic-0.1.1/syllogistic/main.py
+-rw-rw-rw-   0        0        0    20039 2024-04-13 05:36:03.000000 syllogistic-0.1.1/syllogistic/processor.py
+-rw-rw-rw-   0        0        0     3800 2024-04-10 05:21:35.000000 syllogistic-0.1.1/syllogistic/watcher.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:39:00.873360 syllogistic-0.1.1/syllogistic.egg-info/
+-rw-rw-rw-   0        0        0     1899 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-13 06:39:00.000000 syllogistic-0.1.1/syllogistic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 06:39:00.873360 syllogistic-0.1.1/tests/
+-rw-rw-rw-   0        0        0     6926 2024-04-12 17:30:03.000000 syllogistic-0.1.1/tests/test_include.py
+-rw-rw-rw-   0        0        0    10034 2024-04-13 05:34:57.000000 syllogistic-0.1.1/tests/test_require.py
```

### Comparing `syllogistic-0.0.44/PKG-INFO` & `syllogistic-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syllogistic
-Version: 0.0.44
+Version: 0.1.1
 Summary: A simple Lua build system for the TIC-80.
 Author-email: Alastair McBain <mcbain.asm+syllogistic@gmail.com>
 License: Copyright 2024, Alastair McBain
         
         Usage of the works is permitted provided that this instrument is retained with the works, so that any entity that uses the works is notified of this instrument.
         
         DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY.
@@ -26,19 +26,31 @@
 Requires-Dist: pytest~=8.1.1; extra == "dev"
 
 SyllogisTIC
 
 A simple Lua build system for the TIC-80. It supports includes, exports (kinda),
 and modifying named feature inclusion on import, all via magic comments.
 
+Install:
+
+    pip install syllogistic
+
 Usage:
 
     syllogistic yourfile.lua.tic
 
 
 Support for other languages might be added later if there's enough
 demand.
 
 Out of Scope:
 
 - Proper imports (see the docs for why)
 - Preprocessor logic like #define, macros, #ifdef, but open to reconsideration
+
+
+---
+
+💜 to pestis/vsariola for pakettic and the TIC-80 file format parser.
+
+Need something that behaves more like the built-in `require()` syntax? Try
+[RiFT's TIC-80 Bundler](https://github.com/RiftTeam/tic-80-bundler).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syllogistic-0.0.44/pyproject.toml` & `syllogistic-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "syllogistic"
-version = "0.0.44"
+version = "0.1.1"
 description = "A simple Lua build system for the TIC-80."
 authors = [
     { name="Alastair McBain", email="mcbain.asm+syllogistic@gmail.com" }
 ]
 readme = { file="README", content-type="text/plain" }
 license = { file="LICENSE", content-type="text/plain" }
 keywords = ["TIC-80", "Fantasy Console", "Build", "Build System", "LUA"]
```

### Comparing `syllogistic-0.0.44/syllogistic/main.py` & `syllogistic-0.1.1/syllogistic/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import os
 import sys
 
+from enum import StrEnum
 from importlib import metadata
 from syllogistic.watcher import BuildWatcher
 
 
 # test.lua.tic -> test, .lua.tic
 def splitext2(path):
   filename, ext = os.path.splitext(path)
@@ -26,21 +27,22 @@
     prog='syllogistic',
     description=f'Build system for TIC-80 fantasy computer carts. v{version}'
   )
   argparser.add_argument('input', nargs='+', help='input file')
   argparser.add_argument('-o', '--out', default=os.getcwd(), metavar='str', help='output file or directory')
   argparser.add_argument('-s', '--strict', action='store_const', const=True, help='enable strict checking')
   argparser.add_argument('-w', '--watch', action='store_const', const=True, help='watch for file changes')
+  argparser.add_argument('-vv', '--verbose', action='store_const', const=True, help='verbose output (where relevant)')
 
   args = argparser.parse_args()
   file = args.input[0]
   filename = splitext2(args.input[0])
   outfile = os.path.join(args.out, filename[0] + '.build' + filename[1]) if os.path.isdir(args.out) else args.out
 
-  watcher = BuildWatcher(version, file, outfile, args.strict)
+  watcher = BuildWatcher(version, file, outfile, args.strict, args.verbose)
  
   if args.watch:
     watcher.start()
   else:
     watcher.build()
     print('')
```

### Comparing `syllogistic-0.0.44/syllogistic/watcher.py` & `syllogistic-0.1.1/syllogistic/watcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from syllogistic.processor import ProcessorContext, ProcessorException, process_lines
 
 class BuildWatcher(FileSystemEventHandler):
   files = set()
   dirs = set()
   watches = dict()
 
-  def __init__(self, version, file, outfile, strict):
+  def __init__(self, version, file, outfile, strict, default_require_resolution, verbose):
     self.version = version
     self.file = os.path.abspath(file)
     self.outfile = outfile
     self.strict = strict
+    self.default_require_resolution = default_require_resolution
+    self.verbose = verbose
     self.observer = Observer()
     self.last_src = None
     self.last_time = time()
 
   def _build(self):
     dirs = set()
     context = self.build(True)
@@ -53,15 +55,15 @@
       beginmsg = f'\r[{strftime("%H:%M")}] File updated, building...'
       print(beginmsg, end='')
 
       cart = ticfile.join_code(ticfile.read(self.file))
 
       for chunk in [chunk for chunk in cart if chunk[1] == ticfile.ChunkID.CODE]:
         code = cart[chunk].decode('ascii')
-        context = ProcessorContext(self.file, code.split('\n'), strict=self.strict, watched=True);
+        context = ProcessorContext(self.file, code.split('\n'), strict=self.strict, watched=True, verbose=self.verbose);
         result = process_lines(context)
         result = f'-- builder: SyllogisTIC v{self.version}\n-- built: {datetime.now()}Z\n' + result
         cart[chunk] = result.encode('ascii')
         ticfile.write(cart, self.outfile)
 
       end = (time() - start) * 1000
       end = math.floor(end) / 1000 if end > 1000 else str(math.floor(end)) + 'm'
```

### Comparing `syllogistic-0.0.44/syllogistic.egg-info/PKG-INFO` & `syllogistic-0.1.1/syllogistic.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syllogistic
-Version: 0.0.44
+Version: 0.1.1
 Summary: A simple Lua build system for the TIC-80.
 Author-email: Alastair McBain <mcbain.asm+syllogistic@gmail.com>
 License: Copyright 2024, Alastair McBain
         
         Usage of the works is permitted provided that this instrument is retained with the works, so that any entity that uses the works is notified of this instrument.
         
         DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY.
@@ -26,19 +26,31 @@
 Requires-Dist: pytest~=8.1.1; extra == "dev"
 
 SyllogisTIC
 
 A simple Lua build system for the TIC-80. It supports includes, exports (kinda),
 and modifying named feature inclusion on import, all via magic comments.
 
+Install:
+
+    pip install syllogistic
+
 Usage:
 
     syllogistic yourfile.lua.tic
 
 
 Support for other languages might be added later if there's enough
 demand.
 
 Out of Scope:
 
 - Proper imports (see the docs for why)
 - Preprocessor logic like #define, macros, #ifdef, but open to reconsideration
+
+
+---
+
+💜 to pestis/vsariola for pakettic and the TIC-80 file format parser.
+
+Need something that behaves more like the built-in `require()` syntax? Try
+[RiFT's TIC-80 Bundler](https://github.com/RiftTeam/tic-80-bundler).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syllogistic-0.0.44/tests/test_include.py` & `syllogistic-0.1.1/tests/test_include.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pytest
 import unittest
 
-from syllogistic.processor import ProcessorContext, ProcessorException, process_lines
+from syllogistic.processor import ProcessorContext, ProcessorException, ModuleNotFoundProcessorException, InvalidSyntaxProcessorException, process_lines
 
 
 class TestInclude(unittest.TestCase):
     def test_include(self):
       code = "-- #include './sample.lua'"
       context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
       result = process_lines(context)
@@ -225,35 +225,35 @@
     def test_include_no_win_absolute(self):
       with pytest.raises(ProcessorException):
         code = "-- #include 'C:\\tests\\input\\sample.lua'"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
 
     def test_include_malformed_include(self):
-      with pytest.raises(ProcessorException):
+      with pytest.raises(InvalidSyntaxProcessorException):
         code = "-- #include ./sample.lua"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
 
     def test_include_disallowed_prefix(self):
       with pytest.raises(ProcessorException):
         code = "-- #include '~sample.lua'"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
 
     def test_include_malformed_as(self):
-      with pytest.raises(ProcessorException):
+      with pytest.raises(InvalidSyntaxProcessorException):
         code = "-- #include './sample.lua' as"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
 
     def test_include_unknown_package(self):
-      with pytest.raises(ProcessorException):
+      with pytest.raises(ModuleNotFoundProcessorException):
         code = "-- #include 'thisisnotavalidpackagenameandlikelywontexist'"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
 
     def test_include_malformed_groups(self):
-      with pytest.raises(ProcessorException):
+      with pytest.raises(InvalidSyntaxProcessorException):
         code = "-- #include ./groups-bad.lua"
         context = ProcessorContext('tests/input/fake.lua', code.split('\n'), strict=True);
         result = process_lines(context)
```

