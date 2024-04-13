# Comparing `tmp/ds20kdb-avt-1.0.4.tar.gz` & `tmp/ds20kdb_avt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb-avt-1.0.4.tar", last modified: Sat Apr 13 12:42:10 2024, max compression
+gzip compressed data, was "ds20kdb_avt-1.0.5.tar", last modified: Sat Apr 13 17:08:31 2024, max compression
```

## Comparing `ds20kdb-avt-1.0.4.tar` & `ds20kdb_avt-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.303754 ds20kdb-avt-1.0.4/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 12:42:10.302857 ds20kdb-avt-1.0.4/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.4/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 12:42:10.303969 ds20kdb-avt-1.0.4/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 12:41:51.000000 ds20kdb-avt-1.0.4/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.269683 ds20kdb-avt-1.0.4/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.294012 ds20kdb-avt-1.0.4/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.4/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.4/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb-avt-1.0.4/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb-avt-1.0.4/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.4/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.4/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   118397 2024-04-13 12:40:49.000000 ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.4/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.4/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb-avt-1.0.4/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.301742 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.964714 ds20kdb_avt-1.0.5/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:08:31.963760 ds20kdb_avt-1.0.5/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb_avt-1.0.5/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 17:08:31.964925 ds20kdb_avt-1.0.5/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 17:08:12.000000 ds20kdb_avt-1.0.5/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.922153 ds20kdb_avt-1.0.5/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.954575 ds20kdb_avt-1.0.5/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb_avt-1.0.5/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb_avt-1.0.5/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb_avt-1.0.5/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb_avt-1.0.5/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb_avt-1.0.5/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb_avt-1.0.5/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   120272 2024-04-13 16:20:01.000000 ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.5/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb_avt-1.0.5/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb_avt-1.0.5/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.962691 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb-avt-1.0.4/PKG-INFO` & `ds20kdb_avt-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.4
+Version: 1.0.5
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.4/README.md` & `ds20kdb_avt-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/setup.py` & `ds20kdb_avt-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.4",
+    version="1.0.5",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/auth.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/common.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/common.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/create_credentials_file.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/gen_tray_files_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/interface.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/interface.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/qr.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/qrgen.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/scanner_auto.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/scanner_auto.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-GUI for POSTing DarkSide-20k vTiles to the pre-production database.
+GUI for POSTing DarkSide-20k vTiles to the production database.
 """
 
 import collections
 import contextlib
 import datetime
 from enum import IntEnum
 import functools
@@ -295,14 +295,16 @@
         self.table_json = {}
         self.widgets = []
         self.table_json_string = None
 
         self.session_timestamp = timestamp_to_utc(time.time())
         self.wafer_table_dataframe = self.database_alive()
 
+        self.valid_locations = set(interface.wafer_map_valid_locations())
+
         ######################################################################
         # platform specific items related to detecting paste, font handling
         ######################################################################
 
         self.system = platform.system()
 
         default_fonts = [
@@ -321,18 +323,23 @@
 
         ######################################################################
         # Location of file from which to load/save GUI combobox default values
         # on application start.
         ######################################################################
 
         self.defaults_filename = '.ds20kdb_defaults'
+        self.defaults_tray_filename = '.ds20kdb_tray_defaults'
         self.home_directory = os.path.expanduser('~')
         self.defaults_file_path = os.path.join(
             self.home_directory, self.defaults_filename
         )
+        self.defaults_tray_file_path = os.path.join(
+            self.home_directory, self.defaults_tray_filename
+        )
+        self.tray_file_directory = self.home_directory
 
         # build GUI
 
         self.populate_window_with_frames()
 
         self.populate_console_frame()
         self.populate_menu_bar()
@@ -609,17 +616,15 @@
                 width=20,
             ),
             itype=Itype.COMBOBOX,
             cluster='qrcode',
             category=None,
         )
         wtmp.instance.grid(sticky='w', column=1, row=8)
-        wtmp.instance.bind(
-            '<Key>', lambda e: self.handle_ctrl_key_qr(e)
-        )
+        wtmp.instance.bind('<Key>', self.handle_ctrl_key_qr)
         self.widgets.append(wtmp)
 
         # solder_id
 
         # Attempt to get institute name.
         # This is a little inefficient, since we'll load this file again later.
         table_json = quiet_load_json(self.defaults_file_path)
@@ -719,17 +724,15 @@
                 width=96,
             ),
             itype=Itype.COMBOBOX,
             cluster='comment',
             category=None,
         )
         wtmp.instance.grid(sticky='w', column=3, row=8)
-        wtmp.instance.bind(
-            '<Key>', lambda e: self.handle_ctrl_key_comment(e)
-        )
+        wtmp.instance.bind('<Key>', self.handle_ctrl_key_comment)
         self.widgets.append(wtmp)
 
     def populate_production_date_frame(self):
         """
         Populate the GUI production date frame with gridded widgets.
 
         Limited selections for some values:
@@ -1025,15 +1028,15 @@
             22: (0, 3), 16: (1, 3), 10: (2, 3), 4: (3, 3),
             23: (0, 4), 17: (1, 4), 11: (2, 4), 5: (3, 4),
             24: (0, 5), 18: (1, 5), 12: (2, 5), 6: (3, 5),
         }
 
         lots = sorted({lo[0] for lo in self.wafer_table_dataframe[['lot']].values})
         wafs = sorted({wn[0] for wn in self.wafer_table_dataframe[['wafer_number']].values})
-        cols, rows = map(set, zip(*interface.wafer_map_valid_locations()))
+        cols, rows = map(set, zip(*self.valid_locations))
         cols = sorted(cols)
         rows = sorted(rows)
 
         # set up SiPM labels and comboboxes
         for sipm, (column, row) in positions.items():
 
             column_base = col_start + col_offset * column
@@ -1191,14 +1194,19 @@
             label='Clear GUI and load defaults',
             command=self.clear_gui_load_defaults,
         )
         tool_menu.add_command(
             label='Clear cache',
             command=self.clear_cache,
         )
+        tool_menu.add_separator()
+        tool_menu.add_command(
+            label='Set default tray file directory',
+            command=self.set_default_tray_file_directory,
+        )
 
         # ------------------------------------------------------------------------
         sold_menu.add_command(
             label='Add solder syringe to database',
             command=self.add_solder_syringe_popup,
         )
 
@@ -1328,28 +1336,69 @@
         ----------------------------------------------------------------------
         args : none
         ----------------------------------------------------------------------
         returns : none
             GUI state changed
         ----------------------------------------------------------------------
         """
+        # load previously saved GUI default settings
         table_json = self.generic_load_json(self.defaults_file_path)
 
         self.update_gui_from_dict(table_json)
 
         try:
             institute_text = table_json['institute|None']
         except KeyError:
             # No institute name in defaults.
             pass
         else:
             # attempt to limit selection based on institute/date
             institute_id = self.dbi.get_institute_id(institute_text).data
             self.update_solder(institute_id)
 
+        # load default tray file location
+        table_json = self.generic_load_json(self.defaults_tray_file_path)
+
+        try:
+            dtf = table_json['tray_file_directory']
+        except KeyError:
+            self.print_to_console(
+                'Error reading tray file default directory from '
+                f'{self.defaults_tray_file_path}'
+            )
+        else:
+            if os.path.isdir(dtf):
+                self.tray_file_directory = dtf
+            else:
+                self.print_to_console(f'Default tray file directory does not exist: {dtf}')
+
+    def set_default_tray_file_directory(self):
+        """
+        ----------------------------------------------------------------------
+        args : none
+        ----------------------------------------------------------------------
+        returns : none
+        ----------------------------------------------------------------------
+        """
+        # filename will be a tuple for some reason
+        directory = filedialog.askdirectory(
+            initialdir=self.home_directory,
+            title='set default directory for tray files',
+        )
+
+        if directory:
+            self.tray_file_directory = directory
+
+            with open(self.defaults_tray_file_path, 'w', encoding='utf-8') as outfile:
+                outfile.write(
+                    json.dumps(
+                        {'tray_file_directory': directory}
+                    )
+                )
+
     @staticmethod
     def sipm_key(key):
         """
         Check if a string represents a SiPM.
 
         --------------------------------------------------------------------------
         args
@@ -1503,14 +1552,15 @@
                 Contains details of GUI widgets.
         ----------------------------------------------------------------------
         returns : none
             GUI state affected
         ----------------------------------------------------------------------
         """
         filename = filedialog.askopenfilename(
+            initialdir=self.home_directory,
             defaultextension='.json',
             filetypes=[
                 ('JSON Documents', '*.json'),
                 ('All Files', '*.*'),
             ],
             title='load saved GUI state',
         )
@@ -1720,14 +1770,15 @@
                 Contains details of GUI widgets.
         --------------------------------------------------------------------------
         returns : none
             GUI state affected
         --------------------------------------------------------------------------
         """
         filename = filedialog.askopenfilename(
+            initialdir=self.tray_file_directory,
             defaultextension='.txt',
             filetypes=[
                 ('TEXT Documents', '*.txt'),
                 ('All Files', '*.*'),
             ],
             title='load SiPM tray file',
         )
@@ -1859,15 +1910,15 @@
         text.tag_configure('center', justify='center')
         message = (
             '\n'
             '- POST vTile -\n'
             f'ds20kdb interface version {interface.__version__}\n'
             '\n'
             'Adds a veto-tile to the DarkSide-20k\n'
-            'pre-production database.\n'
+            'production database.\n'
             '\n'
             '- support -\n'
             'avt@hep.ph.liv.ac.uk'
         )
         text.insert(tk.END, message)
         text.tag_add(tk.CENTER, '1.0', tk.END)
         text.configure(state=tk.DISABLED)
@@ -2907,28 +2958,27 @@
         else:
             # run_number and comment require no transformation or look-up
             good = True
             table[cluster] = value
 
         self.set_label_colour(other_label_widget, good=good)
 
-    def process_sipm(self, table, used_sipms, valid_locations, sipm_definition, errors):
+    def process_sipm(self, table, used_sipms, sipm_definition, errors):
         """
         Process a single SiPM - check if the user-entered data makes sense:
 
         (1) Have all fields been entered?
         (2) Is the given (column, row) position a valid location on the wafer
         (3) Does the SiPM as defined by wafer and location exist in the
             database?
 
         ----------------------------------------------------------------------
         args
             table : dict
             used_sipms : dict
-            valid_locations : set
             sipm_definition : dict
             errors: list of strings
         ----------------------------------------------------------------------
         returns
             no explicit return, mutable types amended in place
                 errors: list of strings
                 table : dict
@@ -2949,15 +2999,15 @@
             column = sipm_params['column']
             row = sipm_params['row']
         except KeyError:
             # at least one field was missing
             errors.append(f'SiPM {sipm_num:>2}: missing field(s)')
             return
 
-        if (column, row) not in valid_locations:
+        if (column, row) not in self.valid_locations:
             errors.append(
                 f'SiPM {sipm_num:>2}: invalid wafer location (col={column}, row={row})'
             )
             return
 
         # local/database checks
         #
@@ -3030,16 +3080,14 @@
         # container for deferred error messages
         errors = []
 
         ######################################################################
         # check values in user-entered comboboxes - and recolour labels based
         # on their validity
 
-        valid_locations = set(interface.wafer_map_valid_locations())
-
         # e.g. {'year': '2024', 'month': '2', 'day': '3', 'hour': '3', 'minute': '15'})
         timestamp_parts = collections.defaultdict(dict)
 
         # e.g. {'sipm_1: {'lot_number': 9262109, 'wafer_number': 5, ...}, ...'}
         sipm_definitions = collections.defaultdict(dict)
 
         # e.g. {
@@ -3048,33 +3096,32 @@
         #          'qrcode': '22061703000047001',
         #          'run_number': '3'
         #      }
         other_definitions = {}
 
         # collect user-submitted information from GUI widgets
 
-        for widget in self.widgets:
-            if widget.itype != Itype.COMBOBOX:
-                continue
+        combobox_widgets = filter(lambda w: w.itype == Itype.COMBOBOX, self.widgets)
+
+        for widget in combobox_widgets:
 
             if 'sipm' in widget.cluster:
                 with contextlib.suppress(ValueError):
                     sipm_definitions[widget.cluster].update(
                         {widget.category: int(widget.instance.get())}
                     )
             elif widget.cluster == 'production_date':
                 timestamp_parts[widget.category] = widget.instance.get()
             else:
                 other_definitions[widget.cluster] = widget.instance.get()
 
         # check SiPMs, this sets table = {sipm_ident: sipm_pid, ...}
         for sipm_definition in sipm_definitions.items():
             self.process_sipm(
-                table, used_sipms, valid_locations,
-                sipm_definition, errors
+                table, used_sipms, sipm_definition, errors
             )
 
         ######################################################################
         # issue warnings about any locally (GUI) duplicated SiPMs
         for sipm_numbers in used_sipms.values():
             if len(sipm_numbers) < 2:
                 continue
@@ -3167,20 +3214,20 @@
         # Issue reminder for Liverpool
 
         # Liverpool uses version control for SiPM tray files. It's easy to
         # forget to use git pull to ensure the latest files are being used, so
         # remind the user before they press the SUBMIT button.
         if 'Liverpool' in other_definitions['institute']:
             self.print_to_console(
-                f'WARNING: is this tray file up to date? Remember to use "git pull".\n'
+                'WARNING: is this tray file up to date? Remember to use "git pull".\n'
             )
 
     def submit(self):
         """
-        POST vTile to the pre-production database.
+        POST vTile to the production database.
 
         ----------------------------------------------------------------------
         args : none
         ----------------------------------------------------------------------
         returns
             Error log written to console.
         ----------------------------------------------------------------------
@@ -3323,15 +3370,15 @@
 
     return table_json
 
 
 ##############################################################################
 def main():
     """
-    GUI for POSTing DarkSide-20k vTiles to the pre-production database.
+    GUI for POSTing DarkSide-20k vTiles to the production database.
 
     A 1024 x 576 pixel window should fit into any modern computer display
     without needing scrollbars.
     """
     gui = Gui()
     gui.run()
```

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile_json.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile_json.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/veto_location.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/veto_location.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/veto_location_gui.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/veto_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/visual.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_location_gui.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_map_from_db.py` & `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_map_from_db.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.4
+Version: 1.0.5
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

