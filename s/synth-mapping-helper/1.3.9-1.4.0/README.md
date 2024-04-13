# Comparing `tmp/synth_mapping_helper-1.3.9.tar.gz` & `tmp/synth_mapping_helper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.3.9.tar", last modified: Wed Oct  4 19:52:10 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.4.0.tar", last modified: Sat Apr 13 14:19:41 2024, max compression
```

## Comparing `synth_mapping_helper-1.3.9.tar` & `synth_mapping_helper-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.658646 synth_mapping_helper-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-04 19:52:10.658646 synth_mapping_helper-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-04 19:52:10.658646 synth_mapping_helper-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.654646 synth_mapping_helper-1.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.654646 synth_mapping_helper-1.3.9/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28570 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28133 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.658646 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/autobackup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    30626 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12900 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (127)    20847 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.654646 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-04 19:52:10.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-04 19:52:10.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 19:52:10.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-04 19:52:10.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-04 19:52:10.000000 synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 19:52:10.658646 synth_mapping_helper-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-04 19:51:56.000000 synth_mapping_helper-1.3.9/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.225990 synth_mapping_helper-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.229990 synth_mapping_helper-1.4.0/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.229990 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/autobackup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35892 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/map_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/text_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34011 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/wall_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27884 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.3.9/LICENSE` & `synth_mapping_helper-1.4.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 adosikas
+Copyright (c) 2024 adosikas
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `synth_mapping_helper-1.3.9/README.md` & `synth_mapping_helper-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.3.9/setup.py` & `synth_mapping_helper-1.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import setuptools
+[build-system]
+requires = ["setuptools>=46.4.0", "wheel"]
+build-backend = "setuptools.build_meta"
 
-with open('README.md', 'r', encoding='utf-8') as fh:
-    long_description = fh.read()
+[project]
+name = "synth_mapping_helper"
+dependencies = [
+    "numpy>=1.26.4",
+    "scipy>=1.13.0",
+    "matplotlib>=3.8.4",
+    "plotly>=5.20.0",
+    "pyperclip>=1.8.2",
+    "watchdog>=4.0.0",
+    "requests>=2.31.0",
+    "nicegui>=1.4.20",
+    "pywin32>=306; sys_platform=='win32'",
+]
+requires-python = ">=3.10"
+authors = [{"name"="adosikas"}]
+description = "Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard"
+readme = "README.md"
+license = {"file"="LICENSE"}
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: End Users/Desktop",
 
-setuptools.setup(
-    name='synth_mapping_helper',
-    author='adosikas',
-    author_email='',
-    description='Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/adosikas/synth_mapping_helper',
-    project_urls={
-        'Documentation': 'https://github.com/adosikas/synth_mapping_helper',
-        'Bug Reports': 'https://github.com/adosikas/synth_mapping_helper',
-        'Source Code': 'https://github.com/adosikas/synth_mapping_helper',
-    },
-    package_dir={'': 'src'},
-    packages=setuptools.find_packages(where='src'),
-    classifiers=[
-        # see https://pypi.org/classifiers/
-        'Development Status :: 3 - Alpha',
-
-        'Intended Audience :: End Users/Desktop',
-        'Topic :: Artistic Software',
-        'Topic :: Games/Entertainment',
-
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.10',
-    install_requires=[
-        'numpy', 'scipy', 'matplotlib',
-        'pyperclip', 'watchdog',
-        'nicegui',
-        'pywin32;platform_system=="Windows"',
-    ],
-    extras_require={
-        'dev': ['check-manifest'],
-        # 'test': ['coverage'],
-    },
-    # entry_points={
-    #     'console_scripts': [  # This can provide executable scripts
-    #         'run=synth_mapping_helper:main',
-    # You can execute `run` in bash to run `main()` in src/synth_mapping_helper/__init__.py
-    #     ],
-    # },
-)
+    "Topic :: Artistic Software",
+    "Topic :: Games/Entertainment",
+
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "synth_mapping_helper.__version__"}
+
+
+[project.urls]
+Homepage = "https://github.com/adosikas/synth_mapping_helper"
+Documentation = "https://github.com/adosikas/synth_mapping_helper/wiki"
+Repository = "https://github.com/adosikas/synth_mapping_helper"
+"Bug Tracker" = "https://github.com/adosikas/synth_mapping_helper/issues"
+Changelog = "https://github.com/adosikas/synth_mapping_helper/releases"
+
+[project.scripts]
+smh-cli = "synth_mapping_helper.cli:entrypoint"
+smh-gui = "synth_mapping_helper.gui:entrypoint"
+smh-companion = "synth_mapping_helper.companion:entrypoint"
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,21 @@
         data = synth_format.DataContainer(options.start_empty, {}, {}, {}, {}, {})
     else:
         try:
             data = synth_format.import_clipboard(options.use_original)
         except (JSONDecodeError, KeyError) as err:
             abort(f"Could not decode clipboard, did you copy somethinge else?\n\t{err!r}")
         except synth_format.JSONParseError as jpe:
-            abort(f"Detected invalid map data. The editor or your map may be corrupted.\n\tIf you don't have a recent backup and know how to fix the json manually, the following should help (otherwise you may find help on the discord):\n\t{jpe!r}")
+            abort(
+                "Detected invalid map data. The editor or your map may be corrupted.\n"
+                "\tYou can try repairing the file using 'File Utils' tab of the GUI, or restoring from a backup.\n"
+                "\tIf you know how to fix the json manually, the following should help (otherwise you may find help on the discord):\n"
+                f"\t{jpe!r}\n"
+                f"\tCaused by {jpe.__cause__!r}"
+            )
 
     # argument post-parsing
     # convert time parsed in seconds to beats
     for pos_val in "spawn-location", "pivot", "offset", "scale":
         v = getattr(options, pos_val, None)
         if v is not None and isinstance(v[2], utils.SecondFloat):
             setattr(options, pos_val[:2] + (v[2].to_beat(data.bpm),))
@@ -307,23 +313,23 @@
                 # existing notes (that did not get changed) always have priority
                 setattr(data, t, notes | getattr(data, t))
 
     if options.change_walls:
         if len(options.change_walls) == 1:
             # to single type: just merge all arrays the same way
             new_type = synth_format.WALL_TYPES[options.change_walls[0]][0]
-            def _change_wall_type(wall: "numpy array (1, 5)") -> "numpy array (1, 5)":
+            def _change_wall_type(wall: "numpy array (1, 5)", direction: int=1) -> "numpy array (1, 5)":
                 new_wall = wall.copy()
                 new_wall[..., 3] = new_type
                 return new_wall
             data.apply_for_walls(_change_wall_type, types=filter_types)
         else:
             # to multiple types: cycle
             generator = itertools.cycle(synth_format.WALL_TYPES[t][0] for t in options.change_walls)
-            def _change_wall_type(wall: "numpy array (1, 5)") -> "numpy array (1, 5)":
+            def _change_wall_type(wall: "numpy array (1, 5)", direction: int=1) -> "numpy array (1, 5)":
                 new_wall = wall.copy()
                 new_wall[..., 3] = next(generator)
                 return new_wall
             data.apply_for_walls(_change_wall_type, types=filter_types)
 
     if options.spawn:
         loc = options.spawn_location or (0.0,0.0,0.0)
@@ -408,9 +414,12 @@
         data.apply_for_note_types(rails.split_rails, types=filter_types)
     if options.rails_to_singles:
         data.apply_for_note_types(rails.rails_to_singles, keep_rail=bool(options.rails_to_singles[0]), types=filter_types)
     if options.snap_singles_to_rail:
         data.apply_for_note_types(rails.snap_singles_to_rail, types=filter_types)
     synth_format.export_clipboard(data, not options.keep_alignment)
 
+def entrypoint():
+    main(get_parser().parse_args())
+
 if __name__ == "__main__":
-    main(get_parser().parse_args())
+    entrypoint()
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/companion.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,10 +601,13 @@
         if autobackup_interval_min is not None:
             autobackup_interval_min = autobackup_sl.val
     autobackup_sl.on_changed(sl_autobackup)
 
     redraw()
     plt.show()
 
-if __name__ == "__main__":
+def entrypoint():
     logging.basicConfig(level=logging.INFO, format='%(asctime)s [%(levelname)s] %(message)s')
-    main(get_parser().parse_args())
+    main(get_parser().parse_args())
+
+if __name__ == "__main__":
+    entrypoint()
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,27 +7,35 @@
 
 from . import synth_format, cli, __version__
 from .gui_tabs.utils import *
 from .gui_tabs.commands import command_tab
 from .gui_tabs.file_utils import file_utils_tab
 from .gui_tabs.dashboard import dashboard_tab
 from .gui_tabs.autobackup import autobackup_tab
+from .gui_tabs.version import version_tab
+from .gui_tabs.stacking import stacking_tab
+from .gui_tabs.text_gen import text_gen_tab
+from .gui_tabs.wall_art import wall_art_tab
 
 tab_list = [
     ["Dashboard", "dashboard", dashboard_tab, None],
-    ["Autobackup", "manage_history", autobackup_tab, None],
+    ["Stacking", "layers", stacking_tab, None],
+    ["Text", "rtt", text_gen_tab, None],
+    ["Wall Art", "wallpaper", wall_art_tab, None],
     ["Commands", "play_arrow", command_tab, None],
     ["File utils", "construction", file_utils_tab, None],
+    ["Autobackup", "manage_history", autobackup_tab, None],
+    ["Version History", "update", version_tab, None],
 ]
 
 async def stop():
     logger.info("Stopping...")
     await ui.run_javascript("setTimeout(window.close, 100);")
     app.shutdown()
-if __name__ in {"__main__", "__mp_main__"}:
+def entrypoint():
     parser = ArgumentParser()
     parser.add_argument("-l", "--log-level", type=str, default="INFO", help="Set log level")
     parser.add_argument("--host", type=str, default="127.0.0.1",
         help="""Host for the webserver. Defaults to localhost.
             Can be set to a local IP if you want to access the GUI from another device, eg. tablet.\n
             Note that there is NO PASSWORD CHECK, so only use if you trust ALL devices on that network.""")
     parser.add_argument("--port", type=int, default=8080, help="Port for the webserver")
@@ -47,15 +55,17 @@
                 padding: 0 !important;
             }
         </style>""")
         with ui.header(elevated=True):
             with ui.tabs() as tabs:
                 for idx, (name, icon, *_) in enumerate(tab_list):
                     tab_list[idx][3] = ui.tab(name, icon=icon)
-            with ui.element().classes("ml-auto"):
+            with ui.button(icon="bug_report" + "support", color="negative", on_click=lambda _:ui.download("error_report", "smh_gui_error.json")).props("text-color=white").classes("ml-auto"):
+                ui.tooltip("Save report of last error")
+            with ui.element():
                 ui.tooltip("Switch dark mode")
                 dark = ui.dark_mode(True)  # start in dark mode (matching editor)
                 ui.button(icon="dark_mode", on_click=dark.enable).bind_visibility_from(dark, "value", backward=lambda v: v is not True).props('text-color=white')
                 ui.button(icon="light_mode", on_click=dark.disable).bind_visibility_from(dark, "value", backward=lambda v: v is not False).props('text-color=white')
 
             with ui.button(icon="question_mark", color="white", on_click=lambda _:ui.open(wiki_base, new_tab=True)).props("text-color=primary"):
                 ui.tooltip("Open wiki")
@@ -88,8 +98,11 @@
         host=args.host,
         port=args.port,
         title=f"SMH-GUI v{__version__} [beta]",
         favicon="🚧" if args.dev_mode else "🤦",
         reload=args.dev_mode,
         storage_secret="smh_gui",
         show=not args.background,
-    )
+    )
+
+if __name__ in {"__main__", "__mp_main__"}:
+    entrypoint()
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/autobackup.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/autobackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     with ui.row():
         ui.switch("Enable Autobackup", value=False, on_change=dir_changed).classes("my-auto").bind_value(watcher, "active").bind_value(app.storage.user, "autobackup_enabled")
         with ui.number("Check interval", value=60, suffix="s", min=15).props('input-style="text-align: right"').classes("w-20").bind_value(watcher, "interval").bind_value(app.storage.user, "autobackup_interval"):
             ui.tooltip("Amount of time between checks")
         with ui.number("Minimum age", value=300, suffix="s").props('input-style="text-align: right"').classes("w-20").bind_value(app.storage.user, "autobackup_minage"):
             ui.tooltip("If > 0, backups are not created if the last backup was less than X seconds ago")
         with ui.input("Editor working directory", validation={"Not a directory": _isdir}, on_change=dir_changed).classes("w-96").bind_value(app.storage.user, "autobackup_workdir"):
-            workdir_picker = ui.button(on_click=pick_dir, icon="pageview").classes("my-auto")
+            workdir_picker = ui.button(on_click=pick_dir, icon="pageview").props("outline").classes("my-auto")
             ui.tooltip("Directory with the .synth files you want to monitor")
         with ui.input("Backup directory", validation={"Not a directory": _isdir}, on_change=dir_changed).classes("w-96").bind_value(app.storage.user, "autobackup_backupdir"):
-            backupdir_picker = ui.button(on_click=pick_dir, icon="archive").classes("my-auto")
+            backupdir_picker = ui.button(on_click=pick_dir, icon="archive").props("outline").classes("my-auto")
             ui.tooltip("Directory to save the backups to")
 
     @ui.refreshable
     def log():
         for _, b in sorted(last_backup.values(), key=lambda tb: tb[0], reverse=True):
             ui.label(str(b))
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/commands.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 args.append("--use-original")
             if mirror_left_cb.value:
                 args.append("--mirror-left")
 
             try:
                 opts, remaining = p.parse_known_args(args)
             except ArgumentError as exc:
-                error(f"Error parsing line {i+1}: {exc!s}")
+                error(f"Error parsing line {i+1}", exc)
                 break
             if remaining:
                 error(f"Unknown arguments in line {i+1}: {remaining}")
                 break
             try:
                 cli.main(opts)
             except RuntimeError as exc:
@@ -159,18 +159,18 @@
                 ui.tooltip("Select a preset")
             preset_selector.bind_value(app.storage.user, "command_preset")
             with ui.button(icon="delete", color="red", on_click=remove_dialog.open).classes("my-auto").bind_enabled_from(preset_selector, "value"):
                 ui.tooltip("Delete current preset")
             with ui.button(icon="add", color="green", on_click=add_dialog.open).classes("my-auto") as add_button:
                 ui.tooltip("Add current command as preset")
             ui.separator().props("vertical")
-            with ui.button(icon="save", on_click=save_presets).classes("my-auto"):
+            with ui.button(icon="save", on_click=save_presets).props("outline").classes("my-auto"):
                 ui.tooltip("Store presets")
-            ui.upload(label="Load from files", auto_upload=True, multiple=True, on_upload=load_commands).classes("h-14 w-40")
-            with ui.button(icon="post_add", on_click=restore_presets, color="red").classes("my-auto"):
+            ui.upload(label="Load from files", auto_upload=True, multiple=True, on_upload=load_commands).props('color="positive" flat').classes("h-10 w-40")
+            with ui.button(icon="post_add", on_click=restore_presets, color="red").props("outline").classes("my-auto"):
                 ui.tooltip("Restore default presets")
         command_input = ui.textarea("Commands", placeholder="--offset=1,0,0", on_change=lambda e: presets.get(preset_selector.value) == e.value or preset_selector.set_value(None)).props("outlined").classes("w-full")
         command_input.bind_value(app.storage.user, "command_input")
         preset_selector.bind_value_to(command_input, forward=lambda v: v and presets.get(v))
         preset_selector.bind_value_to(remove_confirmation_label, "text", forward=lambda v: f"Really delete '{v}'?")
         add_button.bind_enabled_from(command_input, "value")
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/dashboard.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, Callable, Optional, List
 
 import numpy as np
 from nicegui import app, events, ui
+import pyperclip
 
 from .utils import *
 from .. import movement, pattern_generation, rails, synth_format
 from ..utils import parse_number
 
 def _movement_helper(data: synth_format.DataContainer, mirror_left: bool, base_func, relative_func, pivot_func, relative: bool, pivot: Optional[list[int]], *args, **kwargs) -> None:
     """pick the right function depending on relative or pivot being set"""
@@ -34,71 +35,76 @@
     for t in types:
         if t in synth_format.NOTE_TYPES and t != new_type:
             changed |= getattr(data, t)
             setattr(data, t, {})
     # existing notes always have priority
     setattr(data, new_type, changed | getattr(data, new_type))
 
-class ParseInputError(ValueError):
-    def __init__(self, input_id: str, error: str) -> None:
-        super().__init__(error)
-        self.input_id = input_id
-    def __repr__(self) -> str:
-        return self.args[0]
+def _space_walls(data: synth_format.DataContainer, interval: float) -> None:
+    out: synth_format.WALLS = {}
+    for i, (_, w) in enumerate(sorted(data.walls.items())):
+        out[i*interval] = (w*[1,1,0,1,1]) + [0,0,i*interval,0,0]
+    data.walls = out
 
 def dashboard_tab():
     class SMHInput(ui.input):
         def __init__(self, label: str, value: str|float, storage_id: str, tooltip: Optional[str]=None, suffix: Optional[str] = None, **kwargs):
+            self.on_parsed_value_change: Callable|None = None
             super().__init__(label=label, value=str(value), **kwargs)
             self.bind_value(app.storage.user, f"dashboard_{storage_id}")
             self.classes("w-12 h-10")
             self.props('dense input-style="text-align: right" no-error-icon')
             self.storage_id = storage_id
             if suffix:
                 self.props(f'suffix="{suffix}"')
             with self:
                 if tooltip is not None:
                     ui.tooltip(tooltip)
             with self.add_slot("error"):
                 ui.element().style("visiblity: hidden")
 
-        def on_value_change(self, value: Any) -> None:
-            super().on_value_change(value)
+        def _handle_value_change(self, value: Any) -> None:
+            super()._handle_value_change(value)
             try:
-                parse_number(value)
+                v = parse_number(value)
+                if self.on_parsed_value_change:
+                    self.on_parsed_value_change(v)
                 self.props(remove="error")
             except ValueError:
                 self.props(add="error")
 
         @property
         def parsed_value(self) -> float:
             try:
                 return parse_number(self.value)
             except ValueError as ve:
-                raise ParseInputError(self.storage_id, *ve.args) from ve
+                raise ParseInputError(self.storage_id, self.value) from ve
 
     with ui.row().classes("mb-4"):
         # with ui.card().classes("h-16"), ui.row():
         #     with ui.label("Filter").classes("my-auto"):
         #         wiki_reference("Miscellaneous-Options#filtering")
         #     with ui.button(icon="filter_alt"):
         #         ui.badge("0", color="red").props("floating")
         #     with ui.switch("Delete other"):
         #         wiki_reference("Pre--and-Post-Processing-Options#delete-everything-not-matching-filter")
         with ui.card().classes("h-16"), ui.row():
             with ui.switch("Use original", value=False).bind_value(app.storage.user, "dashboard_use_orig") as sw_use_orig:
+                ui.tooltip("Enable this to quickly try different settings without having to undo and copy the input again")
                 wiki_reference("Miscellaneous-Options#use-original-json")
-            with ui.switch("Mirror left hand", value=False).bind_value(app.storage.user, "dashboard_mirror_left") as sw_mirror_left:
+            with ui.switch("Mirror for left", value=False).bind_value(app.storage.user, "dashboard_mirror_left") as sw_mirror_left:
+                ui.tooltip("Mirrors the operations for left notes and walls, e.g. offseting right will move those left instead")
                 wiki_reference("Miscellaneous-Options#mirror-operations-for-left-hand")
             with ui.switch("Realign start", value=False).bind_value(app.storage.user, "dashboard_realign") as sw_realign:
+                ui.tooltip("This will realign the start of the selection to the very first object AFTER the operation")
                 wiki_reference("Pre--and-Post-Processing-Options#keep-selection-alignment")
         with ui.card().classes("h-16"), ui.row():
-            with ui.label("Coordinates").classes("my-auto"):
+            with ui.label("Coordinates").classes("my-2"):
                 wiki_reference("Movement-Options#pivot-and-relative")
-            coordinate_mode = ui.toggle(["absolute", "relative", "pivot"], value="absolute").classes("my-auto").bind_value(app.storage.user, "dashboard_coord_mode")
+            coordinate_mode = ui.toggle(["absolute", "relative", "pivot"], value="absolute").props('color="grey-7" rounded').bind_value(app.storage.user, "dashboard_coord_mode")
             with ui.row() as pivot_settings:
                 pivot_x = SMHInput("X", 0, "pivot_x", suffix="sq")
                 pivot_y = SMHInput("Y", 0, "pivot_y", suffix="sq")
                 pivot_t = SMHInput("Time", 0, "pivot_t", suffix="b")
                 pivot_settings.bind_visibility_from(coordinate_mode, "value", backward=lambda v: v=="pivot")        
 
     class SMHActionButton(ui.button):
@@ -107,41 +113,47 @@
             self._tooltip = tooltip
             self._func = func
             self.classes("w-12 h-10")
             with self:
                 ui.tooltip(tooltip)
                 if icon_angle:
                     # create dedicated object, which can rotate independently from button
-                    ui.icon(icon).classes(f"rotate-{icon_angle}")
+                    ui.icon(icon).style(f"rotate: {icon_angle}deg")
                 if wiki_ref is not None:
                     wiki_reference(wiki_ref, True).props("floating")
 
         def do_action(self, e: events.ClickEventArguments):
+            clipboard = pyperclip.paste()
+            settings = {
+                k.removeprefix("dashboard_"): v for k, v in app.storage.user.items()
+                if k.startswith("dashboard_")
+            }
             try:
-                d = synth_format.import_clipboard(use_original=sw_use_orig.value)
+                d = synth_format.import_clipboard_json(clipboard, use_original=sw_use_orig.value)
             except ValueError as ve:
-                error(f"Error reading data from clipboard", ve)
+                error(f"Error reading data from clipboard", ve, settings=settings, data=clipboard)
                 return
             try:
                 self._func(
                     data=d,
                     types=synth_format.ALL_TYPES,  # placeholder
                     mirror_left=sw_mirror_left.value,
                     relative=(coordinate_mode.value=="relative"),
                     pivot=[pivot_x.parsed_value, pivot_y.parsed_value, pivot_t.parsed_value] if (coordinate_mode.value=="pivot") else None
                 )
             except ParseInputError as pie:
-                error(f"Error parsing value: {pie.input_id}", pie)
+                error(f"Error parsing value: {pie.input_id}", pie, settings=settings, data=pie.value)
                 return
             except Exception as exc:
-                error(f"Error executing action", exc)
+                error(f"Error executing '{self._tooltip}'", exc, settings=settings, data=clipboard)
                 return
+            counts = d.get_counts()
             info(
                 f"Completed: '{self._tooltip}'",
-                caption=f"{d.notecount} note{'s' if d.notecount != 1 else ''}, {d.wallcount} wall{'s' if d.wallcount != 1 else ''}",
+                caption=", ".join(f"{counts[t]['total']} {t if counts[t]['total'] != 1 else t.rstrip('s')}" for t in ("notes", "rails", "rail_nodes", "walls")),
             )
             synth_format.export_clipboard(d, realign_start=sw_realign.value)
 
     with ui.row():
         with ui.card():
             with ui.label("Offset"):
                 wiki_reference("Movement-Options#offset")
@@ -277,66 +289,97 @@
                         ),
                         setattr(data, "bpm", scale_bpm.parsed_value),
                     ),
                     wiki_ref="Pre--and-Post-Processing-Options#change-bpm",
                 )
 
             ui.separator()
-            with ui.label("Mirror and Flatten"):
+            with ui.label("Flatten and Mirror"):
                 ui.tooltip("Just scaling, but with -1 or 0")
             with ui.row():
                 SMHActionButton(
-                    tooltip="Mirror X (left<->right)",
-                    icon="align_horizontal_center",
+                    tooltip="Flatten to Y axis (X=0)",
+                    icon="vertical_align_center", icon_angle=90,
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([-1,1,1]),
+                        scale_3d=np.array([0,1,1]),
                     ),
                 )
                 SMHActionButton(
-                    tooltip="Mirror Y (up<->down)",
-                    icon="align_vertical_center",
+                    tooltip="Flatten to X axis (Y=0)",
+                    icon="vertical_align_center",
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([1,-1,1]),
+                        scale_3d=np.array([1,0,1]),
                     ),
                 )
                 SMHActionButton(
-                    tooltip="Mirror time (reverse)",
-                    icon="fast_rewind",
+                    tooltip="Move to pivot (X=Y=0)",
+                    icon="adjust",
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([1,1,-1]),
+                        scale_3d=np.array([0,0,1]),
                     ),
                 )
             with ui.row():
                 SMHActionButton(
-                    tooltip="Flatten to Y axis (X=0)",
-                    icon="vertical_align_center", icon_angle=90,
+                    tooltip="Mirror X (left<->right)",
+                    icon="align_horizontal_center",
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([0,1,1]),
+                        scale_3d=np.array([-1,1,1]),
                     ),
                 )
                 SMHActionButton(
-                    tooltip="Flatten to X axis (Y=0)",
-                    icon="vertical_align_center",
+                    tooltip="Mirror Y (up<->down)",
+                    icon="align_vertical_center",
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([1,0,1]),
+                        scale_3d=np.array([1,-1,1]),
                     ),
                 )
                 SMHActionButton(
-                    tooltip="Move to pivot (X=Y=0)",
-                    icon="adjust",
+                    tooltip="Mirror time (reverse)",
+                    icon="fast_rewind",
                     func=lambda **kwargs: _movement_helper(**kwargs,
                         base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
-                        scale_3d=np.array([0,0,1]),
+                        scale_3d=np.array([1,1,-1]),
                     ),
                 )
+            ui.separator()
+            with ui.row():
+                mirror_angle = SMHInput("Angle", 45, "mirror_angle", suffix="°", tooltip="Angle of the mirror line. 0=horizontal, ±90=vertical, +45=/, -45=\\")
+                mirror_stack = SMHInput("Stack time", 0, "mirror_stack", suffix="b", tooltip="Instead of just mirroring, stack a mirrored copy onto the input using this as interval. 0=disabled.")
+                def _do_mirror(data: synth_format.DataContainer, **kwargs):
+                        # work on copy when stacking, else directly on data
+                        tmp = data.filtered() if mirror_stack.parsed_value else data
+                        # subtract rotation, mirror, add back rotation
+                        _movement_helper(tmp, **kwargs,
+                            base_func=movement.rotate, relative_func=movement.rotate_relative, pivot_func=movement.rotate_around,
+                            angle=-mirror_angle.parsed_value,
+                        )
+                        _movement_helper(tmp, **kwargs,
+                            base_func=movement.scale, relative_func=movement.scale_relative, pivot_func=movement.scale_from,
+                            scale_3d=np.array([1,-1,1]),
+                        )
+                        _movement_helper(tmp, **kwargs,
+                            base_func=movement.rotate, relative_func=movement.rotate_relative, pivot_func=movement.rotate_around,
+                            angle=mirror_angle.parsed_value,
+                        )
+                        if mirror_stack.parsed_value:
+                            tmp.apply_for_all(movement.offset, [0,0,mirror_stack.parsed_value])
+                            data.merge(tmp)
+                            
+                with SMHActionButton(
+                    tooltip="Mirror with custom angle. Depending on coordinate mode, the mirror line passes through grid center, object center or pivot",
+                    icon="",
+                    func=_do_mirror
+                ):
+                    mirror_icon = ui.icon("flip").style(f"rotate: {90-mirror_angle.parsed_value}deg")
+                mirror_angle.on_parsed_value_change = lambda v: mirror_icon.style(f"rotate: {90-v}deg")
 
         with ui.card():
             with ui.label("Rotation"):
                 wiki_reference("Movement-Options#rotate")
             with ui.row():
                 SMHActionButton(
                     tooltip="Rotate counterclockwise",
@@ -457,40 +500,56 @@
                     tooltip="Interpolate rail nodes",
                     icon="format_line_spacing"+"commit",
                     func=lambda data, types, **kwargs: data.apply_for_all(rails.interpolate_nodes, mode="spline", interval=rail_interval.parsed_value, types=types),
                     wiki_ref="Rail-Options#interpolate",
                 )
             with ui.row():
                 SMHActionButton(
-                    tooltip="To notestack (delete rail)",
+                    tooltip="Rail to notestack (delete rail)",
                     icon="animation",
                     func=lambda data, types, **kwargs: data.apply_for_note_types(rails.rails_to_notestacks, interval=rail_interval.parsed_value, keep_rail=False, types=types),
                 )
                 SMHActionButton(
-                    tooltip="To notestack (keep rail)",
+                    tooltip="Rail to notestack (keep rail)",
                     icon="animation"+"show_chart",
                     func=lambda data, types, **kwargs: data.apply_for_note_types(rails.rails_to_notestacks, interval=rail_interval.parsed_value, keep_rail=True, types=types),
                 )
                 SMHActionButton(
                     tooltip="Shorten rail (cuts from start if negative)",
                     icon="content_cut",
                     func=lambda data, types, **kwargs: data.apply_for_all(rails.shorten_rail, distance=rail_interval.parsed_value, types=types),
                     wiki_ref="Rail-Options#shorten-rails",
                 )
+            with ui.row():
+                SMHActionButton(
+                    tooltip="Extend level",
+                    icon="swipe_right_alt" + "horizontal_rule",
+                    func=lambda data, types, **kwargs: data.apply_for_all(rails.extend_level, distance=rail_interval.parsed_value, types=types),
+                )
+                SMHActionButton(
+                    tooltip="Extend directional / straight",
+                    icon="swipe_right_alt" + "double_arrow",
+                    func=lambda data, types, **kwargs: data.apply_for_all(rails.extend_straight, distance=rail_interval.parsed_value, types=types),
+                )
+                SMHActionButton(
+                    tooltip="Extend pointing to next",
+                    icon="swipe_right_alt" + "swipe_right_alt",
+                    func=lambda data, types, **kwargs: data.apply_for_note_types(rails.extend_to_next, distance=rail_interval.parsed_value, types=types),
+                )
 
         with ui.card():
             with ui.label("Color"):
                 wiki_reference("Pre--and-Post-Processing-Options#change-note-type")
 
             SMHActionButton(
                 tooltip="Swap Hands",
                 icon="swap_horizontal_circle",
                 func=_swap_hands,
                 wiki_ref="Pre--and-Post-Processing-Options#swap-hands",
-            )
+            ).props("outline")
             SMHActionButton(
                 tooltip="Change to left hand",
                 icon="change_circle",
                 func=lambda **kwargs: _change_color(new_type="left", **kwargs),
                 color="#009BAA",
             )
             SMHActionButton(
@@ -527,25 +586,25 @@
                         spiral_start.parsed_value if direction == 1 else 180 - spiral_start.parsed_value
                     ) * spiral_radius.parsed_value
                     return nodes
                 SMHActionButton(
                     tooltip="Spiral (counter-clockwise)",
                     icon="rotate_left",
                     func=lambda data, types, mirror_left, **kwargs: data.apply_for_notes(_add_spiral, fidelity=360*_safe_inverse(spiral_angle.parsed_value), types=types, mirror_left=mirror_left),
-                )
+                ).props("rounded")
                 SMHActionButton(
                     tooltip="Spiral (clockwise)",
                     icon="rotate_right",
                     func=lambda data, types, mirror_left, **kwargs: data.apply_for_notes(_add_spiral, fidelity=360*_safe_inverse(-spiral_angle.parsed_value), types=types, mirror_left=mirror_left),
-                )
+                ).props("rounded")
                 SMHActionButton(
                     tooltip="Random nodes",
                     icon="casino",
                     func=lambda data, types, mirror_left, **kwargs: data.apply_for_notes(_add_spiral, fidelity=0, types=types, mirror_left=mirror_left),
-                )
+                ).props("rounded outline")
             with ui.row():
                 with ui.label("Spikes"):
                     wiki_reference("Rail-Options#spikes")
                 spike_duration = SMHInput("Duration", 0, "spike_duration", suffix="b", tooltip="Duration of spikes.")
             with ui.row():
                 def _add_spikes(nodes: "numpy array (n, 3)", fidelity: float, direction: int = 1) -> "numpy array (n, 3)":
                     node_count = nodes.shape[0]  # backup count before repeat
@@ -568,8 +627,27 @@
                     icon="rotate_right",
                     func=lambda data, types, mirror_left, **kwargs: data.apply_for_notes(_add_spikes, fidelity=360*_safe_inverse(-spiral_angle.parsed_value), types=types, mirror_left=mirror_left),
                 )
                 SMHActionButton(
                     tooltip="Spikes (random)",
                     icon="casino",
                     func=lambda data, types, mirror_left, **kwargs: data.apply_for_notes(_add_spikes, fidelity=0, types=types, mirror_left=mirror_left),
-                )
+                )
+
+        with ui.card():
+            ui.label("Wall spacing")
+            with ui.row():
+                compress_interval = SMHInput("Spacing", "1/64", "compress_interval", suffix="b", tooltip="Space between walls")
+                SMHActionButton(
+                    tooltip="Compress",
+                    icon="compress",
+                    icon_angle=90,
+                    func=lambda data, **kwargs: _space_walls(data, interval=compress_interval.parsed_value),
+                )
+            with ui.row():
+                wall_limit = SMHInput("Walls/4s", 195, "spawn_limit", tooltip="200=wireframe limit, 500=spawn limit")
+                SMHActionButton(
+                    tooltip="Distribute walls to configured density",
+                    icon="expand",
+                    icon_angle=90,
+                    func=lambda data, **kwargs: _space_walls(data, interval=(4*data.bpm/60)/wall_limit.parsed_value),
+                )
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/gui_tabs/local_dir_picker.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/local_dir_picker.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/movement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 
+from .synth_format import WALL_MIRROR_ID
+
 # Note: None of these functions are allowed to *modify* the input array instance. Returning the same array (if nothing needed to be changed) is allowed.
 
 MIRROR_VEC_2D = np.array([-1, 1])
 MIRROR_VEC_3D = np.array([-1, 1, 1])
 
 # movement
 def offset(
@@ -87,25 +89,32 @@
     if scale_3d[2] == 0:
         raise ValueError("Cannot have 0 for time scale")
     scale_nd = np.ones((data.shape[-1]))
     scale_nd[..., :3] = scale_3d
     output = data * scale_nd
     if scale_nd[2] < 0:  # reverse order of elements
         output = output[::-1]
+    if data.shape[-1] == 5: # walls
+        if (scale_nd[0] < 0) != (scale_nd[1] < 0):  # mirror X *or* Y: swap type and invert angle (both: do nothing)
+            output[:,3] = [WALL_MIRROR_ID[i] for i in output[:,3]]
+            output[:,4] = -output[:,4]
+        if (scale_nd[1] < 0):  # mirror Y: add 180
+            output[:,4] += 180
+
     return output
 
 
 def scale_from(
     data: "numpy array (n, 3+)",
     scale_3d: "numpy array (3)",
     pivot_3d: "numpy array (3)",
     direction: int = 1,
 ) -> "numpy array (n, 3+)":
     """scale positions relative to pivot"""
-    pivot_nd = np.ones((data.shape[-1]))
+    pivot_nd = np.zeros((data.shape[-1]))
     pivot_nd[..., :3] = pivot_3d
     return scale(data - pivot_nd, scale_3d, direction=direction) + pivot_nd
 
 
 def scale_relative(
     data: "numpy array (n, 3+)", scale_3d: "numpy array (3)", direction: int = 1
 ) -> "numpy array (n, 3+)":
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/rails.py`

 * *Files 22% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 def snap_singles_to_rail(notes: SINGLE_COLOR_NOTES, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """snap single notes to rail"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
 
     for time in sorted(notes):
-        if current_rail_start is not None and time >= current_rail_end:  # current time is past end of stored rail -> forget stored rail
+        if current_rail_start is not None and time > current_rail_end:  # current time is past end of stored rail -> forget stored rail
             current_rail_start = None
             current_rail_end = None
         nodes = notes[time]
         if nodes.shape[0] > 1:  # rail: store start/end and keep as-is
             current_rail_start = nodes[0, 2]
             current_rail_end = nodes[-1, 2]
             out[time] = nodes
@@ -271,37 +271,89 @@
 
     return out
 
 def shorten_rail(
     data: "numpy array (n, 3)", distance: float, *, direction: bool = 1
 ) -> "numpy array (n, 3)":
     """Cut a bit of the end or start (if negative) of the rail"""
-    if data.shape[0] == 1:  # ignore single nodes or shorter rails
+    if data.shape[0] == 1 or not distance:  # ignore single nodes or shorter rails
         return data
     if distance > 0:  # cut at the end
         if (data[-1,2] - data[0,2]) <= distance:  # shorter -> return rail start only
             return data[0][np.newaxis]
         new_z = data[-1,2] - distance
         last_index = np.argwhere(data[:, 2] < new_z)[-1][0]  # last node before new end
         return np.concatenate((data[:last_index+1], interpolate_spline(data, [new_z])))
     else:  # cut at the start
         if (data[-1,2] - data[0,2]) <= -distance:  # shorter -> return rail end only
             return data[-1][np.newaxis]
         new_z = data[0,2] - distance  # distance is negative, so "- distance" is correct here
         first_index = np.argwhere(data[:, 2] > new_z)[0][0]  # first node after new start
         return np.concatenate((interpolate_spline(data, [new_z]), data[first_index:]))
 
+def extend_level(
+    data: "numpy array (n, 3)", distance: float, *, direction: bool = 1
+) -> "numpy array (n, 3)":
+    """Add a level rail section at the end or start (if negative). Turns single notes into rails"""
+    if not distance:
+        return data
+    elif distance > 0:
+        return np.concatenate((data, data[np.newaxis,-1]+[0,0,distance]))
+    else:
+        return np.concatenate((data[np.newaxis,0]+[0,0,distance], data))
+
+def extend_straight(
+    data: "numpy array (n, 3)", distance: float, *, direction: bool = 1
+) -> "numpy array (n, 3)":
+    """Add a straight rail section at the end or start (if negative) which keeps the same direction of the previous segment"""
+    if data.shape[0] == 1 or not distance:  # ignore single nodes or shorter rails
+        return data
+    elif distance > 0:
+        delta = data[-1] - data[-2]
+        return np.concatenate((data, data[np.newaxis,-1]+delta*(distance/delta[2])))
+    else:
+        delta = data[0] - data[1]
+        return np.concatenate((data[np.newaxis,0]+delta*(distance/delta[2]), data))
+
+def extend_to_next(
+    notes: SINGLE_COLOR_NOTES, distance: float, *, direction: bool = 1
+) -> "numpy array (n, 3)":
+    """Add a rail section at the end pointing to next note/rail. Vice-versa for negative. Turns single notes into rails."""
+    if len(notes) < 2 or not distance:  # ignore when there is nothing to work with
+        return notes
+    out: SINGLE_COLOR_NOTES = {}
+    last_nodes: "numpy array (n, 3)" = None
+    if distance > 0:
+        for time in sorted(notes):
+            nodes = notes[time]
+            if last_nodes is not None:
+                delta = nodes[0] - last_nodes[-1]
+                out[last_nodes[0,2]] = np.concatenate((last_nodes, last_nodes[np.newaxis,-1]+delta*(distance/delta[2])))
+            last_nodes = nodes
+        out[last_nodes[0,2]] = last_nodes
+    else:
+        for time in sorted(notes):
+            nodes = notes[time]
+            if last_nodes is not None:
+                delta = nodes[0] - last_nodes[-1]
+                new = np.concatenate((nodes[np.newaxis,0]+delta*(distance/delta[2]), nodes))
+                out[new[0,2]] = new
+            else:
+                out[nodes[0,2]] = nodes
+            last_nodes = nodes
+    return out
+
 def segment_rail(
     notes: SINGLE_COLOR_NOTES, max_length: float, *, direction: bool = 1
 ) -> "numpy array (n, 3)":
     """Segment rails into multiple range of maximum length. Can be negative to segment from end"""
     out: SINGLE_COLOR_NOTES = {}
     for time in sorted(notes):
         nodes = notes[time]
-        if nodes.shape[0] == 1:  # ignore single nodes
+        if nodes.shape[0] == 1 or (nodes[-1,2]-nodes[0,2]) <= max_length:  # ignore single nodes or short rails
             out[time] = nodes
             continue
 
         steps = bounded_arange_plusminus(nodes[0,2], nodes[-1,2], max_length)
         new_z = np.union1d(nodes[:,2], steps)
         for start in steps[:-1]:
             out[start] = interpolate_spline(nodes, new_z=new_z[np.logical_and(new_z>=start, new_z<=(start+abs(max_length)))])
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/synth_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #/usr/bin/env python3
 from io import BytesIO
+import codecs
 import dataclasses
 import json
 from pathlib import Path
 import time
 from typing import Union
 from zipfile import ZipFile
 
@@ -23,15 +24,18 @@
 Y_OFFSET = 0.0012
 
 # not sure where this comes from, but is needed to work with z coordinates
 # z_coord = index * (bpm / BPM_DIVISOR)
 # also maybe useful: bpm = (z_coord / index) * BPM_DIVISOR
 BPM_DIVISOR = 1200
 
+MS_PER_MIN = 60 * 1000
+
 NOTE_TYPES = ("right", "left", "single", "both")
+NOTE_TYPE_STRINGS = ("RightHanded", "LeftHanded", "OneHandSpecial", "BothHandsSpecial")
 # Note: wall offsets are eyeballed
 WALL_TYPES = {
     # name: (index, center_offset)
     # index 0-4 are the same "slideType" used in the JSON in the "slides" list
     "wall_right": (0, [4.05, -1.85]),
     "wall_left": (1, [-3.95, -1.85]),
     "angle_right": (2, [2.5, -2.2]),
@@ -41,36 +45,81 @@
     # Since there can be only be one wall anyway, just treat these three the same as slides
     "crouch": (100, [0.1, 7.5]),
     "square": (101, [0, -2]),
     "triangle": (102, [0, -4.7]),
 }
 WALL_LOOKUP = {id: name for name, (id, _) in WALL_TYPES.items()}
 WALL_OFFSETS = {id: np.array(offset + [0]) for _, (id, offset) in WALL_TYPES.items()}
+WALL_MIRROR_ID = {id: WALL_TYPES[
+        name.replace("left", "right") if "left" in name
+        else name.replace("right", "left") if "right" in name
+        else name
+    ][0]
+    for name, (id, _) in WALL_TYPES.items()
+}
+# symmetry angles in degrees, 360=no symmetry
+WALL_SYMMETRY = {
+    "wall_right": 180,
+    "wall_left": 180,
+    "angle_right": 360,
+    "center": 180,
+    "angle_left": 360,
+    "crouch": 360,
+    "square": 90,
+    "triangle": 120,
+}
 SLIDE_TYPES = [name for name, (id, _) in WALL_TYPES.items() if id < 100]
+LEFT_WALLS = [id for name, (id, _) in WALL_TYPES.items() if "left" in name]
+WALL_VERTS = {
+    "angle_right": (
+        (7.4, -8.75), (-4.6, 8.75), (-5.85, 8.75), (-5.85, 0.2), (5.25, -8.75)
+    ),
+    "square": (  # drawn as single, concave polygon (similar to a "c", but with the ends touching)
+        (8.4, 8.4), (8.4, -8.4), (-8.4, -8.4), (-8.4, 8.4),
+        (8.4, 8.4),  # complete the outer ring
+        (7.5, 7.5), (-7.5, 7.5), (-7.5, -7.5), (7.5, -7.5),  # inner ring in reverse order (going "back")
+        (7.5, 7.5)  # complete inner ring
+    ),
+    "triangle": (
+        (0, -11.2), (-9.7, 5.6), (9.7, 5.6),
+        (0, -11.2),
+        (0, -10), (8.6, 5), (-8.6, 5),
+        (0, -10),
+    )
+}
+# mirror x/y:
+for w, (x1, y1), (x2, y2) in (
+    ("wall_right", (2.8, 8.4), (4, 6)),
+    ("center", (0.15, 11), (2.1, 7.5)),
+    ("crouch", (5.6, 5.6), (8, 4)),
+):
+    WALL_VERTS[w] = ((x1, y1), (x2, y2), (x2, -y2), (x1, -y1), (-x1, -y1), (-x2, -y2), (-x2, y2), (-x1, y1))
+# mirror _right to _left:
+for w in ("wall_", "angle_"):
+    WALL_VERTS[w + "left"] = tuple((-x, y) for x, y in WALL_VERTS[w + "right"][::-1])
 
-ALL_TYPES = NOTE_TYPES + tuple(WALL_TYPES)
+ALL_TYPES = NOTE_TYPES + tuple(WALL_TYPES) + ("lights", "effects")
 
 SINGLE_COLOR_NOTES = dict[float, "numpy array (n, 3)"]   # rail segment (n>1) and x,y,t
 WALLS = dict[float, "numpy array (1, 5)"]    # x,y,t, type, angle
 
 BEATMAP_JSON_FILE = "beatmap.meta.bin"
 DIFFICULTIES = ("Easy", "Normal", "Hard", "Expert", "Master", "Custom")
 META_KEYS = ("Name", "Author", "Beatmapper", "CustomDifficultyName", "BPM")
 
 BETA_WARNING_SHOWN = False
 
 class JSONParseError(ValueError):
-    def __init__(self, d: dict, t: str, exc: Exception) -> None:
+    def __init__(self, d: dict, t: str) -> None:
         super().__init__()
         self.dict = d
         self.type = t
-        self.exc = exc
 
     def __str__(self) -> str:
-        return f"{self.exc!r} while parsing JSON of {self.type}: {self.dict}"
+        return f"Error while parsing JSON of {self.type}: {self.dict}"
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self})"
 
 
 def beta_warning() -> None:
     global BETA_WARNING_SHOWN
@@ -78,73 +127,106 @@
         print("\n\n ⚠️  W A R N I N G ⚠️")
         print("\tThis was tested with the beta version of the editor only.")
         print("\tYou may want to switch to it if you encounter bugs or weird behavior.\n\n")
         BETA_WARNING_SHOWN = True
         time.sleep(0.5)
 
 def round_time_to_fractions(time: float) -> float:
-    # 192 is the lowest common multiple of 64 and 48, so this covers all steps the editor supports and more
-    # effectively this is 3 intermediate steps for each 1/64 step, or 4 for each 1/48 step
-    # those intermediate steps are also possible in the editor by abusing snap or copy-paste and switching
-    # between 1/64 and 1/48 step.
-    # But the editor does no rounding at all, leading to float erros creeping up. 
-    return round(time * 192) / 192
+    # Round to 1/64 or 1/48, whichever is closer
+    r64 = round(time * 64) / 64
+    r48 = round(time * 48) / 48
+    return r64 if abs(time-r64) <= abs(time-r48) else round(r48, 11)
 
 def round_tick_for_json(time: float) -> float:
     # same as above, but in 1/64 ticks the json needs for some things
     # this is a seperate function to only do one float operation after rounding before output, to minimize errors
-    return round(time * 3) / 3
+    r64 = float(round(time))
+    r48 = round(time * 0.75) / 0.75  # 0.75 = 48/64
+    return r64 if abs(time-r64) <= abs(time-r48) else round(r48, 11)
+
+def round_tick_for_json_index(time: float) -> float | int:
+    # same as above, but for notes dict, which uses int when possible
+    if time.is_integer():
+        return int(time)
+    return round_tick_for_json(time)
+    
 
 @dataclasses.dataclass
 class DataContainer:
-    bpm: float
-    right: SINGLE_COLOR_NOTES
-    left: SINGLE_COLOR_NOTES
-    single: SINGLE_COLOR_NOTES
-    both: SINGLE_COLOR_NOTES
-    walls: WALLS
-
-    @property
-    def notecount(self) -> None:
-        return len(self.right) + len(self.left) + len(self.single) + len(self.both)
-
-    @property
-    def wallcount(self) -> None:
-        return len(self.walls)
+    bpm: float = 60.0
+    right: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+    left: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+    single: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+    both: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+    walls: WALLS = dataclasses.field(default_factory=dict)
+    # reuse same structure as notes for common code
+    lights: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+    effects: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
+
+    def get_counts(self) -> dict[str, dict[str, int]]:
+        out = {
+            "walls": {k: 0 for k in WALL_TYPES},
+            "notes": {},
+            "rails": {},
+            "rail_nodes": {},
+            "lights": len(self.lights),
+            "effects": len(self.effects),
+        }
+        for wall in self.walls.values():
+            out["walls"][WALL_LOOKUP[wall[0, 3]]] += 1
+        for t in NOTE_TYPES:
+            n_nodes = [n.shape[0] for n in getattr(self, t).values()]
+            notes = sum(1 if n==1 else 0 for n in n_nodes)
+            out["notes"][t] = notes
+            out["rails"][t] = len(n_nodes) - notes
+            out["rail_nodes"][t] = sum(n_nodes) - len(n_nodes)
+        for e in ("walls", "notes", "rails", "rail_nodes"):
+            out[e]["total"] = sum(out[e].values())
+        return out
 
     # Note: None of these functions are allowed to *modify* the dicts, instead they must create new dicts
     # This avoids requring deep copies for everything
 
     def apply_for_notes(self, f, *args, types: list = NOTE_TYPES, mirror_left: bool = False, **kwargs) -> None:
-        for t in types:
-            if t not in NOTE_TYPES:
+        for t in NOTE_TYPES:
+            if t not in types:
                 continue
             notes = getattr(self, t)
             out = {}
             for _, nodes in sorted(notes.items()):
                 out_nodes = f(nodes, *args, direction=(-1 if mirror_left and t == "left" else 1), **kwargs)
                 out[out_nodes[0, 2]] = out_nodes
             setattr(self, str(t), out)
 
     def apply_for_walls(self, f, *args, types: list = WALL_TYPES, mirror_left: bool = False, **kwargs) -> None:
-        wall_types = [WALL_TYPES[t][0] for t in types if t in WALL_TYPES]
+        wall_types = [WALL_TYPES[t][0] for t in WALL_TYPES if t in types]
         out_walls = {}
         for time_index, wall in sorted(self.walls.items()):
             if wall[0, 3] in wall_types:
-                wall = f(wall, *args, **kwargs)  # TODO: support mirror_left
+                wall = f(wall, *args, direction=(-1 if mirror_left and wall[0, 3] in LEFT_WALLS else 1), **kwargs)
                 out_walls[wall[0, 2]] = wall
             else:
                 out_walls[time_index] = wall
         self.walls = out_walls
 
     def apply_for_all(self, f, *args, types: list = ALL_TYPES, mirror_left: bool = False, **kwargs) -> None:
         self.apply_for_notes(f, *args, types=types, mirror_left=mirror_left, **kwargs)
         self.apply_for_walls(f, *args, types=types, mirror_left=mirror_left, **kwargs)
+        for t in ("lights", "effects"):
+            if t not in types:
+                continue
+            objs = getattr(self, t)
+            out = {}
+            for _, nodes in sorted(objs.items()):
+                out_nodes = f(nodes, *args, **kwargs)
+                out[out_nodes[0, 2]] = out_nodes
+            setattr(self, t, out)
+
 
-    # used when the functions needs access to all notes and rails of a color at one
+    # used when the functions needs access to all notes and rails of a color at once
     def apply_for_note_types(self, f, *args, types: list = NOTE_TYPES, mirror_left: bool = False, **kwargs) -> None:
         for t in types:
             if t not in NOTE_TYPES:
                 continue
             setattr(self, t, f(getattr(self, t), *args, direction=(-1 if mirror_left and t == "left" else 1), **kwargs))
 
     def filtered(self, types: list = ALL_TYPES) -> "DataContainer":
@@ -162,65 +244,74 @@
         
     def merge(self, other: "DataContainer") -> None:
         for t in NOTE_TYPES:
             self_notes = getattr(self, t)
             other_notes = getattr(other, t)
             setattr(self, t, self_notes | other_notes)
         self.walls |= other.walls
+        self.lights |= other.lights
+        self.effects |= other.effects
 
     def get_object_dict(self, type_name: str) -> Union[SINGLE_COLOR_NOTES, WALLS]:
-        if type_name in NOTE_TYPES:
+        if type_name in NOTE_TYPES + ("lights", "effects"):
             return getattr(self, type_name)
         wall_type = WALL_TYPES[type_name][0]
         return {
             time_index: wall
             for time_index, wall in sorted(self.walls.items())
             if wall[0, 3] == wall_type
         }
 
 @dataclasses.dataclass
 class ClipboardDataContainer(DataContainer):
-    original_json: str
+    original_json: str = ""
+    selection_length: float = 0.0
 
 @dataclasses.dataclass
 class SynthFile:
     input_file: Union[Path, BytesIO]
     meta: dict[str, str]
     bookmarks: dict[float, str]
     difficulties: dict[str, DataContainer]
 
     errors: dict[str, list[tuple[str, JSONParseError]]] = dataclasses.field(default_factory=dict)
+    offset_ms: float = 0.0
 
     @property
     def bpm(self) -> float:
         for d, c in self.difficulties.items():
             return c.bpm
 
     def reload(self) -> None:
         self.errors: dict[str, list[tuple[str, JSONParseError]]] = {}
         in_bio = self.input_file if isinstance(self.input_file, BytesIO) else BytesIO(self.input_file.read_bytes())
         with ZipFile(in_bio) as inzip:
             # load beatmap json
             beatmap = json.loads(inzip.read(BEATMAP_JSON_FILE))
             bpm: float = beatmap["BPM"]
+            self.offset_ms = beatmap["Offset"]
             self.meta = {k: beatmap[k] for k in META_KEYS}
             self.bookmarks = {
                 # bookmarks are stored in steps of 64 per beat (regardless of BPM)
                 round_time_to_fractions(bookmark_dict["time"] / 64): bookmark_dict["name"]
                 for bookmark_dict in beatmap["Bookmarks"]["BookmarksList"]
             }
 
             for diff in DIFFICULTIES:
                 diff_removed : list[tuple[str, JSONParseError]] = []
                 # r, l, s, b
                 notes: list[SINGLE_COLOR_NOTES] = [{} for _ in range(4)]
                 for time, time_notes in beatmap["Track"][diff].items():
+                    time_types = set()
                     for note in time_notes:
                         try:
                             note_type, nodes = note_from_synth(bpm, 0, note)
+                            if note_type in time_types:
+                                raise JSONParseError(note, "duplicate note type")
+                            time_types.add(note_type)
                             notes[note_type][nodes[0,2]] = nodes
                         except JSONParseError as jpe:
                             try:
                                 time = f"{time} (measure {float(time)/64})"
                             except:
                                 pass
                             diff_removed.append((jpe, time))
@@ -250,59 +341,86 @@
                         except JSONParseError as jpe:
                             time = str(wall_dict.get("time"))
                             try:
                                 time = f"{time} (measure {float(time)/64})"
                             except:
                                 pass
                             diff_removed.append((jpe, time))
-                # add difficulty when there is a note of any type or a wall
-                if any(nt for nt in notes) or walls:
-                    self.difficulties[diff] = DataContainer(bpm, *notes, walls)
+                lights = {
+                    b: np.array([[0,0,b]])
+                    for t in beatmap["Lights"][diff]
+                    for b in [round_time_to_fractions(t / 64)]
+                }
+                effects = {
+                    b: np.array([[0,0,b]])
+                    for t in beatmap["Effects"][diff]
+                    for b in [round_time_to_fractions(t / 64)]
+                }
+                # add difficulty when there is a note of any type, a wall or lights/effects
+                if any(notes) or walls or lights or effects:
+                    self.difficulties[diff] = DataContainer(bpm, *notes, walls, lights, effects)
 
                 if diff_removed:
                     self.errors[diff] = diff_removed
 
     def save_as(self, output_file: Union[Path, BytesIO]) -> None:
         out_buffer = output_file if isinstance(output_file, BytesIO) else BytesIO()  # buffer output zip file in memory, only write on success
         in_bio = self.input_file if isinstance(self.input_file, BytesIO) else BytesIO(self.input_file.read_bytes())
         with ZipFile(in_bio) as inzip, ZipFile(out_buffer, "w") as outzip:
             # copy all content except beatmap json
             outzip.comment = inzip.comment
             for info in inzip.infolist():
-                if info.filename != BEATMAP_JSON_FILE:
+                if info.filename == BEATMAP_JSON_FILE:
+                    beatmap_info = info
+                else:
                     outzip.writestr(info, inzip.read(info.filename))
 
             beatmap = json.loads(inzip.read(BEATMAP_JSON_FILE))
             beatmap["BPM"] = self.bpm
+            beatmap["Offset"] = self.offset_ms
+            beatmap["ModifiedTime"] = int(time.time())
 
             beatmap["Bookmarks"]["BookmarksList"] = [
                 {"time": round_tick_for_json(t * 64), "name": n}
                 for t, n in sorted(self.bookmarks.items())
             ]
 
             for diff, data in self.difficulties.items():
                 new_notes = {}
                 for note_type, notes in enumerate((data.right, data.left, data.single, data.both)):
+                    type_notes = {}  # buffer single type to avoid multiple of the same type at the same time
                     for time_index, nodes in sorted(notes.items()):
-                        new_notes.setdefault(round_tick_for_json(time_index * 64), []).append(note_to_synth(data.bpm, note_type, nodes))
-                beatmap["Track"][diff] = new_notes
+                        type_notes[round_tick_for_json_index(time_index * 64)] = note_to_synth(data.bpm, note_type, nodes)
+                    for time_tick, synth_dict in sorted(type_notes.items()):
+                        existing = new_notes.setdefault(time_tick, [])
+                        # edit by reference
+                        existing.append(
+                            # keep same order as editor
+                            {"Id": f"Note_{time_tick}{NOTE_TYPE_STRINGS[note_type]}{len(existing)}", "ComboId": -1}
+                            | synth_dict
+                            | {"Direction": 0}
+                        )
+                beatmap["Track"][diff] = {k: v for k,v in sorted(new_notes.items())}
                 walls = {
                     "crouchs": [],
                     "squares": [],
                     "triangles": [],
                     "slides": [],
                 }
                 for _, wall in sorted(data.walls.items()):
                     dest_list, wall_dict = wall_to_synth(data.bpm, wall)
                     walls[dest_list].append(wall_dict)
                 for t, wall_list in walls.items():
                     beatmap[t.capitalize()][diff] = wall_list
+                beatmap["Lights"][diff] = [round_tick_for_json(t * 64) for t in data.lights]
+                beatmap["Effects"][diff] = [round_tick_for_json(t * 64) for t in data.effects]
 
-            # write modified beatmap json
-            outzip.writestr(inzip.getinfo(BEATMAP_JSON_FILE), json.dumps(beatmap))
+            # write modified beatmap json, in a way that closely mirrors the editor
+            beatmap_json = json.dumps(beatmap, indent=2, allow_nan=False)
+            outzip.writestr(beatmap_info, codecs.BOM_UTF8 + beatmap_json.encode("utf-8").replace(b"\n", b"\r\n"))
         # write output zip
         if isinstance(output_file, BytesIO):
             output_file.seek(0)
         else:
             output_file.write_bytes(out_buffer.getbuffer())
 
     def change_bpm(self, bpm: float) -> None:
@@ -311,19 +429,32 @@
             self.bookmarks = {
                 time * ratio: name
                 for time, name in self.bookmarks.items()
             }
             for c in self.difficulties.values():
                 c.apply_for_all(movement.scale, [1,1,ratio])
                 c.bpm = bpm
+    def change_offset(self, offset_ms: float) -> None:
+        if self.offset_ms != offset_ms:
+            delta = (offset_ms - self.offset_ms) / MS_PER_MIN * self.bpm
+            self.bookmarks = {
+                time + delta: name
+                for time, name in self.bookmarks.items()
+            }
+            for c in self.difficulties.values():
+                c.apply_for_all(movement.offset, [0,0,delta])
+            self.offset_ms = offset_ms
 
-    def merge(self, other: "SynthFile", adjust_bpm:bool = True) -> None:
+    def merge(self, other: "SynthFile", adjust_bpm: bool = True, merge_bookmarks: bool = True) -> None:
         if adjust_bpm and self.bpm != other.bpm:
             other.change_bpm(self.bpm)
-        self.bookmarks |= other.bookmarks
+        if adjust_bpm and self.offset_ms != other.offset_ms:
+            other.change_offset(self.offset_ms)
+        if merge_bookmarks:
+            self.bookmarks |= other.bookmarks
         for d, c in other.difficulties.items():
             if d in self.difficulties:
                 self.difficulties[d].merge(c)
             else:
                 self.difficulties[d] = c
         for d, e in other.errors.items():
             if d in self.errors:
@@ -337,21 +468,21 @@
         return np.array([
             (coord[0] - X_OFFSET) / GRID_SCALE,
             (coord[1] - Y_OFFSET) / GRID_SCALE,
             # convert absolute coordinate to number of beats since start
             round_time_to_fractions(coord[2] * bpm / BPM_DIVISOR - startMeasure / 64),
         ])
     except (ValueError, TypeError) as exc:
-        raise JSONParseError(coord, c_type, exc)
+        raise JSONParseError(coord, c_type) from exc
 
 def coord_to_synth(bpm: float, coord: "numpy array (3)") -> list[float]:
     return [
-        (coord[0] * GRID_SCALE) + X_OFFSET,
-        (coord[1] * GRID_SCALE) + Y_OFFSET,
-        (round_time_to_fractions(coord[2]) / bpm) * BPM_DIVISOR,  # ([beat] / [beat / minute]) * 1200 = ([sec] * 60) * 1200
+        round((coord[0] * GRID_SCALE) + X_OFFSET, 11),
+        round((coord[1] * GRID_SCALE) + Y_OFFSET, 11),
+        round((round_time_to_fractions(coord[2]) / bpm) * BPM_DIVISOR, 11),  # ([beat] / [beat / minute]) * 1200 = ([sec] * 60) * 1200
     ]
 
 # full note dict
 def note_from_synth(bpm: float, startMeasure: float, note_dict: dict) -> tuple[int, "numpy array (n, 3)"]:
     start = coord_from_synth(bpm, startMeasure, note_dict["Position"], "note" if note_dict["Segments"] is None else "rail head")
     note_type = note_dict["Type"]
     if note_dict["Segments"] is None:
@@ -359,23 +490,23 @@
     else:
         return note_type, np.stack((start,) + tuple(coord_from_synth(
             bpm, startMeasure, node, f"rail node #{i} of rail starting at json index {startMeasure + start[2]*64}"
         ) for i, node in enumerate(note_dict["Segments"])))
 
 def note_to_synth(bpm: float, note_type: int, nodes: "numpy array (n, 3)") -> dict:
     return {
-        "Type": note_type,
         "Position": coord_to_synth(bpm, nodes[0]),
         "Segments": [coord_to_synth(bpm, node) for node in nodes[1:]] if nodes.shape[0] > 1 else None,
+        "Type": note_type,
     }
 
 # full wall dict
 def wall_from_synth(bpm: float, startMeasure: float, wall_dict: dict, wall_type: int) -> tuple[int, "numpy array (1, 5)"]:
     if wall_type not in WALL_LOOKUP:
-        raise JSONParseError(wall_dict, "wall", ValueError(f"Unexpected wall type ({wall_type})"))
+        raise JSONParseError(wall_dict, "wall") from ValueError(f"Unexpected wall type ({wall_type})")
     return np.concatenate((
         coord_from_synth(bpm, startMeasure, wall_dict["position"], f"{WALL_LOOKUP[wall_type]} wall") + WALL_OFFSETS[wall_type],
         (wall_type, wall_dict.get("zRotation", 0.0))
     ))[np.newaxis]
 
 def wall_to_synth(bpm: float, wall: "numpy array (1, 5)") -> tuple[str, dict]:
     wall_type = int(wall[0, 3])
@@ -389,19 +520,24 @@
     }
     # crouch, square and triangle are not in the "slides" list, each has their own list and they do not use the "slideType" key
     if wall_type < 100:  # we gave crouch, square and triangle the types 100, 101 and 102
         dest_list = "slides"
     else:
         dest_list = WALL_LOOKUP[wall_type] + "s"
         del wall_dict["slideType"]
+        if wall_type == WALL_TYPES["crouch"][0]:
+            # cannot rotate crouch walls
+            del wall_dict["zRotation"]
     return dest_list, wall_dict
 
 # full json
 def import_clipboard_json(original_json: str, use_original: bool = False) -> ClipboardDataContainer:
     clipboard = json.loads(original_json)
+    if not isinstance(clipboard, dict):
+        raise ValueError("clipboard did not contain json dict")
     if "original_json" in clipboard:
         original_json = clipboard["original_json"]
     if use_original:
         clipboard = json.loads(original_json)
     bpm = clipboard["BPM"]
     startMeasure = clipboard["startMeasure"]
     # r, l, s, b
@@ -420,16 +556,27 @@
     for wall_type in ("crouch", "square", "triangle"):
         if wall_type + "s" not in clipboard:
             beta_warning()
             continue  # these are only in the beta editor
         for wall_dict in clipboard[wall_type + "s"]:
             wall = wall_from_synth(bpm, startMeasure, wall_dict, WALL_TYPES[wall_type][0])
             walls[wall[0, 2]] = wall
+    
+    lights = {
+        b: np.array([[0,0,b]])
+        for t in clipboard["lights"]
+        for b in [round_time_to_fractions((t-startMeasure)/64)]
+    }
+    effects = {
+        b: np.array([[0,0,b]])
+        for t in clipboard["effects"]
+        for b in [round_time_to_fractions((t-startMeasure)/64)]
+    }
 
-    return ClipboardDataContainer(bpm, *notes, walls, original_json)
+    return ClipboardDataContainer(bpm, *notes, walls, lights, effects, original_json, clipboard["lenght"] / MS_PER_MIN * bpm)
 
 def import_clipboard(use_original: bool = False) -> ClipboardDataContainer:
     return import_clipboard_json(pyperclip.paste(), use_original)
 
 def export_clipboard_json(data: DataContainer, realign_start: bool = True) -> str:
     clipboard = {
         "BPM": data.bpm,
@@ -441,46 +588,60 @@
         "jumps": [],
         "crouchs": [],
         "squares": [],
         "triangles": [],
         "slides": [],
         "lights": [],
     }
-    if isinstance(data, ClipboardDataContainer):
+    if isinstance(data, ClipboardDataContainer) and data.original_json:
         clipboard["original_json"] = data.original_json
 
     first = 99999
     last = -99999
     for note_type, notes in enumerate((data.right, data.left, data.single, data.both)):
-        for time_index, nodes in notes.items():
-            clipboard["notes"].setdefault(round_tick_for_json(time_index * 64), []).append(note_to_synth(data.bpm, note_type, nodes))
+        type_notes = {}  # buffer single type to avoid multiple of the same type at the same time
+        for time_index, nodes in notes.items(): 
+            type_notes[round_tick_for_json(time_index * 64)] = note_to_synth(data.bpm, note_type, nodes)
             if nodes[0, 2] < first:
                 first = nodes[0, 2]
             if nodes[-1, 2] > last:
                 last = nodes[-1, 2]
+        for time_tick, synth_dict in sorted(type_notes.items()):
+            clipboard["notes"].setdefault(time_tick, []).append(synth_dict)
     for _, wall in data.walls.items():
         if wall[0, 2] < first:
             first = wall[0, 2]
         if wall[0, 2] > last:
             last = wall[0, 2]
         dest_list, wall_dict = wall_to_synth(data.bpm, wall)
         clipboard[dest_list].append(wall_dict)
 
+    for t in data.lights:
+        if t < first:
+            first = t
+        if t > last:
+            last = t
+        clipboard["lights"].append(round_tick_for_json(t * 64))
+    for t in data.effects:
+        if t < first:
+            first = t
+        if t > last:
+            last = t
+        clipboard["effects"].append(round_tick_for_json(t * 64))
 
-    ms_per_min = 60 * 1000
     if realign_start:
         # position of selection start in beats*64 
         clipboard["startMeasure"] = round_tick_for_json(first * 64)
         # position of selection start in ms
-        clipboard["startTime"] = first * ms_per_min / data.bpm
+        clipboard["startTime"] = first * MS_PER_MIN / data.bpm
         # length of the selection in milliseconds
         # and yes, the editor has a typo, so we need to missspell it too
-        clipboard["lenght"] = last * ms_per_min / data.bpm
+        clipboard["lenght"] = last * MS_PER_MIN / data.bpm
     # always update length
-    clipboard["lenght"] = (last - first) * ms_per_min / data.bpm
+    clipboard["lenght"] = (last - first) * MS_PER_MIN / data.bpm
     return json.dumps(clipboard)
 
 def export_clipboard(data: DataContainer, realign_start: bool = True):
     pyperclip.copy(export_clipboard_json(data, realign_start))
 
 def import_file(file_path: Union[Path, BytesIO]) -> SynthFile:
     out = SynthFile(file_path, {}, {}, {})
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -105,7 +105,43 @@
     except ValueError:
         raise ValueError("Error parsing y")
     try:
         t = parse_time(split[2])
     except ValueError:
         raise ValueError("Error parsing t")
     return (x, y, t)
+
+def pretty_fraction(val: float) -> str:
+    if round(val, 4).is_integer():
+        return str(int(round(val, 4)))
+    if round(val*192, 4).is_integer():
+        if val < 1:
+            # regular fraction: a/b
+            v = int(round(val*192, 4))
+            gcd = np.gcd(v,192)
+            return f"{v//gcd}/{192//gcd}"
+        else:
+            # mixed fraction: i a/b
+            i = int(val)
+            v = int(round((val-i)*192, 4))
+            gcd = np.gcd(v,192)
+            return f"{i} {v//gcd}/{192//gcd}"
+    return str(val)
+
+def pretty_time_delta(seconds: float) -> str:
+    seconds = abs(seconds)
+    if seconds < 1:
+        return f"{seconds*1000:.0f} ms"
+    if seconds < 60:
+        return f"{seconds:.0f} seconds"
+    if seconds < 3600:
+        return f"{seconds//60} minutes"
+    if seconds < 24*3600:
+        return f"{seconds//3600} hours"
+    days = seconds // (24*3600)
+    if days < 7:
+        return f"{days} days"
+    if days < 30:
+        return f"{days//7} weeks"
+    if days < 365:
+        return f"{days//30} months"
+    return f"{days//365} years"
```

### Comparing `synth_mapping_helper-1.3.9/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 src/synth_mapping_helper/__init__.py
 src/synth_mapping_helper/cli.py
 src/synth_mapping_helper/companion.py
 src/synth_mapping_helper/finalize.py
 src/synth_mapping_helper/gui.py
 src/synth_mapping_helper/movement.py
 src/synth_mapping_helper/pattern_generation.py
 src/synth_mapping_helper/rails.py
 src/synth_mapping_helper/synth_format.py
 src/synth_mapping_helper/utils.py
 src/synth_mapping_helper.egg-info/PKG-INFO
 src/synth_mapping_helper.egg-info/SOURCES.txt
 src/synth_mapping_helper.egg-info/dependency_links.txt
+src/synth_mapping_helper.egg-info/entry_points.txt
 src/synth_mapping_helper.egg-info/requires.txt
 src/synth_mapping_helper.egg-info/top_level.txt
 src/synth_mapping_helper/gui_tabs/__init__.py
 src/synth_mapping_helper/gui_tabs/autobackup.py
 src/synth_mapping_helper/gui_tabs/commands.py
 src/synth_mapping_helper/gui_tabs/dashboard.py
 src/synth_mapping_helper/gui_tabs/file_utils.py
 src/synth_mapping_helper/gui_tabs/local_dir_picker.py
+src/synth_mapping_helper/gui_tabs/map_render.py
+src/synth_mapping_helper/gui_tabs/stacking.py
+src/synth_mapping_helper/gui_tabs/text_gen.py
 src/synth_mapping_helper/gui_tabs/utils.py
+src/synth_mapping_helper/gui_tabs/version.py
+src/synth_mapping_helper/gui_tabs/wall_art.py
 tests/test_synth_format.py
```

