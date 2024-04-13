# Comparing `tmp/ds20kdb_avt-1.0.5.tar.gz` & `tmp/ds20kdb_avt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb_avt-1.0.5.tar", last modified: Sat Apr 13 17:08:31 2024, max compression
+gzip compressed data, was "ds20kdb_avt-1.0.6.tar", last modified: Sat Apr 13 17:35:59 2024, max compression
```

## Comparing `ds20kdb_avt-1.0.5.tar` & `ds20kdb_avt-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.964714 ds20kdb_avt-1.0.5/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:08:31.963760 ds20kdb_avt-1.0.5/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb_avt-1.0.5/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 17:08:31.964925 ds20kdb_avt-1.0.5/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 17:08:12.000000 ds20kdb_avt-1.0.5/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.922153 ds20kdb_avt-1.0.5/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.954575 ds20kdb_avt-1.0.5/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb_avt-1.0.5/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb_avt-1.0.5/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.5/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb_avt-1.0.5/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb_avt-1.0.5/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb_avt-1.0.5/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb_avt-1.0.5/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   120272 2024-04-13 16:20:01.000000 ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.5/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.5/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb_avt-1.0.5/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb_avt-1.0.5/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.5/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:08:31.962691 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 17:08:31.000000 ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:35:59.331123 ds20kdb_avt-1.0.6/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.6/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:35:59.330210 ds20kdb_avt-1.0.6/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb_avt-1.0.6/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.6/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 17:35:59.331313 ds20kdb_avt-1.0.6/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 17:35:43.000000 ds20kdb_avt-1.0.6/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:35:59.302467 ds20kdb_avt-1.0.6/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:35:59.321618 ds20kdb_avt-1.0.6/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.6/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb_avt-1.0.6/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.6/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb_avt-1.0.6/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.6/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb_avt-1.0.6/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb_avt-1.0.6/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb_avt-1.0.6/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb_avt-1.0.6/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.6/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   120315 2024-04-13 17:35:32.000000 ds20kdb_avt-1.0.6/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.6/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.6/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.6/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb_avt-1.0.6/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb_avt-1.0.6/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb_avt-1.0.6/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb_avt-1.0.6/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.6/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 17:35:59.328826 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 17:35:59.000000 ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb_avt-1.0.5/PKG-INFO` & `ds20kdb_avt-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.5
+Version: 1.0.6
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb_avt-1.0.5/README.md` & `ds20kdb_avt-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/setup.py` & `ds20kdb_avt-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.5",
+    version="1.0.6",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/auth.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/common.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/common.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/create_credentials_file.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/gen_tray_files_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/interface.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/interface.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/qr.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/qrgen.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/scanner_auto.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/scanner_auto.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/submit_vtile.py`

 * *Files 0% similar despite different names*

```diff
@@ -3199,30 +3199,31 @@
         ######################################################################
         self.print_to_console(
             f'Check complete: {timestamp_to_utc_ds20k(time.time())}\n'
         )
 
         ######################################################################
         # if the check passed, we can enable the submit button
+        complete = len(table) == 30
 
         button_submit_widget = next(
             w.instance for w in self.widgets
             if w.cluster == 'submit' and w.itype == Itype.BUTTON
         )
-        self.set_button_state(button_submit_widget, disabled=len(table) != 30)
+        self.set_button_state(button_submit_widget, disabled=not complete)
 
         ######################################################################
         # Issue reminder for Liverpool
 
         # Liverpool uses version control for SiPM tray files. It's easy to
         # forget to use git pull to ensure the latest files are being used, so
         # remind the user before they press the SUBMIT button.
-        if 'Liverpool' in other_definitions['institute']:
+        if complete and 'Liverpool' in other_definitions['institute']:
             self.print_to_console(
-                'WARNING: is this tray file up to date? Remember to use "git pull".\n'
+                'CHECK: is this tray file up to date? Remember to use "git pull".\n'
             )
 
     def submit(self):
         """
         POST vTile to the production database.
 
         ----------------------------------------------------------------------
```

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/submit_vtile_json.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/submit_vtile_json.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/veto_location.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/veto_location.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/veto_location_gui.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/veto_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/visual.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_location_gui.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb/wafer_map_from_db.py` & `ds20kdb_avt-1.0.6/src/ds20kdb/wafer_map_from_db.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.5
+Version: 1.0.6
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.5/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb_avt-1.0.6/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

