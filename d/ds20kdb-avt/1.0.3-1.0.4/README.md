# Comparing `tmp/ds20kdb-avt-1.0.3.tar.gz` & `tmp/ds20kdb-avt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb-avt-1.0.3.tar", last modified: Thu Apr 11 07:49:10 2024, max compression
+gzip compressed data, was "ds20kdb-avt-1.0.4.tar", last modified: Sat Apr 13 12:42:10 2024, max compression
```

## Comparing `ds20kdb-avt-1.0.3.tar` & `ds20kdb-avt-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.418032 ds20kdb-avt-1.0.3/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-11 07:49:10.417028 ds20kdb-avt-1.0.3/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.3/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-11 07:49:10.418317 ds20kdb-avt-1.0.3/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-11 07:48:39.000000 ds20kdb-avt-1.0.3/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.380797 ds20kdb-avt-1.0.3/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.408246 ds20kdb-avt-1.0.3/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.3/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.3/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.3/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb-avt-1.0.3/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93422 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.3/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.3/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   117866 2024-03-28 13:27:09.000000 ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.3/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.3/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.3/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8909 2023-09-17 11:55:13.000000 ds20kdb-avt-1.0.3/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.3/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-11 07:49:10.415727 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-11 07:49:10.000000 ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.303754 ds20kdb-avt-1.0.4/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 12:42:10.302857 ds20kdb-avt-1.0.4/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.4/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 12:42:10.303969 ds20kdb-avt-1.0.4/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 12:41:51.000000 ds20kdb-avt-1.0.4/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.269683 ds20kdb-avt-1.0.4/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.294012 ds20kdb-avt-1.0.4/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.4/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.4/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.4/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb-avt-1.0.4/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb-avt-1.0.4/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.4/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.4/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   118397 2024-04-13 12:40:49.000000 ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.4/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.4/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.4/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb-avt-1.0.4/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.4/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 12:42:10.301742 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 12:42:10.000000 ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb-avt-1.0.3/PKG-INFO` & `ds20kdb-avt-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.3
+Version: 1.0.4
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.3/README.md` & `ds20kdb-avt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/setup.py` & `ds20kdb-avt-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.3",
+    version="1.0.4",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/auth.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/common.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/common.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/create_credentials_file.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/gen_tray_files_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/interface.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -2966,2874 +2966,2875 @@
 0000b950: 2548 3a25 4d3a 2553 270a 2020 2020 2020  %H:%M:%S'.      
 0000b960: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
 0000b970: 2020 2020 6474 5f72 7464 5f70 3330 203d      dt_rtd_p30 =
 0000b980: 2064 745f 7274 6420 2b20 6461 7465 7469   dt_rtd + dateti
 0000b990: 6d65 2e74 696d 6564 656c 7461 2864 6179  me.timedelta(day
 0000b9a0: 733d 3330 290a 0a20 2020 2020 2020 2020  s=30)..         
 0000b9b0: 2020 2072 6574 7572 6e20 6474 5f6e 6f77     return dt_now
-0000b9c0: 203c 2064 745f 6578 7020 6f72 2064 745f   < dt_exp or dt_
-0000b9d0: 6e6f 7720 3c20 6474 5f72 7464 5f70 3330  now < dt_rtd_p30
-0000b9e0: 0a0a 2020 2020 2020 2020 7661 6c69 6420  ..        valid 
-0000b9f0: 3d20 6675 6e63 746f 6f6c 732e 7061 7274  = functools.part
-0000ba00: 6961 6c28 7373 5f76 616c 6964 2c20 6474  ial(ss_valid, dt
-0000ba10: 5f6e 6f77 3d64 6174 6574 696d 652e 6461  _now=datetime.da
-0000ba20: 7465 7469 6d65 2e6e 6f77 2829 290a 0a20  tetime.now()).. 
-0000ba30: 2020 2020 2020 2072 6574 7572 6e20 5b73         return [s
-0000ba40: 6f6c 645b 2773 6f6c 6465 725f 7069 6427  old['solder_pid'
-0000ba50: 5d20 666f 7220 736f 6c64 2069 6e20 7265  ] for sold in re
-0000ba60: 7476 616c 2069 6620 7661 6c69 6428 736f  tval if valid(so
-0000ba70: 6c64 295d 0a0a 2020 2020 6465 6620 6765  ld)]..    def ge
-0000ba80: 745f 7369 706d 735f 616c 6c6f 6361 7465  t_sipms_allocate
-0000ba90: 6428 7365 6c66 2c20 7369 706d 5f70 6964  d(self, sipm_pid
-0000baa0: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-0000bab0: 2020 2020 2020 2020 496e 6469 6361 7465          Indicate
-0000bac0: 2069 6620 7468 6520 6769 7665 6e20 7369   if the given si
-0000bad0: 706d 5f70 6964 2873 2920 6861 7665 2062  pm_pid(s) have b
-0000bae0: 6565 6e20 616c 6c6f 6361 7465 6420 746f  een allocated to
-0000baf0: 2076 5469 6c65 2873 292e 0a0a 2020 2020   vTile(s)...    
-0000bb00: 2020 2020 5468 6572 6520 6172 6520 7477      There are tw
-0000bb10: 6f20 7761 7973 206f 6620 6170 7072 6f61  o ways of approa
-0000bb20: 6368 696e 6720 7468 6973 206f 7065 7261  ching this opera
-0000bb30: 7469 6f6e 2c20 2831 2920 6f62 7461 696e  tion, (1) obtain
-0000bb40: 2074 6865 0a20 2020 2020 2020 2077 686f   the.        who
-0000bb50: 6c65 2076 7469 6c65 2074 6162 6c65 2077  le vtile table w
-0000bb60: 6974 6820 6120 7369 6e67 6c65 2047 4554  ith a single GET
-0000bb70: 206f 7065 7261 7469 6f6e 2061 6e64 2070   operation and p
-0000bb80: 6572 666f 726d 2074 6865 2073 6561 7263  erform the searc
-0000bb90: 680a 2020 2020 2020 2020 6c6f 6361 6c6c  h.        locall
-0000bba0: 7920 2861 7320 646f 6e65 2069 6e20 7468  y (as done in th
-0000bbb0: 6973 206d 6574 686f 6429 206f 7220 2832  is method) or (2
-0000bbc0: 2920 6d61 6b65 2032 3420 7461 7267 6574  ) make 24 target
-0000bbd0: 6564 2047 4554 0a20 2020 2020 2020 206f  ed GET.        o
-0000bbe0: 7065 7261 7469 6f6e 7320 2d20 6f6e 6520  perations - one 
-0000bbf0: 666f 7220 6561 6368 2053 6950 4d20 636f  for each SiPM co
-0000bc00: 6c75 6d6e 202d 206c 6574 7469 6e67 2074  lumn - letting t
-0000bc10: 6865 2064 6220 7065 7266 6f72 6d20 7468  he db perform th
-0000bc20: 650a 2020 2020 2020 2020 7365 6172 6368  e.        search
-0000bc30: 206f 7065 7261 7469 6f6e 2e0a 0a20 2020   operation...   
-0000bc40: 2020 2020 2054 6865 206c 6174 7465 7220       The latter 
-0000bc50: 7368 6f75 6c64 2070 6572 666f 726d 2062  should perform b
-0000bc60: 6574 7465 7220 7768 656e 2074 6865 2064  etter when the d
-0000bc70: 6174 6162 6173 6520 6675 6c6c 7920 706f  atabase fully po
-0000bc80: 7075 6c61 7465 642c 0a20 2020 2020 2020  pulated,.       
-0000bc90: 2062 7574 2069 6e20 7072 652d 7072 6f64   but in pre-prod
-0000bca0: 7563 7469 6f6e 2074 6869 7320 6973 2061  uction this is a
-0000bcb0: 6e20 6f72 6465 7220 6f66 206d 6167 6e69  n order of magni
-0000bcc0: 7475 6465 2073 6c6f 7765 722c 2065 2e67  tude slower, e.g
-0000bcd0: 2e0a 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0000bce0: 6e20 616e 7928 0a20 2020 2020 2020 2020  n any(.         
-0000bcf0: 2020 206e 6f74 2073 656c 662e 6765 7428     not self.get(
-0000bd00: 2776 7469 6c65 272c 202a 2a7b 633a 2073  'vtile', **{c: s
-0000bd10: 6970 6d5f 7069 647d 292e 6461 7461 2e65  ipm_pid}).data.e
-0000bd20: 6d70 7479 0a20 2020 2020 2020 2020 2020  mpty.           
-0000bd30: 2066 6f72 2063 2069 6e20 7369 706d 5f63   for c in sipm_c
-0000bd40: 6f6c 756d 6e73 0a20 2020 2020 2020 2029  olumns.        )
-0000bd50: 0a0a 2020 2020 2020 2020 436f 6c75 6d6e  ..        Column
-0000bd60: 206e 616d 6573 2063 616e 2061 6c73 6f20   names can also 
-0000bd70: 6265 206f 6274 6169 6e65 6420 6672 6f6d  be obtained from
-0000bd80: 2074 6865 2064 6174 6162 6173 6520 6966   the database if
-0000bd90: 2072 6571 7569 7265 643a 0a0a 2020 2020   required:..    
-0000bda0: 2020 2020 7369 706d 5f63 6f6c 756d 6e73      sipm_columns
-0000bdb0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0000bdc0: 2063 2066 6f72 2063 2069 6e20 7365 6c66   c for c in self
-0000bdd0: 2e64 6573 6372 6962 6528 2776 7469 6c65  .describe('vtile
-0000bde0: 2729 2e64 6174 6120 6966 2063 2e73 7461  ').data if c.sta
-0000bdf0: 7274 7377 6974 6828 2773 6970 6d5f 2729  rtswith('sipm_')
-0000be00: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000be10: 2020 2020 5741 524e 494e 473a 2054 6869      WARNING: Thi
-0000be20: 7320 6d65 7468 6f64 2077 696c 6c20 6265  s method will be
-0000be30: 636f 6d65 2065 7870 656e 7369 7665 2074  come expensive t
-0000be40: 6f20 7275 6e20 6f6e 6365 2074 6865 2064  o run once the d
-0000be50: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-0000be60: 6265 636f 6d65 7320 6d6f 7265 2070 6f70  becomes more pop
-0000be70: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
-0000be80: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000b9c0: 203c 3d20 6474 5f65 7870 2061 6e64 2064   <= dt_exp and d
+0000b9d0: 745f 6e6f 7720 3c3d 2064 745f 7274 645f  t_now <= dt_rtd_
+0000b9e0: 7033 300a 0a20 2020 2020 2020 2076 616c  p30..        val
+0000b9f0: 6964 203d 2066 756e 6374 6f6f 6c73 2e70  id = functools.p
+0000ba00: 6172 7469 616c 2873 735f 7661 6c69 642c  artial(ss_valid,
+0000ba10: 2064 745f 6e6f 773d 6461 7465 7469 6d65   dt_now=datetime
+0000ba20: 2e64 6174 6574 696d 652e 6e6f 7728 2929  .datetime.now())
+0000ba30: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000ba40: 205b 736f 6c64 5b27 736f 6c64 6572 5f70   [sold['solder_p
+0000ba50: 6964 275d 2066 6f72 2073 6f6c 6420 696e  id'] for sold in
+0000ba60: 2072 6574 7661 6c20 6966 2076 616c 6964   retval if valid
+0000ba70: 2873 6f6c 6429 5d0a 0a20 2020 2064 6566  (sold)]..    def
+0000ba80: 2067 6574 5f73 6970 6d73 5f61 6c6c 6f63   get_sipms_alloc
+0000ba90: 6174 6564 2873 656c 662c 2073 6970 6d5f  ated(self, sipm_
+0000baa0: 7069 6473 293a 0a20 2020 2020 2020 2022  pids):.        "
+0000bab0: 2222 0a20 2020 2020 2020 2049 6e64 6963  "".        Indic
+0000bac0: 6174 6520 6966 2074 6865 2067 6976 656e  ate if the given
+0000bad0: 2073 6970 6d5f 7069 6428 7329 2068 6176   sipm_pid(s) hav
+0000bae0: 6520 6265 656e 2061 6c6c 6f63 6174 6564  e been allocated
+0000baf0: 2074 6f20 7654 696c 6528 7329 2e0a 0a20   to vTile(s)... 
+0000bb00: 2020 2020 2020 2054 6865 7265 2061 7265         There are
+0000bb10: 2074 776f 2077 6179 7320 6f66 2061 7070   two ways of app
+0000bb20: 726f 6163 6869 6e67 2074 6869 7320 6f70  roaching this op
+0000bb30: 6572 6174 696f 6e2c 2028 3129 206f 6274  eration, (1) obt
+0000bb40: 6169 6e20 7468 650a 2020 2020 2020 2020  ain the.        
+0000bb50: 7768 6f6c 6520 7674 696c 6520 7461 626c  whole vtile tabl
+0000bb60: 6520 7769 7468 2061 2073 696e 676c 6520  e with a single 
+0000bb70: 4745 5420 6f70 6572 6174 696f 6e20 616e  GET operation an
+0000bb80: 6420 7065 7266 6f72 6d20 7468 6520 7365  d perform the se
+0000bb90: 6172 6368 0a20 2020 2020 2020 206c 6f63  arch.        loc
+0000bba0: 616c 6c79 2028 6173 2064 6f6e 6520 696e  ally (as done in
+0000bbb0: 2074 6869 7320 6d65 7468 6f64 2920 6f72   this method) or
+0000bbc0: 2028 3229 206d 616b 6520 3234 2074 6172   (2) make 24 tar
+0000bbd0: 6765 7465 6420 4745 540a 2020 2020 2020  geted GET.      
+0000bbe0: 2020 6f70 6572 6174 696f 6e73 202d 206f    operations - o
+0000bbf0: 6e65 2066 6f72 2065 6163 6820 5369 504d  ne for each SiPM
+0000bc00: 2063 6f6c 756d 6e20 2d20 6c65 7474 696e   column - lettin
+0000bc10: 6720 7468 6520 6462 2070 6572 666f 726d  g the db perform
+0000bc20: 2074 6865 0a20 2020 2020 2020 2073 6561   the.        sea
+0000bc30: 7263 6820 6f70 6572 6174 696f 6e2e 0a0a  rch operation...
+0000bc40: 2020 2020 2020 2020 5468 6520 6c61 7474          The latt
+0000bc50: 6572 2073 686f 756c 6420 7065 7266 6f72  er should perfor
+0000bc60: 6d20 6265 7474 6572 2077 6865 6e20 7468  m better when th
+0000bc70: 6520 6461 7461 6261 7365 2066 756c 6c79  e database fully
+0000bc80: 2070 6f70 756c 6174 6564 2c0a 2020 2020   populated,.    
+0000bc90: 2020 2020 6275 7420 696e 2070 7265 2d70      but in pre-p
+0000bca0: 726f 6475 6374 696f 6e20 7468 6973 2069  roduction this i
+0000bcb0: 7320 616e 206f 7264 6572 206f 6620 6d61  s an order of ma
+0000bcc0: 676e 6974 7564 6520 736c 6f77 6572 2c20  gnitude slower, 
+0000bcd0: 652e 672e 0a0a 2020 2020 2020 2020 7265  e.g...        re
+0000bce0: 7475 726e 2061 6e79 280a 2020 2020 2020  turn any(.      
+0000bcf0: 2020 2020 2020 6e6f 7420 7365 6c66 2e67        not self.g
+0000bd00: 6574 2827 7674 696c 6527 2c20 2a2a 7b63  et('vtile', **{c
+0000bd10: 3a20 7369 706d 5f70 6964 7d29 2e64 6174  : sipm_pid}).dat
+0000bd20: 612e 656d 7074 790a 2020 2020 2020 2020  a.empty.        
+0000bd30: 2020 2020 666f 7220 6320 696e 2073 6970      for c in sip
+0000bd40: 6d5f 636f 6c75 6d6e 730a 2020 2020 2020  m_columns.      
+0000bd50: 2020 290a 0a20 2020 2020 2020 2043 6f6c    )..        Col
+0000bd60: 756d 6e20 6e61 6d65 7320 6361 6e20 616c  umn names can al
+0000bd70: 736f 2062 6520 6f62 7461 696e 6564 2066  so be obtained f
+0000bd80: 726f 6d20 7468 6520 6461 7461 6261 7365  rom the database
+0000bd90: 2069 6620 7265 7175 6972 6564 3a0a 0a20   if required:.. 
+0000bda0: 2020 2020 2020 2073 6970 6d5f 636f 6c75         sipm_colu
+0000bdb0: 6d6e 7320 3d20 280a 2020 2020 2020 2020  mns = (.        
+0000bdc0: 2020 2020 6320 666f 7220 6320 696e 2073      c for c in s
+0000bdd0: 656c 662e 6465 7363 7269 6265 2827 7674  elf.describe('vt
+0000bde0: 696c 6527 292e 6461 7461 2069 6620 632e  ile').data if c.
+0000bdf0: 7374 6172 7473 7769 7468 2827 7369 706d  startswith('sipm
+0000be00: 5f27 290a 2020 2020 2020 2020 290a 0a20  _').        ).. 
+0000be10: 2020 2020 2020 2057 4152 4e49 4e47 3a20         WARNING: 
+0000be20: 5468 6973 206d 6574 686f 6420 7769 6c6c  This method will
+0000be30: 2062 6563 6f6d 6520 6578 7065 6e73 6976   become expensiv
+0000be40: 6520 746f 2072 756e 206f 6e63 6520 7468  e to run once th
+0000be50: 6520 6461 7461 6261 7365 0a20 2020 2020  e database.     
+0000be60: 2020 2062 6563 6f6d 6573 206d 6f72 6520     becomes more 
+0000be70: 706f 7075 6c61 7465 642e 0a0a 2020 2020  populated...    
+0000be80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 0000be90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000bea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000beb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bec0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000bed0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-0000bee0: 2073 6970 6d5f 7069 6473 203a 2069 7465   sipm_pids : ite
-0000bef0: 7261 626c 6520 2863 6f6e 7461 696e 696e  rable (containin
-0000bf00: 6720 696e 7428 7329 290a 2020 2020 2020  g int(s)).      
-0000bf10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000bec0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000bed0: 2020 2061 7267 730a 2020 2020 2020 2020     args.        
+0000bee0: 2020 2020 7369 706d 5f70 6964 7320 3a20      sipm_pids : 
+0000bef0: 6974 6572 6162 6c65 2028 636f 6e74 6169  iterable (contai
+0000bf00: 6e69 6e67 2069 6e74 2873 2929 0a20 2020  ning int(s)).   
+0000bf10: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 0000bf20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000bf30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000bf40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bf50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000bf60: 2072 6574 7572 6e73 203a 2064 6963 7420   returns : dict 
-0000bf70: 286f 7220 4e6f 6e65 2069 6620 7468 6520  (or None if the 
-0000bf80: 6361 6c6c 6572 2073 7570 706c 6965 6420  caller supplied 
-0000bf90: 6120 6e6f 6e2d 6974 6572 6162 6c65 290a  a non-iterable).
-0000bfa0: 2020 2020 2020 2020 2020 2020 7b73 6970              {sip
-0000bfb0: 6d5f 7069 643a 2054 7275 6520 6966 2061  m_pid: True if a
-0000bfc0: 6c6c 6f63 6174 6564 7d0a 2020 2020 2020  llocated}.      
-0000bfd0: 2020 2020 2020 2020 2020 452e 672e 207b            E.g. {
-0000bfe0: 3139 3a20 5472 7565 2c20 3333 3a20 5472  19: True, 33: Tr
-0000bff0: 7565 2c20 3130 3030 3030 303a 2046 616c  ue, 1000000: Fal
-0000c000: 7365 7d0a 2020 2020 2020 2020 2d2d 2d2d  se}.        ----
+0000bf50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000bf60: 2020 2020 7265 7475 726e 7320 3a20 6469      returns : di
+0000bf70: 6374 2028 6f72 204e 6f6e 6520 6966 2074  ct (or None if t
+0000bf80: 6865 2063 616c 6c65 7220 7375 7070 6c69  he caller suppli
+0000bf90: 6564 2061 206e 6f6e 2d69 7465 7261 626c  ed a non-iterabl
+0000bfa0: 6529 0a20 2020 2020 2020 2020 2020 207b  e).            {
+0000bfb0: 7369 706d 5f70 6964 3a20 5472 7565 2069  sipm_pid: True i
+0000bfc0: 6620 616c 6c6f 6361 7465 647d 0a20 2020  f allocated}.   
+0000bfd0: 2020 2020 2020 2020 2020 2020 2045 2e67               E.g
+0000bfe0: 2e20 7b31 393a 2054 7275 652c 2033 333a  . {19: True, 33:
+0000bff0: 2054 7275 652c 2031 3030 3030 3030 3a20   True, 1000000: 
+0000c000: 4661 6c73 657d 0a20 2020 2020 2020 202d  False}.        -
 0000c010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c050: 2d2d 0a20 2020 2020 2020 2022 2222 0a20  --.        """. 
-0000c060: 2020 2020 2020 2076 7469 6c65 5f74 6162         vtile_tab
-0000c070: 6c65 203d 2073 656c 662e 6765 7428 2776  le = self.get('v
-0000c080: 7469 6c65 2729 2e64 6174 610a 0a20 2020  tile').data..   
-0000c090: 2020 2020 2073 6970 6d5f 636f 6c75 6d6e       sipm_column
-0000c0a0: 7320 3d20 2866 2773 6970 6d5f 7b78 7d27  s = (f'sipm_{x}'
-0000c0b0: 2066 6f72 2078 2069 6e20 7261 6e67 6528   for x in range(
-0000c0c0: 312c 2032 342b 3129 290a 2020 2020 2020  1, 24+1)).      
-0000c0d0: 2020 616c 6c5f 7369 706d 7320 3d20 7365    all_sipms = se
-0000c0e0: 7428 6974 6572 746f 6f6c 732e 6368 6169  t(itertools.chai
-0000c0f0: 6e28 2a76 7469 6c65 5f74 6162 6c65 5b73  n(*vtile_table[s
-0000c100: 6970 6d5f 636f 6c75 6d6e 735d 2e76 616c  ipm_columns].val
-0000c110: 7565 7329 290a 0a20 2020 2020 2020 2074  ues))..        t
-0000c120: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000c130: 7265 7475 726e 207b 733a 2073 2069 6e20  return {s: s in 
-0000c140: 616c 6c5f 7369 706d 7320 666f 7220 7320  all_sipms for s 
-0000c150: 696e 2073 6970 6d5f 7069 6473 7d0a 2020  in sipm_pids}.  
-0000c160: 2020 2020 2020 6578 6365 7074 2054 7970        except Typ
-0000c170: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-0000c180: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0000c190: 0a20 2020 2064 6566 2067 6574 5f74 6162  .    def get_tab
-0000c1a0: 6c65 5f72 6f77 5f61 6e64 5f6d 6f64 6966  le_row_and_modif
-0000c1b0: 7928 7365 6c66 2c20 7461 626c 655f 6e61  y(self, table_na
-0000c1c0: 6d65 2c20 7365 6c65 6374 2c20 7265 706c  me, select, repl
-0000c1d0: 6163 656d 656e 7473 3d4e 6f6e 652c 206f  acements=None, o
-0000c1e0: 6d69 745f 7069 643d 5472 7565 293a 0a20  mit_pid=True):. 
-0000c1f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c200: 2020 2047 656e 6572 6963 206d 6574 686f     Generic metho
-0000c210: 6420 7468 6174 2072 6561 6473 2061 2072  d that reads a r
-0000c220: 6f77 2066 726f 6d20 6120 7265 6d6f 7465  ow from a remote
-0000c230: 2064 6174 6162 6173 6520 7461 626c 652c   database table,
-0000c240: 0a20 2020 2020 2020 2072 6570 6c61 6365  .        replace
-0000c250: 7320 7661 6c75 6573 206f 6620 6769 7665  s values of give
-0000c260: 6e20 6669 656c 6473 2c20 7468 656e 2072  n fields, then r
-0000c270: 6574 7572 6e73 2074 6865 2072 6573 756c  eturns the resul
-0000c280: 7420 6173 2061 2064 6963 740a 2020 2020  t as a dict.    
-0000c290: 2020 2020 2877 6869 6368 206d 6179 2074      (which may t
-0000c2a0: 6865 6e20 6265 2050 4f53 5465 6420 746f  hen be POSTed to
-0000c2b0: 2074 6865 2064 6174 6162 6173 6520 6c61   the database la
-0000c2c0: 7465 7229 2e0a 0a20 2020 2020 2020 2047  ter)...        G
-0000c2d0: 6976 656e 2074 6861 7420 7468 6973 2066  iven that this f
-0000c2e0: 756e 6374 696f 6e20 6973 2067 656e 6572  unction is gener
-0000c2f0: 6963 2069 6e20 6e61 7475 7265 2c20 6974  ic in nature, it
-0000c300: 2077 6f6e 2774 2063 6f6d 706c 6169 6e20   won't complain 
-0000c310: 746f 6f0a 2020 2020 2020 2020 6c6f 7564  too.        loud
-0000c320: 6c79 2069 6620 6d6f 7265 2074 6861 6e20  ly if more than 
-0000c330: 6f6e 6520 726f 7720 7761 7320 7265 7475  one row was retu
-0000c340: 726e 6564 2066 726f 6d20 7468 6520 4745  rned from the GE
-0000c350: 5420 6f70 6572 6174 696f 6e2c 2069 740a  T operation, it.
-0000c360: 2020 2020 2020 2020 7369 6d70 6c79 2072          simply r
-0000c370: 6574 7572 6e73 2074 6865 206c 6173 7420  eturns the last 
-0000c380: 726f 772e 2054 6869 7320 6265 6861 7669  row. This behavi
-0000c390: 6f75 7220 6973 206e 6f74 2070 6172 7469  our is not parti
-0000c3a0: 6375 6c61 726c 790a 2020 2020 2020 2020  cularly.        
-0000c3b0: 6465 7369 7261 626c 6520 6e6f 772c 2062  desirable now, b
-0000c3c0: 7574 206d 6179 2062 6520 736f 2061 7420  ut may be so at 
-0000c3d0: 736f 6d65 2073 7461 6765 2069 6e20 7468  some stage in th
-0000c3e0: 6520 6675 7475 7265 2077 6865 6e20 7468  e future when th
-0000c3f0: 650a 2020 2020 2020 2020 6461 7461 6261  e.        databa
-0000c400: 7365 206d 6179 2073 7570 706f 7274 206d  se may support m
-0000c410: 756c 7469 706c 6520 7461 626c 6520 726f  ultiple table ro
-0000c420: 7773 2077 6974 6820 7468 6520 7361 6d65  ws with the same
-0000c430: 2050 4944 2066 6965 6c64 0a20 2020 2020   PID field.     
-0000c440: 2020 2076 616c 7565 3b20 6461 7461 6261     value; databa
-0000c450: 7365 2068 6f75 7365 6b65 6570 696e 6720  se housekeeping 
-0000c460: 6d61 7920 7468 656e 2063 6f6e 736f 6c69  may then consoli
-0000c470: 6461 7465 2074 6865 6d20 6c61 7465 7220  date them later 
-0000c480: 696e 746f 2061 0a20 2020 2020 2020 2073  into a.        s
-0000c490: 696e 676c 6520 726f 772e 2054 6869 7320  ingle row. This 
-0000c4a0: 6265 6861 7669 6f75 7220 6d61 7920 6265  behaviour may be
-0000c4b0: 2070 726f 626c 656d 6174 6963 2069 6e20   problematic in 
-0000c4c0: 7468 6520 6361 7365 2077 6865 7265 2074  the case where t
-0000c4d0: 6865 0a20 2020 2020 2020 2063 616c 6c65  he.        calle
-0000c4e0: 7227 7320 7365 6c65 6374 696f 6e20 6f66  r's selection of
-0000c4f0: 2072 6f77 7320 6973 2074 6f6f 2062 726f   rows is too bro
-0000c500: 6164 2e0a 0a20 2020 2020 2020 2046 6965  ad...        Fie
-0000c510: 6c64 7320 2877 6869 6368 206d 6170 2074  lds (which map t
-0000c520: 6f20 4461 7461 4672 616d 6520 636f 6c75  o DataFrame colu
-0000c530: 6d6e 7329 2074 6861 7420 636f 6e74 6169  mns) that contai
-0000c540: 6e20 4e61 4e2f 4e61 5420 7661 6c75 6573  n NaN/NaT values
-0000c550: 0a20 2020 2020 2020 2061 7265 2072 656d  .        are rem
-0000c560: 6f76 6564 2e0a 0a20 2020 2020 2020 2045  oved...        E
-0000c570: 2e67 2e20 746f 2061 6464 2061 206e 6577  .g. to add a new
-0000c580: 2069 6e64 6975 6d20 736f 6c64 6572 2073   indium solder s
-0000c590: 7972 696e 6765 2074 6f20 7468 6520 6461  yringe to the da
-0000c5a0: 7461 6261 7365 202d 2067 6976 656e 2074  tabase - given t
-0000c5b0: 6861 740a 2020 2020 2020 2020 6d61 6e79  hat.        many
-0000c5c0: 2066 6965 6c64 7320 7769 6c6c 2062 6520   fields will be 
-0000c5d0: 7369 6d69 6c61 7220 6265 7477 6565 6e20  similar between 
-0000c5e0: 7379 7269 6e67 6573 202d 2069 7420 6d61  syringes - it ma
-0000c5f0: 7920 6265 2068 656c 7066 756c 2074 6f0a  y be helpful to.
-0000c600: 2020 2020 2020 2020 6765 7420 616e 2065          get an e
-0000c610: 7869 7374 696e 6720 726f 7720 616e 6420  xisting row and 
-0000c620: 6d6f 6469 6679 2069 742e 2049 6e20 7468  modify it. In th
-0000c630: 6973 2069 6e73 7461 6e63 652c 2061 6464  is instance, add
-0000c640: 696e 6720 6120 7379 7269 6e67 650a 2020  ing a syringe.  
-0000c650: 2020 2020 2020 6672 6f6d 2074 6865 2073        from the s
-0000c660: 616d 6520 6c6f 7420 616e 6420 7468 6520  ame lot and the 
-0000c670: 7361 6d65 2069 6e73 7469 7475 7465 2c20  same institute, 
-0000c680: 7765 2063 616e 206a 7573 7420 6368 616e  we can just chan
-0000c690: 6765 2074 6865 0a20 2020 2020 2020 206c  ge the.        l
-0000c6a0: 6f63 616c 2073 7972 696e 6765 2050 4944  ocal syringe PID
-0000c6b0: 2074 6f20 6765 7420 6120 6469 6374 2073   to get a dict s
-0000c6c0: 7569 7461 626c 6520 666f 7220 504f 5354  uitable for POST
-0000c6d0: 696e 6720 6974 2074 6f20 7468 650a 2020  ing it to the.  
-0000c6e0: 2020 2020 2020 6461 7461 6261 7365 3a0a        database:.
-0000c6f0: 0a20 2020 2020 2020 2067 6574 5f74 6162  .        get_tab
-0000c700: 6c65 5f72 6f77 5f61 6e64 5f6d 6f64 6966  le_row_and_modif
-0000c710: 7928 0a20 2020 2020 2020 2020 2020 2027  y(.            '
-0000c720: 736f 6c64 6572 272c 207b 2773 6f6c 6465  solder', {'solde
-0000c730: 725f 7069 6427 3a20 317d 2c20 7b27 7379  r_pid': 1}, {'sy
-0000c740: 7269 6e67 655f 6964 273a 2031 327d 0a20  ringe_id': 12}. 
-0000c750: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000c760: 2020 5768 6963 6820 776f 756c 6420 7265    Which would re
-0000c770: 7475 726e 3a0a 0a20 2020 2020 2020 207b  turn:..        {
-0000c780: 0a20 2020 2020 2020 2020 2020 2027 6d61  .            'ma
-0000c790: 6e75 6661 6374 7572 6572 273a 2034 2c0a  nufacturer': 4,.
-0000c7a0: 2020 2020 2020 2020 2020 2020 2773 6f6c              'sol
-0000c7b0: 6465 725f 7479 7065 273a 2027 496e 6469  der_type': 'Indi
-0000c7c0: 756d 2050 6173 7465 204e 432d 534d 5138  um Paste NC-SMQ8
-0000c7d0: 3020 496e 6423 3145 2035 3249 6e34 3853  0 Ind#1E 52In48S
-0000c7e0: 6e20 5479 7065 2034 202e 2e2e 272c 0a20  n Type 4 ...',. 
-0000c7f0: 2020 2020 2020 2020 2020 2027 7072 6f64             'prod
-0000c800: 7563 7469 6f6e 5f64 6174 6527 3a20 2732  uction_date': '2
-0000c810: 3032 322d 3036 2d30 3220 3030 3a30 303a  022-06-02 00:00:
-0000c820: 3030 272c 0a20 2020 2020 2020 2020 2020  00',.           
-0000c830: 2027 726f 6f6d 5f74 656d 7065 7261 7475   'room_temperatu
-0000c840: 7265 5f64 6174 6527 3a20 2732 3032 322d  re_date': '2022-
-0000c850: 3037 2d31 3820 3136 3a30 303a 3030 272c  07-18 16:00:00',
-0000c860: 0a20 2020 2020 2020 2020 2020 2027 6578  .            'ex
-0000c870: 7069 7279 5f64 6174 6527 3a20 2732 3032  piry_date': '202
-0000c880: 322d 3132 2d30 3220 3030 3a30 303a 3030  2-12-02 00:00:00
-0000c890: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-0000c8a0: 7379 7269 6e67 655f 6964 273a 2031 322c  syringe_id': 12,
-0000c8b0: 2027 6c6f 7427 3a20 2750 5331 3131 3230   'lot': 'PS11120
-0000c8c0: 3733 3427 2c20 276d 6173 7327 3a20 3235  734', 'mass': 25
-0000c8d0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-0000c8e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000c050: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
+0000c060: 220a 2020 2020 2020 2020 7674 696c 655f  ".        vtile_
+0000c070: 7461 626c 6520 3d20 7365 6c66 2e67 6574  table = self.get
+0000c080: 2827 7674 696c 6527 292e 6461 7461 0a0a  ('vtile').data..
+0000c090: 2020 2020 2020 2020 7369 706d 5f63 6f6c          sipm_col
+0000c0a0: 756d 6e73 203d 2028 6627 7369 706d 5f7b  umns = (f'sipm_{
+0000c0b0: 787d 2720 666f 7220 7820 696e 2072 616e  x}' for x in ran
+0000c0c0: 6765 2831 2c20 3234 2b31 2929 0a20 2020  ge(1, 24+1)).   
+0000c0d0: 2020 2020 2061 6c6c 5f73 6970 6d73 203d       all_sipms =
+0000c0e0: 2073 6574 2869 7465 7274 6f6f 6c73 2e63   set(itertools.c
+0000c0f0: 6861 696e 282a 7674 696c 655f 7461 626c  hain(*vtile_tabl
+0000c100: 655b 7369 706d 5f63 6f6c 756d 6e73 5d2e  e[sipm_columns].
+0000c110: 7661 6c75 6573 2929 0a0a 2020 2020 2020  values))..      
+0000c120: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000c130: 2020 2072 6574 7572 6e20 7b73 3a20 7320     return {s: s 
+0000c140: 696e 2061 6c6c 5f73 6970 6d73 2066 6f72  in all_sipms for
+0000c150: 2073 2069 6e20 7369 706d 5f70 6964 737d   s in sipm_pids}
+0000c160: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000c170: 5479 7065 4572 726f 723a 0a20 2020 2020  TypeError:.     
+0000c180: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000c190: 6e65 0a0a 2020 2020 6465 6620 6765 745f  ne..    def get_
+0000c1a0: 7461 626c 655f 726f 775f 616e 645f 6d6f  table_row_and_mo
+0000c1b0: 6469 6679 2873 656c 662c 2074 6162 6c65  dify(self, table
+0000c1c0: 5f6e 616d 652c 2073 656c 6563 742c 2072  _name, select, r
+0000c1d0: 6570 6c61 6365 6d65 6e74 733d 4e6f 6e65  eplacements=None
+0000c1e0: 2c20 6f6d 6974 5f70 6964 3d54 7275 6529  , omit_pid=True)
+0000c1f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c200: 2020 2020 2020 4765 6e65 7269 6320 6d65        Generic me
+0000c210: 7468 6f64 2074 6861 7420 7265 6164 7320  thod that reads 
+0000c220: 6120 726f 7720 6672 6f6d 2061 2072 656d  a row from a rem
+0000c230: 6f74 6520 6461 7461 6261 7365 2074 6162  ote database tab
+0000c240: 6c65 2c0a 2020 2020 2020 2020 7265 706c  le,.        repl
+0000c250: 6163 6573 2076 616c 7565 7320 6f66 2067  aces values of g
+0000c260: 6976 656e 2066 6965 6c64 732c 2074 6865  iven fields, the
+0000c270: 6e20 7265 7475 726e 7320 7468 6520 7265  n returns the re
+0000c280: 7375 6c74 2061 7320 6120 6469 6374 0a20  sult as a dict. 
+0000c290: 2020 2020 2020 2028 7768 6963 6820 6d61         (which ma
+0000c2a0: 7920 7468 656e 2062 6520 504f 5354 6564  y then be POSTed
+0000c2b0: 2074 6f20 7468 6520 6461 7461 6261 7365   to the database
+0000c2c0: 206c 6174 6572 292e 0a0a 2020 2020 2020   later)...      
+0000c2d0: 2020 4769 7665 6e20 7468 6174 2074 6869    Given that thi
+0000c2e0: 7320 6675 6e63 7469 6f6e 2069 7320 6765  s function is ge
+0000c2f0: 6e65 7269 6320 696e 206e 6174 7572 652c  neric in nature,
+0000c300: 2069 7420 776f 6e27 7420 636f 6d70 6c61   it won't compla
+0000c310: 696e 2074 6f6f 0a20 2020 2020 2020 206c  in too.        l
+0000c320: 6f75 646c 7920 6966 206d 6f72 6520 7468  oudly if more th
+0000c330: 616e 206f 6e65 2072 6f77 2077 6173 2072  an one row was r
+0000c340: 6574 7572 6e65 6420 6672 6f6d 2074 6865  eturned from the
+0000c350: 2047 4554 206f 7065 7261 7469 6f6e 2c20   GET operation, 
+0000c360: 6974 0a20 2020 2020 2020 2073 696d 706c  it.        simpl
+0000c370: 7920 7265 7475 726e 7320 7468 6520 6c61  y returns the la
+0000c380: 7374 2072 6f77 2e20 5468 6973 2062 6568  st row. This beh
+0000c390: 6176 696f 7572 2069 7320 6e6f 7420 7061  aviour is not pa
+0000c3a0: 7274 6963 756c 6172 6c79 0a20 2020 2020  rticularly.     
+0000c3b0: 2020 2064 6573 6972 6162 6c65 206e 6f77     desirable now
+0000c3c0: 2c20 6275 7420 6d61 7920 6265 2073 6f20  , but may be so 
+0000c3d0: 6174 2073 6f6d 6520 7374 6167 6520 696e  at some stage in
+0000c3e0: 2074 6865 2066 7574 7572 6520 7768 656e   the future when
+0000c3f0: 2074 6865 0a20 2020 2020 2020 2064 6174   the.        dat
+0000c400: 6162 6173 6520 6d61 7920 7375 7070 6f72  abase may suppor
+0000c410: 7420 6d75 6c74 6970 6c65 2074 6162 6c65  t multiple table
+0000c420: 2072 6f77 7320 7769 7468 2074 6865 2073   rows with the s
+0000c430: 616d 6520 5049 4420 6669 656c 640a 2020  ame PID field.  
+0000c440: 2020 2020 2020 7661 6c75 653b 2064 6174        value; dat
+0000c450: 6162 6173 6520 686f 7573 656b 6565 7069  abase housekeepi
+0000c460: 6e67 206d 6179 2074 6865 6e20 636f 6e73  ng may then cons
+0000c470: 6f6c 6964 6174 6520 7468 656d 206c 6174  olidate them lat
+0000c480: 6572 2069 6e74 6f20 610a 2020 2020 2020  er into a.      
+0000c490: 2020 7369 6e67 6c65 2072 6f77 2e20 5468    single row. Th
+0000c4a0: 6973 2062 6568 6176 696f 7572 206d 6179  is behaviour may
+0000c4b0: 2062 6520 7072 6f62 6c65 6d61 7469 6320   be problematic 
+0000c4c0: 696e 2074 6865 2063 6173 6520 7768 6572  in the case wher
+0000c4d0: 6520 7468 650a 2020 2020 2020 2020 6361  e the.        ca
+0000c4e0: 6c6c 6572 2773 2073 656c 6563 7469 6f6e  ller's selection
+0000c4f0: 206f 6620 726f 7773 2069 7320 746f 6f20   of rows is too 
+0000c500: 6272 6f61 642e 0a0a 2020 2020 2020 2020  broad...        
+0000c510: 4669 656c 6473 2028 7768 6963 6820 6d61  Fields (which ma
+0000c520: 7020 746f 2044 6174 6146 7261 6d65 2063  p to DataFrame c
+0000c530: 6f6c 756d 6e73 2920 7468 6174 2063 6f6e  olumns) that con
+0000c540: 7461 696e 204e 614e 2f4e 6154 2076 616c  tain NaN/NaT val
+0000c550: 7565 730a 2020 2020 2020 2020 6172 6520  ues.        are 
+0000c560: 7265 6d6f 7665 642e 0a0a 2020 2020 2020  removed...      
+0000c570: 2020 452e 672e 2074 6f20 6164 6420 6120    E.g. to add a 
+0000c580: 6e65 7720 696e 6469 756d 2073 6f6c 6465  new indium solde
+0000c590: 7220 7379 7269 6e67 6520 746f 2074 6865  r syringe to the
+0000c5a0: 2064 6174 6162 6173 6520 2d20 6769 7665   database - give
+0000c5b0: 6e20 7468 6174 0a20 2020 2020 2020 206d  n that.        m
+0000c5c0: 616e 7920 6669 656c 6473 2077 696c 6c20  any fields will 
+0000c5d0: 6265 2073 696d 696c 6172 2062 6574 7765  be similar betwe
+0000c5e0: 656e 2073 7972 696e 6765 7320 2d20 6974  en syringes - it
+0000c5f0: 206d 6179 2062 6520 6865 6c70 6675 6c20   may be helpful 
+0000c600: 746f 0a20 2020 2020 2020 2067 6574 2061  to.        get a
+0000c610: 6e20 6578 6973 7469 6e67 2072 6f77 2061  n existing row a
+0000c620: 6e64 206d 6f64 6966 7920 6974 2e20 496e  nd modify it. In
+0000c630: 2074 6869 7320 696e 7374 616e 6365 2c20   this instance, 
+0000c640: 6164 6469 6e67 2061 2073 7972 696e 6765  adding a syringe
+0000c650: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+0000c660: 6520 7361 6d65 206c 6f74 2061 6e64 2074  e same lot and t
+0000c670: 6865 2073 616d 6520 696e 7374 6974 7574  he same institut
+0000c680: 652c 2077 6520 6361 6e20 6a75 7374 2063  e, we can just c
+0000c690: 6861 6e67 6520 7468 650a 2020 2020 2020  hange the.      
+0000c6a0: 2020 6c6f 6361 6c20 7379 7269 6e67 6520    local syringe 
+0000c6b0: 5049 4420 746f 2067 6574 2061 2064 6963  PID to get a dic
+0000c6c0: 7420 7375 6974 6162 6c65 2066 6f72 2050  t suitable for P
+0000c6d0: 4f53 5469 6e67 2069 7420 746f 2074 6865  OSTing it to the
+0000c6e0: 0a20 2020 2020 2020 2064 6174 6162 6173  .        databas
+0000c6f0: 653a 0a0a 2020 2020 2020 2020 6765 745f  e:..        get_
+0000c700: 7461 626c 655f 726f 775f 616e 645f 6d6f  table_row_and_mo
+0000c710: 6469 6679 280a 2020 2020 2020 2020 2020  dify(.          
+0000c720: 2020 2773 6f6c 6465 7227 2c20 7b27 736f    'solder', {'so
+0000c730: 6c64 6572 5f70 6964 273a 2031 7d2c 207b  lder_pid': 1}, {
+0000c740: 2773 7972 696e 6765 5f69 6427 3a20 3132  'syringe_id': 12
+0000c750: 7d0a 2020 2020 2020 2020 290a 0a20 2020  }.        )..   
+0000c760: 2020 2020 2057 6869 6368 2077 6f75 6c64       Which would
+0000c770: 2072 6574 7572 6e3a 0a0a 2020 2020 2020   return:..      
+0000c780: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+0000c790: 276d 616e 7566 6163 7475 7265 7227 3a20  'manufacturer': 
+0000c7a0: 342c 0a20 2020 2020 2020 2020 2020 2027  4,.            '
+0000c7b0: 736f 6c64 6572 5f74 7970 6527 3a20 2749  solder_type': 'I
+0000c7c0: 6e64 6975 6d20 5061 7374 6520 4e43 2d53  ndium Paste NC-S
+0000c7d0: 4d51 3830 2049 6e64 2331 4520 3532 496e  MQ80 Ind#1E 52In
+0000c7e0: 3438 536e 2054 7970 6520 3420 2e2e 2e27  48Sn Type 4 ...'
+0000c7f0: 2c0a 2020 2020 2020 2020 2020 2020 2770  ,.            'p
+0000c800: 726f 6475 6374 696f 6e5f 6461 7465 273a  roduction_date':
+0000c810: 2027 3230 3232 2d30 362d 3032 2030 303a   '2022-06-02 00:
+0000c820: 3030 3a30 3027 2c0a 2020 2020 2020 2020  00:00',.        
+0000c830: 2020 2020 2772 6f6f 6d5f 7465 6d70 6572      'room_temper
+0000c840: 6174 7572 655f 6461 7465 273a 2027 3230  ature_date': '20
+0000c850: 3232 2d30 372d 3138 2031 363a 3030 3a30  22-07-18 16:00:0
+0000c860: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+0000c870: 2765 7870 6972 795f 6461 7465 273a 2027  'expiry_date': '
+0000c880: 3230 3232 2d31 322d 3032 2030 303a 3030  2022-12-02 00:00
+0000c890: 3a30 3027 2c0a 2020 2020 2020 2020 2020  :00',.          
+0000c8a0: 2020 2773 7972 696e 6765 5f69 6427 3a20    'syringe_id': 
+0000c8b0: 3132 2c20 276c 6f74 273a 2027 5053 3131  12, 'lot': 'PS11
+0000c8c0: 3132 3037 3334 272c 2027 6d61 7373 273a  120734', 'mass':
+0000c8d0: 2032 350a 2020 2020 2020 2020 7d0a 0a20   25.        }.. 
+0000c8e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
 0000c8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c920: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000c930: 2020 2061 7267 730a 2020 2020 2020 2020     args.        
-0000c940: 2020 2020 7461 626c 655f 6e61 6d65 203a      table_name :
-0000c950: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0000c960: 2020 2020 2020 2020 5468 6520 6361 6c6c          The call
-0000c970: 6572 2073 686f 756c 6420 656e 7375 7265  er should ensure
-0000c980: 2074 6865 2074 6162 6c65 206e 616d 6520   the table name 
-0000c990: 6973 2063 6f72 7265 6374 2c20 7369 6e63  is correct, sinc
-0000c9a0: 6520 6e6f 0a20 2020 2020 2020 2020 2020  e no.           
-0000c9b0: 2020 2020 2063 6865 636b 2069 7320 6d61       check is ma
-0000c9c0: 6465 2e0a 2020 2020 2020 2020 2020 2020  de..            
-0000c9d0: 7365 6c65 6374 203a 2064 6963 740a 2020  select : dict.  
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-0000c9f0: 6666 6963 6965 6e74 207b 6669 656c 643a  fficient {field:
-0000ca00: 2076 616c 7565 2c20 2e2e 2e7d 2070 6169   value, ...} pai
-0000ca10: 7273 2074 6f20 6f62 7461 696e 2074 6865  rs to obtain the
-0000ca20: 2064 6573 6972 6564 2072 6f77 0a20 2020   desired row.   
-0000ca30: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-0000ca40: 6d20 7468 6520 7461 626c 652e 2054 6869  m the table. Thi
-0000ca50: 7320 7769 6c6c 2070 726f 6261 626c 7920  s will probably 
-0000ca60: 6a75 7374 2063 6f6e 7461 696e 2074 6865  just contain the
-0000ca70: 205f 7069 6420 6669 656c 640a 2020 2020   _pid field.    
-0000ca80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ca90: 7468 6520 6769 7665 6e20 7461 626c 652e  the given table.
-0000caa0: 0a20 2020 2020 2020 2020 2020 2072 6570  .            rep
-0000cab0: 6c61 6365 6d65 6e74 7320 3a20 6469 6374  lacements : dict
-0000cac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cad0: 2052 6570 6c61 6365 6d65 6e74 2076 616c   Replacement val
-0000cae0: 7565 7320 666f 7220 6669 656c 6473 207b  ues for fields {
-0000caf0: 6669 656c 643a 2076 616c 7565 2c20 2e2e  field: value, ..
-0000cb00: 2e7d 2e20 4966 2074 6869 730a 2020 2020  .}. If this.    
-0000cb10: 2020 2020 2020 2020 2020 2020 6172 6775              argu
-0000cb20: 6d65 6e74 2069 7320 6e6f 7420 7375 7070  ment is not supp
-0000cb30: 6c69 6564 2069 7420 6465 6661 756c 7473  lied it defaults
-0000cb40: 2074 6f20 4e6f 6e65 2c20 7768 6963 6820   to None, which 
-0000cb50: 6973 206c 6174 6572 0a20 2020 2020 2020  is later.       
-0000cb60: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-0000cb70: 726d 6564 2069 6e74 6f20 616e 2065 6d70  rmed into an emp
-0000cb80: 7479 2064 6963 742e 0a20 2020 2020 2020  ty dict..       
-0000cb90: 2020 2020 206f 6d69 745f 7069 6420 3a20       omit_pid : 
-0000cba0: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-0000cbb0: 2020 2020 2054 6865 2070 7269 6e63 6970       The princip
-0000cbc0: 616c 206f 626a 6563 7469 7665 206f 6620  al objective of 
-0000cbd0: 7468 6973 206d 6574 686f 6420 6973 2074  this method is t
-0000cbe0: 6f20 7265 7475 726e 2061 2064 6963 740a  o return a dict.
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 7468 6174 2063 616e 2062 6520 504f 5354  that can be POST
-0000cc10: 6564 2074 6f20 7468 6520 6461 7461 6261  ed to the databa
-0000cc20: 7365 2e20 5369 6e63 6520 7468 6520 6461  se. Since the da
-0000cc30: 7461 6261 7365 2064 6f65 736e 2774 0a20  tabase doesn't. 
-0000cc40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cc50: 7572 7265 6e74 6c79 2073 7570 706f 7274  urrently support
-0000cc60: 2050 4f53 5469 6e67 2074 6162 6c65 7320   POSTing tables 
-0000cc70: 7769 7468 2061 6e20 6578 6973 7469 6e67  with an existing
-0000cc80: 2070 7269 6d61 7279 206b 6579 2c0a 2020   primary key,.  
-0000cc90: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0000cca0: 6572 6527 7320 6c69 7474 6c65 2070 6f69  ere's little poi
-0000ccb0: 6e74 2072 6574 7572 6e69 6e67 2061 2064  nt returning a d
-0000ccc0: 6963 7420 636f 6e74 6169 6e69 6e67 206f  ict containing o
-0000ccd0: 6e65 3b20 7468 6973 0a20 2020 2020 2020  ne; this.       
-0000cce0: 2020 2020 2020 2020 2062 6568 6176 696f           behavio
-0000ccf0: 7572 206d 6179 2063 6861 6e67 6520 696e  ur may change in
-0000cd00: 2074 6865 2066 7574 7572 652e 2041 6e79   the future. Any
-0000cd10: 2066 6965 6c64 2065 6e64 696e 6720 7769   field ending wi
-0000cd20: 7468 205f 7069 640a 2020 2020 2020 2020  th _pid.        
-0000cd30: 2020 2020 2020 2020 2861 6e64 2074 6865          (and the
-0000cd40: 7265 2073 686f 756c 6420 6265 206f 6e6c  re should be onl
-0000cd50: 7920 6f6e 6520 7375 6368 2066 6965 6c64  y one such field
-0000cd60: 2920 6973 2061 2070 7269 6d61 7279 206b  ) is a primary k
-0000cd70: 6579 2061 6e64 0a20 2020 2020 2020 2020  ey and.         
-0000cd80: 2020 2020 2020 2077 696c 6c20 6265 2072         will be r
-0000cd90: 656d 6f76 6564 2062 7920 6465 6661 756c  emoved by defaul
-0000cda0: 742e 0a20 2020 2020 2020 202d 2d2d 2d2d  t..        -----
+0000c920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000c930: 2020 2020 2020 6172 6773 0a20 2020 2020        args.     
+0000c940: 2020 2020 2020 2074 6162 6c65 5f6e 616d         table_nam
+0000c950: 6520 3a20 7374 7269 6e67 0a20 2020 2020  e : string.     
+0000c960: 2020 2020 2020 2020 2020 2054 6865 2063             The c
+0000c970: 616c 6c65 7220 7368 6f75 6c64 2065 6e73  aller should ens
+0000c980: 7572 6520 7468 6520 7461 626c 6520 6e61  ure the table na
+0000c990: 6d65 2069 7320 636f 7272 6563 742c 2073  me is correct, s
+0000c9a0: 696e 6365 206e 6f0a 2020 2020 2020 2020  ince no.        
+0000c9b0: 2020 2020 2020 2020 6368 6563 6b20 6973          check is
+0000c9c0: 206d 6164 652e 0a20 2020 2020 2020 2020   made..         
+0000c9d0: 2020 2073 656c 6563 7420 3a20 6469 6374     select : dict
+0000c9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c9f0: 2073 7566 6669 6369 656e 7420 7b66 6965   sufficient {fie
+0000ca00: 6c64 3a20 7661 6c75 652c 202e 2e2e 7d20  ld: value, ...} 
+0000ca10: 7061 6972 7320 746f 206f 6274 6169 6e20  pairs to obtain 
+0000ca20: 7468 6520 6465 7369 7265 6420 726f 770a  the desired row.
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 6672 6f6d 2074 6865 2074 6162 6c65 2e20  from the table. 
+0000ca50: 5468 6973 2077 696c 6c20 7072 6f62 6162  This will probab
+0000ca60: 6c79 206a 7573 7420 636f 6e74 6169 6e20  ly just contain 
+0000ca70: 7468 6520 5f70 6964 2066 6965 6c64 0a20  the _pid field. 
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000ca90: 6f72 2074 6865 2067 6976 656e 2074 6162  or the given tab
+0000caa0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+0000cab0: 7265 706c 6163 656d 656e 7473 203a 2064  replacements : d
+0000cac0: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+0000cad0: 2020 2020 5265 706c 6163 656d 656e 7420      Replacement 
+0000cae0: 7661 6c75 6573 2066 6f72 2066 6965 6c64  values for field
+0000caf0: 7320 7b66 6965 6c64 3a20 7661 6c75 652c  s {field: value,
+0000cb00: 202e 2e2e 7d2e 2049 6620 7468 6973 0a20   ...}. If this. 
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000cb20: 7267 756d 656e 7420 6973 206e 6f74 2073  rgument is not s
+0000cb30: 7570 706c 6965 6420 6974 2064 6566 6175  upplied it defau
+0000cb40: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
+0000cb50: 6368 2069 7320 6c61 7465 720a 2020 2020  ch is later.    
+0000cb60: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+0000cb70: 7366 6f72 6d65 6420 696e 746f 2061 6e20  sformed into an 
+0000cb80: 656d 7074 7920 6469 6374 2e0a 2020 2020  empty dict..    
+0000cb90: 2020 2020 2020 2020 6f6d 6974 5f70 6964          omit_pid
+0000cba0: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
+0000cbb0: 2020 2020 2020 2020 5468 6520 7072 696e          The prin
+0000cbc0: 6369 7061 6c20 6f62 6a65 6374 6976 6520  cipal objective 
+0000cbd0: 6f66 2074 6869 7320 6d65 7468 6f64 2069  of this method i
+0000cbe0: 7320 746f 2072 6574 7572 6e20 6120 6469  s to return a di
+0000cbf0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+0000cc00: 2020 2074 6861 7420 6361 6e20 6265 2050     that can be P
+0000cc10: 4f53 5465 6420 746f 2074 6865 2064 6174  OSTed to the dat
+0000cc20: 6162 6173 652e 2053 696e 6365 2074 6865  abase. Since the
+0000cc30: 2064 6174 6162 6173 6520 646f 6573 6e27   database doesn'
+0000cc40: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000cc50: 2020 6375 7272 656e 746c 7920 7375 7070    currently supp
+0000cc60: 6f72 7420 504f 5354 696e 6720 7461 626c  ort POSTing tabl
+0000cc70: 6573 2077 6974 6820 616e 2065 7869 7374  es with an exist
+0000cc80: 696e 6720 7072 696d 6172 7920 6b65 792c  ing primary key,
+0000cc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cca0: 2074 6865 7265 2773 206c 6974 746c 6520   there's little 
+0000ccb0: 706f 696e 7420 7265 7475 726e 696e 6720  point returning 
+0000ccc0: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
+0000ccd0: 6720 6f6e 653b 2074 6869 730a 2020 2020  g one; this.    
+0000cce0: 2020 2020 2020 2020 2020 2020 6265 6861              beha
+0000ccf0: 7669 6f75 7220 6d61 7920 6368 616e 6765  viour may change
+0000cd00: 2069 6e20 7468 6520 6675 7475 7265 2e20   in the future. 
+0000cd10: 416e 7920 6669 656c 6420 656e 6469 6e67  Any field ending
+0000cd20: 2077 6974 6820 5f70 6964 0a20 2020 2020   with _pid.     
+0000cd30: 2020 2020 2020 2020 2020 2028 616e 6420             (and 
+0000cd40: 7468 6572 6520 7368 6f75 6c64 2062 6520  there should be 
+0000cd50: 6f6e 6c79 206f 6e65 2073 7563 6820 6669  only one such fi
+0000cd60: 656c 6429 2069 7320 6120 7072 696d 6172  eld) is a primar
+0000cd70: 7920 6b65 7920 616e 640a 2020 2020 2020  y key and.      
+0000cd80: 2020 2020 2020 2020 2020 7769 6c6c 2062            will b
+0000cd90: 6520 7265 6d6f 7665 6420 6279 2064 6566  e removed by def
+0000cda0: 6175 6c74 2e0a 2020 2020 2020 2020 2d2d  ault..        --
 0000cdb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000cdc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000cdd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000cde0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cdf0: 2d0a 2020 2020 2020 2020 7265 7475 726e  -.        return
-0000ce00: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
-0000ce10: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
-0000ce20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000cdf0: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
+0000ce00: 7572 6e73 0a20 2020 2020 2020 2020 2020  urns.           
+0000ce10: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
+0000ce20: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 0000ce30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ce40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ce50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ce60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-0000ce70: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-0000ce80: 5065 7266 6f72 6d20 736f 6d65 2073 616e  Perform some san
-0000ce90: 6974 7920 6368 6563 6b73 206f 6e20 7468  ity checks on th
-0000cea0: 6520 7375 7070 6c69 6564 2074 6162 6c65  e supplied table
-0000ceb0: 2061 6e64 2066 6965 6c64 206e 616d 6573   and field names
-0000cec0: 2e0a 2020 2020 2020 2020 2320 4361 6c6c  ..        # Call
-0000ced0: 7320 746f 2064 6573 6372 6962 6528 2920  s to describe() 
-0000cee0: 6172 6520 6361 6368 6564 2c20 736f 2074  are cached, so t
-0000cef0: 6865 2063 6f73 7420 666f 7220 7468 6573  he cost for thes
-0000cf00: 6520 6368 6563 6b73 2069 730a 2020 2020  e checks is.    
-0000cf10: 2020 2020 2320 6d69 6e69 6d61 6c2e 0a0a      # minimal...
-0000cf20: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-0000cf30: 7461 626c 6520 6e61 6d65 2065 7869 7374  table name exist
-0000cf40: 7320 696e 2074 6865 2064 620a 2020 2020  s in the db.    
-0000cf50: 2020 2020 6462 5f74 6162 6c65 5f6e 616d      db_table_nam
-0000cf60: 6573 203d 2073 656c 662e 6465 7363 7269  es = self.descri
-0000cf70: 6265 2829 2e64 6174 610a 2020 2020 2020  be().data.      
-0000cf80: 2020 6966 2074 6162 6c65 5f6e 616d 6520    if table_name 
-0000cf90: 6e6f 7420 696e 2064 625f 7461 626c 655f  not in db_table_
-0000cfa0: 6e61 6d65 733a 0a20 2020 2020 2020 2020  names:.         
-0000cfb0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-0000cfc0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-0000cfd0: 2020 2020 2767 6574 5f74 6162 6c65 5f72      'get_table_r
-0000cfe0: 6f77 5f61 6e64 5f6d 6f64 6966 793a 2075  ow_and_modify: u
-0000cff0: 6e72 6563 6f67 6e69 7365 6420 7461 626c  nrecognised tabl
-0000d000: 6520 2225 7322 272c 2074 6162 6c65 5f6e  e "%s"', table_n
-0000d010: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0000d020: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0000d030: 7475 726e 207b 7d0a 0a20 2020 2020 2020  turn {}..       
-0000d040: 2023 2063 6865 636b 2066 6965 6c64 206e   # check field n
-0000d050: 616d 6573 2063 6f6e 7461 696e 6564 2069  ames contained i
-0000d060: 6e20 6d65 7468 6f64 2061 7267 756d 656e  n method argumen
-0000d070: 7473 2061 7265 2076 616c 6964 0a20 2020  ts are valid.   
-0000d080: 2020 2020 2064 625f 6669 656c 645f 6e61       db_field_na
-0000d090: 6d65 7320 3d20 7365 6c66 2e64 6573 6372  mes = self.descr
-0000d0a0: 6962 6528 7461 626c 655f 6e61 6d65 292e  ibe(table_name).
-0000d0b0: 6461 7461 0a20 2020 2020 2020 2069 6620  data.        if 
-0000d0c0: 7265 706c 6163 656d 656e 7473 2069 7320  replacements is 
-0000d0d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d0e0: 2020 7265 706c 6163 656d 656e 7473 203d    replacements =
-0000d0f0: 207b 7d0a 2020 2020 2020 2020 6361 7465   {}.        cate
-0000d100: 676f 7269 6573 203d 207b 2773 656c 6563  gories = {'selec
-0000d110: 7427 3a20 7365 6c65 6374 2c20 2772 6570  t': select, 'rep
-0000d120: 6c61 6365 6d65 6e74 7327 3a20 7265 706c  lacements': repl
-0000d130: 6163 656d 656e 7473 7d0a 2020 2020 2020  acements}.      
-0000d140: 2020 7365 6c65 6374 5f66 6169 6c20 3d20    select_fail = 
-0000d150: 4661 6c73 650a 0a20 2020 2020 2020 2066  False..        f
-0000d160: 6f72 2063 6174 6567 6f72 792c 2066 6965  or category, fie
-0000d170: 6c64 7320 696e 2063 6174 6567 6f72 6965  lds in categorie
-0000d180: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-0000d190: 2020 2020 2020 2066 6f72 2066 6965 6c64         for field
-0000d1a0: 2069 6e20 6669 656c 6473 3a0a 2020 2020   in fields:.    
-0000d1b0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0000d1c0: 6965 6c64 206e 6f74 2069 6e20 6462 5f66  ield not in db_f
-0000d1d0: 6965 6c64 5f6e 616d 6573 3a0a 2020 2020  ield_names:.    
+0000ce60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000ce70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ce80: 2023 2050 6572 666f 726d 2073 6f6d 6520   # Perform some 
+0000ce90: 7361 6e69 7479 2063 6865 636b 7320 6f6e  sanity checks on
+0000cea0: 2074 6865 2073 7570 706c 6965 6420 7461   the supplied ta
+0000ceb0: 626c 6520 616e 6420 6669 656c 6420 6e61  ble and field na
+0000cec0: 6d65 732e 0a20 2020 2020 2020 2023 2043  mes..        # C
+0000ced0: 616c 6c73 2074 6f20 6465 7363 7269 6265  alls to describe
+0000cee0: 2829 2061 7265 2063 6163 6865 642c 2073  () are cached, s
+0000cef0: 6f20 7468 6520 636f 7374 2066 6f72 2074  o the cost for t
+0000cf00: 6865 7365 2063 6865 636b 7320 6973 0a20  hese checks is. 
+0000cf10: 2020 2020 2020 2023 206d 696e 696d 616c         # minimal
+0000cf20: 2e0a 0a20 2020 2020 2020 2023 2063 6865  ...        # che
+0000cf30: 636b 2074 6162 6c65 206e 616d 6520 6578  ck table name ex
+0000cf40: 6973 7473 2069 6e20 7468 6520 6462 0a20  ists in the db. 
+0000cf50: 2020 2020 2020 2064 625f 7461 626c 655f         db_table_
+0000cf60: 6e61 6d65 7320 3d20 7365 6c66 2e64 6573  names = self.des
+0000cf70: 6372 6962 6528 292e 6461 7461 0a20 2020  cribe().data.   
+0000cf80: 2020 2020 2069 6620 7461 626c 655f 6e61       if table_na
+0000cf90: 6d65 206e 6f74 2069 6e20 6462 5f74 6162  me not in db_tab
+0000cfa0: 6c65 5f6e 616d 6573 3a0a 2020 2020 2020  le_names:.      
+0000cfb0: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
+0000cfc0: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0000cfd0: 2020 2020 2020 2027 6765 745f 7461 626c         'get_tabl
+0000cfe0: 655f 726f 775f 616e 645f 6d6f 6469 6679  e_row_and_modify
+0000cff0: 3a20 756e 7265 636f 676e 6973 6564 2074  : unrecognised t
+0000d000: 6162 6c65 2022 2573 2227 2c20 7461 626c  able "%s"', tabl
+0000d010: 655f 6e61 6d65 0a20 2020 2020 2020 2020  e_name.         
+0000d020: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000d030: 2072 6574 7572 6e20 7b7d 0a0a 2020 2020   return {}..    
+0000d040: 2020 2020 2320 6368 6563 6b20 6669 656c      # check fiel
+0000d050: 6420 6e61 6d65 7320 636f 6e74 6169 6e65  d names containe
+0000d060: 6420 696e 206d 6574 686f 6420 6172 6775  d in method argu
+0000d070: 6d65 6e74 7320 6172 6520 7661 6c69 640a  ments are valid.
+0000d080: 2020 2020 2020 2020 6462 5f66 6965 6c64          db_field
+0000d090: 5f6e 616d 6573 203d 2073 656c 662e 6465  _names = self.de
+0000d0a0: 7363 7269 6265 2874 6162 6c65 5f6e 616d  scribe(table_nam
+0000d0b0: 6529 2e64 6174 610a 2020 2020 2020 2020  e).data.        
+0000d0c0: 6966 2072 6570 6c61 6365 6d65 6e74 7320  if replacements 
+0000d0d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000d0e0: 2020 2020 2072 6570 6c61 6365 6d65 6e74       replacement
+0000d0f0: 7320 3d20 7b7d 0a20 2020 2020 2020 2063  s = {}.        c
+0000d100: 6174 6567 6f72 6965 7320 3d20 7b27 7365  ategories = {'se
+0000d110: 6c65 6374 273a 2073 656c 6563 742c 2027  lect': select, '
+0000d120: 7265 706c 6163 656d 656e 7473 273a 2072  replacements': r
+0000d130: 6570 6c61 6365 6d65 6e74 737d 0a20 2020  eplacements}.   
+0000d140: 2020 2020 2073 656c 6563 745f 6661 696c       select_fail
+0000d150: 203d 2046 616c 7365 0a0a 2020 2020 2020   = False..      
+0000d160: 2020 666f 7220 6361 7465 676f 7279 2c20    for category, 
+0000d170: 6669 656c 6473 2069 6e20 6361 7465 676f  fields in catego
+0000d180: 7269 6573 2e69 7465 6d73 2829 3a0a 2020  ries.items():.  
+0000d190: 2020 2020 2020 2020 2020 666f 7220 6669            for fi
+0000d1a0: 656c 6420 696e 2066 6965 6c64 733a 0a20  eld in fields:. 
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d1c0: 6620 6669 656c 6420 6e6f 7420 696e 2064  f field not in d
+0000d1d0: 625f 6669 656c 645f 6e61 6d65 733a 0a20  b_field_names:. 
 0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1f0: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-0000d200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d210: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000d1f0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+0000d200: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000d210: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
 0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d230: 2020 2020 2020 2027 6765 745f 7461 626c         'get_tabl
-0000d240: 655f 726f 775f 616e 645f 6d6f 6469 6679  e_row_and_modify
-0000d250: 3a20 270a 2020 2020 2020 2020 2020 2020  : '.            
+0000d230: 2020 2020 2020 2020 2020 2767 6574 5f74            'get_t
+0000d240: 6162 6c65 5f72 6f77 5f61 6e64 5f6d 6f64  able_row_and_mod
+0000d250: 6966 793a 2027 0a20 2020 2020 2020 2020  ify: '.         
 0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2774 6162 6c65 2022 2573 222c 2075 6e72  'table "%s", unr
-0000d280: 6563 6f67 6e69 7365 6420 6669 656c 6420  ecognised field 
-0000d290: 2225 7322 2028 2573 2927 0a20 2020 2020  "%s" (%s)'.     
+0000d270: 2020 2027 7461 626c 6520 2225 7322 2c20     'table "%s", 
+0000d280: 756e 7265 636f 676e 6973 6564 2066 6965  unrecognised fie
+0000d290: 6c64 2022 2573 2220 2825 7329 270a 2020  ld "%s" (%s)'.  
 0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2b0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-0000d2c0: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000d2d0: 626c 655f 6e61 6d65 2c20 6669 656c 642c  ble_name, field,
-0000d2e0: 2063 6174 6567 6f72 790a 2020 2020 2020   category.      
-0000d2f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2020 2020 7365 6c65 6374 5f66 6169 6c20      select_fail 
-0000d320: 3d20 5472 7565 0a0a 2020 2020 2020 2020  = True..        
-0000d330: 6966 2073 656c 6563 745f 6661 696c 3a0a  if select_fail:.
-0000d340: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d350: 726e 207b 7d0a 0a20 2020 2020 2020 2023  rn {}..        #
-0000d360: 2063 6865 636b 7320 636f 6d70 6c65 7465   checks complete
-0000d370: 3a20 7072 6f63 6573 7320 656e 7175 6972  : process enquir
-0000d380: 790a 0a20 2020 2020 2020 2023 2067 6574  y..        # get
-0000d390: 2074 6865 2050 616e 6461 7320 4461 7461   the Pandas Data
-0000d3a0: 4672 616d 6520 666f 7220 6120 7375 6273  Frame for a subs
-0000d3b0: 6574 206f 6620 7468 6973 2074 6162 6c65  et of this table
-0000d3c0: 0a20 2020 2020 2020 2070 6466 5f6f 7269  .        pdf_ori
-0000d3d0: 6769 6e61 6c20 3d20 7365 6c66 2e67 6574  ginal = self.get
-0000d3e0: 2874 6162 6c65 5f6e 616d 652c 202a 2a73  (table_name, **s
-0000d3f0: 656c 6563 7429 2e64 6174 610a 0a20 2020  elect).data..   
-0000d400: 2020 2020 2023 2064 726f 7020 616c 6c20       # drop all 
-0000d410: 636f 6c75 6d6e 7320 7769 7468 204e 617b  columns with Na{
-0000d420: 4e2f 547d 2076 616c 7565 730a 2020 2020  N/T} values.    
-0000d430: 2020 2020 7064 6620 3d20 7064 665f 6f72      pdf = pdf_or
-0000d440: 6967 696e 616c 2e64 726f 706e 6128 6178  iginal.dropna(ax
-0000d450: 6973 3d31 290a 0a20 2020 2020 2020 2023  is=1)..        #
-0000d460: 2063 6f6e 7665 7274 2074 6f20 6469 6374   convert to dict
-0000d470: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-0000d480: 7064 662e 746f 5f64 6963 7428 2772 6563  pdf.to_dict('rec
-0000d490: 6f72 6473 2729 0a0a 2020 2020 2020 2020  ords')..        
-0000d4a0: 2320 6966 2074 6865 2072 6573 756c 7420  # if the result 
-0000d4b0: 6973 2065 6d70 7479 2c20 6578 6974 2065  is empty, exit e
-0000d4c0: 6172 6c79 0a20 2020 2020 2020 2069 6620  arly.        if 
-0000d4d0: 6e6f 7420 726f 7773 3a0a 2020 2020 2020  not rows:.      
-0000d4e0: 2020 2020 2020 7265 7475 726e 207b 7d0a        return {}.
-0000d4f0: 0a20 2020 2020 2020 206e 756d 5f72 6f77  .        num_row
-0000d500: 7320 3d20 6c65 6e28 726f 7773 290a 2020  s = len(rows).  
-0000d510: 2020 2020 2020 6966 206e 756d 5f72 6f77        if num_row
-0000d520: 7320 3e20 313a 0a20 2020 2020 2020 2020  s > 1:.         
-0000d530: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
-0000d540: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-0000d550: 2020 2020 2767 6574 5f74 6162 6c65 5f72      'get_table_r
-0000d560: 6f77 5f61 6e64 5f6d 6f64 6966 793a 2071  ow_and_modify: q
-0000d570: 7565 7279 2072 6574 7572 6e65 6420 2573  uery returned %s
-0000d580: 2072 6f77 7320 2865 7870 6563 7465 6420   rows (expected 
-0000d590: 3129 272c 206e 756d 5f72 6f77 730a 2020  1)', num_rows.  
-0000d5a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d5b0: 2020 2020 7461 626c 6520 3d20 726f 7773      table = rows
-0000d5c0: 5b2d 315d 0a0a 2020 2020 2020 2020 666f  [-1]..        fo
-0000d5d0: 7220 6669 656c 642c 2076 616c 7565 2069  r field, value i
-0000d5e0: 6e20 7265 706c 6163 656d 656e 7473 2e69  n replacements.i
-0000d5f0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000d600: 2020 2020 7461 626c 655b 6669 656c 645d      table[field]
-0000d610: 203d 2076 616c 7565 0a0a 2020 2020 2020   = value..      
-0000d620: 2020 2320 7265 6d6f 7665 2050 4944 2066    # remove PID f
-0000d630: 6965 6c64 0a20 2020 2020 2020 2069 6620  ield.        if 
-0000d640: 6f6d 6974 5f70 6964 3a0a 2020 2020 2020  omit_pid:.      
-0000d650: 2020 2020 2020 7461 626c 6520 3d20 7b0a        table = {.
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 6b3a 2076 2066 6f72 206b 2c20 7620 696e  k: v for k, v in
-0000d680: 2074 6162 6c65 2e69 7465 6d73 2829 0a20   table.items(). 
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d6a0: 6620 6e6f 7420 6b2e 6c6f 7765 7228 292e  f not k.lower().
-0000d6b0: 656e 6473 7769 7468 2827 5f70 6964 2729  endswith('_pid')
-0000d6c0: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
-0000d6d0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-0000d6e0: 6162 6c65 0a0a 2020 2020 6465 6620 6765  able..    def ge
-0000d6f0: 745f 7674 696c 655f 696e 666f 2873 656c  t_vtile_info(sel
-0000d700: 662c 2071 7263 6f64 6529 3a0a 2020 2020  f, qrcode):.    
-0000d710: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d720: 436f 6c6c 6174 6520 636f 6d70 7265 6865  Collate comprehe
-0000d730: 6e73 6976 6520 696e 666f 726d 6174 696f  nsive informatio
-0000d740: 6e20 6162 6f75 7420 6120 7654 696c 6520  n about a vTile 
-0000d750: 6769 7665 6e20 6974 7320 5152 2d63 6f64  given its QR-cod
-0000d760: 652e 0a20 2020 2020 2020 2041 6d6f 6e67  e..        Among
-0000d770: 7374 206f 7468 6572 2069 6e66 6f72 6d61  st other informa
-0000d780: 7469 6f6e 2c20 7468 6520 6f72 6967 696e  tion, the origin
-0000d790: 616c 2077 6166 6572 2070 6f73 6974 696f  al wafer positio
-0000d7a0: 6e20 6f66 2065 6163 6820 5369 504d 2069  n of each SiPM i
-0000d7b0: 730a 2020 2020 2020 2020 6f62 7461 696e  s.        obtain
-0000d7c0: 6564 2e0a 0a20 2020 2020 2020 2054 6869  ed...        Thi
-0000d7d0: 7320 6973 2061 6e20 4558 5045 4e53 4956  s is an EXPENSIV
-0000d7e0: 4520 6d65 7468 6f64 2074 6f20 6361 6c6c  E method to call
-0000d7f0: 2077 6974 6820 6d61 6e79 2073 6571 7565   with many seque
-0000d800: 6e74 6961 6c20 6461 7461 6261 7365 0a20  ntial database. 
-0000d810: 2020 2020 2020 206c 6f6f 6b75 7073 2e20         lookups. 
-0000d820: 4974 206d 6179 2074 616b 6520 6120 6d69  It may take a mi
-0000d830: 6e75 7465 2074 6f20 636f 6d70 6c65 7465  nute to complete
-0000d840: 2e0a 0a20 2020 2020 2020 202d 2d2d 2d2d  ...        -----
+0000d2b0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2d0: 2074 6162 6c65 5f6e 616d 652c 2066 6965   table_name, fie
+0000d2e0: 6c64 2c20 6361 7465 676f 7279 0a20 2020  ld, category.   
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000d310: 2020 2020 2020 2073 656c 6563 745f 6661         select_fa
+0000d320: 696c 203d 2054 7275 650a 0a20 2020 2020  il = True..     
+0000d330: 2020 2069 6620 7365 6c65 6374 5f66 6169     if select_fai
+0000d340: 6c3a 0a20 2020 2020 2020 2020 2020 2072  l:.            r
+0000d350: 6574 7572 6e20 7b7d 0a0a 2020 2020 2020  eturn {}..      
+0000d360: 2020 2320 6368 6563 6b73 2063 6f6d 706c    # checks compl
+0000d370: 6574 653a 2070 726f 6365 7373 2065 6e71  ete: process enq
+0000d380: 7569 7279 0a0a 2020 2020 2020 2020 2320  uiry..        # 
+0000d390: 6765 7420 7468 6520 5061 6e64 6173 2044  get the Pandas D
+0000d3a0: 6174 6146 7261 6d65 2066 6f72 2061 2073  ataFrame for a s
+0000d3b0: 7562 7365 7420 6f66 2074 6869 7320 7461  ubset of this ta
+0000d3c0: 626c 650a 2020 2020 2020 2020 7064 665f  ble.        pdf_
+0000d3d0: 6f72 6967 696e 616c 203d 2073 656c 662e  original = self.
+0000d3e0: 6765 7428 7461 626c 655f 6e61 6d65 2c20  get(table_name, 
+0000d3f0: 2a2a 7365 6c65 6374 292e 6461 7461 0a0a  **select).data..
+0000d400: 2020 2020 2020 2020 2320 6472 6f70 2061          # drop a
+0000d410: 6c6c 2063 6f6c 756d 6e73 2077 6974 6820  ll columns with 
+0000d420: 4e61 7b4e 2f54 7d20 7661 6c75 6573 0a20  Na{N/T} values. 
+0000d430: 2020 2020 2020 2070 6466 203d 2070 6466         pdf = pdf
+0000d440: 5f6f 7269 6769 6e61 6c2e 6472 6f70 6e61  _original.dropna
+0000d450: 2861 7869 733d 3129 0a0a 2020 2020 2020  (axis=1)..      
+0000d460: 2020 2320 636f 6e76 6572 7420 746f 2064    # convert to d
+0000d470: 6963 740a 2020 2020 2020 2020 726f 7773  ict.        rows
+0000d480: 203d 2070 6466 2e74 6f5f 6469 6374 2827   = pdf.to_dict('
+0000d490: 7265 636f 7264 7327 290a 0a20 2020 2020  records')..     
+0000d4a0: 2020 2023 2069 6620 7468 6520 7265 7375     # if the resu
+0000d4b0: 6c74 2069 7320 656d 7074 792c 2065 7869  lt is empty, exi
+0000d4c0: 7420 6561 726c 790a 2020 2020 2020 2020  t early.        
+0000d4d0: 6966 206e 6f74 2072 6f77 733a 0a20 2020  if not rows:.   
+0000d4e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d4f0: 7b7d 0a0a 2020 2020 2020 2020 6e75 6d5f  {}..        num_
+0000d500: 726f 7773 203d 206c 656e 2872 6f77 7329  rows = len(rows)
+0000d510: 0a20 2020 2020 2020 2069 6620 6e75 6d5f  .        if num_
+0000d520: 726f 7773 203e 2031 3a0a 2020 2020 2020  rows > 1:.      
+0000d530: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
+0000d540: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0000d550: 2020 2020 2020 2027 6765 745f 7461 626c         'get_tabl
+0000d560: 655f 726f 775f 616e 645f 6d6f 6469 6679  e_row_and_modify
+0000d570: 3a20 7175 6572 7920 7265 7475 726e 6564  : query returned
+0000d580: 2025 7320 726f 7773 2028 6578 7065 6374   %s rows (expect
+0000d590: 6564 2031 2927 2c20 6e75 6d5f 726f 7773  ed 1)', num_rows
+0000d5a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d5b0: 2020 2020 2020 2074 6162 6c65 203d 2072         table = r
+0000d5c0: 6f77 735b 2d31 5d0a 0a20 2020 2020 2020  ows[-1]..       
+0000d5d0: 2066 6f72 2066 6965 6c64 2c20 7661 6c75   for field, valu
+0000d5e0: 6520 696e 2072 6570 6c61 6365 6d65 6e74  e in replacement
+0000d5f0: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
+0000d600: 2020 2020 2020 2074 6162 6c65 5b66 6965         table[fie
+0000d610: 6c64 5d20 3d20 7661 6c75 650a 0a20 2020  ld] = value..   
+0000d620: 2020 2020 2023 2072 656d 6f76 6520 5049       # remove PI
+0000d630: 4420 6669 656c 640a 2020 2020 2020 2020  D field.        
+0000d640: 6966 206f 6d69 745f 7069 643a 0a20 2020  if omit_pid:.   
+0000d650: 2020 2020 2020 2020 2074 6162 6c65 203d           table =
+0000d660: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000d670: 2020 206b 3a20 7620 666f 7220 6b2c 2076     k: v for k, v
+0000d680: 2069 6e20 7461 626c 652e 6974 656d 7328   in table.items(
+0000d690: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d6a0: 2020 6966 206e 6f74 206b 2e6c 6f77 6572    if not k.lower
+0000d6b0: 2829 2e65 6e64 7377 6974 6828 275f 7069  ().endswith('_pi
+0000d6c0: 6427 290a 2020 2020 2020 2020 2020 2020  d').            
+0000d6d0: 7d0a 0a20 2020 2020 2020 2072 6574 7572  }..        retur
+0000d6e0: 6e20 7461 626c 650a 0a20 2020 2064 6566  n table..    def
+0000d6f0: 2067 6574 5f76 7469 6c65 5f69 6e66 6f28   get_vtile_info(
+0000d700: 7365 6c66 2c20 7172 636f 6465 293a 0a20  self, qrcode):. 
+0000d710: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d720: 2020 2043 6f6c 6c61 7465 2063 6f6d 7072     Collate compr
+0000d730: 6568 656e 7369 7665 2069 6e66 6f72 6d61  ehensive informa
+0000d740: 7469 6f6e 2061 626f 7574 2061 2076 5469  tion about a vTi
+0000d750: 6c65 2067 6976 656e 2069 7473 2051 522d  le given its QR-
+0000d760: 636f 6465 2e0a 2020 2020 2020 2020 416d  code..        Am
+0000d770: 6f6e 6773 7420 6f74 6865 7220 696e 666f  ongst other info
+0000d780: 726d 6174 696f 6e2c 2074 6865 206f 7269  rmation, the ori
+0000d790: 6769 6e61 6c20 7761 6665 7220 706f 7369  ginal wafer posi
+0000d7a0: 7469 6f6e 206f 6620 6561 6368 2053 6950  tion of each SiP
+0000d7b0: 4d20 6973 0a20 2020 2020 2020 206f 6274  M is.        obt
+0000d7c0: 6169 6e65 642e 0a0a 2020 2020 2020 2020  ained...        
+0000d7d0: 5468 6973 2069 7320 616e 2045 5850 454e  This is an EXPEN
+0000d7e0: 5349 5645 206d 6574 686f 6420 746f 2063  SIVE method to c
+0000d7f0: 616c 6c20 7769 7468 206d 616e 7920 7365  all with many se
+0000d800: 7175 656e 7469 616c 2064 6174 6162 6173  quential databas
+0000d810: 650a 2020 2020 2020 2020 6c6f 6f6b 7570  e.        lookup
+0000d820: 732e 2049 7420 6d61 7920 7461 6b65 2061  s. It may take a
+0000d830: 206d 696e 7574 6520 746f 2063 6f6d 706c   minute to compl
+0000d840: 6574 652e 0a0a 2020 2020 2020 2020 2d2d  ete...        --
 0000d850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000d860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000d870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000d880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d890: 2d0a 2020 2020 2020 2020 6172 6773 0a20  -.        args. 
-0000d8a0: 2020 2020 2020 2020 2020 2071 7263 6f64             qrcod
-0000d8b0: 6520 3a20 696e 740a 2020 2020 2020 2020  e : int.        
-0000d8c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d890: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
+0000d8a0: 730a 2020 2020 2020 2020 2020 2020 7172  s.            qr
+0000d8b0: 636f 6465 203a 2069 6e74 0a20 2020 2020  code : int.     
+0000d8c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 0000d8d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000d8e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000d8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d900: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2072  ------.        r
-0000d910: 6574 7572 6e73 203a 2064 6963 7420 6f72  eturns : dict or
-0000d920: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000d930: 2020 4e6f 6e65 2069 7320 7265 7475 726e    None is return
-0000d940: 6564 2069 6620 616e 7920 7265 7175 6972  ed if any requir
-0000d950: 6564 2064 6174 756d 2063 6f75 6c64 206e  ed datum could n
-0000d960: 6f74 2062 6520 6f62 7461 696e 6564 2e0a  ot be obtained..
-0000d970: 2020 2020 2020 2020 2020 2020 652e 672e              e.g.
-0000d980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d990: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000d9a0: 2020 2020 2020 2027 7172 636f 6465 273a         'qrcode':
-0000d9b0: 2032 3330 3130 3630 3330 3030 3038 3330   230106030000830
-0000d9c0: 3031 2c0a 2020 2020 2020 2020 2020 2020  01,.            
-0000d9d0: 2020 2020 2020 2020 2776 7063 625f 7069          'vpcb_pi
-0000d9e0: 6427 3a20 3538 2c0a 2020 2020 2020 2020  d': 58,.        
-0000d9f0: 2020 2020 2020 2020 2020 2020 2776 7063              'vpc
-0000da00: 625f 6173 6963 5f70 6964 273a 2037 352c  b_asic_pid': 75,
-0000da10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da20: 2020 2020 2027 7674 696c 655f 7069 6427       'vtile_pid'
-0000da30: 3a20 3633 2c0a 2020 2020 2020 2020 2020  : 63,.          
-0000da40: 2020 2020 2020 2020 2020 2773 6970 6d5f            'sipm_
-0000da50: 3127 3a20 7b0a 2020 2020 2020 2020 2020  1': {.          
-0000da60: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000da70: 6970 6d5f 6964 273a 2036 3931 2c0a 2020  ipm_id': 691,.  
-0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da90: 2020 2020 2020 276c 6f74 273a 2039 3236        'lot': 926
-0000daa0: 3231 3039 2c0a 2020 2020 2020 2020 2020  2109,.          
-0000dab0: 2020 2020 2020 2020 2020 2020 2020 2777                'w
-0000dac0: 6166 6572 5f6e 756d 6265 7227 3a20 3135  afer_number': 15
-0000dad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dae0: 2020 2020 2020 2020 2020 2763 6f6c 756d            'colum
-0000daf0: 6e27 3a20 342c 0a20 2020 2020 2020 2020  n': 4,.         
-0000db00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000db10: 726f 7727 3a20 360a 2020 2020 2020 2020  row': 6.        
-0000db20: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-0000db50: 2020 2020 2020 2020 2020 2027 7369 706d             'sipm
-0000db60: 5f32 3427 3a20 7b0a 2020 2020 2020 2020  _24': {.        
+0000d900: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000d910: 2020 7265 7475 726e 7320 3a20 6469 6374    returns : dict
+0000d920: 206f 7220 4e6f 6e65 0a20 2020 2020 2020   or None.       
+0000d930: 2020 2020 204e 6f6e 6520 6973 2072 6574       None is ret
+0000d940: 7572 6e65 6420 6966 2061 6e79 2072 6571  urned if any req
+0000d950: 7569 7265 6420 6461 7475 6d20 636f 756c  uired datum coul
+0000d960: 6420 6e6f 7420 6265 206f 6274 6169 6e65  d not be obtaine
+0000d970: 642e 0a20 2020 2020 2020 2020 2020 2065  d..            e
+0000d980: 2e67 2e0a 2020 2020 2020 2020 2020 2020  .g..            
+0000d990: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000d9a0: 2020 2020 2020 2020 2020 2771 7263 6f64            'qrcod
+0000d9b0: 6527 3a20 3233 3031 3036 3033 3030 3030  e': 230106030000
+0000d9c0: 3833 3030 312c 0a20 2020 2020 2020 2020  83001,.         
+0000d9d0: 2020 2020 2020 2020 2020 2027 7670 6362             'vpcb
+0000d9e0: 5f70 6964 273a 2035 382c 0a20 2020 2020  _pid': 58,.     
+0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000da00: 7670 6362 5f61 7369 635f 7069 6427 3a20  vpcb_asic_pid': 
+0000da10: 3735 2c0a 2020 2020 2020 2020 2020 2020  75,.            
+0000da20: 2020 2020 2020 2020 2776 7469 6c65 5f70          'vtile_p
+0000da30: 6964 273a 2036 332c 0a20 2020 2020 2020  id': 63,.       
+0000da40: 2020 2020 2020 2020 2020 2020 2027 7369               'si
+0000da50: 706d 5f31 273a 207b 0a20 2020 2020 2020  pm_1': {.       
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da70: 2027 7369 706d 5f69 6427 3a20 3639 312c   'sipm_id': 691,
+0000da80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da90: 2020 2020 2020 2020 2027 6c6f 7427 3a20           'lot': 
+0000daa0: 3932 3632 3130 392c 0a20 2020 2020 2020  9262109,.       
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2027 7761 6665 725f 6e75 6d62 6572 273a   'wafer_number':
+0000dad0: 2031 352c 0a20 2020 2020 2020 2020 2020   15,.           
+0000dae0: 2020 2020 2020 2020 2020 2020 2027 636f               'co
+0000daf0: 6c75 6d6e 273a 2034 2c0a 2020 2020 2020  lumn': 4,.      
+0000db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db10: 2020 2772 6f77 273a 2036 0a20 2020 2020    'row': 6.     
+0000db20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0000db30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000db40: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2773                's
+0000db60: 6970 6d5f 3234 273a 207b 0a20 2020 2020  ipm_24': {.     
 0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2773 6970 6d5f 6964 273a 2037 3236 2c0a  'sipm_id': 726,.
-0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dba0: 2020 2020 2020 2020 276c 6f74 273a 2039          'lot': 9
-0000dbb0: 3236 3231 3039 2c0a 2020 2020 2020 2020  262109,.        
+0000db80: 2020 2027 7369 706d 5f69 6427 3a20 3732     'sipm_id': 72
+0000db90: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+0000dba0: 2020 2020 2020 2020 2020 2027 6c6f 7427             'lot'
+0000dbb0: 3a20 3932 3632 3130 392c 0a20 2020 2020  : 9262109,.     
 0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2777 6166 6572 5f6e 756d 6265 7227 3a20  'wafer_number': 
-0000dbe0: 3135 2c0a 2020 2020 2020 2020 2020 2020  15,.            
-0000dbf0: 2020 2020 2020 2020 2020 2020 2763 6f6c              'col
-0000dc00: 756d 6e27 3a20 3130 2c0a 2020 2020 2020  umn': 10,.      
+0000dbd0: 2020 2027 7761 6665 725f 6e75 6d62 6572     'wafer_number
+0000dbe0: 273a 2031 352c 0a20 2020 2020 2020 2020  ': 15,.         
+0000dbf0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000dc00: 636f 6c75 6d6e 273a 2031 302c 0a20 2020  column': 10,.   
 0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2772 6f77 273a 2034 0a20 2020 2020    'row': 4.     
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-0000dc40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dc50: 2020 2020 2020 2776 7064 755f 6964 273a        'vpdu_id':
-0000dc60: 206e 616e 2c0a 2020 2020 2020 2020 2020   nan,.          
-0000dc70: 2020 2020 2020 2020 2020 2772 756e 5f6e            'run_n
-0000dc80: 756d 6265 7227 3a20 322c 0a20 2020 2020  umber': 2,.     
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000dca0: 7072 6f64 7563 7469 6f6e 5f64 6174 6527  production_date'
-0000dcb0: 3a20 2732 3032 332d 3031 2d31 3220 3133  : '2023-01-12 13
-0000dcc0: 3a30 303a 3030 272c 0a20 2020 2020 2020  :00:00',.       
-0000dcd0: 2020 2020 2020 2020 2020 2020 2027 736f               'so
-0000dce0: 6c64 6572 5f69 6427 3a20 3133 2c0a 2020  lder_id': 13,.  
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd00: 2020 2769 6e73 7469 7475 7465 5f69 6427    'institute_id'
-0000dd10: 3a20 352c 0a20 2020 2020 2020 2020 2020  : 5,.           
-0000dd20: 2020 2020 2020 2020 2027 696e 7374 6974           'instit
-0000dd30: 7574 655f 7465 7874 273a 2027 556e 6976  ute_text': 'Univ
-0000dd40: 6572 7369 7479 206f 6620 4c69 7665 7270  ersity of Liverp
-0000dd50: 6f6f 6c27 2c0a 2020 2020 2020 2020 2020  ool',.          
-0000dd60: 2020 2020 2020 2020 2020 2773 6f6c 6465            'solde
-0000dd70: 7227 3a20 7b0a 2020 2020 2020 2020 2020  r': {.          
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000dd90: 6f6c 6465 725f 7069 6427 3a20 3133 2c0a  older_pid': 13,.
-0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddb0: 2020 2020 2020 2020 276d 616e 7566 6163          'manufac
-0000ddc0: 7475 7265 7227 3a20 342c 0a20 2020 2020  turer': 4,.     
+0000dc20: 2020 2020 2027 726f 7727 3a20 340a 2020       'row': 4.  
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+0000dc50: 2020 2020 2020 2020 2027 7670 6475 5f69           'vpdu_i
+0000dc60: 6427 3a20 6e61 6e2c 0a20 2020 2020 2020  d': nan,.       
+0000dc70: 2020 2020 2020 2020 2020 2020 2027 7275               'ru
+0000dc80: 6e5f 6e75 6d62 6572 273a 2032 2c0a 2020  n_number': 2,.  
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2770 726f 6475 6374 696f 6e5f 6461    'production_da
+0000dcb0: 7465 273a 2027 3230 3233 2d30 312d 3132  te': '2023-01-12
+0000dcc0: 2031 333a 3030 3a30 3027 2c0a 2020 2020   13:00:00',.    
+0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dce0: 2773 6f6c 6465 725f 6964 273a 2031 332c  'solder_id': 13,
+0000dcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd00: 2020 2020 2027 696e 7374 6974 7574 655f       'institute_
+0000dd10: 6964 273a 2035 2c0a 2020 2020 2020 2020  id': 5,.        
+0000dd20: 2020 2020 2020 2020 2020 2020 2769 6e73              'ins
+0000dd30: 7469 7475 7465 5f74 6578 7427 3a20 2755  titute_text': 'U
+0000dd40: 6e69 7665 7273 6974 7920 6f66 204c 6976  niversity of Liv
+0000dd50: 6572 706f 6f6c 272c 0a20 2020 2020 2020  erpool',.       
+0000dd60: 2020 2020 2020 2020 2020 2020 2027 736f               'so
+0000dd70: 6c64 6572 273a 207b 0a20 2020 2020 2020  lder': {.       
+0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd90: 2027 736f 6c64 6572 5f70 6964 273a 2031   'solder_pid': 1
+0000dda0: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+0000ddb0: 2020 2020 2020 2020 2020 2027 6d61 6e75             'manu
+0000ddc0: 6661 6374 7572 6572 273a 2034 2c0a 2020  facturer': 4,.  
 0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dde0: 2020 2027 736f 6c64 6572 5f74 7970 6527     'solder_type'
-0000ddf0: 3a20 2749 6e64 6975 6d20 5061 7374 6520  : 'Indium Paste 
-0000de00: 4e43 2d53 4d51 3830 2049 6e64 2331 4520  NC-SMQ80 Ind#1E 
-0000de10: 3532 496e 3438 536e 2e2e 2e27 2c0a 2020  52In48Sn...',.  
-0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de30: 2020 2020 2020 2770 726f 6475 6374 696f        'productio
-0000de40: 6e5f 6461 7465 273a 2027 3230 3232 2d31  n_date': '2022-1
-0000de50: 312d 3130 2030 303a 3030 3a30 3027 2c0a  1-10 00:00:00',.
-0000de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de70: 2020 2020 2020 2020 2772 6f6f 6d5f 7465          'room_te
-0000de80: 6d70 6572 6174 7572 655f 6461 7465 273a  mperature_date':
-0000de90: 2027 3230 3232 2d31 322d 3132 2031 353a   '2022-12-12 15:
-0000dea0: 3030 3a30 3027 2c0a 2020 2020 2020 2020  00:00',.        
+0000dde0: 2020 2020 2020 2773 6f6c 6465 725f 7479        'solder_ty
+0000ddf0: 7065 273a 2027 496e 6469 756d 2050 6173  pe': 'Indium Pas
+0000de00: 7465 204e 432d 534d 5138 3020 496e 6423  te NC-SMQ80 Ind#
+0000de10: 3145 2035 3249 6e34 3853 6e2e 2e2e 272c  1E 52In48Sn...',
+0000de20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000de30: 2020 2020 2020 2020 2027 7072 6f64 7563           'produc
+0000de40: 7469 6f6e 5f64 6174 6527 3a20 2732 3032  tion_date': '202
+0000de50: 322d 3131 2d31 3020 3030 3a30 303a 3030  2-11-10 00:00:00
+0000de60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000de70: 2020 2020 2020 2020 2020 2027 726f 6f6d             'room
+0000de80: 5f74 656d 7065 7261 7475 7265 5f64 6174  _temperature_dat
+0000de90: 6527 3a20 2732 3032 322d 3132 2d31 3220  e': '2022-12-12 
+0000dea0: 3135 3a30 303a 3030 272c 0a20 2020 2020  15:00:00',.     
 0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 2765 7870 6972 795f 6461 7465 273a 2027  'expiry_date': '
-0000ded0: 3230 3233 2d30 352d 3130 2030 303a 3030  2023-05-10 00:00
-0000dee0: 3a30 3027 2c0a 2020 2020 2020 2020 2020  :00',.          
-0000def0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000df00: 7972 696e 6765 5f69 6427 3a20 392c 0a20  yringe_id': 9,. 
-0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df20: 2020 2020 2020 2027 6c6f 7427 3a20 2750         'lot': 'P
-0000df30: 5331 3131 3234 3734 3027 2c0a 2020 2020  S11124740',.    
+0000dec0: 2020 2027 6578 7069 7279 5f64 6174 6527     'expiry_date'
+0000ded0: 3a20 2732 3032 332d 3035 2d31 3020 3030  : '2023-05-10 00
+0000dee0: 3a30 303a 3030 272c 0a20 2020 2020 2020  :00:00',.       
+0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df00: 2027 7379 7269 6e67 655f 6964 273a 2039   'syringe_id': 9
+0000df10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000df20: 2020 2020 2020 2020 2020 276c 6f74 273a            'lot':
+0000df30: 2027 5053 3131 3132 3437 3430 272c 0a20   'PS11124740',. 
 0000df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df50: 2020 2020 276d 6173 7327 3a20 3235 2c0a      'mass': 25,.
-0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df70: 2020 2020 2020 2020 2769 6e73 7469 7475          'institu
-0000df80: 7465 5f69 6427 3a20 350a 2020 2020 2020  te_id': 5.      
-0000df90: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-0000dfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dfb0: 2020 2020 2027 756e 6971 7565 5f77 6166       'unique_waf
-0000dfc0: 6572 7327 3a20 7b28 3932 3632 3130 392c  ers': {(9262109,
-0000dfd0: 2031 3529 2c20 2839 3236 3231 3039 2c20   15), (9262109, 
-0000dfe0: 3133 297d 0a20 2020 2020 2020 2020 2020  13)}.           
-0000dff0: 2020 2020 207d 0a20 2020 2020 2020 202d       }.        -
-0000e000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000df50: 2020 2020 2020 2027 6d61 7373 273a 2032         'mass': 2
+0000df60: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+0000df70: 2020 2020 2020 2020 2020 2027 696e 7374             'inst
+0000df80: 6974 7574 655f 6964 273a 2035 0a20 2020  itute_id': 5.   
+0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfa0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0000dfb0: 2020 2020 2020 2020 2775 6e69 7175 655f          'unique_
+0000dfc0: 7761 6665 7273 273a 207b 2839 3236 3231  wafers': {(92621
+0000dfd0: 3039 2c20 3135 292c 2028 3932 3632 3130  09, 15), (926210
+0000dfe0: 392c 2031 3329 7d0a 2020 2020 2020 2020  9, 13)}.        
+0000dff0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0000e000: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
 0000e010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000e020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000e030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e040: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
-0000e050: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0000e060: 2071 725f 636f 6465 5f76 616c 6964 2871   qr_code_valid(q
-0000e070: 7263 6f64 6529 3a0a 2020 2020 2020 2020  rcode):.        
-0000e080: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0000e090: 0a20 2020 2020 2020 2073 756d 6d61 7279  .        summary
-0000e0a0: 203d 207b 2771 7263 6f64 6527 3a20 7172   = {'qrcode': qr
-0000e0b0: 636f 6465 7d0a 0a20 2020 2020 2020 2023  code}..        #
-0000e0c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e040: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000e050: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+0000e060: 6e6f 7420 7172 5f63 6f64 655f 7661 6c69  not qr_code_vali
+0000e070: 6428 7172 636f 6465 293a 0a20 2020 2020  d(qrcode):.     
+0000e080: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000e090: 6e65 0a0a 2020 2020 2020 2020 7375 6d6d  ne..        summ
+0000e0a0: 6172 7920 3d20 7b27 7172 636f 6465 273a  ary = {'qrcode':
+0000e0b0: 2071 7263 6f64 657d 0a0a 2020 2020 2020   qrcode}..      
+0000e0c0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
 0000e0d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e0e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e0f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e100: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
-0000e110: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-0000e120: 662e 6765 7428 2776 7063 6227 2c20 7172  f.get('vpcb', qr
-0000e130: 636f 6465 3d66 277b 7172 636f 6465 7d27  code=f'{qrcode}'
-0000e140: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
-0000e150: 706f 6e73 652e 6e65 7477 6f72 6b5f 7469  ponse.network_ti
-0000e160: 6d65 6f75 743a 0a20 2020 2020 2020 2020  meout:.         
-0000e170: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-0000e180: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000e190: 2020 2020 2020 2020 2076 7063 625f 7069           vpcb_pi
-0000e1a0: 6420 3d20 696e 7428 7265 7370 6f6e 7365  d = int(response
-0000e1b0: 2e64 6174 612e 7670 6362 5f70 6964 2e76  .data.vpcb_pid.v
-0000e1c0: 616c 7565 7329 0a20 2020 2020 2020 2065  alues).        e
-0000e1d0: 7863 6570 7420 5479 7065 4572 726f 723a  xcept TypeError:
-0000e1e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000e1f0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
-0000e200: 2020 7375 6d6d 6172 795b 2776 7063 625f    summary['vpcb_
-0000e210: 7069 6427 5d20 3d20 7670 6362 5f70 6964  pid'] = vpcb_pid
-0000e220: 0a0a 2020 2020 2020 2020 2323 2323 2323  ..        ######
+0000e100: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+0000e110: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000e120: 7365 6c66 2e67 6574 2827 7670 6362 272c  self.get('vpcb',
+0000e130: 2071 7263 6f64 653d 6627 7b71 7263 6f64   qrcode=f'{qrcod
+0000e140: 657d 2729 0a20 2020 2020 2020 2069 6620  e}').        if 
+0000e150: 7265 7370 6f6e 7365 2e6e 6574 776f 726b  response.network
+0000e160: 5f74 696d 656f 7574 3a0a 2020 2020 2020  _timeout:.      
+0000e170: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+0000e180: 650a 0a20 2020 2020 2020 2074 7279 3a0a  e..        try:.
+0000e190: 2020 2020 2020 2020 2020 2020 7670 6362              vpcb
+0000e1a0: 5f70 6964 203d 2069 6e74 2872 6573 706f  _pid = int(respo
+0000e1b0: 6e73 652e 6461 7461 2e76 7063 625f 7069  nse.data.vpcb_pi
+0000e1c0: 642e 7661 6c75 6573 290a 2020 2020 2020  d.values).      
+0000e1d0: 2020 6578 6365 7074 2054 7970 6545 7272    except TypeErr
+0000e1e0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000e1f0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+0000e200: 2020 2020 2073 756d 6d61 7279 5b27 7670       summary['vp
+0000e210: 6362 5f70 6964 275d 203d 2076 7063 625f  cb_pid'] = vpcb_
+0000e220: 7069 640a 0a20 2020 2020 2020 2023 2323  pid..        ###
 0000e230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e260: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e270: 2323 2323 0a20 2020 2020 2020 2072 6573  ####.        res
-0000e280: 706f 6e73 6520 3d20 7365 6c66 2e67 6574  ponse = self.get
-0000e290: 2827 7670 6362 5f61 7369 6327 2c20 7670  ('vpcb_asic', vp
-0000e2a0: 6362 5f69 643d 7670 6362 5f70 6964 290a  cb_id=vpcb_pid).
-0000e2b0: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-0000e2c0: 6e73 652e 6e65 7477 6f72 6b5f 7469 6d65  nse.network_time
-0000e2d0: 6f75 743a 0a20 2020 2020 2020 2020 2020  out:.           
-0000e2e0: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-0000e2f0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000e300: 2020 2020 2020 7670 6362 5f61 7369 635f        vpcb_asic_
-0000e310: 7069 6420 3d20 696e 7428 7265 7370 6f6e  pid = int(respon
-0000e320: 7365 2e64 6174 612e 7670 6362 5f61 7369  se.data.vpcb_asi
-0000e330: 635f 7069 642e 7661 6c75 6573 290a 2020  c_pid.values).  
-0000e340: 2020 2020 2020 6578 6365 7074 2054 7970        except Typ
-0000e350: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-0000e360: 2020 2020 2320 736f 6d65 2076 7063 6273      # some vpcbs
-0000e370: 206e 6576 6572 2062 6563 616d 6520 7670   never became vp
-0000e380: 6362 5f61 7369 630a 2020 2020 2020 2020  cb_asic.        
-0000e390: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0000e3a0: 0a20 2020 2020 2020 2073 756d 6d61 7279  .        summary
-0000e3b0: 5b27 7670 6362 5f61 7369 635f 7069 6427  ['vpcb_asic_pid'
-0000e3c0: 5d20 3d20 7670 6362 5f61 7369 635f 7069  ] = vpcb_asic_pi
-0000e3d0: 640a 0a20 2020 2020 2020 2023 2323 2323  d..        #####
+0000e270: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+0000e280: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+0000e290: 6765 7428 2776 7063 625f 6173 6963 272c  get('vpcb_asic',
+0000e2a0: 2076 7063 625f 6964 3d76 7063 625f 7069   vpcb_id=vpcb_pi
+0000e2b0: 6429 0a20 2020 2020 2020 2069 6620 7265  d).        if re
+0000e2c0: 7370 6f6e 7365 2e6e 6574 776f 726b 5f74  sponse.network_t
+0000e2d0: 696d 656f 7574 3a0a 2020 2020 2020 2020  imeout:.        
+0000e2e0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+0000e2f0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000e300: 2020 2020 2020 2020 2076 7063 625f 6173           vpcb_as
+0000e310: 6963 5f70 6964 203d 2069 6e74 2872 6573  ic_pid = int(res
+0000e320: 706f 6e73 652e 6461 7461 2e76 7063 625f  ponse.data.vpcb_
+0000e330: 6173 6963 5f70 6964 2e76 616c 7565 7329  asic_pid.values)
+0000e340: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000e350: 5479 7065 4572 726f 723a 0a20 2020 2020  TypeError:.     
+0000e360: 2020 2020 2020 2023 2073 6f6d 6520 7670         # some vp
+0000e370: 6362 7320 6e65 7665 7220 6265 6361 6d65  cbs never became
+0000e380: 2076 7063 625f 6173 6963 0a20 2020 2020   vpcb_asic.     
+0000e390: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000e3a0: 6e65 0a0a 2020 2020 2020 2020 7375 6d6d  ne..        summ
+0000e3b0: 6172 795b 2776 7063 625f 6173 6963 5f70  ary['vpcb_asic_p
+0000e3c0: 6964 275d 203d 2076 7063 625f 6173 6963  id'] = vpcb_asic
+0000e3d0: 5f70 6964 0a0a 2020 2020 2020 2020 2323  _pid..        ##
 0000e3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e420: 2323 2323 230a 2020 2020 2020 2020 7265  #####.        re
-0000e430: 7370 6f6e 7365 203d 2073 656c 662e 6765  sponse = self.ge
-0000e440: 7428 2776 7469 6c65 272c 2076 7063 625f  t('vtile', vpcb_
-0000e450: 6173 6963 5f69 643d 7670 6362 5f61 7369  asic_id=vpcb_asi
-0000e460: 635f 7069 6429 0a20 2020 2020 2020 2069  c_pid).        i
-0000e470: 6620 7265 7370 6f6e 7365 2e6e 6574 776f  f response.netwo
-0000e480: 726b 5f74 696d 656f 7574 3a0a 2020 2020  rk_timeout:.    
-0000e490: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-0000e4a0: 6f6e 650a 2020 2020 2020 2020 7472 793a  one.        try:
-0000e4b0: 0a20 2020 2020 2020 2020 2020 2076 7469  .            vti
-0000e4c0: 6c65 5f74 6162 6c65 203d 2072 6573 706f  le_table = respo
-0000e4d0: 6e73 652e 6461 7461 2e74 6f5f 6469 6374  nse.data.to_dict
-0000e4e0: 2827 7265 636f 7264 7327 295b 2d31 5d0a  ('records')[-1].
-0000e4f0: 2020 2020 2020 2020 6578 6365 7074 2049          except I
-0000e500: 6e64 6578 4572 726f 723a 0a20 2020 2020  ndexError:.     
-0000e510: 2020 2020 2020 2023 2073 6f6d 6520 6561         # some ea
-0000e520: 726c 7920 7650 4342 2065 6e74 7269 6573  rly vPCB entries
-0000e530: 206e 6576 6572 2062 6563 616d 6520 7654   never became vT
-0000e540: 696c 6573 0a20 2020 2020 2020 2020 2020  iles.           
-0000e550: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-0000e560: 2020 2020 2020 7375 6d6d 6172 792e 7570        summary.up
-0000e570: 6461 7465 2876 7469 6c65 5f74 6162 6c65  date(vtile_table
-0000e580: 290a 2020 2020 2020 2020 6465 6c20 7375  ).        del su
-0000e590: 6d6d 6172 795b 2776 7063 625f 6173 6963  mmary['vpcb_asic
-0000e5a0: 5f69 6427 5d0a 0a20 2020 2020 2020 2023  _id']..        #
-0000e5b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e420: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+0000e430: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+0000e440: 2e67 6574 2827 7674 696c 6527 2c20 7670  .get('vtile', vp
+0000e450: 6362 5f61 7369 635f 6964 3d76 7063 625f  cb_asic_id=vpcb_
+0000e460: 6173 6963 5f70 6964 290a 2020 2020 2020  asic_pid).      
+0000e470: 2020 6966 2072 6573 706f 6e73 652e 6e65    if response.ne
+0000e480: 7477 6f72 6b5f 7469 6d65 6f75 743a 0a20  twork_timeout:. 
+0000e490: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e4a0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2074  n None.        t
+0000e4b0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000e4c0: 7674 696c 655f 7461 626c 6520 3d20 7265  vtile_table = re
+0000e4d0: 7370 6f6e 7365 2e64 6174 612e 746f 5f64  sponse.data.to_d
+0000e4e0: 6963 7428 2772 6563 6f72 6473 2729 5b2d  ict('records')[-
+0000e4f0: 315d 0a20 2020 2020 2020 2065 7863 6570  1].        excep
+0000e500: 7420 496e 6465 7845 7272 6f72 3a0a 2020  t IndexError:.  
+0000e510: 2020 2020 2020 2020 2020 2320 736f 6d65            # some
+0000e520: 2065 6172 6c79 2076 5043 4220 656e 7472   early vPCB entr
+0000e530: 6965 7320 6e65 7665 7220 6265 6361 6d65  ies never became
+0000e540: 2076 5469 6c65 730a 2020 2020 2020 2020   vTiles.        
+0000e550: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+0000e560: 0a20 2020 2020 2020 2073 756d 6d61 7279  .        summary
+0000e570: 2e75 7064 6174 6528 7674 696c 655f 7461  .update(vtile_ta
+0000e580: 626c 6529 0a20 2020 2020 2020 2064 656c  ble).        del
+0000e590: 2073 756d 6d61 7279 5b27 7670 6362 5f61   summary['vpcb_a
+0000e5a0: 7369 635f 6964 275d 0a0a 2020 2020 2020  sic_id']..      
+0000e5b0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
 0000e5c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e5d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e5e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e5f0: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
-0000e600: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-0000e610: 662e 6765 7428 2769 6e73 7469 7475 7465  f.get('institute
-0000e620: 272c 2069 643d 7674 696c 655f 7461 626c  ', id=vtile_tabl
-0000e630: 655b 2769 6e73 7469 7475 7465 5f69 6427  e['institute_id'
-0000e640: 5d29 0a20 2020 2020 2020 2069 6620 7265  ]).        if re
-0000e650: 7370 6f6e 7365 2e6e 6574 776f 726b 5f74  sponse.network_t
-0000e660: 696d 656f 7574 3a0a 2020 2020 2020 2020  imeout:.        
-0000e670: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-0000e680: 2020 2020 2020 2020 696e 7374 6974 7574          institut
-0000e690: 655f 7465 7874 203d 2072 6573 706f 6e73  e_text = respons
-0000e6a0: 652e 6461 7461 2e6e 616d 652e 7661 6c75  e.data.name.valu
-0000e6b0: 6573 5b2d 315d 0a20 2020 2020 2020 2073  es[-1].        s
-0000e6c0: 756d 6d61 7279 5b27 696e 7374 6974 7574  ummary['institut
-0000e6d0: 655f 7465 7874 275d 203d 2069 6e73 7469  e_text'] = insti
-0000e6e0: 7475 7465 5f74 6578 740a 0a20 2020 2020  tute_text..     
-0000e6f0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+0000e5f0: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
+0000e600: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000e610: 7365 6c66 2e67 6574 2827 696e 7374 6974  self.get('instit
+0000e620: 7574 6527 2c20 6964 3d76 7469 6c65 5f74  ute', id=vtile_t
+0000e630: 6162 6c65 5b27 696e 7374 6974 7574 655f  able['institute_
+0000e640: 6964 275d 290a 2020 2020 2020 2020 6966  id']).        if
+0000e650: 2072 6573 706f 6e73 652e 6e65 7477 6f72   response.networ
+0000e660: 6b5f 7469 6d65 6f75 743a 0a20 2020 2020  k_timeout:.     
+0000e670: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000e680: 6e65 0a20 2020 2020 2020 2069 6e73 7469  ne.        insti
+0000e690: 7475 7465 5f74 6578 7420 3d20 7265 7370  tute_text = resp
+0000e6a0: 6f6e 7365 2e64 6174 612e 6e61 6d65 2e76  onse.data.name.v
+0000e6b0: 616c 7565 735b 2d31 5d0a 2020 2020 2020  alues[-1].      
+0000e6c0: 2020 7375 6d6d 6172 795b 2769 6e73 7469    summary['insti
+0000e6d0: 7475 7465 5f74 6578 7427 5d20 3d20 696e  tute_text'] = in
+0000e6e0: 7374 6974 7574 655f 7465 7874 0a0a 2020  stitute_text..  
+0000e6f0: 2020 2020 2020 2323 2323 2323 2323 2323        ##########
 0000e700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e730: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
-0000e740: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000e750: 2073 656c 662e 6765 7428 2773 6f6c 6465   self.get('solde
-0000e760: 7227 2c20 736f 6c64 6572 5f70 6964 3d76  r', solder_pid=v
-0000e770: 7469 6c65 5f74 6162 6c65 5b27 736f 6c64  tile_table['sold
-0000e780: 6572 5f69 6427 5d29 0a20 2020 2020 2020  er_id']).       
-0000e790: 2069 6620 7265 7370 6f6e 7365 2e6e 6574   if response.net
-0000e7a0: 776f 726b 5f74 696d 656f 7574 3a0a 2020  work_timeout:.  
-0000e7b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e7c0: 204e 6f6e 650a 2020 2020 2020 2020 736f   None.        so
-0000e7d0: 6c64 6572 203d 2072 6573 706f 6e73 652e  lder = response.
-0000e7e0: 6461 7461 2e74 6f5f 6469 6374 2827 7265  data.to_dict('re
-0000e7f0: 636f 7264 7327 295b 2d31 5d0a 2020 2020  cords')[-1].    
-0000e800: 2020 2020 7375 6d6d 6172 795b 2773 6f6c      summary['sol
-0000e810: 6465 7227 5d20 3d20 736f 6c64 6572 0a0a  der'] = solder..
-0000e820: 2020 2020 2020 2020 2323 2323 2323 2323          ########
+0000e730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e740: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0000e750: 6520 3d20 7365 6c66 2e67 6574 2827 736f  e = self.get('so
+0000e760: 6c64 6572 272c 2073 6f6c 6465 725f 7069  lder', solder_pi
+0000e770: 643d 7674 696c 655f 7461 626c 655b 2773  d=vtile_table['s
+0000e780: 6f6c 6465 725f 6964 275d 290a 2020 2020  older_id']).    
+0000e790: 2020 2020 6966 2072 6573 706f 6e73 652e      if response.
+0000e7a0: 6e65 7477 6f72 6b5f 7469 6d65 6f75 743a  network_timeout:
+0000e7b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e7c0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+0000e7d0: 2073 6f6c 6465 7220 3d20 7265 7370 6f6e   solder = respon
+0000e7e0: 7365 2e64 6174 612e 746f 5f64 6963 7428  se.data.to_dict(
+0000e7f0: 2772 6563 6f72 6473 2729 5b2d 315d 0a20  'records')[-1]. 
+0000e800: 2020 2020 2020 2073 756d 6d61 7279 5b27         summary['
+0000e810: 736f 6c64 6572 275d 203d 2073 6f6c 6465  solder'] = solde
+0000e820: 720a 0a20 2020 2020 2020 2023 2323 2323  r..        #####
 0000e830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000e860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e870: 2323 0a20 2020 2020 2020 2023 2063 6f6d  ##.        # com
-0000e880: 7075 7465 206f 7269 6769 6e61 6c20 7761  pute original wa
-0000e890: 6665 7220 6c6f 6361 7469 6f6e 7320 666f  fer locations fo
-0000e8a0: 7220 5369 504d 730a 2020 2020 2020 2020  r SiPMs.        
-0000e8b0: 230a 2020 2020 2020 2020 2320 4974 2073  #.        # It s
-0000e8c0: 6565 6d73 2073 6166 6573 7420 746f 2061  eems safest to a
-0000e8d0: 7373 756d 6520 7468 6174 2072 6571 7565  ssume that reque
-0000e8e0: 7374 732e 5365 7373 696f 6e20 6973 206e  sts.Session is n
-0000e8f0: 6f74 2074 6872 6561 642d 7361 6665 2e0a  ot thread-safe..
-0000e900: 2020 2020 2020 2020 2320 4c65 7427 7320          # Let's 
-0000e910: 646f 2074 6869 7320 7365 7175 656e 7469  do this sequenti
-0000e920: 616c 6c79 2066 6f72 2074 6865 206d 6f6d  ally for the mom
-0000e930: 656e 742c 2061 6e64 2069 6d70 6c65 6d65  ent, and impleme
-0000e940: 6e74 2070 726f 7065 7220 7573 6520 6f66  nt proper use of
-0000e950: 0a20 2020 2020 2020 2023 2074 6865 2063  .        # the c
-0000e960: 6f6e 6e65 6374 696f 6e20 706f 6f6c 206c  onnection pool l
-0000e970: 6174 6572 2e0a 2020 2020 2020 2020 7369  ater..        si
-0000e980: 706d 7320 3d20 7b6b 3a20 7620 666f 7220  pms = {k: v for 
-0000e990: 6b2c 2076 2069 6e20 7375 6d6d 6172 792e  k, v in summary.
-0000e9a0: 6974 656d 7328 2920 6966 206b 2e73 7461  items() if k.sta
-0000e9b0: 7274 7377 6974 6828 2773 6970 6d5f 2729  rtswith('sipm_')
-0000e9c0: 7d0a 0a20 2020 2020 2020 2066 6f72 2073  }..        for s
-0000e9d0: 6970 6d5f 6e61 6d65 2c20 7369 706d 5f69  ipm_name, sipm_i
-0000e9e0: 6420 696e 2073 6970 6d73 2e69 7465 6d73  d in sipms.items
-0000e9f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000ea00: 6c6f 6361 7469 6f6e 203d 2073 656c 662e  location = self.
-0000ea10: 6765 745f 7761 6665 725f 6c6f 6361 7469  get_wafer_locati
-0000ea20: 6f6e 5f66 726f 6d5f 7369 706d 5f70 6964  on_from_sipm_pid
-0000ea30: 2873 6970 6d5f 6964 290a 2020 2020 2020  (sipm_id).      
-0000ea40: 2020 2020 2020 7375 6d6d 6172 795b 7369        summary[si
-0000ea50: 706d 5f6e 616d 655d 203d 207b 2a2a 7b27  pm_name] = {**{'
-0000ea60: 7369 706d 5f69 6427 3a20 7369 706d 5f69  sipm_id': sipm_i
-0000ea70: 647d 2c20 2a2a 6c6f 6361 7469 6f6e 7d0a  d}, **location}.
-0000ea80: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
+0000e870: 2323 2323 230a 2020 2020 2020 2020 2320  #####.        # 
+0000e880: 636f 6d70 7574 6520 6f72 6967 696e 616c  compute original
+0000e890: 2077 6166 6572 206c 6f63 6174 696f 6e73   wafer locations
+0000e8a0: 2066 6f72 2053 6950 4d73 0a20 2020 2020   for SiPMs.     
+0000e8b0: 2020 2023 0a20 2020 2020 2020 2023 2049     #.        # I
+0000e8c0: 7420 7365 656d 7320 7361 6665 7374 2074  t seems safest t
+0000e8d0: 6f20 6173 7375 6d65 2074 6861 7420 7265  o assume that re
+0000e8e0: 7175 6573 7473 2e53 6573 7369 6f6e 2069  quests.Session i
+0000e8f0: 7320 6e6f 7420 7468 7265 6164 2d73 6166  s not thread-saf
+0000e900: 652e 0a20 2020 2020 2020 2023 204c 6574  e..        # Let
+0000e910: 2773 2064 6f20 7468 6973 2073 6571 7565  's do this seque
+0000e920: 6e74 6961 6c6c 7920 666f 7220 7468 6520  ntially for the 
+0000e930: 6d6f 6d65 6e74 2c20 616e 6420 696d 706c  moment, and impl
+0000e940: 656d 656e 7420 7072 6f70 6572 2075 7365  ement proper use
+0000e950: 206f 660a 2020 2020 2020 2020 2320 7468   of.        # th
+0000e960: 6520 636f 6e6e 6563 7469 6f6e 2070 6f6f  e connection poo
+0000e970: 6c20 6c61 7465 722e 0a20 2020 2020 2020  l later..       
+0000e980: 2073 6970 6d73 203d 207b 6b3a 2076 2066   sipms = {k: v f
+0000e990: 6f72 206b 2c20 7620 696e 2073 756d 6d61  or k, v in summa
+0000e9a0: 7279 2e69 7465 6d73 2829 2069 6620 6b2e  ry.items() if k.
+0000e9b0: 7374 6172 7473 7769 7468 2827 7369 706d  startswith('sipm
+0000e9c0: 5f27 297d 0a0a 2020 2020 2020 2020 666f  _')}..        fo
+0000e9d0: 7220 7369 706d 5f6e 616d 652c 2073 6970  r sipm_name, sip
+0000e9e0: 6d5f 6964 2069 6e20 7369 706d 732e 6974  m_id in sipms.it
+0000e9f0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+0000ea00: 2020 206c 6f63 6174 696f 6e20 3d20 7365     location = se
+0000ea10: 6c66 2e67 6574 5f77 6166 6572 5f6c 6f63  lf.get_wafer_loc
+0000ea20: 6174 696f 6e5f 6672 6f6d 5f73 6970 6d5f  ation_from_sipm_
+0000ea30: 7069 6428 7369 706d 5f69 6429 0a20 2020  pid(sipm_id).   
+0000ea40: 2020 2020 2020 2020 2073 756d 6d61 7279           summary
+0000ea50: 5b73 6970 6d5f 6e61 6d65 5d20 3d20 7b2a  [sipm_name] = {*
+0000ea60: 2a7b 2773 6970 6d5f 6964 273a 2073 6970  *{'sipm_id': sip
+0000ea70: 6d5f 6964 7d2c 202a 2a6c 6f63 6174 696f  m_id}, **locatio
+0000ea80: 6e7d 0a0a 2020 2020 2020 2020 2323 2323  n}..        ####
 0000ea90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000eaa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000eab0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000eac0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000ead0: 2323 230a 2020 2020 2020 2020 2320 6765  ###.        # ge
-0000eae0: 7420 756e 6971 7565 2077 6166 6572 730a  t unique wafers.
-0000eaf0: 2020 2020 2020 2020 7375 6d6d 6172 795b          summary[
-0000eb00: 2775 6e69 7175 655f 7761 6665 7273 275d  'unique_wafers']
-0000eb10: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-0000eb20: 2028 765b 276c 6f74 275d 2c20 765b 2777   (v['lot'], v['w
-0000eb30: 6166 6572 5f6e 756d 6265 7227 5d29 0a20  afer_number']). 
-0000eb40: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0000eb50: 2c20 7620 696e 2073 756d 6d61 7279 2e69  , v in summary.i
-0000eb60: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
-0000eb70: 2020 2069 6620 6b2e 7374 6172 7473 7769     if k.startswi
-0000eb80: 7468 2827 7369 706d 5f27 290a 2020 2020  th('sipm_').    
-0000eb90: 2020 2020 7d0a 0a20 2020 2020 2020 2072      }..        r
-0000eba0: 6574 7572 6e20 7375 6d6d 6172 790a 0a20  eturn summary.. 
-0000ebb0: 2020 2064 6566 2067 6574 5f76 7469 6c65     def get_vtile
-0000ebc0: 5f70 6964 735f 6672 6f6d 5f73 6970 6d5f  _pids_from_sipm_
-0000ebd0: 7069 6473 2873 656c 662c 2073 6970 6d5f  pids(self, sipm_
-0000ebe0: 7069 6473 293a 0a20 2020 2020 2020 2022  pids):.        "
-0000ebf0: 2222 0a20 2020 2020 2020 2046 696e 6420  "".        Find 
-0000ec00: 6f75 7420 7768 6963 6820 7654 696c 6528  out which vTile(
-0000ec10: 7329 2053 6950 4d73 2068 6176 6520 6265  s) SiPMs have be
-0000ec20: 656e 2061 6c6c 6f63 6174 6564 2074 6f2e  en allocated to.
-0000ec30: 0a0a 2020 2020 2020 2020 5369 6e63 6520  ..        Since 
-0000ec40: 6120 5369 504d 2063 616e 206f 6e6c 7920  a SiPM can only 
-0000ec50: 6265 2061 7474 6163 6865 6420 746f 206f  be attached to o
-0000ec60: 6e65 2076 5469 6c65 2c20 7468 6520 7075  ne vTile, the pu
-0000ec70: 7270 6f73 6520 6f66 2074 6869 730a 2020  rpose of this.  
-0000ec80: 2020 2020 2020 6d65 7468 6f64 2069 7320        method is 
-0000ec90: 746f 2068 656c 7020 7472 6163 6b20 646f  to help track do
-0000eca0: 776e 2070 726f 626c 656d 6174 6963 2064  wn problematic d
-0000ecb0: 6174 6120 656e 7472 792e 0a0a 2020 2020  ata entry...    
-0000ecc0: 2020 2020 5741 524e 494e 473a 2054 6869      WARNING: Thi
-0000ecd0: 7320 6d65 7468 6f64 2077 696c 6c20 6265  s method will be
-0000ece0: 636f 6d65 2065 7870 656e 7369 7665 2074  come expensive t
-0000ecf0: 6f20 7275 6e20 6f6e 6365 2074 6865 2064  o run once the d
-0000ed00: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-0000ed10: 6265 636f 6d65 7320 6d6f 7265 2070 6f70  becomes more pop
-0000ed20: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
-0000ed30: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000ead0: 2323 2323 2323 0a20 2020 2020 2020 2023  ######.        #
+0000eae0: 2067 6574 2075 6e69 7175 6520 7761 6665   get unique wafe
+0000eaf0: 7273 0a20 2020 2020 2020 2073 756d 6d61  rs.        summa
+0000eb00: 7279 5b27 756e 6971 7565 5f77 6166 6572  ry['unique_wafer
+0000eb10: 7327 5d20 3d20 7b0a 2020 2020 2020 2020  s'] = {.        
+0000eb20: 2020 2020 2876 5b27 6c6f 7427 5d2c 2076      (v['lot'], v
+0000eb30: 5b27 7761 6665 725f 6e75 6d62 6572 275d  ['wafer_number']
+0000eb40: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000eb50: 7220 6b2c 2076 2069 6e20 7375 6d6d 6172  r k, v in summar
+0000eb60: 792e 6974 656d 7328 290a 2020 2020 2020  y.items().      
+0000eb70: 2020 2020 2020 6966 206b 2e73 7461 7274        if k.start
+0000eb80: 7377 6974 6828 2773 6970 6d5f 2729 0a20  swith('sipm_'). 
+0000eb90: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+0000eba0: 2020 7265 7475 726e 2073 756d 6d61 7279    return summary
+0000ebb0: 0a0a 2020 2020 6465 6620 6765 745f 7674  ..    def get_vt
+0000ebc0: 696c 655f 7069 6473 5f66 726f 6d5f 7369  ile_pids_from_si
+0000ebd0: 706d 5f70 6964 7328 7365 6c66 2c20 7369  pm_pids(self, si
+0000ebe0: 706d 5f70 6964 7329 3a0a 2020 2020 2020  pm_pids):.      
+0000ebf0: 2020 2222 220a 2020 2020 2020 2020 4669    """.        Fi
+0000ec00: 6e64 206f 7574 2077 6869 6368 2076 5469  nd out which vTi
+0000ec10: 6c65 2873 2920 5369 504d 7320 6861 7665  le(s) SiPMs have
+0000ec20: 2062 6565 6e20 616c 6c6f 6361 7465 6420   been allocated 
+0000ec30: 746f 2e0a 0a20 2020 2020 2020 2053 696e  to...        Sin
+0000ec40: 6365 2061 2053 6950 4d20 6361 6e20 6f6e  ce a SiPM can on
+0000ec50: 6c79 2062 6520 6174 7461 6368 6564 2074  ly be attached t
+0000ec60: 6f20 6f6e 6520 7654 696c 652c 2074 6865  o one vTile, the
+0000ec70: 2070 7572 706f 7365 206f 6620 7468 6973   purpose of this
+0000ec80: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
+0000ec90: 6973 2074 6f20 6865 6c70 2074 7261 636b  is to help track
+0000eca0: 2064 6f77 6e20 7072 6f62 6c65 6d61 7469   down problemati
+0000ecb0: 6320 6461 7461 2065 6e74 7279 2e0a 0a20  c data entry... 
+0000ecc0: 2020 2020 2020 2057 4152 4e49 4e47 3a20         WARNING: 
+0000ecd0: 5468 6973 206d 6574 686f 6420 7769 6c6c  This method will
+0000ece0: 2062 6563 6f6d 6520 6578 7065 6e73 6976   become expensiv
+0000ecf0: 6520 746f 2072 756e 206f 6e63 6520 7468  e to run once th
+0000ed00: 6520 6461 7461 6261 7365 0a20 2020 2020  e database.     
+0000ed10: 2020 2062 6563 6f6d 6573 206d 6f72 6520     becomes more 
+0000ed20: 706f 7075 6c61 7465 642e 0a0a 2020 2020  populated...    
+0000ed30: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 0000ed40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ed50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ed60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ed70: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000ed80: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-0000ed90: 2073 6970 6d5f 7069 6473 203a 2069 7465   sipm_pids : ite
-0000eda0: 7261 626c 6520 2863 6f6e 7461 696e 696e  rable (containin
-0000edb0: 6720 696e 7428 7329 290a 2020 2020 2020  g int(s)).      
-0000edc0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000ed70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000ed80: 2020 2061 7267 730a 2020 2020 2020 2020     args.        
+0000ed90: 2020 2020 7369 706d 5f70 6964 7320 3a20      sipm_pids : 
+0000eda0: 6974 6572 6162 6c65 2028 636f 6e74 6169  iterable (contai
+0000edb0: 6e69 6e67 2069 6e74 2873 2929 0a20 2020  ning int(s)).   
+0000edc0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 0000edd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000ede0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000edf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ee00: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000ee10: 2072 6574 7572 6e73 203a 2064 6963 7420   returns : dict 
-0000ee20: 286f 7220 4e6f 6e65 2069 6620 7468 6520  (or None if the 
-0000ee30: 6361 6c6c 6572 2073 7570 706c 6965 6420  caller supplied 
-0000ee40: 6120 6e6f 6e2d 6974 6572 6162 6c65 290a  a non-iterable).
-0000ee50: 2020 2020 2020 2020 2020 2020 7b73 6970              {sip
-0000ee60: 6d5f 7069 643a 205b 7674 696c 655f 7069  m_pid: [vtile_pi
-0000ee70: 642c 202e 2e2e 5d2c 202e 2e2e 7d0a 2020  d, ...], ...}.  
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 452e                E.
-0000ee90: 672e 207b 3139 3a20 5b36 2c20 3132 5d2c  g. {19: [6, 12],
-0000eea0: 2033 333a 205b 3132 2c20 3436 5d7d 0a20   33: [12, 46]}. 
-0000eeb0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000ee00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000ee10: 2020 2020 7265 7475 726e 7320 3a20 6469      returns : di
+0000ee20: 6374 2028 6f72 204e 6f6e 6520 6966 2074  ct (or None if t
+0000ee30: 6865 2063 616c 6c65 7220 7375 7070 6c69  he caller suppli
+0000ee40: 6564 2061 206e 6f6e 2d69 7465 7261 626c  ed a non-iterabl
+0000ee50: 6529 0a20 2020 2020 2020 2020 2020 207b  e).            {
+0000ee60: 7369 706d 5f70 6964 3a20 5b76 7469 6c65  sipm_pid: [vtile
+0000ee70: 5f70 6964 2c20 2e2e 2e5d 2c20 2e2e 2e7d  _pid, ...], ...}
+0000ee80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ee90: 2045 2e67 2e20 7b31 393a 205b 362c 2031   E.g. {19: [6, 1
+0000eea0: 325d 2c20 3333 3a20 5b31 322c 2034 365d  2], 33: [12, 46]
+0000eeb0: 7d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  }.        ------
 0000eec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000eed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000eee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000ef00: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ef10: 2020 6465 6620 7370 6964 5f74 6f5f 7670    def spid_to_vp
-0000ef20: 6964 7328 7674 5f74 6162 2c20 636f 6c6e  ids(vt_tab, coln
-0000ef30: 616d 6573 2c20 7369 706d 5f70 6964 293a  ames, sipm_pid):
-0000ef40: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0000ef50: 7369 706d 5f70 6964 202d 3e20 5b76 7469  sipm_pid -> [vti
-0000ef60: 6c65 5f70 6964 2c20 7674 696c 655f 7069  le_pid, vtile_pi
-0000ef70: 642c 202e 2e2e 5d22 2222 0a20 2020 2020  d, ...]""".     
-0000ef80: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efa0: 696e 7428 7829 0a20 2020 2020 2020 2020  int(x).         
-0000efb0: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-0000efc0: 7674 5f74 6162 2e6c 6f63 5b0a 2020 2020  vt_tab.loc[.    
+0000eef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ef00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ef10: 2020 2020 2064 6566 2073 7069 645f 746f       def spid_to
+0000ef20: 5f76 7069 6473 2876 745f 7461 622c 2063  _vpids(vt_tab, c
+0000ef30: 6f6c 6e61 6d65 732c 2073 6970 6d5f 7069  olnames, sipm_pi
+0000ef40: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+0000ef50: 2222 2273 6970 6d5f 7069 6420 2d3e 205b  """sipm_pid -> [
+0000ef60: 7674 696c 655f 7069 642c 2076 7469 6c65  vtile_pid, vtile
+0000ef70: 5f70 6964 2c20 2e2e 2e5d 2222 220a 2020  _pid, ...]""".  
+0000ef80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ef90: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0000efa0: 2020 2069 6e74 2878 290a 2020 2020 2020     int(x).      
+0000efb0: 2020 2020 2020 2020 2020 666f 7220 7820            for x 
+0000efc0: 696e 2076 745f 7461 622e 6c6f 635b 0a20  in vt_tab.loc[. 
 0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efe0: 6e70 2e77 6865 7265 2876 745f 7461 625b  np.where(vt_tab[
-0000eff0: 636f 6c6e 616d 6573 5d2e 6973 696e 285b  colnames].isin([
-0000f000: 7369 706d 5f70 6964 5d29 295b 305d 0a20  sipm_pid]))[0]. 
-0000f010: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-0000f020: 2e76 7469 6c65 5f70 6964 2e76 616c 7565  .vtile_pid.value
-0000f030: 730a 2020 2020 2020 2020 2020 2020 5d0a  s.            ].
-0000f040: 0a20 2020 2020 2020 2076 7469 6c65 5f74  .        vtile_t
-0000f050: 6162 6c65 203d 2073 656c 662e 6765 7428  able = self.get(
-0000f060: 2776 7469 6c65 2729 2e64 6174 610a 2020  'vtile').data.  
-0000f070: 2020 2020 2020 636f 6c75 6d6e 5f6e 616d        column_nam
-0000f080: 6573 203d 205b 6627 7369 706d 5f7b 787d  es = [f'sipm_{x}
-0000f090: 2720 666f 7220 7820 696e 2072 616e 6765  ' for x in range
-0000f0a0: 2831 2c20 3234 202b 2031 295d 0a0a 2020  (1, 24 + 1)]..  
-0000f0b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000f0c0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0e0: 7369 706d 5f70 6964 3a20 7370 6964 5f74  sipm_pid: spid_t
-0000f0f0: 6f5f 7670 6964 7328 7674 696c 655f 7461  o_vpids(vtile_ta
-0000f100: 626c 652c 2063 6f6c 756d 6e5f 6e61 6d65  ble, column_name
-0000f110: 732c 2073 6970 6d5f 7069 6429 0a20 2020  s, sipm_pid).   
-0000f120: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f130: 2073 6970 6d5f 7069 6420 696e 2073 6970   sipm_pid in sip
-0000f140: 6d5f 7069 6473 0a20 2020 2020 2020 2020  m_pids.         
-0000f150: 2020 207d 0a20 2020 2020 2020 2065 7863     }.        exc
-0000f160: 6570 7420 5479 7065 4572 726f 723a 0a20  ept TypeError:. 
-0000f170: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f180: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-0000f190: 6765 745f 7761 6665 725f 6c6f 6361 7469  get_wafer_locati
-0000f1a0: 6f6e 5f66 726f 6d5f 7369 706d 5f70 6964  on_from_sipm_pid
-0000f1b0: 2873 656c 662c 2073 6970 6d5f 7069 6429  (self, sipm_pid)
-0000f1c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000f1d0: 2020 2020 2020 4964 656e 7469 6679 2061        Identify a
-0000f1e0: 2053 6950 4d27 7320 6f72 6967 696e 616c   SiPM's original
-0000f1f0: 2077 6166 6572 206c 6f63 6174 696f 6e20   wafer location 
-0000f200: 6261 7365 6420 6f6e 2069 7473 2050 4944  based on its PID
-0000f210: 2e0a 0a20 2020 2020 2020 202d 2d2d 2d2d  ...        -----
+0000efe0: 2020 206e 702e 7768 6572 6528 7674 5f74     np.where(vt_t
+0000eff0: 6162 5b63 6f6c 6e61 6d65 735d 2e69 7369  ab[colnames].isi
+0000f000: 6e28 5b73 6970 6d5f 7069 645d 2929 5b30  n([sipm_pid]))[0
+0000f010: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000f020: 2020 5d2e 7674 696c 655f 7069 642e 7661    ].vtile_pid.va
+0000f030: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+0000f040: 205d 0a0a 2020 2020 2020 2020 7674 696c   ]..        vtil
+0000f050: 655f 7461 626c 6520 3d20 7365 6c66 2e67  e_table = self.g
+0000f060: 6574 2827 7674 696c 6527 292e 6461 7461  et('vtile').data
+0000f070: 0a20 2020 2020 2020 2063 6f6c 756d 6e5f  .        column_
+0000f080: 6e61 6d65 7320 3d20 5b66 2773 6970 6d5f  names = [f'sipm_
+0000f090: 7b78 7d27 2066 6f72 2078 2069 6e20 7261  {x}' for x in ra
+0000f0a0: 6e67 6528 312c 2032 3420 2b20 3129 5d0a  nge(1, 24 + 1)].
+0000f0b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000f0c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f0d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000f0e0: 2020 2073 6970 6d5f 7069 643a 2073 7069     sipm_pid: spi
+0000f0f0: 645f 746f 5f76 7069 6473 2876 7469 6c65  d_to_vpids(vtile
+0000f100: 5f74 6162 6c65 2c20 636f 6c75 6d6e 5f6e  _table, column_n
+0000f110: 616d 6573 2c20 7369 706d 5f70 6964 290a  ames, sipm_pid).
+0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f130: 666f 7220 7369 706d 5f70 6964 2069 6e20  for sipm_pid in 
+0000f140: 7369 706d 5f70 6964 730a 2020 2020 2020  sipm_pids.      
+0000f150: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0000f160: 6578 6365 7074 2054 7970 6545 7272 6f72  except TypeError
+0000f170: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f180: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
+0000f190: 6566 2067 6574 5f77 6166 6572 5f6c 6f63  ef get_wafer_loc
+0000f1a0: 6174 696f 6e5f 6672 6f6d 5f73 6970 6d5f  ation_from_sipm_
+0000f1b0: 7069 6428 7365 6c66 2c20 7369 706d 5f70  pid(self, sipm_p
+0000f1c0: 6964 293a 0a20 2020 2020 2020 2022 2222  id):.        """
+0000f1d0: 0a20 2020 2020 2020 2049 6465 6e74 6966  .        Identif
+0000f1e0: 7920 6120 5369 504d 2773 206f 7269 6769  y a SiPM's origi
+0000f1f0: 6e61 6c20 7761 6665 7220 6c6f 6361 7469  nal wafer locati
+0000f200: 6f6e 2062 6173 6564 206f 6e20 6974 7320  on based on its 
+0000f210: 5049 442e 0a0a 2020 2020 2020 2020 2d2d  PID...        --
 0000f220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f260: 2d0a 2020 2020 2020 2020 6172 6773 0a20  -.        args. 
-0000f270: 2020 2020 2020 2020 2020 2073 6970 6d5f             sipm_
-0000f280: 7069 6420 3a20 696e 740a 2020 2020 2020  pid : int.      
-0000f290: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000f260: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
+0000f270: 730a 2020 2020 2020 2020 2020 2020 7369  s.            si
+0000f280: 706d 5f70 6964 203a 2069 6e74 0a20 2020  pm_pid : int.   
+0000f290: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 0000f2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f2d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0000f2e0: 2072 6574 7572 6e73 203a 2064 6963 740a   returns : dict.
-0000f2f0: 2020 2020 2020 2020 2020 2020 452e 672e              E.g.
-0000f300: 207b 276c 6f74 273a 2039 3236 3231 3039   {'lot': 9262109
-0000f310: 2c20 2777 6166 6572 5f6e 756d 6265 7227  , 'wafer_number'
-0000f320: 3a20 3133 2c20 2763 6f6c 756d 6e27 3a20  : 13, 'column': 
-0000f330: 3132 2c20 2772 6f77 273a 2031 337d 0a20  12, 'row': 13}. 
-0000f340: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000f2d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000f2e0: 2020 2020 7265 7475 726e 7320 3a20 6469      returns : di
+0000f2f0: 6374 0a20 2020 2020 2020 2020 2020 2045  ct.            E
+0000f300: 2e67 2e20 7b27 6c6f 7427 3a20 3932 3632  .g. {'lot': 9262
+0000f310: 3130 392c 2027 7761 6665 725f 6e75 6d62  109, 'wafer_numb
+0000f320: 6572 273a 2031 332c 2027 636f 6c75 6d6e  er': 13, 'column
+0000f330: 273a 2031 322c 2027 726f 7727 3a20 3133  ': 12, 'row': 13
+0000f340: 7d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  }.        ------
 0000f350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000f390: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f3a0: 2020 7369 706d 203d 2073 656c 662e 6765    sipm = self.ge
-0000f3b0: 7428 2773 6970 6d27 2c20 7369 706d 5f70  t('sipm', sipm_p
-0000f3c0: 6964 3d73 6970 6d5f 7069 6429 2e64 6174  id=sipm_pid).dat
-0000f3d0: 612e 746f 5f64 6963 7428 2772 6563 6f72  a.to_dict('recor
-0000f3e0: 6473 2729 5b2d 315d 0a20 2020 2020 2020  ds')[-1].       
-0000f3f0: 2077 6166 6572 203d 2073 656c 662e 6765   wafer = self.ge
-0000f400: 7428 2777 6166 6572 272c 2077 6166 6572  t('wafer', wafer
-0000f410: 5f70 6964 3d73 6970 6d5b 2777 6166 6572  _pid=sipm['wafer
-0000f420: 5f69 6427 5d29 2e64 6174 612e 746f 5f64  _id']).data.to_d
-0000f430: 6963 7428 2772 6563 6f72 6473 2729 5b2d  ict('records')[-
-0000f440: 315d 0a0a 2020 2020 2020 2020 7265 7475  1]..        retu
-0000f450: 726e 207b 0a20 2020 2020 2020 2020 2020  rn {.           
-0000f460: 2027 6c6f 7427 3a20 7761 6665 725b 276c   'lot': wafer['l
-0000f470: 6f74 275d 2c0a 2020 2020 2020 2020 2020  ot'],.          
-0000f480: 2020 2777 6166 6572 5f6e 756d 6265 7227    'wafer_number'
-0000f490: 3a20 7761 6665 725b 2777 6166 6572 5f6e  : wafer['wafer_n
-0000f4a0: 756d 6265 7227 5d2c 0a20 2020 2020 2020  umber'],.       
-0000f4b0: 2020 2020 2027 636f 6c75 6d6e 273a 2073       'column': s
-0000f4c0: 6970 6d5b 2763 6f6c 756d 6e27 5d2c 0a20  ipm['column'],. 
-0000f4d0: 2020 2020 2020 2020 2020 2027 726f 7727             'row'
-0000f4e0: 3a20 7369 706d 5b27 726f 7727 5d2c 0a20  : sipm['row'],. 
-0000f4f0: 2020 2020 2020 207d 0a0a 2020 2020 2323         }..    ##
-0000f500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000f380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000f390: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f3a0: 2020 2020 2073 6970 6d20 3d20 7365 6c66       sipm = self
+0000f3b0: 2e67 6574 2827 7369 706d 272c 2073 6970  .get('sipm', sip
+0000f3c0: 6d5f 7069 643d 7369 706d 5f70 6964 292e  m_pid=sipm_pid).
+0000f3d0: 6461 7461 2e74 6f5f 6469 6374 2827 7265  data.to_dict('re
+0000f3e0: 636f 7264 7327 295b 2d31 5d0a 2020 2020  cords')[-1].    
+0000f3f0: 2020 2020 7761 6665 7220 3d20 7365 6c66      wafer = self
+0000f400: 2e67 6574 2827 7761 6665 7227 2c20 7761  .get('wafer', wa
+0000f410: 6665 725f 7069 643d 7369 706d 5b27 7761  fer_pid=sipm['wa
+0000f420: 6665 725f 6964 275d 292e 6461 7461 2e74  fer_id']).data.t
+0000f430: 6f5f 6469 6374 2827 7265 636f 7264 7327  o_dict('records'
+0000f440: 295b 2d31 5d0a 0a20 2020 2020 2020 2072  )[-1]..        r
+0000f450: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+0000f460: 2020 2020 276c 6f74 273a 2077 6166 6572      'lot': wafer
+0000f470: 5b27 6c6f 7427 5d2c 0a20 2020 2020 2020  ['lot'],.       
+0000f480: 2020 2020 2027 7761 6665 725f 6e75 6d62       'wafer_numb
+0000f490: 6572 273a 2077 6166 6572 5b27 7761 6665  er': wafer['wafe
+0000f4a0: 725f 6e75 6d62 6572 275d 2c0a 2020 2020  r_number'],.    
+0000f4b0: 2020 2020 2020 2020 2763 6f6c 756d 6e27          'column'
+0000f4c0: 3a20 7369 706d 5b27 636f 6c75 6d6e 275d  : sipm['column']
+0000f4d0: 2c0a 2020 2020 2020 2020 2020 2020 2772  ,.            'r
+0000f4e0: 6f77 273a 2073 6970 6d5b 2772 6f77 275d  ow': sipm['row']
+0000f4f0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+0000f500: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
 0000f510: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f540: 2323 2323 2323 2323 0a20 2020 2023 2072  ########.    # r
-0000f550: 6571 7565 7374 7320 4845 4144 0a20 2020  equests HEAD.   
-0000f560: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+0000f540: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+0000f550: 2320 7265 7175 6573 7473 2048 4541 440a  # requests HEAD.
+0000f560: 2020 2020 2323 2323 2323 2323 2323 2323      ############
 0000f570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f590: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f5a0: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
-0000f5b0: 2064 6566 2072 656d 6f74 655f 6669 6c65   def remote_file
-0000f5c0: 5f65 7869 7374 7328 7365 6c66 2c20 7572  _exists(self, ur
-0000f5d0: 6c29 3a0a 2020 2020 2020 2020 2222 220a  l):.        """.
-0000f5e0: 2020 2020 2020 2020 4368 6563 6b20 6966          Check if
-0000f5f0: 2061 2072 656d 6f74 6520 6669 6c65 2065   a remote file e
-0000f600: 7869 7374 7320 6174 2074 6865 2067 6976  xists at the giv
-0000f610: 656e 2055 524c 2e20 4974 2773 206f 6e6c  en URL. It's onl
-0000f620: 7920 6e65 6365 7373 6172 7920 746f 0a20  y necessary to. 
-0000f630: 2020 2020 2020 2066 6574 6368 2074 6865         fetch the
-0000f640: 2068 6561 6465 7273 2e0a 2020 2020 2020   headers..      
-0000f650: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-0000f660: 7375 6c74 203d 2046 616c 7365 0a0a 2020  sult = False..  
-0000f670: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000f680: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0000f690: 3d20 7365 6c66 2e73 6573 7369 6f6e 2e68  = self.session.h
-0000f6a0: 6561 6428 7572 6c2c 2074 696d 656f 7574  ead(url, timeout
-0000f6b0: 3d34 3629 0a20 2020 2020 2020 2065 7863  =46).        exc
-0000f6c0: 6570 7420 2872 6571 7565 7374 732e 436f  ept (requests.Co
-0000f6d0: 6e6e 6563 7469 6f6e 4572 726f 722c 2072  nnectionError, r
-0000f6e0: 6571 7565 7374 732e 6578 6365 7074 696f  equests.exceptio
-0000f6f0: 6e73 2e43 6f6e 6e65 6374 5469 6d65 6f75  ns.ConnectTimeou
-0000f700: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000f710: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0000f720: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
-0000f730: 7365 2e73 7461 7475 735f 636f 6465 2021  se.status_code !
-0000f740: 3d20 7265 7175 6573 7473 2e63 6f64 6573  = requests.codes
-0000f750: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
-0000f760: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0000f770: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000f780: 7275 650a 0a20 2020 2023 2323 2323 2323  rue..    #######
+0000f5a0: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+0000f5b0: 2020 2020 6465 6620 7265 6d6f 7465 5f66      def remote_f
+0000f5c0: 696c 655f 6578 6973 7473 2873 656c 662c  ile_exists(self,
+0000f5d0: 2075 726c 293a 0a20 2020 2020 2020 2022   url):.        "
+0000f5e0: 2222 0a20 2020 2020 2020 2043 6865 636b  "".        Check
+0000f5f0: 2069 6620 6120 7265 6d6f 7465 2066 696c   if a remote fil
+0000f600: 6520 6578 6973 7473 2061 7420 7468 6520  e exists at the 
+0000f610: 6769 7665 6e20 5552 4c2e 2049 7427 7320  given URL. It's 
+0000f620: 6f6e 6c79 206e 6563 6573 7361 7279 2074  only necessary t
+0000f630: 6f0a 2020 2020 2020 2020 6665 7463 6820  o.        fetch 
+0000f640: 7468 6520 6865 6164 6572 732e 0a20 2020  the headers..   
+0000f650: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f660: 2072 6573 756c 7420 3d20 4661 6c73 650a   result = False.
+0000f670: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+0000f680: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000f690: 7365 203d 2073 656c 662e 7365 7373 696f  se = self.sessio
+0000f6a0: 6e2e 6865 6164 2875 726c 2c20 7469 6d65  n.head(url, time
+0000f6b0: 6f75 743d 3436 290a 2020 2020 2020 2020  out=46).        
+0000f6c0: 6578 6365 7074 2028 7265 7175 6573 7473  except (requests
+0000f6d0: 2e43 6f6e 6e65 6374 696f 6e45 7272 6f72  .ConnectionError
+0000f6e0: 2c20 7265 7175 6573 7473 2e65 7863 6570  , requests.excep
+0000f6f0: 7469 6f6e 732e 436f 6e6e 6563 7454 696d  tions.ConnectTim
+0000f700: 656f 7574 293a 0a20 2020 2020 2020 2020  eout):.         
+0000f710: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000f720: 0a0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
+0000f730: 706f 6e73 652e 7374 6174 7573 5f63 6f64  ponse.status_cod
+0000f740: 6520 213d 2072 6571 7565 7374 732e 636f  e != requests.co
+0000f750: 6465 732e 6f6b 3a0a 2020 2020 2020 2020  des.ok:.        
+0000f760: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0000f770: 740a 0a20 2020 2020 2020 2072 6574 7572  t..        retur
+0000f780: 6e20 5472 7565 0a0a 2020 2020 2323 2323  n True..    ####
 0000f790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f7a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f7b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f7c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f7d0: 2323 230a 2020 2020 2320 7265 7175 6573  ###.    # reques
-0000f7e0: 7473 2050 4f53 540a 2020 2020 2323 2323  ts POST.    ####
+0000f7d0: 2323 2323 2323 0a20 2020 2023 2072 6571  ######.    # req
+0000f7e0: 7565 7374 7320 504f 5354 0a20 2020 2023  uests POST.    #
 0000f7f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f800: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f810: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f820: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f830: 2323 2323 2323 0a0a 2020 2020 2323 2323  ######..    ####
+0000f830: 2323 2323 2323 2323 230a 0a20 2020 2023  #########..    #
 0000f840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000f870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f880: 2323 2323 2323 0a20 2020 2023 2067 656e  ######.    # gen
-0000f890: 6572 6963 0a0a 2020 2020 4073 7461 7469  eric..    @stati
-0000f8a0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-0000f8b0: 5f64 6963 745f 746f 5f63 7376 5f73 7472  _dict_to_csv_str
-0000f8c0: 696e 6728 7461 626c 6529 3a0a 2020 2020  ing(table):.    
-0000f8d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f8e0: 436f 6e76 6572 7420 6120 6469 6374 696f  Convert a dictio
-0000f8f0: 6e61 7279 2069 6e74 6f20 6120 4353 562d  nary into a CSV-
-0000f900: 666f 726d 6174 7465 6420 7374 7269 6e67  formatted string
-0000f910: 2074 6861 7420 7265 7175 6573 7473 2e70   that requests.p
-0000f920: 6f73 740a 2020 2020 2020 2020 7769 6c6c  ost.        will
-0000f930: 2061 6363 6570 7420 6173 2061 2066 696c   accept as a fil
-0000f940: 652e 0a0a 2020 2020 2020 2020 5375 7070  e...        Supp
-0000f950: 6f72 7420 6675 6e63 7469 6f6e 2066 6f72  ort function for
-0000f960: 205f 706f 7374 5f67 656e 6572 6963 2829   _post_generic()
-0000f970: 2e0a 0a20 2020 2020 2020 202d 2d2d 2d2d  ...        -----
+0000f880: 2323 2323 2323 2323 230a 2020 2020 2320  #########.    # 
+0000f890: 6765 6e65 7269 630a 0a20 2020 2040 7374  generic..    @st
+0000f8a0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+0000f8b0: 6566 205f 6469 6374 5f74 6f5f 6373 765f  ef _dict_to_csv_
+0000f8c0: 7374 7269 6e67 2874 6162 6c65 293a 0a20  string(table):. 
+0000f8d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000f8e0: 2020 2043 6f6e 7665 7274 2061 2064 6963     Convert a dic
+0000f8f0: 7469 6f6e 6172 7920 696e 746f 2061 2043  tionary into a C
+0000f900: 5356 2d66 6f72 6d61 7474 6564 2073 7472  SV-formatted str
+0000f910: 696e 6720 7468 6174 2072 6571 7565 7374  ing that request
+0000f920: 732e 706f 7374 0a20 2020 2020 2020 2077  s.post.        w
+0000f930: 696c 6c20 6163 6365 7074 2061 7320 6120  ill accept as a 
+0000f940: 6669 6c65 2e0a 0a20 2020 2020 2020 2053  file...        S
+0000f950: 7570 706f 7274 2066 756e 6374 696f 6e20  upport function 
+0000f960: 666f 7220 5f70 6f73 745f 6765 6e65 7269  for _post_generi
+0000f970: 6328 292e 0a0a 2020 2020 2020 2020 2d2d  c()...        --
 0000f980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000f9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f9c0: 2d0a 2020 2020 2020 2020 6172 6773 0a20  -.        args. 
-0000f9d0: 2020 2020 2020 2020 2020 2074 6162 6c65             table
-0000f9e0: 203a 2064 6963 740a 2020 2020 2020 2020   : dict.        
-0000f9f0: 2020 2020 2020 2020 652e 672e 0a20 2020          e.g..   
+0000f9c0: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
+0000f9d0: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
+0000f9e0: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
+0000f9f0: 2020 2020 2020 2020 2020 2065 2e67 2e0a             e.g..
 0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000fa20: 2020 2020 2020 2020 2020 2027 6d61 6e75             'manu
-0000fa30: 6661 6374 7572 6572 273a 2032 2c0a 2020  facturer': 2,.  
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 2020 2020 276c 6f74 273a 2033 2c0a        'lot': 3,.
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 2020 2020 2020 2020 2777 6166 6572 5f6e          'wafer_n
-0000fa80: 756d 6265 7227 3a20 362c 0a20 2020 2020  umber': 6,.     
+0000fa10: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+0000fa30: 616e 7566 6163 7475 7265 7227 3a20 322c  anufacturer': 2,
+0000fa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fa50: 2020 2020 2020 2020 2027 6c6f 7427 3a20           'lot': 
+0000fa60: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+0000fa70: 2020 2020 2020 2020 2020 2027 7761 6665             'wafe
+0000fa80: 725f 6e75 6d62 6572 273a 2036 2c0a 2020  r_number': 6,.  
 0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faa0: 2020 2027 7370 6164 5f73 697a 6527 3a20     'spad_size': 
-0000fab0: 3330 2c0a 2020 2020 2020 2020 2020 2020  30,.            
-0000fac0: 2020 2020 2020 2020 2020 2020 2764 6f73              'dos
-0000fad0: 6527 3a20 332c 0a20 2020 2020 2020 2020  e': 3,.         
-0000fae0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000faf0: 7072 6f64 7563 7469 6f6e 5f64 6174 6527  production_date'
-0000fb00: 3a20 2732 3032 322d 3039 2d30 3620 3135  : '2022-09-06 15
-0000fb10: 3a33 303a 3134 272c 0a20 2020 2020 2020  :30:14',.       
+0000faa0: 2020 2020 2020 2773 7061 645f 7369 7a65        'spad_size
+0000fab0: 273a 2033 302c 0a20 2020 2020 2020 2020  ': 30,.         
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000fad0: 646f 7365 273a 2033 2c0a 2020 2020 2020  dose': 3,.      
+0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faf0: 2020 2770 726f 6475 6374 696f 6e5f 6461    'production_da
+0000fb00: 7465 273a 2027 3230 3232 2d30 392d 3036  te': '2022-09-06
+0000fb10: 2031 353a 3330 3a31 3427 2c0a 2020 2020   15:30:14',.    
 0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb30: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-0000fb40: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-0000fb50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0000fb60: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000fb30: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
+0000fb40: 273a 2035 2c0a 2020 2020 2020 2020 2020  ': 5,.          
+0000fb50: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+0000fb60: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 0000fb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fb80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fb90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fba0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000fbb0: 7265 7475 726e 7320 3a20 7374 7269 6e67  returns : string
-0000fbc0: 0a20 2020 2020 2020 2020 2020 2065 2e67  .            e.g
-0000fbd0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fbe0: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-0000fbf0: 2020 2020 2020 2020 276d 616e 7566 6163          'manufac
-0000fc00: 7475 7265 722c 6c6f 742c 7761 6665 725f  turer,lot,wafer_
-0000fc10: 6e75 6d62 6572 2c73 7061 645f 7369 7a65  number,spad_size
-0000fc20: 2c64 6f73 652c 270a 2020 2020 2020 2020  ,dose,'.        
-0000fc30: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-0000fc40: 6475 6374 696f 6e5f 6461 7465 2c64 6573  duction_date,des
-0000fc50: 6372 6970 7469 6f6e 5c6e 270a 2020 2020  cription\n'.    
+0000fba0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000fbb0: 2020 2072 6574 7572 6e73 203a 2073 7472     returns : str
+0000fbc0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0000fbd0: 652e 672e 0a20 2020 2020 2020 2020 2020  e.g..           
+0000fbe0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+0000fbf0: 2020 2020 2020 2020 2020 2027 6d61 6e75             'manu
+0000fc00: 6661 6374 7572 6572 2c6c 6f74 2c77 6166  facturer,lot,waf
+0000fc10: 6572 5f6e 756d 6265 722c 7370 6164 5f73  er_number,spad_s
+0000fc20: 697a 652c 646f 7365 2c27 0a20 2020 2020  ize,dose,'.     
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000fc40: 7072 6f64 7563 7469 6f6e 5f64 6174 652c  production_date,
+0000fc50: 6465 7363 7269 7074 696f 6e5c 6e27 0a20  description\n'. 
 0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2732 2c33 2c36 2c33 302c 332c 3230 3232  '2,3,6,30,3,2022
-0000fc80: 2d30 392d 3036 2031 353a 3330 3a31 342c  -09-06 15:30:14,
-0000fc90: 355c 6e27 0a20 2020 2020 2020 2020 2020  5\n'.           
-0000fca0: 2020 2020 2029 0a20 2020 2020 2020 202d       ).        -
-0000fcb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000fc70: 2020 2027 322c 332c 362c 3330 2c33 2c32     '2,3,6,30,3,2
+0000fc80: 3032 322d 3039 2d30 3620 3135 3a33 303a  022-09-06 15:30:
+0000fc90: 3134 2c35 5c6e 270a 2020 2020 2020 2020  14,5\n'.        
+0000fca0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fcb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
 0000fcc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fcd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fcf0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
-0000fd00: 220a 2020 2020 2020 2020 7369 6f20 3d20  ".        sio = 
-0000fd10: 696f 2e53 7472 696e 6749 4f28 290a 0a20  io.StringIO().. 
-0000fd20: 2020 2020 2020 2023 206d 6174 6368 206c         # match l
-0000fd30: 696e 6520 7465 726d 696e 6174 6f72 2075  ine terminator u
-0000fd40: 7365 6420 6279 2070 616e 6461 732e 4461  sed by pandas.Da
-0000fd50: 7461 4672 616d 652e 6672 6f6d 5f64 6963  taFrame.from_dic
-0000fd60: 740a 2020 2020 2020 2020 6373 7677 203d  t.        csvw =
-0000fd70: 2063 7376 2e77 7269 7465 7228 7369 6f2c   csv.writer(sio,
-0000fd80: 206c 696e 6574 6572 6d69 6e61 746f 723d   lineterminator=
-0000fd90: 275c 6e27 290a 0a20 2020 2020 2020 2063  '\n')..        c
-0000fda0: 7376 772e 7772 6974 6572 6f77 2874 6162  svw.writerow(tab
-0000fdb0: 6c65 2e6b 6579 7328 2929 0a20 2020 2020  le.keys()).     
-0000fdc0: 2020 2063 7376 772e 7772 6974 6572 6f77     csvw.writerow
-0000fdd0: 2874 6162 6c65 2e76 616c 7565 7328 2929  (table.values())
-0000fde0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000fdf0: 2073 696f 2e67 6574 7661 6c75 6528 290a   sio.getvalue().
-0000fe00: 0a20 2020 2064 6566 205f 706f 7374 5f67  .    def _post_g
-0000fe10: 656e 6572 6963 2873 656c 662c 2074 6162  eneric(self, tab
-0000fe20: 6c65 2c20 7572 6c5f 7375 6666 6978 293a  le, url_suffix):
-0000fe30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000fe40: 2020 2020 2047 656e 6572 6963 2069 6e74       Generic int
-0000fe50: 6572 6e61 6c20 6d65 6d62 6572 2066 756e  ernal member fun
-0000fe60: 6374 696f 6e20 746f 2050 4f53 5420 6120  ction to POST a 
-0000fe70: 7461 626c 6520 746f 2074 6865 2064 6174  table to the dat
-0000fe80: 6162 6173 652e 0a0a 2020 2020 2020 2020  abase...        
-0000fe90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000fcf0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000fd00: 2022 2222 0a20 2020 2020 2020 2073 696f   """.        sio
+0000fd10: 203d 2069 6f2e 5374 7269 6e67 494f 2829   = io.StringIO()
+0000fd20: 0a0a 2020 2020 2020 2020 2320 6d61 7463  ..        # matc
+0000fd30: 6820 6c69 6e65 2074 6572 6d69 6e61 746f  h line terminato
+0000fd40: 7220 7573 6564 2062 7920 7061 6e64 6173  r used by pandas
+0000fd50: 2e44 6174 6146 7261 6d65 2e66 726f 6d5f  .DataFrame.from_
+0000fd60: 6469 6374 0a20 2020 2020 2020 2063 7376  dict.        csv
+0000fd70: 7720 3d20 6373 762e 7772 6974 6572 2873  w = csv.writer(s
+0000fd80: 696f 2c20 6c69 6e65 7465 726d 696e 6174  io, lineterminat
+0000fd90: 6f72 3d27 5c6e 2729 0a0a 2020 2020 2020  or='\n')..      
+0000fda0: 2020 6373 7677 2e77 7269 7465 726f 7728    csvw.writerow(
+0000fdb0: 7461 626c 652e 6b65 7973 2829 290a 2020  table.keys()).  
+0000fdc0: 2020 2020 2020 6373 7677 2e77 7269 7465        csvw.write
+0000fdd0: 726f 7728 7461 626c 652e 7661 6c75 6573  row(table.values
+0000fde0: 2829 290a 0a20 2020 2020 2020 2072 6574  ())..        ret
+0000fdf0: 7572 6e20 7369 6f2e 6765 7476 616c 7565  urn sio.getvalue
+0000fe00: 2829 0a0a 2020 2020 6465 6620 5f70 6f73  ()..    def _pos
+0000fe10: 745f 6765 6e65 7269 6328 7365 6c66 2c20  t_generic(self, 
+0000fe20: 7461 626c 652c 2075 726c 5f73 7566 6669  table, url_suffi
+0000fe30: 7829 3a0a 2020 2020 2020 2020 2222 220a  x):.        """.
+0000fe40: 2020 2020 2020 2020 4765 6e65 7269 6320          Generic 
+0000fe50: 696e 7465 726e 616c 206d 656d 6265 7220  internal member 
+0000fe60: 6675 6e63 7469 6f6e 2074 6f20 504f 5354  function to POST
+0000fe70: 2061 2074 6162 6c65 2074 6f20 7468 6520   a table to the 
+0000fe80: 6461 7461 6261 7365 2e0a 0a20 2020 2020  database...     
+0000fe90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 0000fea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000feb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000fec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fed0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
-0000fee0: 7267 730a 2020 2020 2020 2020 2020 2020  rgs.            
-0000fef0: 7461 626c 6520 3a20 6469 6374 0a20 2020  table : dict.   
-0000ff00: 2020 2020 2020 2020 2020 2020 2065 2e67               e.g
-0000ff10: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ff20: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0000fed0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000fee0: 2020 6172 6773 0a20 2020 2020 2020 2020    args.         
+0000fef0: 2020 2074 6162 6c65 203a 2064 6963 740a     table : dict.
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff10: 652e 672e 0a20 2020 2020 2020 2020 2020  e.g..           
+0000ff20: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
 0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 276d 616e 7566 6163 7475 7265 7227 3a20  'manufacturer': 
-0000ff50: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-0000ff60: 2020 2020 2020 2020 2020 2027 6c6f 7427             'lot'
-0000ff70: 3a20 332c 0a20 2020 2020 2020 2020 2020  : 3,.           
-0000ff80: 2020 2020 2020 2020 2020 2020 2027 7761               'wa
-0000ff90: 6665 725f 6e75 6d62 6572 273a 2036 2c0a  fer_number': 6,.
-0000ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffb0: 2020 2020 2020 2020 2773 7061 645f 7369          'spad_si
-0000ffc0: 7a65 273a 2033 302c 0a20 2020 2020 2020  ze': 30,.       
+0000ff40: 2020 2027 6d61 6e75 6661 6374 7572 6572     'manufacturer
+0000ff50: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
+0000ff60: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+0000ff70: 6f74 273a 2033 2c0a 2020 2020 2020 2020  ot': 3,.        
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2777 6166 6572 5f6e 756d 6265 7227 3a20  'wafer_number': 
+0000ffa0: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+0000ffb0: 2020 2020 2020 2020 2020 2027 7370 6164             'spad
+0000ffc0: 5f73 697a 6527 3a20 3330 2c0a 2020 2020  _size': 30,.    
 0000ffd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffe0: 2027 646f 7365 273a 2033 2c0a 2020 2020   'dose': 3,.    
+0000ffe0: 2020 2020 2764 6f73 6527 3a20 332c 0a20      'dose': 3,. 
 0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010000: 2020 2020 2770 726f 6475 6374 696f 6e5f      'production_
-00010010: 6461 7465 273a 2027 3230 3232 2d30 392d  date': '2022-09-
-00010020: 3036 2031 353a 3330 3a31 3427 2c0a 2020  06 15:30:14',.  
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-00010050: 6f6e 273a 2035 2c0a 2020 2020 2020 2020  on': 5,.        
-00010060: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00010070: 2020 2020 2020 2020 2020 7572 6c5f 7375            url_su
-00010080: 6666 6978 203a 2073 7472 696e 670a 2020  ffix : string.  
-00010090: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00010000: 2020 2020 2020 2027 7072 6f64 7563 7469         'producti
+00010010: 6f6e 5f64 6174 6527 3a20 2732 3032 322d  on_date': '2022-
+00010020: 3039 2d30 3620 3135 3a33 303a 3134 272c  09-06 15:30:14',
+00010030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010040: 2020 2020 2020 2020 2027 6465 7363 7269           'descri
+00010050: 7074 696f 6e27 3a20 352c 0a20 2020 2020  ption': 5,.     
+00010060: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00010070: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+00010080: 5f73 7566 6669 7820 3a20 7374 7269 6e67  _suffix : string
+00010090: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
 000100a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000100b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000100c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000100d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-000100e0: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
-000100f0: 6f6f 6c0a 2020 2020 2020 2020 2d2d 2d2d  ool.        ----
+000100d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000100e0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+000100f0: 3a20 626f 6f6c 0a20 2020 2020 2020 202d  : bool.        -
 00010100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010140: 2d2d 0a20 2020 2020 2020 2065 7863 6570  --.        excep
-00010150: 7469 6f6e 7320 3a20 6d61 7920 7261 6973  tions : may rais
-00010160: 6520 5479 7065 4572 726f 720a 2020 2020  e TypeError.    
-00010170: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00010140: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6578  -----.        ex
+00010150: 6365 7074 696f 6e73 203a 206d 6179 2072  ceptions : may r
+00010160: 6169 7365 2054 7970 6545 7272 6f72 0a20  aise TypeError. 
+00010170: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
 00010180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000101a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000101b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-000101c0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000101d0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-000101e0: 2874 6162 6c65 2c20 6469 6374 293a 0a20  (table, dict):. 
-000101f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00010200: 2054 7970 6545 7272 6f72 2827 4578 7065   TypeError('Expe
-00010210: 6374 6564 2061 7267 756d 656e 7420 3c74  cted argument <t
-00010220: 6162 6c65 3e20 746f 2062 6520 6120 6469  able> to be a di
-00010230: 6374 696f 6e61 7279 2e27 290a 0a20 2020  ctionary.')..   
-00010240: 2020 2020 2066 756c 6c5f 7572 6c20 3d20       full_url = 
-00010250: 7572 6c6c 6962 2e70 6172 7365 2e75 726c  urllib.parse.url
-00010260: 6a6f 696e 2873 656c 662e 6261 7365 5f75  join(self.base_u
-00010270: 726c 2c20 6627 7b75 726c 5f73 7566 6669  rl, f'{url_suffi
-00010280: 787d 3f64 3d2c 2666 3d63 7376 2729 0a0a  x}?d=,&f=csv')..
-00010290: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-000102a0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000102b0: 6520 3d20 7365 6c66 2e73 6573 7369 6f6e  e = self.session
-000102c0: 2e70 6f73 7428 0a20 2020 2020 2020 2020  .post(.         
-000102d0: 2020 2020 2020 2066 756c 6c5f 7572 6c2c         full_url,
-000102e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102f0: 2066 696c 6573 3d7b 2766 696c 6527 3a20   files={'file': 
-00010300: 2827 7461 626c 652e 6373 7627 2c20 7365  ('table.csv', se
-00010310: 6c66 2e5f 6469 6374 5f74 6f5f 6373 765f  lf._dict_to_csv_
-00010320: 7374 7269 6e67 2874 6162 6c65 2929 7d0a  string(table))}.
-00010330: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00010340: 2020 2020 2020 6578 6365 7074 2068 7474        except htt
-00010350: 705f 636c 6965 6e74 2e52 656d 6f74 6544  p_client.RemoteD
-00010360: 6973 636f 6e6e 6563 7465 643a 0a20 2020  isconnected:.   
-00010370: 2020 2020 2020 2020 2073 7461 7475 7320           status 
-00010380: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00010390: 2020 2020 6c6f 6767 696e 672e 6572 726f      logging.erro
-000103a0: 7228 2772 656d 6f74 6520 6469 7363 6f6e  r('remote discon
-000103b0: 6e65 6374 6564 2729 0a20 2020 2020 2020  nected').       
-000103c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000103d0: 2020 2073 7461 7475 7320 3d20 7265 7370     status = resp
-000103e0: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
-000103f0: 203d 3d20 7265 7175 6573 7473 2e63 6f64   == requests.cod
-00010400: 6573 2e6f 6b0a 0a20 2020 2020 2020 2072  es.ok..        r
-00010410: 6574 7572 6e20 7374 6174 7573 0a0a 2020  eturn status..  
-00010420: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+000101b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+000101c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000101d0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+000101e0: 6e63 6528 7461 626c 652c 2064 6963 7429  nce(table, dict)
+000101f0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00010200: 6973 6520 5479 7065 4572 726f 7228 2745  ise TypeError('E
+00010210: 7870 6563 7465 6420 6172 6775 6d65 6e74  xpected argument
+00010220: 203c 7461 626c 653e 2074 6f20 6265 2061   <table> to be a
+00010230: 2064 6963 7469 6f6e 6172 792e 2729 0a0a   dictionary.')..
+00010240: 2020 2020 2020 2020 6675 6c6c 5f75 726c          full_url
+00010250: 203d 2075 726c 6c69 622e 7061 7273 652e   = urllib.parse.
+00010260: 7572 6c6a 6f69 6e28 7365 6c66 2e62 6173  urljoin(self.bas
+00010270: 655f 7572 6c2c 2066 277b 7572 6c5f 7375  e_url, f'{url_su
+00010280: 6666 6978 7d3f 643d 2c26 663d 6373 7627  ffix}?d=,&f=csv'
+00010290: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
+000102a0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+000102b0: 6f6e 7365 203d 2073 656c 662e 7365 7373  onse = self.sess
+000102c0: 696f 6e2e 706f 7374 280a 2020 2020 2020  ion.post(.      
+000102d0: 2020 2020 2020 2020 2020 6675 6c6c 5f75            full_u
+000102e0: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
+000102f0: 2020 2020 6669 6c65 733d 7b27 6669 6c65      files={'file
+00010300: 273a 2028 2774 6162 6c65 2e63 7376 272c  ': ('table.csv',
+00010310: 2073 656c 662e 5f64 6963 745f 746f 5f63   self._dict_to_c
+00010320: 7376 5f73 7472 696e 6728 7461 626c 6529  sv_string(table)
+00010330: 297d 0a20 2020 2020 2020 2020 2020 2029  )}.            )
+00010340: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00010350: 6874 7470 5f63 6c69 656e 742e 5265 6d6f  http_client.Remo
+00010360: 7465 4469 7363 6f6e 6e65 6374 6564 3a0a  teDisconnected:.
+00010370: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00010380: 7573 203d 2046 616c 7365 0a20 2020 2020  us = False.     
+00010390: 2020 2020 2020 206c 6f67 6769 6e67 2e65         logging.e
+000103a0: 7272 6f72 2827 7265 6d6f 7465 2064 6973  rror('remote dis
+000103b0: 636f 6e6e 6563 7465 6427 290a 2020 2020  connected').    
+000103c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000103d0: 2020 2020 2020 7374 6174 7573 203d 2072        status = r
+000103e0: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
+000103f0: 6f64 6520 3d3d 2072 6571 7565 7374 732e  ode == requests.
+00010400: 636f 6465 732e 6f6b 0a0a 2020 2020 2020  codes.ok..      
+00010410: 2020 7265 7475 726e 2073 7461 7475 730a    return status.
+00010420: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
 00010430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00010440: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00010450: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010460: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-00010470: 2023 2063 6174 6567 6f72 6963 616c 0a0a   # categorical..
-00010480: 2020 2020 6465 6620 5f62 6164 5f66 6965      def _bad_fie
-00010490: 6c64 7328 7365 6c66 2c20 7461 626c 652c  lds(self, table,
-000104a0: 2074 6162 6c65 5f6e 616d 652c 2063 6f6d   table_name, com
-000104b0: 705f 666e 293a 0a20 2020 2020 2020 2022  p_fn):.        "
-000104c0: 2222 0a20 2020 2020 2020 2054 7279 2061  "".        Try a
-000104d0: 6e64 2068 656c 7020 7468 6520 504f 5354  nd help the POST
-000104e0: 206f 7065 7261 7469 6f6e 2063 616c 6c65   operation calle
-000104f0: 7220 6279 2069 6465 6e74 6966 7969 6e67  r by identifying
-00010500: 2061 6e79 2061 6e6e 6f75 6e63 696e 670a   any announcing.
-00010510: 2020 2020 2020 2020 616e 7920 696e 636f          any inco
-00010520: 7272 6563 7420 6669 656c 6473 2c20 7261  rrect fields, ra
-00010530: 7468 6572 2074 6861 6e20 6765 7474 696e  ther than gettin
-00010540: 6720 6120 3430 3020 6261 6420 7265 7175  g a 400 bad requ
-00010550: 6573 7420 616e 6420 6c65 6176 696e 670a  est and leaving.
-00010560: 2020 2020 2020 2020 7468 6520 6361 6c6c          the call
-00010570: 6572 2077 6974 6820 6120 7265 7475 726e  er with a return
-00010580: 2076 616c 7565 206f 6620 4661 6c73 652e   value of False.
-00010590: 0a0a 2020 2020 2020 2020 4974 2773 2068  ..        It's h
-000105a0: 6967 686c 7920 6c69 6b65 6c79 2074 6865  ighly likely the
-000105b0: 2063 616c 6c65 7220 7769 6c6c 2067 6574   caller will get
-000105c0: 2074 6865 206f 7264 6572 206f 6620 7468   the order of th
-000105d0: 6520 6172 6775 6d65 6e74 730a 2020 2020  e arguments.    
-000105e0: 2020 2020 7772 6f6e 6720 6174 2073 6f6d      wrong at som
-000105f0: 6520 7374 6167 6520 7768 656e 2063 616c  e stage when cal
-00010600: 6c69 6e67 2061 2050 4f53 5420 6f70 6572  ling a POST oper
-00010610: 6174 696f 6e2e 2054 7279 2061 6e64 2061  ation. Try and a
-00010620: 766f 6964 0a20 2020 2020 2020 2073 7570  void.        sup
-00010630: 706f 7274 2069 7373 7565 7320 6279 2070  port issues by p
-00010640: 726f 7669 6469 6e67 2068 656c 7066 756c  roviding helpful
-00010650: 2066 6565 6462 6163 6b20 7768 656e 2074   feedback when t
-00010660: 6861 7420 6861 7070 656e 732e 0a0a 2020  hat happens...  
-00010670: 2020 2020 2020 4174 7465 6d70 7469 6e67        Attempting
-00010680: 2074 6f20 7772 6974 6520 6120 7461 626c   to write a tabl
-00010690: 6520 7769 7468 2061 6e20 6578 706c 6963  e with an explic
-000106a0: 6974 6c79 2073 7065 6369 6669 6564 2070  itly specified p
-000106b0: 7269 6d61 7279 206b 6579 0a20 2020 2020  rimary key.     
-000106c0: 2020 2069 7320 756e 7375 7070 6f72 7465     is unsupporte
-000106d0: 6420 6279 2074 6865 2064 6174 6162 6173  d by the databas
-000106e0: 652c 2073 6f20 616e 6e6f 756e 6365 2074  e, so announce t
-000106f0: 6869 7320 746f 2074 6865 2075 7365 722e  his to the user.
-00010700: 0a0a 2020 2020 2020 2020 636f 6d70 5f66  ..        comp_f
-00010710: 6e20 6973 2061 206c 616d 6264 6120 6578  n is a lambda ex
-00010720: 7072 6573 7369 6f6e 2075 7365 6420 746f  pression used to
-00010730: 2064 6574 6563 7420 7573 6572 2d73 7562   detect user-sub
-00010740: 6d69 7474 6564 2070 7269 6d61 7279 0a20  mitted primary. 
-00010750: 2020 2020 2020 206b 6579 732c 2073 7563         keys, suc
-00010760: 6820 7468 6174 2074 6869 7320 6d65 7468  h that this meth
-00010770: 6f64 2063 616e 2062 6520 7573 6564 2066  od can be used f
-00010780: 6f72 2063 6865 636b 696e 6720 6669 656c  or checking fiel
-00010790: 6473 2066 6f72 2069 7465 6d73 0a20 2020  ds for items.   
-000107a0: 2020 2020 2061 6e64 206d 6561 7375 7265       and measure
-000107b0: 6d65 6e74 732e 0a0a 2020 2020 2020 2020  ments...        
-000107c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010460: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00010470: 2020 2020 2320 6361 7465 676f 7269 6361      # categorica
+00010480: 6c0a 0a20 2020 2064 6566 205f 6261 645f  l..    def _bad_
+00010490: 6669 656c 6473 2873 656c 662c 2074 6162  fields(self, tab
+000104a0: 6c65 2c20 7461 626c 655f 6e61 6d65 2c20  le, table_name, 
+000104b0: 636f 6d70 5f66 6e29 3a0a 2020 2020 2020  comp_fn):.      
+000104c0: 2020 2222 220a 2020 2020 2020 2020 5472    """.        Tr
+000104d0: 7920 616e 6420 6865 6c70 2074 6865 2050  y and help the P
+000104e0: 4f53 5420 6f70 6572 6174 696f 6e20 6361  OST operation ca
+000104f0: 6c6c 6572 2062 7920 6964 656e 7469 6679  ller by identify
+00010500: 696e 6720 616e 7920 616e 6e6f 756e 6369  ing any announci
+00010510: 6e67 0a20 2020 2020 2020 2061 6e79 2069  ng.        any i
+00010520: 6e63 6f72 7265 6374 2066 6965 6c64 732c  ncorrect fields,
+00010530: 2072 6174 6865 7220 7468 616e 2067 6574   rather than get
+00010540: 7469 6e67 2061 2034 3030 2062 6164 2072  ting a 400 bad r
+00010550: 6571 7565 7374 2061 6e64 206c 6561 7669  equest and leavi
+00010560: 6e67 0a20 2020 2020 2020 2074 6865 2063  ng.        the c
+00010570: 616c 6c65 7220 7769 7468 2061 2072 6574  aller with a ret
+00010580: 7572 6e20 7661 6c75 6520 6f66 2046 616c  urn value of Fal
+00010590: 7365 2e0a 0a20 2020 2020 2020 2049 7427  se...        It'
+000105a0: 7320 6869 6768 6c79 206c 696b 656c 7920  s highly likely 
+000105b0: 7468 6520 6361 6c6c 6572 2077 696c 6c20  the caller will 
+000105c0: 6765 7420 7468 6520 6f72 6465 7220 6f66  get the order of
+000105d0: 2074 6865 2061 7267 756d 656e 7473 0a20   the arguments. 
+000105e0: 2020 2020 2020 2077 726f 6e67 2061 7420         wrong at 
+000105f0: 736f 6d65 2073 7461 6765 2077 6865 6e20  some stage when 
+00010600: 6361 6c6c 696e 6720 6120 504f 5354 206f  calling a POST o
+00010610: 7065 7261 7469 6f6e 2e20 5472 7920 616e  peration. Try an
+00010620: 6420 6176 6f69 640a 2020 2020 2020 2020  d avoid.        
+00010630: 7375 7070 6f72 7420 6973 7375 6573 2062  support issues b
+00010640: 7920 7072 6f76 6964 696e 6720 6865 6c70  y providing help
+00010650: 6675 6c20 6665 6564 6261 636b 2077 6865  ful feedback whe
+00010660: 6e20 7468 6174 2068 6170 7065 6e73 2e0a  n that happens..
+00010670: 0a20 2020 2020 2020 2041 7474 656d 7074  .        Attempt
+00010680: 696e 6720 746f 2077 7269 7465 2061 2074  ing to write a t
+00010690: 6162 6c65 2077 6974 6820 616e 2065 7870  able with an exp
+000106a0: 6c69 6369 746c 7920 7370 6563 6966 6965  licitly specifie
+000106b0: 6420 7072 696d 6172 7920 6b65 790a 2020  d primary key.  
+000106c0: 2020 2020 2020 6973 2075 6e73 7570 706f        is unsuppo
+000106d0: 7274 6564 2062 7920 7468 6520 6461 7461  rted by the data
+000106e0: 6261 7365 2c20 736f 2061 6e6e 6f75 6e63  base, so announc
+000106f0: 6520 7468 6973 2074 6f20 7468 6520 7573  e this to the us
+00010700: 6572 2e0a 0a20 2020 2020 2020 2063 6f6d  er...        com
+00010710: 705f 666e 2069 7320 6120 6c61 6d62 6461  p_fn is a lambda
+00010720: 2065 7870 7265 7373 696f 6e20 7573 6564   expression used
+00010730: 2074 6f20 6465 7465 6374 2075 7365 722d   to detect user-
+00010740: 7375 626d 6974 7465 6420 7072 696d 6172  submitted primar
+00010750: 790a 2020 2020 2020 2020 6b65 7973 2c20  y.        keys, 
+00010760: 7375 6368 2074 6861 7420 7468 6973 206d  such that this m
+00010770: 6574 686f 6420 6361 6e20 6265 2075 7365  ethod can be use
+00010780: 6420 666f 7220 6368 6563 6b69 6e67 2066  d for checking f
+00010790: 6965 6c64 7320 666f 7220 6974 656d 730a  ields for items.
+000107a0: 2020 2020 2020 2020 616e 6420 6d65 6173          and meas
+000107b0: 7572 656d 656e 7473 2e0a 0a20 2020 2020  urements...     
+000107c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 000107d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000107e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000107f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010800: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
-00010810: 7267 730a 2020 2020 2020 2020 2020 2020  rgs.            
-00010820: 7461 626c 6520 3a20 6469 6374 0a20 2020  table : dict.   
-00010830: 2020 2020 2020 2020 2020 2020 2065 2e67               e.g
-00010840: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010850: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00010800: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00010810: 2020 6172 6773 0a20 2020 2020 2020 2020    args.         
+00010820: 2020 2074 6162 6c65 203a 2064 6963 740a     table : dict.
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 652e 672e 0a20 2020 2020 2020 2020 2020  e.g..           
+00010850: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
 00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 276d 616e 7566 6163 7475 7265 7227 3a20  'manufacturer': 
-00010880: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00010890: 2020 2020 2020 2020 2020 2027 6c6f 7427             'lot'
-000108a0: 3a20 332c 0a20 2020 2020 2020 2020 2020  : 3,.           
-000108b0: 2020 2020 2020 2020 2020 2020 2027 7761               'wa
-000108c0: 6665 725f 6e75 6d62 6572 273a 2036 2c0a  fer_number': 6,.
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2020 2773 7061 645f 7369          'spad_si
-000108f0: 7a65 273a 2033 302c 0a20 2020 2020 2020  ze': 30,.       
+00010870: 2020 2027 6d61 6e75 6661 6374 7572 6572     'manufacturer
+00010880: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
+00010890: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+000108a0: 6f74 273a 2033 2c0a 2020 2020 2020 2020  ot': 3,.        
+000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2777 6166 6572 5f6e 756d 6265 7227 3a20  'wafer_number': 
+000108d0: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+000108e0: 2020 2020 2020 2020 2020 2027 7370 6164             'spad
+000108f0: 5f73 697a 6527 3a20 3330 2c0a 2020 2020  _size': 30,.    
 00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2027 646f 7365 273a 2033 2c0a 2020 2020   'dose': 3,.    
+00010910: 2020 2020 2764 6f73 6527 3a20 332c 0a20      'dose': 3,. 
 00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010930: 2020 2020 2770 726f 6475 6374 696f 6e5f      'production_
-00010940: 6461 7465 273a 2027 3230 3232 2d30 392d  date': '2022-09-
-00010950: 3036 2031 353a 3330 3a31 3427 2c0a 2020  06 15:30:14',.  
-00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
-00010980: 6f6e 273a 2035 2c0a 2020 2020 2020 2020  on': 5,.        
-00010990: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000109a0: 2020 2020 2020 2020 2020 7461 626c 655f            table_
-000109b0: 6e61 6d65 203a 2073 7472 696e 670a 2020  name : string.  
-000109c0: 2020 2020 2020 2020 2020 636f 6d70 5f66            comp_f
-000109d0: 6e20 3a20 6c61 6d62 6461 2066 756e 6374  n : lambda funct
-000109e0: 696f 6e0a 2020 2020 2020 2020 2d2d 2d2d  ion.        ----
+00010930: 2020 2020 2020 2027 7072 6f64 7563 7469         'producti
+00010940: 6f6e 5f64 6174 6527 3a20 2732 3032 322d  on_date': '2022-
+00010950: 3039 2d30 3620 3135 3a33 303a 3134 272c  09-06 15:30:14',
+00010960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010970: 2020 2020 2020 2020 2027 6465 7363 7269           'descri
+00010980: 7074 696f 6e27 3a20 352c 0a20 2020 2020  ption': 5,.     
+00010990: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000109a0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+000109b0: 6c65 5f6e 616d 6520 3a20 7374 7269 6e67  le_name : string
+000109c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000109d0: 705f 666e 203a 206c 616d 6264 6120 6675  p_fn : lambda fu
+000109e0: 6e63 7469 6f6e 0a20 2020 2020 2020 202d  nction.        -
 000109f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010a30: 2d2d 0a20 2020 2020 2020 2072 6574 7572  --.        retur
-00010a40: 6e73 203a 2062 6f6f 6c0a 2020 2020 2020  ns : bool.      
-00010a50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00010a30: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
+00010a40: 7475 726e 7320 3a20 626f 6f6c 0a20 2020  turns : bool.   
+00010a50: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 00010a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010a90: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00010aa0: 2065 7863 6570 7469 6f6e 7320 3a20 6d61   exceptions : ma
-00010ab0: 7920 7261 6973 6520 5479 7065 4572 726f  y raise TypeErro
-00010ac0: 720a 2020 2020 2020 2020 2d2d 2d2d 2d2d  r.        ------
+00010a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00010aa0: 2020 2020 6578 6365 7074 696f 6e73 203a      exceptions :
+00010ab0: 206d 6179 2072 6169 7365 2054 7970 6545   may raise TypeE
+00010ac0: 7272 6f72 0a20 2020 2020 2020 202d 2d2d  rror.        ---
 00010ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00010b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010b10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010b20: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00010b30: 7374 616e 6365 2874 6162 6c65 2c20 6469  stance(table, di
-00010b40: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-00010b50: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-00010b60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010b70: 2020 2745 7870 6563 7465 6420 6172 6775    'Expected argu
-00010b80: 6d65 6e74 203c 7461 626c 653e 2074 6f20  ment <table> to 
-00010b90: 6265 2061 2064 6963 7469 6f6e 6172 792e  be a dictionary.
-00010ba0: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00010bb0: 2020 2027 4368 6563 6b20 6172 6775 6d65     'Check argume
-00010bc0: 6e74 206f 7264 6572 2069 6e20 6675 6e63  nt order in func
-00010bd0: 7469 6f6e 2063 616c 6c2e 270a 2020 2020  tion call.'.    
-00010be0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00010bf0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00010c00: 2020 2020 6462 5f66 6965 6c64 7320 3d20      db_fields = 
-00010c10: 7365 6c66 2e64 6573 6372 6962 6528 7461  self.describe(ta
-00010c20: 626c 655f 6e61 6d65 292e 6461 7461 0a20  ble_name).data. 
-00010c30: 2020 2020 2020 2065 7863 6570 7420 5479         except Ty
-00010c40: 7065 4572 726f 723a 0a20 2020 2020 2020  peError:.       
-00010c50: 2020 2020 206c 6f67 6769 6e67 2e65 7272       logging.err
-00010c60: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00010c70: 2020 2020 2741 7267 756d 656e 7420 6f72      'Argument or
-00010c80: 6465 7220 7375 7070 6c69 6564 2074 6f20  der supplied to 
-00010c90: 6675 6e63 7469 6f6e 206d 6179 2062 6520  function may be 
-00010ca0: 696e 636f 7272 6563 742e 270a 2020 2020  incorrect.'.    
-00010cb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010cc0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00010cd0: 650a 0a20 2020 2020 2020 2075 6e72 6563  e..        unrec
-00010ce0: 6f67 6e69 7365 645f 6669 656c 6473 203d  ognised_fields =
-00010cf0: 207b 0a20 2020 2020 2020 2020 2020 2075   {.            u
-00010d00: 7365 725f 6669 656c 640a 2020 2020 2020  ser_field.      
-00010d10: 2020 2020 2020 666f 7220 7573 6572 5f66        for user_f
-00010d20: 6965 6c64 2069 6e20 7461 626c 650a 2020  ield in table.  
-00010d30: 2020 2020 2020 2020 2020 6966 2075 7365            if use
-00010d40: 725f 6669 656c 6420 6e6f 7420 696e 2064  r_field not in d
-00010d50: 625f 6669 656c 6473 0a20 2020 2020 2020  b_fields.       
-00010d60: 207d 0a0a 2020 2020 2020 2020 666f 7220   }..        for 
-00010d70: 6669 656c 6420 696e 2075 6e72 6563 6f67  field in unrecog
-00010d80: 6e69 7365 645f 6669 656c 6473 3a0a 2020  nised_fields:.  
-00010d90: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-00010da0: 672e 6572 726f 7228 0a20 2020 2020 2020  g.error(.       
-00010db0: 2020 2020 2020 2020 2027 7461 626c 6520           'table 
-00010dc0: 2573 2c20 756e 7265 636f 676e 6973 6564  %s, unrecognised
-00010dd0: 2066 6965 6c64 3a20 2573 272c 2074 6162   field: %s', tab
-00010de0: 6c65 5f6e 616d 652c 2066 6965 6c64 0a20  le_name, field. 
-00010df0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00010e00: 2020 2020 2020 2320 6164 6469 7469 6f6e        # addition
-00010e10: 616c 2063 6865 636b 2066 6f72 2070 7269  al check for pri
-00010e20: 6d61 7279 206b 6579 730a 2020 2020 2020  mary keys.      
-00010e30: 2020 7072 696d 6172 795f 6b65 7973 203d    primary_keys =
-00010e40: 207b 7573 6572 5f66 6965 6c64 2066 6f72   {user_field for
-00010e50: 2075 7365 725f 6669 656c 6420 696e 2074   user_field in t
-00010e60: 6162 6c65 2069 6620 636f 6d70 5f66 6e28  able if comp_fn(
-00010e70: 7573 6572 5f66 6965 6c64 297d 0a20 2020  user_field)}.   
-00010e80: 2020 2020 2066 6f72 2070 7269 6d61 7279       for primary
-00010e90: 5f6b 6579 2069 6e20 7072 696d 6172 795f  _key in primary_
-00010ea0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00010eb0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
-00010ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ed0: 2027 6578 706c 6963 6974 6c79 2073 7065   'explicitly spe
-00010ee0: 6369 6669 6564 2070 7269 6d61 7279 206b  cified primary k
-00010ef0: 6579 7320 6172 6520 756e 7375 7070 6f72  eys are unsuppor
-00010f00: 7465 643a 2025 7327 2c20 7072 696d 6172  ted: %s', primar
-00010f10: 795f 6b65 790a 2020 2020 2020 2020 2020  y_key.          
-00010f20: 2020 290a 0a20 2020 2020 2020 2023 2063    )..        # c
-00010f30: 6865 636b 2066 6f72 2028 706f 7465 6e74  heck for (potent
-00010f40: 6961 6c6c 7929 206d 6973 7369 6e67 2066  ially) missing f
-00010f50: 6965 6c64 730a 2020 2020 2020 2020 2320  ields.        # 
-00010f60: 5468 6973 206d 6179 2067 656e 6572 6174  This may generat
-00010f70: 6520 736f 6d65 2066 616c 7365 2070 6f73  e some false pos
-00010f80: 6974 6976 6573 2066 6f72 2066 6965 6c64  itives for field
-00010f90: 7320 7468 6174 2061 7265 206f 7074 696f  s that are optio
-00010fa0: 6e61 6c0a 2020 2020 2020 2020 2320 286e  nal.        # (n
-00010fb0: 6f74 2073 7065 6369 6669 6564 2061 7320  ot specified as 
-00010fc0: 6e6f 6e2d 4e55 4c4c 292e 0a20 2020 2020  non-NULL)..     
-00010fd0: 2020 2066 6f72 2064 625f 6669 656c 6420     for db_field 
-00010fe0: 696e 2064 625f 6669 656c 6473 3a0a 2020  in db_fields:.  
-00010ff0: 2020 2020 2020 2020 2020 6966 2063 6f6d            if com
-00011000: 705f 666e 2864 625f 6669 656c 6429 3a0a  p_fn(db_field):.
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-00011030: 2020 2020 2020 6966 2064 625f 6669 656c        if db_fiel
-00011040: 6420 6e6f 7420 696e 2074 6162 6c65 3a0a  d not in table:.
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-00011070: 276d 6973 7369 6e67 2066 6965 6c64 3a20  'missing field: 
-00011080: 2573 272c 2064 625f 6669 656c 6429 0a0a  %s', db_field)..
-00011090: 2020 2020 2020 2020 7265 7475 726e 2062          return b
-000110a0: 6f6f 6c28 756e 7265 636f 676e 6973 6564  ool(unrecognised
-000110b0: 5f66 6965 6c64 7329 0a0a 2020 2020 6465  _fields)..    de
-000110c0: 6620 706f 7374 5f69 7465 6d28 7365 6c66  f post_item(self
-000110d0: 2c20 7461 626c 652c 2074 6162 6c65 5f6e  , table, table_n
-000110e0: 616d 6529 3a0a 2020 2020 2020 2020 2222  ame):.        ""
-000110f0: 220a 2020 2020 2020 2020 504f 5354 2061  ".        POST a
-00011100: 2074 6162 6c65 2066 6f72 2061 2022 7068   table for a "ph
-00011110: 7973 6963 616c 2220 6974 656d 2074 6f20  ysical" item to 
-00011120: 7468 6520 6461 7461 6261 7365 2e0a 0a20  the database... 
-00011130: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00010b10: 2d2d 2d0a 2020 2020 2020 2020 2222 220a  ---.        """.
+00010b20: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00010b30: 7369 6e73 7461 6e63 6528 7461 626c 652c  sinstance(table,
+00010b40: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00010b50: 2020 2020 7261 6973 6520 5479 7065 4572      raise TypeEr
+00010b60: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00010b70: 2020 2020 2027 4578 7065 6374 6564 2061       'Expected a
+00010b80: 7267 756d 656e 7420 3c74 6162 6c65 3e20  rgument <table> 
+00010b90: 746f 2062 6520 6120 6469 6374 696f 6e61  to be a dictiona
+00010ba0: 7279 2e20 270a 2020 2020 2020 2020 2020  ry. '.          
+00010bb0: 2020 2020 2020 2743 6865 636b 2061 7267        'Check arg
+00010bc0: 756d 656e 7420 6f72 6465 7220 696e 2066  ument order in f
+00010bd0: 756e 6374 696f 6e20 6361 6c6c 2e27 0a20  unction call.'. 
+00010be0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00010bf0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00010c00: 2020 2020 2020 2064 625f 6669 656c 6473         db_fields
+00010c10: 203d 2073 656c 662e 6465 7363 7269 6265   = self.describe
+00010c20: 2874 6162 6c65 5f6e 616d 6529 2e64 6174  (table_name).dat
+00010c30: 610a 2020 2020 2020 2020 6578 6365 7074  a.        except
+00010c40: 2054 7970 6545 7272 6f72 3a0a 2020 2020   TypeError:.    
+00010c50: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00010c60: 6572 726f 7228 0a20 2020 2020 2020 2020  error(.         
+00010c70: 2020 2020 2020 2027 4172 6775 6d65 6e74         'Argument
+00010c80: 206f 7264 6572 2073 7570 706c 6965 6420   order supplied 
+00010c90: 746f 2066 756e 6374 696f 6e20 6d61 7920  to function may 
+00010ca0: 6265 2069 6e63 6f72 7265 6374 2e27 0a20  be incorrect.'. 
+00010cb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010cc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00010cd0: 5472 7565 0a0a 2020 2020 2020 2020 756e  True..        un
+00010ce0: 7265 636f 676e 6973 6564 5f66 6965 6c64  recognised_field
+00010cf0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
+00010d00: 2020 7573 6572 5f66 6965 6c64 0a20 2020    user_field.   
+00010d10: 2020 2020 2020 2020 2066 6f72 2075 7365           for use
+00010d20: 725f 6669 656c 6420 696e 2074 6162 6c65  r_field in table
+00010d30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00010d40: 7573 6572 5f66 6965 6c64 206e 6f74 2069  user_field not i
+00010d50: 6e20 6462 5f66 6965 6c64 730a 2020 2020  n db_fields.    
+00010d60: 2020 2020 7d0a 0a20 2020 2020 2020 2066      }..        f
+00010d70: 6f72 2066 6965 6c64 2069 6e20 756e 7265  or field in unre
+00010d80: 636f 676e 6973 6564 5f66 6965 6c64 733a  cognised_fields:
+00010d90: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00010da0: 6769 6e67 2e65 7272 6f72 280a 2020 2020  ging.error(.    
+00010db0: 2020 2020 2020 2020 2020 2020 2774 6162              'tab
+00010dc0: 6c65 2025 732c 2075 6e72 6563 6f67 6e69  le %s, unrecogni
+00010dd0: 7365 6420 6669 656c 643a 2025 7327 2c20  sed field: %s', 
+00010de0: 7461 626c 655f 6e61 6d65 2c20 6669 656c  table_name, fiel
+00010df0: 640a 2020 2020 2020 2020 2020 2020 290a  d.            ).
+00010e00: 0a20 2020 2020 2020 2023 2061 6464 6974  .        # addit
+00010e10: 696f 6e61 6c20 6368 6563 6b20 666f 7220  ional check for 
+00010e20: 7072 696d 6172 7920 6b65 7973 0a20 2020  primary keys.   
+00010e30: 2020 2020 2070 7269 6d61 7279 5f6b 6579       primary_key
+00010e40: 7320 3d20 7b75 7365 725f 6669 656c 6420  s = {user_field 
+00010e50: 666f 7220 7573 6572 5f66 6965 6c64 2069  for user_field i
+00010e60: 6e20 7461 626c 6520 6966 2063 6f6d 705f  n table if comp_
+00010e70: 666e 2875 7365 725f 6669 656c 6429 7d0a  fn(user_field)}.
+00010e80: 2020 2020 2020 2020 666f 7220 7072 696d          for prim
+00010e90: 6172 795f 6b65 7920 696e 2070 7269 6d61  ary_key in prima
+00010ea0: 7279 5f6b 6579 733a 0a20 2020 2020 2020  ry_keys:.       
+00010eb0: 2020 2020 206c 6f67 6769 6e67 2e65 7272       logging.err
+00010ec0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00010ed0: 2020 2020 2765 7870 6c69 6369 746c 7920      'explicitly 
+00010ee0: 7370 6563 6966 6965 6420 7072 696d 6172  specified primar
+00010ef0: 7920 6b65 7973 2061 7265 2075 6e73 7570  y keys are unsup
+00010f00: 706f 7274 6564 3a20 2573 272c 2070 7269  ported: %s', pri
+00010f10: 6d61 7279 5f6b 6579 0a20 2020 2020 2020  mary_key.       
+00010f20: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00010f30: 2320 6368 6563 6b20 666f 7220 2870 6f74  # check for (pot
+00010f40: 656e 7469 616c 6c79 2920 6d69 7373 696e  entially) missin
+00010f50: 6720 6669 656c 6473 0a20 2020 2020 2020  g fields.       
+00010f60: 2023 2054 6869 7320 6d61 7920 6765 6e65   # This may gene
+00010f70: 7261 7465 2073 6f6d 6520 6661 6c73 6520  rate some false 
+00010f80: 706f 7369 7469 7665 7320 666f 7220 6669  positives for fi
+00010f90: 656c 6473 2074 6861 7420 6172 6520 6f70  elds that are op
+00010fa0: 7469 6f6e 616c 0a20 2020 2020 2020 2023  tional.        #
+00010fb0: 2028 6e6f 7420 7370 6563 6966 6965 6420   (not specified 
+00010fc0: 6173 206e 6f6e 2d4e 554c 4c29 2e0a 2020  as non-NULL)..  
+00010fd0: 2020 2020 2020 666f 7220 6462 5f66 6965        for db_fie
+00010fe0: 6c64 2069 6e20 6462 5f66 6965 6c64 733a  ld in db_fields:
+00010ff0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011000: 636f 6d70 5f66 6e28 6462 5f66 6965 6c64  comp_fn(db_field
+00011010: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011020: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+00011030: 2020 2020 2020 2020 2069 6620 6462 5f66           if db_f
+00011040: 6965 6c64 206e 6f74 2069 6e20 7461 626c  ield not in tabl
+00011050: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011060: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+00011070: 6e67 2827 6d69 7373 696e 6720 6669 656c  ng('missing fiel
+00011080: 643a 2025 7327 2c20 6462 5f66 6965 6c64  d: %s', db_field
+00011090: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+000110a0: 6e20 626f 6f6c 2875 6e72 6563 6f67 6e69  n bool(unrecogni
+000110b0: 7365 645f 6669 656c 6473 290a 0a20 2020  sed_fields)..   
+000110c0: 2064 6566 2070 6f73 745f 6974 656d 2873   def post_item(s
+000110d0: 656c 662c 2074 6162 6c65 2c20 7461 626c  elf, table, tabl
+000110e0: 655f 6e61 6d65 293a 0a20 2020 2020 2020  e_name):.       
+000110f0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
+00011100: 5420 6120 7461 626c 6520 666f 7220 6120  T a table for a 
+00011110: 2270 6879 7369 6361 6c22 2069 7465 6d20  "physical" item 
+00011120: 746f 2074 6865 2064 6174 6162 6173 652e  to the database.
+00011130: 0a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
 00011140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00011180: 2020 2020 2020 6172 6773 0a20 2020 2020        args.     
-00011190: 2020 2020 2020 2074 6162 6c65 203a 2064         table : d
-000111a0: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
-000111b0: 2020 2020 652e 672e 0a20 2020 2020 2020      e.g..       
-000111c0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 2027 6d61 6e75 6661 6374         'manufact
-000111f0: 7572 6572 273a 2032 2c0a 2020 2020 2020  urer': 2,.      
+00011170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011180: 0a20 2020 2020 2020 2061 7267 730a 2020  .        args.  
+00011190: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+000111a0: 3a20 6469 6374 0a20 2020 2020 2020 2020  : dict.         
+000111b0: 2020 2020 2020 2065 2e67 2e0a 2020 2020         e.g..    
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000111e0: 2020 2020 2020 2020 2020 276d 616e 7566            'manuf
+000111f0: 6163 7475 7265 7227 3a20 322c 0a20 2020  acturer': 2,.   
 00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 276c 6f74 273a 2033 2c0a 2020 2020    'lot': 3,.    
+00011210: 2020 2020 2027 6c6f 7427 3a20 332c 0a20       'lot': 3,. 
 00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 2020 2777 6166 6572 5f6e 756d 6265      'wafer_numbe
-00011240: 7227 3a20 362c 0a20 2020 2020 2020 2020  r': 6,.         
-00011250: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00011260: 7370 6164 5f73 697a 6527 3a20 3330 2c0a  spad_size': 30,.
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2020 2020 2020 2764 6f73 6527 3a20          'dose': 
-00011290: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-000112a0: 2020 2020 2020 2020 2020 2027 7072 6f64             'prod
-000112b0: 7563 7469 6f6e 5f64 6174 6527 3a20 2732  uction_date': '2
-000112c0: 3032 322d 3039 2d30 3620 3135 3a33 303a  022-09-06 15:30:
-000112d0: 3134 272c 0a20 2020 2020 2020 2020 2020  14',.           
-000112e0: 2020 2020 2020 2020 2020 2020 2027 6465               'de
-000112f0: 7363 7269 7074 696f 6e27 3a20 352c 0a20  scription': 5,. 
-00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011310: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00011320: 2074 6162 6c65 5f6e 616d 6520 3a20 7374   table_name : st
-00011330: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
-00011340: 2020 2020 2065 2e67 2e20 2777 6166 6572       e.g. 'wafer
-00011350: 270a 2020 2020 2020 2020 2d2d 2d2d 2d2d  '.        ------
+00011230: 2020 2020 2020 2027 7761 6665 725f 6e75         'wafer_nu
+00011240: 6d62 6572 273a 2036 2c0a 2020 2020 2020  mber': 6,.      
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011260: 2020 2773 7061 645f 7369 7a65 273a 2033    'spad_size': 3
+00011270: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00011280: 2020 2020 2020 2020 2020 2027 646f 7365             'dose
+00011290: 273a 2033 2c0a 2020 2020 2020 2020 2020  ': 3,.          
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+000112b0: 726f 6475 6374 696f 6e5f 6461 7465 273a  roduction_date':
+000112c0: 2027 3230 3232 2d30 392d 3036 2031 353a   '2022-09-06 15:
+000112d0: 3330 3a31 3427 2c0a 2020 2020 2020 2020  30:14',.        
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2764 6573 6372 6970 7469 6f6e 273a 2035  'description': 5
+00011300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011310: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00011320: 2020 2020 7461 626c 655f 6e61 6d65 203a      table_name :
+00011330: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00011340: 2020 2020 2020 2020 652e 672e 2027 7761          e.g. 'wa
+00011350: 6665 7227 0a20 2020 2020 2020 202d 2d2d  fer'.        ---
 00011360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000113a0: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
-000113b0: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
-000113c0: 2020 2020 5375 6363 6573 7320 6f66 2050      Success of P
-000113d0: 4f53 5420 6f70 6572 6174 696f 6e2e 0a20  OST operation.. 
-000113e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000113a0: 2d2d 2d0a 2020 2020 2020 2020 7265 7475  ---.        retu
+000113b0: 726e 7320 3a20 626f 6f6c 0a20 2020 2020  rns : bool.     
+000113c0: 2020 2020 2020 2053 7563 6365 7373 206f         Success o
+000113d0: 6620 504f 5354 206f 7065 7261 7469 6f6e  f POST operation
+000113e0: 2e0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
 000113f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00011430: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011440: 2020 2320 736b 6970 2074 6865 2050 4f53    # skip the POS
-00011450: 5420 6f70 6572 6174 696f 6e20 6966 2069  T operation if i
-00011460: 7420 7769 6c6c 2063 6572 7461 696e 6c79  t will certainly
-00011470: 2066 6169 6c0a 2020 2020 2020 2020 6966   fail.        if
-00011480: 2073 656c 662e 5f62 6164 5f66 6965 6c64   self._bad_field
-00011490: 7328 7461 626c 652c 2074 6162 6c65 5f6e  s(table, table_n
-000114a0: 616d 652c 206c 616d 6264 6120 663a 2066  ame, lambda f: f
-000114b0: 2e65 6e64 7377 6974 6828 275f 7069 6427  .endswith('_pid'
-000114c0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-000114d0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-000114e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000114f0: 662e 5f70 6f73 745f 6765 6e65 7269 6328  f._post_generic(
-00011500: 7461 626c 652c 2066 2769 7465 6d2f 7b74  table, f'item/{t
-00011510: 6162 6c65 5f6e 616d 657d 2729 0a0a 2020  able_name}')..  
-00011520: 2020 6465 6620 706f 7374 5f6d 6561 7375    def post_measu
-00011530: 7265 6d65 6e74 2873 656c 662c 2074 6162  rement(self, tab
-00011540: 6c65 2c20 7461 626c 655f 6e61 6d65 293a  le, table_name):
-00011550: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011560: 2020 2020 2050 4f53 5420 6120 7461 626c       POST a tabl
-00011570: 6520 666f 7220 6120 7465 7374 2072 6573  e for a test res
-00011580: 756c 7420 746f 2074 6865 2064 6174 6162  ult to the datab
-00011590: 6173 652e 0a0a 2020 2020 2020 2020 2d2d  ase...        --
-000115a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011430: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011440: 2020 2020 2023 2073 6b69 7020 7468 6520       # skip the 
+00011450: 504f 5354 206f 7065 7261 7469 6f6e 2069  POST operation i
+00011460: 6620 6974 2077 696c 6c20 6365 7274 6169  f it will certai
+00011470: 6e6c 7920 6661 696c 0a20 2020 2020 2020  nly fail.       
+00011480: 2069 6620 7365 6c66 2e5f 6261 645f 6669   if self._bad_fi
+00011490: 656c 6473 2874 6162 6c65 2c20 7461 626c  elds(table, tabl
+000114a0: 655f 6e61 6d65 2c20 6c61 6d62 6461 2066  e_name, lambda f
+000114b0: 3a20 662e 656e 6473 7769 7468 2827 5f70  : f.endswith('_p
+000114c0: 6964 2729 293a 0a20 2020 2020 2020 2020  id')):.         
+000114d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+000114e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000114f0: 7365 6c66 2e5f 706f 7374 5f67 656e 6572  self._post_gener
+00011500: 6963 2874 6162 6c65 2c20 6627 6974 656d  ic(table, f'item
+00011510: 2f7b 7461 626c 655f 6e61 6d65 7d27 290a  /{table_name}').
+00011520: 0a20 2020 2064 6566 2070 6f73 745f 6d65  .    def post_me
+00011530: 6173 7572 656d 656e 7428 7365 6c66 2c20  asurement(self, 
+00011540: 7461 626c 652c 2074 6162 6c65 5f6e 616d  table, table_nam
+00011550: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00011560: 2020 2020 2020 2020 504f 5354 2061 2074          POST a t
+00011570: 6162 6c65 2066 6f72 2061 2074 6573 7420  able for a test 
+00011580: 7265 7375 6c74 2074 6f20 7468 6520 6461  result to the da
+00011590: 7461 6261 7365 2e0a 0a20 2020 2020 2020  tabase...       
+000115a0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 000115b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000115c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000115d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000115e0: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
-000115f0: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
-00011600: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
-00011610: 2020 2020 2020 2020 2020 2065 2e67 2e0a             e.g..
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00011640: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00011650: 616e 7566 6163 7475 7265 7227 3a20 322c  anufacturer': 2,
-00011660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011670: 2020 2020 2020 2020 2027 6c6f 7427 3a20           'lot': 
-00011680: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-00011690: 2020 2020 2020 2020 2020 2027 7761 6665             'wafe
-000116a0: 725f 6e75 6d62 6572 273a 2036 2c0a 2020  r_number': 6,.  
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 2020 2020 2773 7061 645f 7369 7a65        'spad_size
-000116d0: 273a 2033 302c 0a20 2020 2020 2020 2020  ': 30,.         
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000116f0: 646f 7365 273a 2033 2c0a 2020 2020 2020  dose': 3,.      
+000115e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000115f0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
+00011600: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
+00011610: 2020 2020 2020 2020 2020 2020 2020 652e                e.
+00011620: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
+00011630: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 2027 6d61 6e75 6661 6374 7572 6572 273a   'manufacturer':
+00011660: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+00011670: 2020 2020 2020 2020 2020 2020 276c 6f74              'lot
+00011680: 273a 2033 2c0a 2020 2020 2020 2020 2020  ': 3,.          
+00011690: 2020 2020 2020 2020 2020 2020 2020 2777                'w
+000116a0: 6166 6572 5f6e 756d 6265 7227 3a20 362c  afer_number': 6,
+000116b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000116c0: 2020 2020 2020 2020 2027 7370 6164 5f73           'spad_s
+000116d0: 697a 6527 3a20 3330 2c0a 2020 2020 2020  ize': 30,.      
+000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116f0: 2020 2764 6f73 6527 3a20 332c 0a20 2020    'dose': 3,.   
 00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011710: 2020 2770 726f 6475 6374 696f 6e5f 6461    'production_da
-00011720: 7465 273a 2027 3230 3232 2d30 392d 3036  te': '2022-09-06
-00011730: 2031 353a 3330 3a31 3427 2c0a 2020 2020   15:30:14',.    
+00011710: 2020 2020 2027 7072 6f64 7563 7469 6f6e       'production
+00011720: 5f64 6174 6527 3a20 2732 3032 322d 3039  _date': '2022-09
+00011730: 2d30 3620 3135 3a33 303a 3134 272c 0a20  -06 15:30:14',. 
 00011740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011750: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
-00011760: 273a 2035 2c0a 2020 2020 2020 2020 2020  ': 5,.          
-00011770: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00011780: 2020 2020 2020 2020 7461 626c 655f 6e61          table_na
-00011790: 6d65 203a 2073 7472 696e 670a 2020 2020  me : string.    
-000117a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00011750: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
+00011760: 696f 6e27 3a20 352c 0a20 2020 2020 2020  ion': 5,.       
+00011770: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00011780: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00011790: 5f6e 616d 6520 3a20 7374 7269 6e67 0a20  _name : string. 
+000117a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
 000117b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000117c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000117d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000117e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-000117f0: 2020 2072 6574 7572 6e73 203a 2062 6f6f     returns : boo
-00011800: 6c0a 2020 2020 2020 2020 2020 2020 5375  l.            Su
-00011810: 6363 6573 7320 6f66 2050 4f53 5420 6f70  ccess of POST op
-00011820: 6572 6174 696f 6e2e 0a20 2020 2020 2020  eration..       
-00011830: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000117e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+000117f0: 2020 2020 2020 7265 7475 726e 7320 3a20        returns : 
+00011800: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
+00011810: 2053 7563 6365 7373 206f 6620 504f 5354   Success of POST
+00011820: 206f 7065 7261 7469 6f6e 2e0a 2020 2020   operation..    
+00011830: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 00011840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011870: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00011880: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-00011890: 6f74 2074 6162 6c65 5f6e 616d 652e 656e  ot table_name.en
-000118a0: 6473 7769 7468 2827 5f74 6573 7427 293a  dswith('_test'):
-000118b0: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-000118c0: 6c65 5f6e 616d 6520 2b3d 2027 5f74 6573  le_name += '_tes
-000118d0: 7427 0a0a 2020 2020 2020 2020 2320 736b  t'..        # sk
-000118e0: 6970 2074 6865 2050 4f53 5420 6f70 6572  ip the POST oper
-000118f0: 6174 696f 6e20 6966 2069 7420 7769 6c6c  ation if it will
-00011900: 2063 6572 7461 696e 6c79 2066 6169 6c0a   certainly fail.
-00011910: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011920: 5f62 6164 5f66 6965 6c64 7328 7461 626c  _bad_fields(tabl
-00011930: 652c 2074 6162 6c65 5f6e 616d 652c 206c  e, table_name, l
-00011940: 616d 6264 6120 663a 2066 203d 3d20 2769  ambda f: f == 'i
-00011950: 6427 293a 0a20 2020 2020 2020 2020 2020  d'):.           
-00011960: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00011970: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011980: 6c66 2e5f 706f 7374 5f67 656e 6572 6963  lf._post_generic
-00011990: 280a 2020 2020 2020 2020 2020 2020 7461  (.            ta
-000119a0: 626c 652c 2066 276d 6561 7375 7265 2f7b  ble, f'measure/{
-000119b0: 7265 6d6f 7665 7375 6666 6978 2874 6162  removesuffix(tab
-000119c0: 6c65 5f6e 616d 652c 2022 5f74 6573 7422  le_name, "_test"
-000119d0: 297d 270a 2020 2020 2020 2020 290a 0a20  )}'.        ).. 
-000119e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00011870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00011880: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00011890: 6620 6e6f 7420 7461 626c 655f 6e61 6d65  f not table_name
+000118a0: 2e65 6e64 7377 6974 6828 275f 7465 7374  .endswith('_test
+000118b0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+000118c0: 7461 626c 655f 6e61 6d65 202b 3d20 275f  table_name += '_
+000118d0: 7465 7374 270a 0a20 2020 2020 2020 2023  test'..        #
+000118e0: 2073 6b69 7020 7468 6520 504f 5354 206f   skip the POST o
+000118f0: 7065 7261 7469 6f6e 2069 6620 6974 2077  peration if it w
+00011900: 696c 6c20 6365 7274 6169 6e6c 7920 6661  ill certainly fa
+00011910: 696c 0a20 2020 2020 2020 2069 6620 7365  il.        if se
+00011920: 6c66 2e5f 6261 645f 6669 656c 6473 2874  lf._bad_fields(t
+00011930: 6162 6c65 2c20 7461 626c 655f 6e61 6d65  able, table_name
+00011940: 2c20 6c61 6d62 6461 2066 3a20 6620 3d3d  , lambda f: f ==
+00011950: 2027 6964 2729 3a0a 2020 2020 2020 2020   'id'):.        
+00011960: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00011970: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00011980: 2073 656c 662e 5f70 6f73 745f 6765 6e65   self._post_gene
+00011990: 7269 6328 0a20 2020 2020 2020 2020 2020  ric(.           
+000119a0: 2074 6162 6c65 2c20 6627 6d65 6173 7572   table, f'measur
+000119b0: 652f 7b72 656d 6f76 6573 7566 6669 7828  e/{removesuffix(
+000119c0: 7461 626c 655f 6e61 6d65 2c20 225f 7465  table_name, "_te
+000119d0: 7374 2229 7d27 0a20 2020 2020 2020 2029  st")}'.        )
+000119e0: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
 000119f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011a20: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
-00011a30: 2020 2320 7370 6563 6966 6963 2070 6879    # specific phy
-00011a40: 7369 6361 6c20 6974 656d 730a 2020 2020  sical items.    
-00011a50: 230a 2020 2020 2320 5468 6573 6520 6d65  #.    # These me
-00011a60: 7468 6f64 7320 6172 6520 7369 6d70 6c79  thods are simply
-00011a70: 2077 7261 7070 6572 7320 666f 7220 7468   wrappers for th
-00011a80: 6520 6765 6e65 7269 6320 706f 7374 5f69  e generic post_i
-00011a90: 7465 6d20 6361 6c6c 2e0a 2020 2020 230a  tem call..    #.
-00011aa0: 2020 2020 2320 5468 6579 2061 7265 206f      # They are o
-00011ab0: 6e6c 7920 6465 6669 6e65 6420 746f 2067  nly defined to g
-00011ac0: 6976 6520 616e 2069 6e74 6572 6163 7469  ive an interacti
-00011ad0: 7665 2075 7365 7220 6120 6368 616e 6365  ve user a chance
-00011ae0: 2074 6f20 6765 7420 7468 650a 2020 2020   to get the.    
-00011af0: 2320 6461 7461 6261 7365 2073 7562 6d69  # database submi
-00011b00: 7373 696f 6e20 7269 6768 7420 6279 2072  ssion right by r
-00011b10: 6566 6572 7269 6e67 2074 6f20 7468 6520  eferring to the 
-00011b20: 6d65 7468 6f64 2064 6f63 756d 656e 7461  method documenta
-00011b30: 7469 6f6e 0a20 2020 2023 2075 7369 6e67  tion.    # using
-00011b40: 2074 6865 2050 7974 686f 6e20 696e 7465   the Python inte
-00011b50: 7270 7265 7465 7227 7320 2768 656c 7028  rpreter's 'help(
-00011b60: 2927 2063 6f6d 6d61 6e64 2e0a 2020 2020  )' command..    
-00011b70: 230a 0a20 2020 2064 6566 2070 6f73 745f  #..    def post_
-00011b80: 7063 6228 7365 6c66 2c20 7461 626c 6529  pcb(self, table)
-00011b90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011ba0: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-00011bb0: 3a20 7063 620a 2020 2020 2020 2020 2222  : pcb.        ""
-00011bc0: 220a 2020 2020 2020 2020 2320 7265 7475  ".        # retu
-00011bd0: 726e 2073 656c 662e 706f 7374 5f69 7465  rn self.post_ite
-00011be0: 6d28 7461 626c 652c 2027 7063 6227 290a  m(table, 'pcb').
-00011bf0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00011c00: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00011c10: 720a 0a20 2020 2064 6566 2070 6f73 745f  r..    def post_
-00011c20: 7064 7528 7365 6c66 2c20 7461 626c 6529  pdu(self, table)
-00011c30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00011c40: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-00011c50: 3a20 7064 750a 2020 2020 2020 2020 2222  : pdu.        ""
-00011c60: 220a 2020 2020 2020 2020 2320 7265 7475  ".        # retu
-00011c70: 726e 2073 656c 662e 706f 7374 5f69 7465  rn self.post_ite
-00011c80: 6d28 7461 626c 652c 2027 7064 7527 290a  m(table, 'pdu').
-00011c90: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00011ca0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00011cb0: 720a 0a20 2020 2064 6566 2070 6f73 745f  r..    def post_
-00011cc0: 6d61 6e75 6661 6374 7572 6572 2873 656c  manufacturer(sel
-00011cd0: 662c 2074 6162 6c65 293a 0a20 2020 2020  f, table):.     
-00011ce0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-00011cf0: 4f53 5420 7461 626c 653a 206d 616e 7566  OST table: manuf
-00011d00: 6163 7475 7265 720a 0a20 2020 2020 2020  acturer..       
-00011d10: 2054 6865 2064 6174 6162 6173 6520 636f   The database co
-00011d20: 6e73 6973 7465 6e74 6c79 2072 6573 706f  nsistently respo
-00011d30: 6e64 7320 7769 7468 2022 6261 6420 7265  nds with "bad re
-00011d40: 7370 6f6e 7365 2220 746f 2074 6869 7320  sponse" to this 
-00011d50: 504f 5354 0a20 2020 2020 2020 206f 7065  POST.        ope
-00011d60: 7261 7469 6f6e 2066 6f72 2073 6f6d 6520  ration for some 
-00011d70: 7265 6173 6f6e 2e20 5468 6520 7369 6d69  reason. The simi
-00011d80: 6c61 7220 6375 726c 206f 7065 7261 7469  lar curl operati
-00011d90: 6f6e 206f 6e20 7468 6520 636f 6d6d 616e  on on the comman
-00011da0: 640a 2020 2020 2020 2020 6c69 6e65 2061  d.        line a
-00011db0: 6c73 6f20 6661 696c 732e 2054 6573 7465  lso fails. Teste
-00011dc0: 6420 3230 3232 2030 3920 3039 2e0a 2020  d 2022 09 09..  
-00011dd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011de0: 2020 2320 7265 7475 726e 2073 656c 662e    # return self.
-00011df0: 706f 7374 5f69 7465 6d28 7461 626c 652c  post_item(table,
-00011e00: 2027 6d61 6e75 6661 6374 7572 6572 2729   'manufacturer')
-00011e10: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-00011e20: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00011e30: 6f72 0a0a 2020 2020 6465 6620 706f 7374  or..    def post
-00011e40: 5f73 6970 6d28 7365 6c66 2c20 7461 626c  _sipm(self, tabl
-00011e50: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
-00011e60: 2020 2020 2020 2020 504f 5354 2074 6162          POST tab
-00011e70: 6c65 3a20 7369 706d 0a0a 2020 2020 2020  le: sipm..      
-00011e80: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00011a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00011a30: 0a20 2020 2023 2073 7065 6369 6669 6320  .    # specific 
+00011a40: 7068 7973 6963 616c 2069 7465 6d73 0a20  physical items. 
+00011a50: 2020 2023 0a20 2020 2023 2054 6865 7365     #.    # These
+00011a60: 206d 6574 686f 6473 2061 7265 2073 696d   methods are sim
+00011a70: 706c 7920 7772 6170 7065 7273 2066 6f72  ply wrappers for
+00011a80: 2074 6865 2067 656e 6572 6963 2070 6f73   the generic pos
+00011a90: 745f 6974 656d 2063 616c 6c2e 0a20 2020  t_item call..   
+00011aa0: 2023 0a20 2020 2023 2054 6865 7920 6172   #.    # They ar
+00011ab0: 6520 6f6e 6c79 2064 6566 696e 6564 2074  e only defined t
+00011ac0: 6f20 6769 7665 2061 6e20 696e 7465 7261  o give an intera
+00011ad0: 6374 6976 6520 7573 6572 2061 2063 6861  ctive user a cha
+00011ae0: 6e63 6520 746f 2067 6574 2074 6865 0a20  nce to get the. 
+00011af0: 2020 2023 2064 6174 6162 6173 6520 7375     # database su
+00011b00: 626d 6973 7369 6f6e 2072 6967 6874 2062  bmission right b
+00011b10: 7920 7265 6665 7272 696e 6720 746f 2074  y referring to t
+00011b20: 6865 206d 6574 686f 6420 646f 6375 6d65  he method docume
+00011b30: 6e74 6174 696f 6e0a 2020 2020 2320 7573  ntation.    # us
+00011b40: 696e 6720 7468 6520 5079 7468 6f6e 2069  ing the Python i
+00011b50: 6e74 6572 7072 6574 6572 2773 2027 6865  nterpreter's 'he
+00011b60: 6c70 2829 2720 636f 6d6d 616e 642e 0a20  lp()' command.. 
+00011b70: 2020 2023 0a0a 2020 2020 6465 6620 706f     #..    def po
+00011b80: 7374 5f70 6362 2873 656c 662c 2074 6162  st_pcb(self, tab
+00011b90: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+00011ba0: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+00011bb0: 626c 653a 2070 6362 0a20 2020 2020 2020  ble: pcb.       
+00011bc0: 2022 2222 0a20 2020 2020 2020 2023 2072   """.        # r
+00011bd0: 6574 7572 6e20 7365 6c66 2e70 6f73 745f  eturn self.post_
+00011be0: 6974 656d 2874 6162 6c65 2c20 2770 6362  item(table, 'pcb
+00011bf0: 2729 0a20 2020 2020 2020 2072 6169 7365  ').        raise
+00011c00: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00011c10: 7272 6f72 0a0a 2020 2020 6465 6620 706f  rror..    def po
+00011c20: 7374 5f70 6475 2873 656c 662c 2074 6162  st_pdu(self, tab
+00011c30: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+00011c40: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+00011c50: 626c 653a 2070 6475 0a20 2020 2020 2020  ble: pdu.       
+00011c60: 2022 2222 0a20 2020 2020 2020 2023 2072   """.        # r
+00011c70: 6574 7572 6e20 7365 6c66 2e70 6f73 745f  eturn self.post_
+00011c80: 6974 656d 2874 6162 6c65 2c20 2770 6475  item(table, 'pdu
+00011c90: 2729 0a20 2020 2020 2020 2072 6169 7365  ').        raise
+00011ca0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00011cb0: 7272 6f72 0a0a 2020 2020 6465 6620 706f  rror..    def po
+00011cc0: 7374 5f6d 616e 7566 6163 7475 7265 7228  st_manufacturer(
+00011cd0: 7365 6c66 2c20 7461 626c 6529 3a0a 2020  self, table):.  
+00011ce0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00011cf0: 2020 504f 5354 2074 6162 6c65 3a20 6d61    POST table: ma
+00011d00: 6e75 6661 6374 7572 6572 0a0a 2020 2020  nufacturer..    
+00011d10: 2020 2020 5468 6520 6461 7461 6261 7365      The database
+00011d20: 2063 6f6e 7369 7374 656e 746c 7920 7265   consistently re
+00011d30: 7370 6f6e 6473 2077 6974 6820 2262 6164  sponds with "bad
+00011d40: 2072 6573 706f 6e73 6522 2074 6f20 7468   response" to th
+00011d50: 6973 2050 4f53 540a 2020 2020 2020 2020  is POST.        
+00011d60: 6f70 6572 6174 696f 6e20 666f 7220 736f  operation for so
+00011d70: 6d65 2072 6561 736f 6e2e 2054 6865 2073  me reason. The s
+00011d80: 696d 696c 6172 2063 7572 6c20 6f70 6572  imilar curl oper
+00011d90: 6174 696f 6e20 6f6e 2074 6865 2063 6f6d  ation on the com
+00011da0: 6d61 6e64 0a20 2020 2020 2020 206c 696e  mand.        lin
+00011db0: 6520 616c 736f 2066 6169 6c73 2e20 5465  e also fails. Te
+00011dc0: 7374 6564 2032 3032 3220 3039 2030 392e  sted 2022 09 09.
+00011dd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011de0: 2020 2020 2023 2072 6574 7572 6e20 7365       # return se
+00011df0: 6c66 2e70 6f73 745f 6974 656d 2874 6162  lf.post_item(tab
+00011e00: 6c65 2c20 276d 616e 7566 6163 7475 7265  le, 'manufacture
+00011e10: 7227 290a 2020 2020 2020 2020 7261 6973  r').        rais
+00011e20: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00011e30: 4572 726f 720a 0a20 2020 2064 6566 2070  Error..    def p
+00011e40: 6f73 745f 7369 706d 2873 656c 662c 2074  ost_sipm(self, t
+00011e50: 6162 6c65 293a 0a20 2020 2020 2020 2022  able):.        "
+00011e60: 2222 0a20 2020 2020 2020 2050 4f53 5420  "".        POST 
+00011e70: 7461 626c 653a 2073 6970 6d0a 0a20 2020  table: sipm..   
+00011e80: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 00011e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00011eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011ec0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00011ed0: 2061 7267 730a 2020 2020 2020 2020 2020   args.          
-00011ee0: 2020 7461 626c 6520 3a20 6469 6374 0a20    table : dict. 
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011f00: 2e67 2e0a 2020 2020 2020 2020 2020 2020  .g..            
-00011f10: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00011ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00011ed0: 2020 2020 6172 6773 0a20 2020 2020 2020      args.       
+00011ee0: 2020 2020 2074 6162 6c65 203a 2064 6963       table : dic
+00011ef0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00011f00: 2020 652e 672e 0a20 2020 2020 2020 2020    e.g..         
+00011f10: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
 00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f30: 2020 2320 7468 6520 7761 6665 7220 7468    # the wafer th
-00011f40: 6973 2064 6576 6963 6520 7761 7320 7069  is device was pi
-00011f50: 636b 6564 2066 726f 6d0a 2020 2020 2020  cked from.      
+00011f30: 2020 2020 2023 2074 6865 2077 6166 6572       # the wafer
+00011f40: 2074 6869 7320 6465 7669 6365 2077 6173   this device was
+00011f50: 2070 6963 6b65 6420 6672 6f6d 0a20 2020   picked from.   
 00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f70: 2020 2777 6166 6572 5f69 6427 3a20 322c    'wafer_id': 2,
-00011f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f90: 2020 2020 2020 2020 2027 7369 706d 5f67           'sipm_g
-00011fa0: 7269 705f 7269 6e67 5f69 6427 3a20 312c  rip_ring_id': 1,
-00011fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011fc0: 2020 2020 2020 2020 2027 636f 6c75 6d6e           'column
-00011fd0: 2c20 3132 2c0a 2020 2020 2020 2020 2020  , 12,.          
-00011fe0: 2020 2020 2020 2020 2020 2020 2020 2772                'r
-00011ff0: 6f77 273a 2036 2c0a 2020 2020 2020 2020  ow': 6,.        
+00011f70: 2020 2020 2027 7761 6665 725f 6964 273a       'wafer_id':
+00011f80: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+00011f90: 2020 2020 2020 2020 2020 2020 2773 6970              'sip
+00011fa0: 6d5f 6772 6970 5f72 696e 675f 6964 273a  m_grip_ring_id':
+00011fb0: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+00011fc0: 2020 2020 2020 2020 2020 2020 2763 6f6c              'col
+00011fd0: 756d 6e2c 2031 322c 0a20 2020 2020 2020  umn, 12,.       
+00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ff0: 2027 726f 7727 3a20 362c 0a20 2020 2020   'row': 6,.     
 00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2774 696c 655f 7479 7065 273a 2027 5645  'tile_type': 'VE
-00012020: 544f 272c 0a20 2020 2020 2020 2020 2020  TO',.           
-00012030: 2020 2020 2020 2020 2020 2020 2023 2074               # t
-00012040: 6865 2074 696c 6520 7468 6973 2053 6950  he tile this SiP
-00012050: 4d20 6973 206d 6f75 6e74 6564 206f 6e2c  M is mounted on,
-00012060: 2069 6620 616e 790a 2020 2020 2020 2020   if any.        
+00012010: 2020 2027 7469 6c65 5f74 7970 6527 3a20     'tile_type': 
+00012020: 2756 4554 4f27 2c0a 2020 2020 2020 2020  'VETO',.        
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2320 7468 6520 7469 6c65 2074 6869 7320  # the tile this 
+00012050: 5369 504d 2069 7320 6d6f 756e 7465 6420  SiPM is mounted 
+00012060: 6f6e 2c20 6966 2061 6e79 0a20 2020 2020  on, if any.     
 00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2774 696c 655f 6964 3a20 3132 2c0a 2020  'tile_id: 12,.  
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 7d0a 2020 2020 2020 2020 2d2d 2d2d    }.        ----
+00012080: 2020 2027 7469 6c65 5f69 643a 2031 322c     'tile_id: 12,
+00012090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000120a0: 2020 2020 207d 0a20 2020 2020 2020 202d       }.        -
 000120b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000120c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000120d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000120e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000120f0: 2d2d 0a20 2020 2020 2020 2072 6574 7572  --.        retur
-00012100: 6e73 203a 2062 6f6f 6c0a 2020 2020 2020  ns : bool.      
-00012110: 2020 2020 2020 5375 6363 6573 7320 6f66        Success of
-00012120: 2050 4f53 5420 6f70 6572 6174 696f 6e2e   POST operation.
-00012130: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000120f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
+00012100: 7475 726e 7320 3a20 626f 6f6c 0a20 2020  turns : bool.   
+00012110: 2020 2020 2020 2020 2053 7563 6365 7373           Success
+00012120: 206f 6620 504f 5354 206f 7065 7261 7469   of POST operati
+00012130: 6f6e 2e0a 2020 2020 2020 2020 2d2d 2d2d  on..        ----
 00012140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00012180: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012190: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000121a0: 706f 7374 5f69 7465 6d28 7461 626c 652c  post_item(table,
-000121b0: 2027 7369 706d 2729 0a0a 2020 2020 6465   'sipm')..    de
-000121c0: 6620 706f 7374 5f73 6f6c 6465 7228 7365  f post_solder(se
-000121d0: 6c66 2c20 7461 626c 6529 3a0a 2020 2020  lf, table):.    
-000121e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000121f0: 504f 5354 2074 6162 6c65 3a20 736f 6c64  POST table: sold
-00012200: 6572 0a0a 2020 2020 2020 2020 4164 6420  er..        Add 
-00012210: 736f 6c64 6572 2070 6173 7465 2073 7972  solder paste syr
-00012220: 696e 6765 2074 6f20 7468 6520 6461 7461  inge to the data
-00012230: 6261 7365 2e0a 0a20 2020 2020 2020 2045  base...        E
-00012240: 7861 6d70 6c65 2073 7972 696e 6765 206c  xample syringe l
-00012250: 6162 656c 3a0a 0a20 2020 2020 2020 2049  abel:..        I
-00012260: 4e44 4955 4d20 434f 5250 4f52 4154 494f  NDIUM CORPORATIO
-00012270: 4e0a 0a20 2020 2020 2020 2049 504e 3a20  N..        IPN: 
-00012280: 5041 5354 4549 4e2d 3833 3735 322d 4330  PASTEIN-83752-C0
-00012290: 3031 2020 2020 2020 2020 454e 474c 4953  01        ENGLIS
-000122a0: 480a 2020 2020 2020 2020 464c 5558 3a20  H.        FLUX: 
-000122b0: 4e43 2d53 4d51 3830 2020 2020 2020 2020  NC-SMQ80        
-000122c0: 2020 2020 2020 2020 204d 4144 4520 494e           MADE IN
-000122d0: 2054 4845 2055 5341 0a20 2020 2020 2020   THE USA.       
-000122e0: 2043 4f4d 503a 2035 3249 4e20 3438 534e   COMP: 52IN 48SN
-000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012300: 494e 4441 4c4c 4f59 3a31 450a 2020 2020  INDALLOY:1E.    
-00012310: 2020 2020 4d45 5348 3a20 2d34 3030 2b36      MESH: -400+6
-00012320: 3335 2020 2020 2020 2020 2020 2020 2020  35              
-00012330: 2020 204c 4f54 3a20 5053 3131 3132 3037     LOT: PS111207
-00012340: 3334 0a20 2020 2020 2020 204d 4554 414c  34.        METAL
-00012350: 3a20 3833 2520 2020 2020 2020 2020 2020  : 83%           
-00012360: 2020 2020 2020 2020 2020 5155 414e 2028            QUAN (
-00012370: 476d 7329 3a20 3235 0a20 2020 2020 2020  Gms): 25.       
+00012170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012180: 2d2d 0a20 2020 2020 2020 2022 2222 0a20  --.        """. 
+00012190: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000121a0: 6c66 2e70 6f73 745f 6974 656d 2874 6162  lf.post_item(tab
+000121b0: 6c65 2c20 2773 6970 6d27 290a 0a20 2020  le, 'sipm')..   
+000121c0: 2064 6566 2070 6f73 745f 736f 6c64 6572   def post_solder
+000121d0: 2873 656c 662c 2074 6162 6c65 293a 0a20  (self, table):. 
+000121e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000121f0: 2020 2050 4f53 5420 7461 626c 653a 2073     POST table: s
+00012200: 6f6c 6465 720a 0a20 2020 2020 2020 2041  older..        A
+00012210: 6464 2073 6f6c 6465 7220 7061 7374 6520  dd solder paste 
+00012220: 7379 7269 6e67 6520 746f 2074 6865 2064  syringe to the d
+00012230: 6174 6162 6173 652e 0a0a 2020 2020 2020  atabase...      
+00012240: 2020 4578 616d 706c 6520 7379 7269 6e67    Example syring
+00012250: 6520 6c61 6265 6c3a 0a0a 2020 2020 2020  e label:..      
+00012260: 2020 494e 4449 554d 2043 4f52 504f 5241    INDIUM CORPORA
+00012270: 5449 4f4e 0a0a 2020 2020 2020 2020 4950  TION..        IP
+00012280: 4e3a 2050 4153 5445 494e 2d38 3337 3532  N: PASTEIN-83752
+00012290: 2d43 3030 3120 2020 2020 2020 2045 4e47  -C001        ENG
+000122a0: 4c49 5348 0a20 2020 2020 2020 2046 4c55  LISH.        FLU
+000122b0: 583a 204e 432d 534d 5138 3020 2020 2020  X: NC-SMQ80     
+000122c0: 2020 2020 2020 2020 2020 2020 4d41 4445              MADE
+000122d0: 2049 4e20 5448 4520 5553 410a 2020 2020   IN THE USA.    
+000122e0: 2020 2020 434f 4d50 3a20 3532 494e 2034      COMP: 52IN 4
+000122f0: 3853 4e20 2020 2020 2020 2020 2020 2020  8SN             
+00012300: 2020 2049 4e44 414c 4c4f 593a 3145 0a20     INDALLOY:1E. 
+00012310: 2020 2020 2020 204d 4553 483a 202d 3430         MESH: -40
+00012320: 302b 3633 3520 2020 2020 2020 2020 2020  0+635           
+00012330: 2020 2020 2020 4c4f 543a 2050 5331 3131        LOT: PS111
+00012340: 3230 3733 340a 2020 2020 2020 2020 4d45  20734.        ME
+00012350: 5441 4c3a 2038 3325 2020 2020 2020 2020  TAL: 83%        
+00012360: 2020 2020 2020 2020 2020 2020 2051 5541               QUA
+00012370: 4e20 2847 6d73 293a 2032 350a 2020 2020  N (Gms): 25.    
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123a0: 4d46 473a 2030 324a 756e 3230 3232 0a20  MFG: 02Jun2022. 
-000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 2020 204d 4647 3a20 3032 4a75 6e32 3032     MFG: 02Jun202
+000123b0: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
 000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123d0: 2020 2020 2020 5553 4520 4259 3a20 3032        USE BY: 02
-000123e0: 4465 6332 3032 320a 2020 2020 2020 2020  Dec2022.        
+000123d0: 2020 2020 2020 2020 2055 5345 2042 593a           USE BY:
+000123e0: 2030 3244 6563 3230 3232 0a20 2020 2020   02Dec2022.     
 000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012400: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00012410: 544f 5245 3a20 2d32 30c2 b043 2074 6f20  TORE: -20..C to 
-00012420: 35c2 b043 0a0a 2020 2020 2020 2020 2d2d  5..C..        --
-00012430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012410: 2020 5354 4f52 453a 202d 3230 c2b0 4320    STORE: -20..C 
+00012420: 746f 2035 c2b0 430a 0a20 2020 2020 2020  to 5..C..       
+00012430: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00012440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012470: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
-00012480: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
-00012490: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
-000124a0: 2020 2020 2020 2020 2020 2065 2e67 2e0a             e.g..
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 7b23 2041 6c6d 6f73 7420 6365      {# Almost ce
-000124d0: 7274 6169 6e6c 7920 496e 6469 756d 2043  rtainly Indium C
-000124e0: 6f72 702e 0a20 2020 2020 2020 2020 2020  orp..           
-000124f0: 2020 2020 2020 2020 2020 276d 616e 7566            'manuf
-00012500: 6163 7475 7265 7227 3a20 342c 0a20 2020  acturer': 4,.   
+00012470: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00012480: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
+00012490: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
+000124a0: 2020 2020 2020 2020 2020 2020 2020 652e                e.
+000124b0: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
+000124c0: 2020 2020 2020 207b 2320 416c 6d6f 7374         {# Almost
+000124d0: 2063 6572 7461 696e 6c79 2049 6e64 6975   certainly Indiu
+000124e0: 6d20 436f 7270 2e0a 2020 2020 2020 2020  m Corp..        
+000124f0: 2020 2020 2020 2020 2020 2020 2027 6d61               'ma
+00012500: 6e75 6661 6374 7572 6572 273a 2034 2c0a  nufacturer': 4,.
 00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 2020 2773 6f6c 6465 725f 7479 7065 273a    'solder_type':
-00012530: 2027 496e 6469 756d 2050 6173 7465 204e   'Indium Paste N
-00012540: 432d 534d 5138 3020 496e 6423 3145 2035  C-SMQ80 Ind#1E 5
-00012550: 3249 6e34 3853 6e2e 2e2e 272c 0a20 2020  2In48Sn...',.   
+00012520: 2020 2020 2027 736f 6c64 6572 5f74 7970       'solder_typ
+00012530: 6527 3a20 2749 6e64 6975 6d20 5061 7374  e': 'Indium Past
+00012540: 6520 4e43 2d53 4d51 3830 2049 6e64 2331  e NC-SMQ80 Ind#1
+00012550: 4520 3532 496e 3438 536e 2e2e 2e27 2c0a  E 52In48Sn...',.
 00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2320 4672 6f6d 2074 6865 2073 7972    # From the syr
-00012580: 696e 6765 206c 6162 656c 2028 224d 4647  inge label ("MFG
-00012590: 2229 2e0a 2020 2020 2020 2020 2020 2020  ")..            
-000125a0: 2020 2020 2020 2020 2027 7072 6f64 7563           'produc
-000125b0: 7469 6f6e 5f64 6174 6527 3a20 2732 3032  tion_date': '202
-000125c0: 322d 3036 2d30 3220 3030 3a30 303a 3030  2-06-02 00:00:00
-000125d0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000125e0: 2020 2020 2020 2020 2320 5468 6520 6461          # The da
-000125f0: 7465 2074 6865 2073 7972 696e 6765 2077  te the syringe w
-00012600: 6173 2074 616b 656e 2066 726f 6d20 636f  as taken from co
-00012610: 6c64 2073 746f 7261 6765 2061 6e64 0a20  ld storage and. 
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 2020 2320 6272 6f75 6768 7420 7570      # brought up
-00012640: 2074 6f20 726f 6f6d 2074 656d 7065 7261   to room tempera
-00012650: 7475 7265 2e0a 2020 2020 2020 2020 2020  ture..          
-00012660: 2020 2020 2020 2020 2020 2027 726f 6f6d             'room
-00012670: 5f74 656d 7065 7261 7475 7265 5f64 6174  _temperature_dat
-00012680: 6527 3a20 2732 3032 322d 3037 2d31 3820  e': '2022-07-18 
-00012690: 3136 3a30 303a 3030 272c 0a20 2020 2020  16:00:00',.     
+00012570: 2020 2020 2023 2046 726f 6d20 7468 6520       # From the 
+00012580: 7379 7269 6e67 6520 6c61 6265 6c20 2822  syringe label ("
+00012590: 4d46 4722 292e 0a20 2020 2020 2020 2020  MFG")..         
+000125a0: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
+000125b0: 6475 6374 696f 6e5f 6461 7465 273a 2027  duction_date': '
+000125c0: 3230 3232 2d30 362d 3032 2030 303a 3030  2022-06-02 00:00
+000125d0: 3a30 3027 2c0a 2020 2020 2020 2020 2020  :00',.          
+000125e0: 2020 2020 2020 2020 2020 2023 2054 6865             # The
+000125f0: 2064 6174 6520 7468 6520 7379 7269 6e67   date the syring
+00012600: 6520 7761 7320 7461 6b65 6e20 6672 6f6d  e was taken from
+00012610: 2063 6f6c 6420 7374 6f72 6167 6520 616e   cold storage an
+00012620: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00012630: 2020 2020 2020 2023 2062 726f 7567 6874         # brought
+00012640: 2075 7020 746f 2072 6f6f 6d20 7465 6d70   up to room temp
+00012650: 6572 6174 7572 652e 0a20 2020 2020 2020  erature..       
+00012660: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00012670: 6f6f 6d5f 7465 6d70 6572 6174 7572 655f  oom_temperature_
+00012680: 6461 7465 273a 2027 3230 3232 2d30 372d  date': '2022-07-
+00012690: 3138 2031 363a 3030 3a30 3027 2c0a 2020  18 16:00:00',.  
 000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126b0: 2320 4672 6f6d 2074 6865 2073 7972 696e  # From the syrin
-000126c0: 6765 206c 6162 656c 2028 2255 5345 2042  ge label ("USE B
-000126d0: 5922 292e 0a20 2020 2020 2020 2020 2020  Y")..           
-000126e0: 2020 2020 2020 2020 2020 2765 7870 6972            'expir
-000126f0: 795f 6461 7465 273a 2027 3230 3232 2d31  y_date': '2022-1
-00012700: 322d 3032 2030 303a 3030 3a30 3027 2c0a  2-02 00:00:00',.
-00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012720: 2020 2020 2023 2054 6865 2073 6974 6527       # The site'
-00012730: 7320 696e 7465 726e 616c 2072 6566 6572  s internal refer
-00012740: 656e 6365 206e 756d 6265 7220 666f 7220  ence number for 
-00012750: 7468 6520 7379 7269 6e67 650a 2020 2020  the syringe.    
+000126b0: 2020 2023 2046 726f 6d20 7468 6520 7379     # From the sy
+000126c0: 7269 6e67 6520 6c61 6265 6c20 2822 5553  ringe label ("US
+000126d0: 4520 4259 2229 2e0a 2020 2020 2020 2020  E BY")..        
+000126e0: 2020 2020 2020 2020 2020 2020 2027 6578               'ex
+000126f0: 7069 7279 5f64 6174 6527 3a20 2732 3032  piry_date': '202
+00012700: 322d 3132 2d30 3220 3030 3a30 303a 3030  2-12-02 00:00:00
+00012710: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00012720: 2020 2020 2020 2020 2320 5468 6520 7369          # The si
+00012730: 7465 2773 2069 6e74 6572 6e61 6c20 7265  te's internal re
+00012740: 6665 7265 6e63 6520 6e75 6d62 6572 2066  ference number f
+00012750: 6f72 2074 6865 2073 7972 696e 6765 0a20  or the syringe. 
 00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2027 7379 7269 6e67 655f 6964 273a 2037   'syringe_id': 7
-00012780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012790: 2020 2020 2020 2023 2046 726f 6d20 7468         # From th
-000127a0: 6520 7379 7269 6e67 6520 6c61 6265 6c20  e syringe label 
-000127b0: 2822 4c4f 5422 292e 0a20 2020 2020 2020  ("LOT")..       
-000127c0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-000127d0: 6f74 273a 2027 5053 3131 3132 3037 3334  ot': 'PS11120734
-000127e0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000127f0: 2020 2020 2020 2020 2320 4d61 7373 206f          # Mass o
-00012800: 6620 736f 6c64 6572 2070 6173 7465 2063  f solder paste c
-00012810: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
-00012820: 7379 7269 6e67 6520 2867 7261 6d73 290a  syringe (grams).
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2020 2020 2027 6d61 7373 273a 2032 357d       'mass': 25}
-00012850: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00012770: 2020 2020 2773 7972 696e 6765 5f69 6427      'syringe_id'
+00012780: 3a20 372c 0a20 2020 2020 2020 2020 2020  : 7,.           
+00012790: 2020 2020 2020 2020 2020 2320 4672 6f6d            # From
+000127a0: 2074 6865 2073 7972 696e 6765 206c 6162   the syringe lab
+000127b0: 656c 2028 224c 4f54 2229 2e0a 2020 2020  el ("LOT")..    
+000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127d0: 2027 6c6f 7427 3a20 2750 5331 3131 3230   'lot': 'PS11120
+000127e0: 3733 3427 2c0a 2020 2020 2020 2020 2020  734',.          
+000127f0: 2020 2020 2020 2020 2020 2023 204d 6173             # Mas
+00012800: 7320 6f66 2073 6f6c 6465 7220 7061 7374  s of solder past
+00012810: 6520 636f 6e74 6169 6e65 6420 696e 2074  e contained in t
+00012820: 6865 2073 7972 696e 6765 2028 6772 616d  he syringe (gram
+00012830: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00012840: 2020 2020 2020 2020 276d 6173 7327 3a20          'mass': 
+00012850: 3235 7d0a 2020 2020 2020 2020 2d2d 2d2d  25}.        ----
 00012860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-000128a0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-000128b0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
-000128c0: 2020 2053 7563 6365 7373 206f 6620 504f     Success of PO
-000128d0: 5354 206f 7065 7261 7469 6f6e 2e0a 2020  ST operation..  
-000128e0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00012890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000128a0: 2d2d 0a20 2020 2020 2020 2072 6574 7572  --.        retur
+000128b0: 6e73 203a 2062 6f6f 6c0a 2020 2020 2020  ns : bool.      
+000128c0: 2020 2020 2020 5375 6363 6573 7320 6f66        Success of
+000128d0: 2050 4f53 5420 6f70 6572 6174 696f 6e2e   POST operation.
+000128e0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
 000128f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00012930: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012940: 2072 6574 7572 6e20 7365 6c66 2e70 6f73   return self.pos
-00012950: 745f 6974 656d 2874 6162 6c65 2c20 2773  t_item(table, 's
-00012960: 6f6c 6465 7227 290a 0a20 2020 2064 6566  older')..    def
-00012970: 2070 6f73 745f 7469 6c65 2873 656c 662c   post_tile(self,
-00012980: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
-00012990: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
-000129a0: 5420 7461 626c 653a 2074 696c 650a 2020  T table: tile.  
-000129b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000129c0: 2020 2320 7265 7475 726e 2073 656c 662e    # return self.
-000129d0: 706f 7374 5f69 7465 6d28 7461 626c 652c  post_item(table,
-000129e0: 2027 7469 6c65 2729 0a20 2020 2020 2020   'tile').       
-000129f0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-00012a00: 656e 7465 6445 7272 6f72 0a0a 2020 2020  entedError..    
-00012a10: 6465 6620 706f 7374 5f76 6173 6963 2873  def post_vasic(s
-00012a20: 656c 662c 2074 6162 6c65 293a 0a20 2020  elf, table):.   
-00012a30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012a40: 2050 4f53 5420 7461 626c 653a 2076 6173   POST table: vas
-00012a50: 6963 0a0a 2020 2020 2020 2020 5468 6973  ic..        This
-00012a60: 2069 7320 666f 7220 6120 5665 746f 2041   is for a Veto A
-00012a70: 5349 432e 0a0a 2020 2020 2020 2020 2d2d  SIC...        --
-00012a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00012930: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012940: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00012950: 706f 7374 5f69 7465 6d28 7461 626c 652c  post_item(table,
+00012960: 2027 736f 6c64 6572 2729 0a0a 2020 2020   'solder')..    
+00012970: 6465 6620 706f 7374 5f74 696c 6528 7365  def post_tile(se
+00012980: 6c66 2c20 7461 626c 6529 3a0a 2020 2020  lf, table):.    
+00012990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000129a0: 504f 5354 2074 6162 6c65 3a20 7469 6c65  POST table: tile
+000129b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000129c0: 2020 2020 2023 2072 6574 7572 6e20 7365       # return se
+000129d0: 6c66 2e70 6f73 745f 6974 656d 2874 6162  lf.post_item(tab
+000129e0: 6c65 2c20 2774 696c 6527 290a 2020 2020  le, 'tile').    
+000129f0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00012a00: 6c65 6d65 6e74 6564 4572 726f 720a 0a20  lementedError.. 
+00012a10: 2020 2064 6566 2070 6f73 745f 7661 7369     def post_vasi
+00012a20: 6328 7365 6c66 2c20 7461 626c 6529 3a0a  c(self, table):.
+00012a30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012a40: 2020 2020 504f 5354 2074 6162 6c65 3a20      POST table: 
+00012a50: 7661 7369 630a 0a20 2020 2020 2020 2054  vasic..        T
+00012a60: 6869 7320 6973 2066 6f72 2061 2056 6574  his is for a Vet
+00012a70: 6f20 4153 4943 2e0a 0a20 2020 2020 2020  o ASIC...       
+00012a80: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00012a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012ac0: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
-00012ad0: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
-00012ae0: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
-00012af0: 2020 2020 2020 2020 2020 2065 2e67 2e0a             e.g..
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00012b20: 2020 2020 2020 2020 2020 2020 2020 2776                'v
-00012b30: 6173 6963 5f67 7269 705f 7269 6e67 5f69  asic_grip_ring_i
-00012b40: 643a 2031 2c0a 2020 2020 2020 2020 2020  d: 1,.          
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2776                'v
-00012b60: 6173 6963 5f77 6166 6572 5f69 6427 3a20  asic_wafer_id': 
-00012b70: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00012b80: 2020 2020 2020 2020 2020 2027 636f 6c75             'colu
-00012b90: 6d6e 273a 2036 2c0a 2020 2020 2020 2020  mn': 6,.        
+00012ac0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00012ad0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
+00012ae0: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
+00012af0: 2020 2020 2020 2020 2020 2020 2020 652e                e.
+00012b00: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
+00012b10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b30: 2027 7661 7369 635f 6772 6970 5f72 696e   'vasic_grip_rin
+00012b40: 675f 6964 3a20 312c 0a20 2020 2020 2020  g_id: 1,.       
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 2027 7661 7369 635f 7761 6665 725f 6964   'vasic_wafer_id
+00012b70: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00012b90: 6f6c 756d 6e27 3a20 362c 0a20 2020 2020  olumn': 6,.     
 00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2772 6f77 273a 2035 2c0a 2020 2020 2020  'row': 5,.      
+00012bb0: 2020 2027 726f 7727 3a20 352c 0a20 2020     'row': 5,.   
 00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 2020 2776 7063 625f 6173 6963 5f69 6427    'vpcb_asic_id'
-00012be0: 3a20 352c 0a20 2020 2020 2020 2020 2020  : 5,.           
-00012bf0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00012c00: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00012bd0: 2020 2020 2027 7670 6362 5f61 7369 635f       'vpcb_asic_
+00012be0: 6964 273a 2035 2c0a 2020 2020 2020 2020  id': 5,.        
+00012bf0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00012c00: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 00012c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012c40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00012c50: 2020 7265 7475 726e 7320 3a20 626f 6f6c    returns : bool
-00012c60: 0a20 2020 2020 2020 2020 2020 2053 7563  .            Suc
-00012c70: 6365 7373 206f 6620 504f 5354 206f 7065  cess of POST ope
-00012c80: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00012c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00012c50: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
+00012c60: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+00012c70: 5375 6363 6573 7320 6f66 2050 4f53 5420  Success of POST 
+00012c80: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
+00012c90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 00012ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012cd0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2022  ------.        "
-00012ce0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00012cf0: 6e20 7365 6c66 2e70 6f73 745f 6974 656d  n self.post_item
-00012d00: 2874 6162 6c65 2c20 2776 6173 6963 2729  (table, 'vasic')
-00012d10: 0a0a 2020 2020 6465 6620 706f 7374 5f76  ..    def post_v
-00012d20: 6173 6963 5f67 7269 705f 7269 6e67 2873  asic_grip_ring(s
-00012d30: 656c 662c 2074 6162 6c65 293a 0a20 2020  elf, table):.   
-00012d40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012d50: 2050 4f53 5420 7461 626c 653a 2076 6173   POST table: vas
-00012d60: 6963 5f67 7269 705f 7269 6e67 0a0a 2020  ic_grip_ring..  
-00012d70: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00012cd0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00012ce0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00012cf0: 7475 726e 2073 656c 662e 706f 7374 5f69  turn self.post_i
+00012d00: 7465 6d28 7461 626c 652c 2027 7661 7369  tem(table, 'vasi
+00012d10: 6327 290a 0a20 2020 2064 6566 2070 6f73  c')..    def pos
+00012d20: 745f 7661 7369 635f 6772 6970 5f72 696e  t_vasic_grip_rin
+00012d30: 6728 7365 6c66 2c20 7461 626c 6529 3a0a  g(self, table):.
+00012d40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00012d50: 2020 2020 504f 5354 2074 6162 6c65 3a20      POST table: 
+00012d60: 7661 7369 635f 6772 6970 5f72 696e 670a  vasic_grip_ring.
+00012d70: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
 00012d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00012dc0: 2020 2020 2061 7267 730a 2020 2020 2020       args.      
-00012dd0: 2020 2020 2020 7461 626c 6520 3a20 6469        table : di
-00012de0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
-00012df0: 2020 2065 2e67 2e20 7b27 7365 7269 616c     e.g. {'serial
-00012e00: 3a20 2731 3233 3427 7d0a 2020 2020 2020  : '1234'}.      
-00012e10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00012db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00012dc0: 2020 2020 2020 2020 6172 6773 0a20 2020          args.   
+00012dd0: 2020 2020 2020 2020 2074 6162 6c65 203a           table :
+00012de0: 2064 6963 740a 2020 2020 2020 2020 2020   dict.          
+00012df0: 2020 2020 2020 652e 672e 207b 2773 6572        e.g. {'ser
+00012e00: 6961 6c3a 2027 3132 3334 277d 0a20 2020  ial: '1234'}.   
+00012e10: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 00012e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e50: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00012e60: 2072 6574 7572 6e73 203a 2062 6f6f 6c0a   returns : bool.
-00012e70: 2020 2020 2020 2020 2020 2020 5375 6363              Succ
-00012e80: 6573 7320 6f66 2050 4f53 5420 6f70 6572  ess of POST oper
-00012e90: 6174 696f 6e2e 0a20 2020 2020 2020 202d  ation..        -
-00012ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00012e60: 2020 2020 7265 7475 726e 7320 3a20 626f      returns : bo
+00012e70: 6f6c 0a20 2020 2020 2020 2020 2020 2053  ol.            S
+00012e80: 7563 6365 7373 206f 6620 504f 5354 206f  uccess of POST o
+00012e90: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
+00012ea0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
 00012eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012ee0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
-00012ef0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00012f00: 2073 656c 662e 706f 7374 5f69 7465 6d28   self.post_item(
-00012f10: 7461 626c 652c 2027 7661 7369 635f 6772  table, 'vasic_gr
-00012f20: 6970 5f72 696e 6727 290a 0a20 2020 2064  ip_ring')..    d
-00012f30: 6566 2070 6f73 745f 7661 7369 635f 7761  ef post_vasic_wa
-00012f40: 6665 7228 7365 6c66 2c20 7461 626c 6529  fer(self, table)
-00012f50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012f60: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-00012f70: 3a20 7661 7369 635f 7761 6665 720a 0a20  : vasic_wafer.. 
-00012f80: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00012ee0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00012ef0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00012f00: 7572 6e20 7365 6c66 2e70 6f73 745f 6974  urn self.post_it
+00012f10: 656d 2874 6162 6c65 2c20 2776 6173 6963  em(table, 'vasic
+00012f20: 5f67 7269 705f 7269 6e67 2729 0a0a 2020  _grip_ring')..  
+00012f30: 2020 6465 6620 706f 7374 5f76 6173 6963    def post_vasic
+00012f40: 5f77 6166 6572 2873 656c 662c 2074 6162  _wafer(self, tab
+00012f50: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+00012f60: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+00012f70: 626c 653a 2076 6173 6963 5f77 6166 6572  ble: vasic_wafer
+00012f80: 0a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
 00012f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00012fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00012fd0: 2020 2020 2020 6172 6773 0a20 2020 2020        args.     
-00012fe0: 2020 2020 2020 2074 6162 6c65 203a 2064         table : d
-00012ff0: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
-00013000: 2020 2020 652e 672e 0a20 2020 2020 2020      e.g..       
-00013010: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00013020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013030: 2020 2020 2020 2027 7072 6f64 7563 7469         'producti
-00013040: 6f6e 5f64 6174 6527 3a20 2732 3032 322d  on_date': '2022-
-00013050: 3039 2d30 3620 3135 3a33 303a 3134 272c  09-06 15:30:14',
-00013060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013070: 2020 2020 2020 2020 2027 6d61 6e75 6661           'manufa
-00013080: 6374 7572 6572 273a 2032 2c0a 2020 2020  cturer': 2,.    
+00012fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012fd0: 0a20 2020 2020 2020 2061 7267 730a 2020  .        args.  
+00012fe0: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00012ff0: 3a20 6469 6374 0a20 2020 2020 2020 2020  : dict.         
+00013000: 2020 2020 2020 2065 2e67 2e0a 2020 2020         e.g..    
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00013030: 2020 2020 2020 2020 2020 2770 726f 6475            'produ
+00013040: 6374 696f 6e5f 6461 7465 273a 2027 3230  ction_date': '20
+00013050: 3232 2d30 392d 3036 2031 353a 3330 3a31  22-09-06 15:30:1
+00013060: 3427 2c0a 2020 2020 2020 2020 2020 2020  4',.            
+00013070: 2020 2020 2020 2020 2020 2020 276d 616e              'man
+00013080: 7566 6163 7475 7265 7227 3a20 322c 0a20  ufacturer': 2,. 
 00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130a0: 2020 2020 2772 756e 5f6e 756d 6265 7227      'run_number'
-000130b0: 2c20 3132 332c 0a20 2020 2020 2020 2020  , 123,.         
-000130c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000130d0: 7365 7269 616c 273a 2027 3132 3327 2c0a  serial': '123',.
-000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 2020 2020 7d0a 2020 2020 2020 2020 2d2d      }.        --
-00013100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000130a0: 2020 2020 2020 2027 7275 6e5f 6e75 6d62         'run_numb
+000130b0: 6572 272c 2031 3233 2c0a 2020 2020 2020  er', 123,.      
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2773 6572 6961 6c27 3a20 2731 3233    'serial': '123
+000130e0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000130f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00013100: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00013110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013140: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
-00013150: 7572 6e73 203a 2062 6f6f 6c0a 2020 2020  urns : bool.    
-00013160: 2020 2020 2020 2020 5375 6363 6573 7320          Success 
-00013170: 6f66 2050 4f53 5420 6f70 6572 6174 696f  of POST operatio
-00013180: 6e2e 0a20 2020 2020 2020 202d 2d2d 2d2d  n..        -----
+00013140: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00013150: 7265 7475 726e 7320 3a20 626f 6f6c 0a20  returns : bool. 
+00013160: 2020 2020 2020 2020 2020 2053 7563 6365             Succe
+00013170: 7373 206f 6620 504f 5354 206f 7065 7261  ss of POST opera
+00013180: 7469 6f6e 2e0a 2020 2020 2020 2020 2d2d  tion..        --
 00013190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000131a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000131b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000131c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000131d0: 2d0a 2020 2020 2020 2020 2222 220a 2020  -.        """.  
-000131e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000131f0: 662e 706f 7374 5f69 7465 6d28 7461 626c  f.post_item(tabl
-00013200: 652c 2027 7661 7369 635f 7761 6665 7227  e, 'vasic_wafer'
-00013210: 290a 0a20 2020 2064 6566 2070 6f73 745f  )..    def post_
-00013220: 7663 6162 6c65 2873 656c 662c 2074 6162  vcable(self, tab
-00013230: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
-00013240: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
-00013250: 626c 653a 2076 6361 626c 650a 0a20 2020  ble: vcable..   
-00013260: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+000131d0: 2d2d 2d2d 0a20 2020 2020 2020 2022 2222  ----.        """
+000131e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000131f0: 7365 6c66 2e70 6f73 745f 6974 656d 2874  self.post_item(t
+00013200: 6162 6c65 2c20 2776 6173 6963 5f77 6166  able, 'vasic_waf
+00013210: 6572 2729 0a0a 2020 2020 6465 6620 706f  er')..    def po
+00013220: 7374 5f76 6361 626c 6528 7365 6c66 2c20  st_vcable(self, 
+00013230: 7461 626c 6529 3a0a 2020 2020 2020 2020  table):.        
+00013240: 2222 220a 2020 2020 2020 2020 504f 5354  """.        POST
+00013250: 2074 6162 6c65 3a20 7663 6162 6c65 0a0a   table: vcable..
+00013260: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
 00013270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000132a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000132b0: 2020 2020 6172 6773 0a20 2020 2020 2020      args.       
-000132c0: 2020 2020 2074 6162 6c65 203a 2064 6963       table : dic
-000132d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000132e0: 2020 652e 672e 0a20 2020 2020 2020 2020    e.g..         
-000132f0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+000132a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000132b0: 2020 2020 2020 2061 7267 730a 2020 2020         args.    
+000132c0: 2020 2020 2020 2020 7461 626c 6520 3a20          table : 
+000132d0: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+000132e0: 2020 2020 2065 2e67 2e0a 2020 2020 2020       e.g..      
+000132f0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
 00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2027 7072 6f64 7563 7469 6f6e       'production
-00013320: 5f64 6174 6527 3a20 2732 3032 322d 3039  _date': '2022-09
-00013330: 2d30 3620 3135 3a33 303a 3134 272c 0a20  -06 15:30:14',. 
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2027 6d61 6e75 6661 6374         'manufact
-00013360: 7572 6572 273a 2036 2c0a 2020 2020 2020  urer': 6,.      
+00013310: 2020 2020 2020 2020 2770 726f 6475 6374          'product
+00013320: 696f 6e5f 6461 7465 273a 2027 3230 3232  ion_date': '2022
+00013330: 2d30 392d 3036 2031 353a 3330 3a31 3427  -09-06 15:30:14'
+00013340: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013350: 2020 2020 2020 2020 2020 276d 616e 7566            'manuf
+00013360: 6163 7475 7265 7227 3a20 362c 0a20 2020  acturer': 6,.   
 00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013380: 2020 2772 756e 5f6e 756d 6265 7227 2c20    'run_number', 
-00013390: 3132 332c 0a20 2020 2020 2020 2020 2020  123,.           
-000133a0: 2020 2020 2020 2020 2020 2020 2027 7365               'se
-000133b0: 7269 616c 273a 2027 3132 3327 2c0a 2020  rial': '123',.  
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133d0: 2020 2020 2020 2774 7970 6527 3a20 2731        'type': '1
-000133e0: 3233 3427 2c0a 2020 2020 2020 2020 2020  234',.          
-000133f0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-00013400: 656e 6774 6827 3a20 312e 362c 0a20 2020  ength': 1.6,.   
+00013380: 2020 2020 2027 7275 6e5f 6e75 6d62 6572       'run_number
+00013390: 272c 2031 3233 2c0a 2020 2020 2020 2020  ', 123,.        
+000133a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133b0: 2773 6572 6961 6c27 3a20 2731 3233 272c  'serial': '123',
+000133c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000133d0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+000133e0: 2027 3132 3334 272c 0a20 2020 2020 2020   '1234',.       
+000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013400: 2027 6c65 6e67 7468 273a 2031 2e36 2c0a   'length': 1.6,.
 00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013420: 207d 0a20 2020 2020 2020 202d 2d2d 2d2d   }.        -----
+00013420: 2020 2020 7d0a 2020 2020 2020 2020 2d2d      }.        --
 00013430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013470: 2d0a 2020 2020 2020 2020 7265 7475 726e  -.        return
-00013480: 7320 3a20 626f 6f6c 0a20 2020 2020 2020  s : bool.       
-00013490: 2020 2020 2053 7563 6365 7373 206f 6620       Success of 
-000134a0: 504f 5354 206f 7065 7261 7469 6f6e 2e0a  POST operation..
-000134b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00013470: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
+00013480: 7572 6e73 203a 2062 6f6f 6c0a 2020 2020  urns : bool.    
+00013490: 2020 2020 2020 2020 5375 6363 6573 7320          Success 
+000134a0: 6f66 2050 4f53 5420 6f70 6572 6174 696f  of POST operatio
+000134b0: 6e2e 0a20 2020 2020 2020 202d 2d2d 2d2d  n..        -----
 000134c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000134d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000134e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000134f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00013500: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013510: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-00013520: 6f73 745f 6974 656d 2874 6162 6c65 2c20  ost_item(table, 
-00013530: 2776 6361 626c 6527 290a 0a20 2020 2064  'vcable')..    d
-00013540: 6566 2070 6f73 745f 766d 6f74 6865 7262  ef post_vmotherb
-00013550: 6f61 7264 2873 656c 662c 2074 6162 6c65  oard(self, table
-00013560: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00013570: 2020 2020 2020 2050 4f53 5420 7461 626c         POST tabl
-00013580: 653a 2076 6d6f 7468 6572 626f 6172 640a  e: vmotherboard.
-00013590: 0a20 2020 2020 2020 2054 6869 7320 6973  .        This is
-000135a0: 2066 6f72 2061 2056 6574 6f20 6d6f 7468   for a Veto moth
-000135b0: 6572 626f 6172 6420 7769 7468 2061 2076  erboard with a v
-000135c0: 7064 7520 696e 7374 616c 6c65 642e 0a0a  pdu installed...
-000135d0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000134f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013500: 2d0a 2020 2020 2020 2020 2222 220a 2020  -.        """.  
+00013510: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00013520: 662e 706f 7374 5f69 7465 6d28 7461 626c  f.post_item(tabl
+00013530: 652c 2027 7663 6162 6c65 2729 0a0a 2020  e, 'vcable')..  
+00013540: 2020 6465 6620 706f 7374 5f76 6d6f 7468    def post_vmoth
+00013550: 6572 626f 6172 6428 7365 6c66 2c20 7461  erboard(self, ta
+00013560: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
+00013570: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
+00013580: 6162 6c65 3a20 766d 6f74 6865 7262 6f61  able: vmotherboa
+00013590: 7264 0a0a 2020 2020 2020 2020 5468 6973  rd..        This
+000135a0: 2069 7320 666f 7220 6120 5665 746f 206d   is for a Veto m
+000135b0: 6f74 6865 7262 6f61 7264 2077 6974 6820  otherboard with 
+000135c0: 6120 7670 6475 2069 6e73 7461 6c6c 6564  a vpdu installed
+000135d0: 2e0a 0a20 2020 2020 2020 202d 2d2d 2d2d  ...        -----
 000135e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000135f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00013620: 2020 2020 2020 2061 7267 730a 2020 2020         args.    
-00013630: 2020 2020 2020 2020 7461 626c 6520 3a20          table : 
-00013640: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
-00013650: 2020 2020 2065 2e67 2e0a 2020 2020 2020       e.g..      
-00013660: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013680: 2020 2020 2020 2020 2770 726f 6475 6374          'product
-00013690: 696f 6e5f 6461 7465 273a 2027 3230 3232  ion_date': '2022
-000136a0: 2d30 392d 3036 2031 353a 3330 3a31 3427  -09-06 15:30:14'
-000136b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000136c0: 2020 2020 2020 2020 2020 276d 616e 7566            'manuf
-000136d0: 6163 7475 7265 7227 3a20 362c 0a20 2020  acturer': 6,.   
+00013610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013620: 2d0a 2020 2020 2020 2020 6172 6773 0a20  -.        args. 
+00013630: 2020 2020 2020 2020 2020 2074 6162 6c65             table
+00013640: 203a 2064 6963 740a 2020 2020 2020 2020   : dict.        
+00013650: 2020 2020 2020 2020 652e 672e 0a20 2020          e.g..   
+00013660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013670: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00013680: 2020 2020 2020 2020 2020 2027 7072 6f64             'prod
+00013690: 7563 7469 6f6e 5f64 6174 6527 3a20 2732  uction_date': '2
+000136a0: 3032 322d 3039 2d30 3620 3135 3a33 303a  022-09-06 15:30:
+000136b0: 3134 272c 0a20 2020 2020 2020 2020 2020  14',.           
+000136c0: 2020 2020 2020 2020 2020 2020 2027 6d61               'ma
+000136d0: 6e75 6661 6374 7572 6572 273a 2036 2c0a  nufacturer': 6,.
 000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136f0: 2020 2020 2027 7275 6e5f 6e75 6d62 6572       'run_number
-00013700: 272c 2031 3233 2c0a 2020 2020 2020 2020  ', 123,.        
+000136f0: 2020 2020 2020 2020 2772 756e 5f6e 756d          'run_num
+00013700: 6265 7227 2c20 3132 332c 0a20 2020 2020  ber', 123,.     
 00013710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013720: 2771 7263 6f64 6527 3a20 2732 3230 3630  'qrcode': '22060
-00013730: 3130 3131 3132 3334 3531 3233 272c 0a20  101112345123',. 
-00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 2020 2020 2020 2027 7670 6475 5f69 6427         'vpdu_id'
-00013760: 3a20 362c 0a20 2020 2020 2020 2020 2020  : 6,.           
-00013770: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00013780: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00013720: 2020 2027 7172 636f 6465 273a 2027 3232     'qrcode': '22
+00013730: 3036 3031 3031 3131 3233 3435 3132 3327  060101112345123'
+00013740: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013750: 2020 2020 2020 2020 2020 2776 7064 755f            'vpdu_
+00013760: 6964 273a 2036 2c0a 2020 2020 2020 2020  id': 6,.        
+00013770: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00013780: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 00013790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000137a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000137b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000137c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000137d0: 2020 7265 7475 726e 7320 3a20 626f 6f6c    returns : bool
-000137e0: 0a20 2020 2020 2020 2020 2020 2053 7563  .            Suc
-000137f0: 6365 7373 206f 6620 504f 5354 206f 7065  cess of POST ope
-00013800: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00013810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000137c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000137d0: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
+000137e0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000137f0: 5375 6363 6573 7320 6f66 2050 4f53 5420  Success of POST 
+00013800: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
+00013810: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 00013820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013850: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2022  ------.        "
-00013860: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00013870: 6e20 7365 6c66 2e70 6f73 745f 6974 656d  n self.post_item
-00013880: 2874 6162 6c65 2c20 2776 6d6f 7468 6572  (table, 'vmother
-00013890: 626f 6172 6427 290a 0a20 2020 2064 6566  board')..    def
-000138a0: 2070 6f73 745f 7670 6362 2873 656c 662c   post_vpcb(self,
-000138b0: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
-000138c0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
-000138d0: 5420 7461 626c 653a 2076 7063 620a 0a20  T table: vpcb.. 
-000138e0: 2020 2020 2020 2054 6869 7320 6973 2066         This is f
-000138f0: 6f72 2061 2062 6172 6520 5665 746f 2050  or a bare Veto P
-00013900: 4342 2e0a 0a20 2020 2020 2020 202d 2d2d  CB...        ---
+00013850: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00013860: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00013870: 7475 726e 2073 656c 662e 706f 7374 5f69  turn self.post_i
+00013880: 7465 6d28 7461 626c 652c 2027 766d 6f74  tem(table, 'vmot
+00013890: 6865 7262 6f61 7264 2729 0a0a 2020 2020  herboard')..    
+000138a0: 6465 6620 706f 7374 5f76 7063 6228 7365  def post_vpcb(se
+000138b0: 6c66 2c20 7461 626c 6529 3a0a 2020 2020  lf, table):.    
+000138c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000138d0: 504f 5354 2074 6162 6c65 3a20 7670 6362  POST table: vpcb
+000138e0: 0a0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+000138f0: 7320 666f 7220 6120 6261 7265 2056 6574  s for a bare Vet
+00013900: 6f20 5043 422e 0a0a 2020 2020 2020 2020  o PCB...        
 00013910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013950: 2d2d 2d0a 2020 2020 2020 2020 6172 6773  ---.        args
-00013960: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00013970: 6c65 203a 2064 6963 740a 2020 2020 2020  le : dict.      
-00013980: 2020 2020 2020 2020 2020 652e 672e 0a20            e.g.. 
-00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139a0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-000139b0: 2020 2020 2020 2020 2020 2020 2027 7072               'pr
-000139c0: 6f64 7563 7469 6f6e 5f64 6174 6527 3a20  oduction_date': 
-000139d0: 2732 3032 322d 3039 2d30 3620 3135 3a33  '2022-09-06 15:3
-000139e0: 303a 3134 272c 0a20 2020 2020 2020 2020  0:14',.         
-000139f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00013a00: 6d61 6e75 6661 6374 7572 6572 273a 2035  manufacturer': 5
-00013a10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013a20: 2020 2020 2020 2020 2020 2772 756e 5f6e            'run_n
-00013a30: 756d 6265 7227 2c20 3132 2c0a 2020 2020  umber', 12,.    
+00013950: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
+00013960: 7267 730a 2020 2020 2020 2020 2020 2020  rgs.            
+00013970: 7461 626c 6520 3a20 6469 6374 0a20 2020  table : dict.   
+00013980: 2020 2020 2020 2020 2020 2020 2065 2e67               e.g
+00013990: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000139a0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139c0: 2770 726f 6475 6374 696f 6e5f 6461 7465  'production_date
+000139d0: 273a 2027 3230 3232 2d30 392d 3036 2031  ': '2022-09-06 1
+000139e0: 353a 3330 3a31 3427 2c0a 2020 2020 2020  5:30:14',.      
+000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a00: 2020 276d 616e 7566 6163 7475 7265 7227    'manufacturer'
+00013a10: 3a20 352c 0a20 2020 2020 2020 2020 2020  : 5,.           
+00013a20: 2020 2020 2020 2020 2020 2020 2027 7275               'ru
+00013a30: 6e5f 6e75 6d62 6572 272c 2031 322c 0a20  n_number', 12,. 
 00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 2020 2020 2771 7263 6f64 6527 3a20 2732      'qrcode': '2
-00013a60: 3230 3630 3130 3131 3132 3334 3537 3839  2060101112345789
-00013a70: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00013a80: 2020 2020 2020 2020 2020 2023 204f 6d69             # Omi
-00013a90: 7420 7468 6973 2066 6965 6c64 2069 6620  t this field if 
-00013aa0: 7375 626d 6974 7469 6e67 2074 6865 2062  submitting the b
-00013ab0: 6c61 6e6b 2050 4342 2066 6f72 2074 6865  lank PCB for the
-00013ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ad0: 2020 2020 2020 2020 2023 2066 6972 7374           # first
-00013ae0: 2074 696d 652e 2057 6865 6e20 7468 6973   time. When this
-00013af0: 2050 4342 2068 6173 2061 6e20 4153 4943   PCB has an ASIC
-00013b00: 2061 6464 6564 206c 6174 6572 0a20 2020   added later.   
+00013a50: 2020 2020 2020 2027 7172 636f 6465 273a         'qrcode':
+00013a60: 2027 3232 3036 3031 3031 3131 3233 3435   '22060101112345
+00013a70: 3738 3927 2c0a 2020 2020 2020 2020 2020  789',.          
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00013a90: 4f6d 6974 2074 6869 7320 6669 656c 6420  Omit this field 
+00013aa0: 6966 2073 7562 6d69 7474 696e 6720 7468  if submitting th
+00013ab0: 6520 626c 616e 6b20 5043 4220 666f 7220  e blank PCB for 
+00013ac0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00013ad0: 2020 2020 2020 2020 2020 2020 2320 6669              # fi
+00013ae0: 7273 7420 7469 6d65 2e20 5768 656e 2074  rst time. When t
+00013af0: 6869 7320 5043 4220 6861 7320 616e 2041  his PCB has an A
+00013b00: 5349 4320 6164 6465 6420 6c61 7465 720a  SIC added later.
 00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b20: 2020 2020 2023 2061 6e64 2062 6563 6f6d       # and becom
-00013b30: 6573 2061 2076 7063 625f 6173 6963 2c20  es a vpcb_asic, 
-00013b40: 7468 6973 2049 4420 6361 6e20 6265 2061  this ID can be a
-00013b50: 6464 6564 2074 6f0a 2020 2020 2020 2020  dded to.        
+00013b20: 2020 2020 2020 2020 2320 616e 6420 6265          # and be
+00013b30: 636f 6d65 7320 6120 7670 6362 5f61 7369  comes a vpcb_asi
+00013b40: 632c 2074 6869 7320 4944 2063 616e 2062  c, this ID can b
+00013b50: 6520 6164 6465 6420 746f 0a20 2020 2020  e added to.     
 00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b70: 2320 706f 696e 7420 746f 2074 6861 742e  # point to that.
-00013b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b90: 2020 2020 2020 2020 2027 7670 6362 5f61           'vpcb_a
-00013ba0: 7369 635f 6964 273a 2033 2c0a 2020 2020  sic_id': 3,.    
+00013b70: 2020 2023 2070 6f69 6e74 2074 6f20 7468     # point to th
+00013b80: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
+00013b90: 2020 2020 2020 2020 2020 2020 2776 7063              'vpc
+00013ba0: 625f 6173 6963 5f69 6427 3a20 332c 0a20  b_asic_id': 3,. 
 00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 7d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  }.        ------
+00013bc0: 2020 207d 0a20 2020 2020 2020 202d 2d2d     }.        ---
 00013bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013c10: 0a20 2020 2020 2020 2072 6574 7572 6e73  .        returns
-00013c20: 203a 2062 6f6f 6c0a 2020 2020 2020 2020   : bool.        
-00013c30: 2020 2020 5375 6363 6573 7320 6f66 2050      Success of P
-00013c40: 4f53 5420 6f70 6572 6174 696f 6e2e 0a20  OST operation.. 
-00013c50: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00013c10: 2d2d 2d0a 2020 2020 2020 2020 7265 7475  ---.        retu
+00013c20: 726e 7320 3a20 626f 6f6c 0a20 2020 2020  rns : bool.     
+00013c30: 2020 2020 2020 2053 7563 6365 7373 206f         Success o
+00013c40: 6620 504f 5354 206f 7065 7261 7469 6f6e  f POST operation
+00013c50: 2e0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
 00013c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00013ca0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013cb0: 2020 7265 7475 726e 2073 656c 662e 706f    return self.po
-00013cc0: 7374 5f69 7465 6d28 7461 626c 652c 2027  st_item(table, '
-00013cd0: 7670 6362 2729 0a0a 2020 2020 6465 6620  vpcb')..    def 
-00013ce0: 706f 7374 5f76 7063 625f 6173 6963 2873  post_vpcb_asic(s
-00013cf0: 656c 662c 2074 6162 6c65 293a 0a20 2020  elf, table):.   
-00013d00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013d10: 2050 4f53 5420 7461 626c 653a 2076 7063   POST table: vpc
-00013d20: 625f 6173 6963 0a0a 2020 2020 2020 2020  b_asic..        
-00013d30: 5468 6973 2069 7320 666f 7220 6120 5665  This is for a Ve
-00013d40: 746f 2050 4342 2077 6974 6820 6261 636b  to PCB with back
-00013d50: 2d73 6964 6520 636f 6d70 6f6e 656e 7473  -side components
-00013d60: 2061 6e64 2061 6e20 4153 4943 2069 6e73   and an ASIC ins
-00013d70: 7461 6c6c 6564 2e0a 0a20 2020 2020 2020  talled...       
-00013d80: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00013c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013ca0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013cb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00013cc0: 2e70 6f73 745f 6974 656d 2874 6162 6c65  .post_item(table
+00013cd0: 2c20 2776 7063 6227 290a 0a20 2020 2064  , 'vpcb')..    d
+00013ce0: 6566 2070 6f73 745f 7670 6362 5f61 7369  ef post_vpcb_asi
+00013cf0: 6328 7365 6c66 2c20 7461 626c 6529 3a0a  c(self, table):.
+00013d00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00013d10: 2020 2020 504f 5354 2074 6162 6c65 3a20      POST table: 
+00013d20: 7670 6362 5f61 7369 630a 0a20 2020 2020  vpcb_asic..     
+00013d30: 2020 2054 6869 7320 6973 2066 6f72 2061     This is for a
+00013d40: 2056 6574 6f20 5043 4220 7769 7468 2062   Veto PCB with b
+00013d50: 6163 6b2d 7369 6465 2063 6f6d 706f 6e65  ack-side compone
+00013d60: 6e74 7320 616e 6420 616e 2041 5349 4320  nts and an ASIC 
+00013d70: 696e 7374 616c 6c65 642e 0a0a 2020 2020  installed...    
+00013d80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 00013d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013dc0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00013dd0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-00013de0: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
-00013df0: 2020 2020 2020 2020 2020 2020 2020 652e                e.
-00013e00: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
-00013e10: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00013dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00013dd0: 2020 2061 7267 730a 2020 2020 2020 2020     args.        
+00013de0: 2020 2020 7461 626c 6520 3a20 6469 6374      table : dict
+00013df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e00: 2065 2e67 2e0a 2020 2020 2020 2020 2020   e.g..          
+00013e10: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
 00013e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e30: 2027 7072 6f64 7563 7469 6f6e 5f64 6174   'production_dat
-00013e40: 6527 3a20 2732 3032 322d 3039 2d30 3620  e': '2022-09-06 
-00013e50: 3135 3a33 303a 3134 272c 0a20 2020 2020  15:30:14',.     
+00013e30: 2020 2020 2770 726f 6475 6374 696f 6e5f      'production_
+00013e40: 6461 7465 273a 2027 3230 3232 2d30 392d  date': '2022-09-
+00013e50: 3036 2031 353a 3330 3a31 3427 2c0a 2020  06 15:30:14',.  
 00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e70: 2020 2027 7670 6362 5f69 6427 3a20 352c     'vpcb_id': 5,
-00013e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013e90: 2020 2020 2020 2020 2027 7661 7369 635f           'vasic_
-00013ea0: 6964 272c 2031 322c 0a20 2020 2020 2020  id', 12,.       
+00013e70: 2020 2020 2020 2776 7063 625f 6964 273a        'vpcb_id':
+00013e80: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
+00013e90: 2020 2020 2020 2020 2020 2020 2776 6173              'vas
+00013ea0: 6963 5f69 6427 2c20 3132 2c0a 2020 2020  ic_id', 12,.    
 00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ec0: 2027 736f 6c64 6572 5f6d 6173 7327 3a20   'solder_mass': 
-00013ed0: 3138 2e31 2c0a 2020 2020 2020 2020 2020  18.1,.          
-00013ee0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00013ef0: 7468 6973 2072 6566 6572 7320 746f 2074  this refers to t
-00013f00: 6865 206f 7269 6769 6e61 6c20 6261 7265  he original bare
-00013f10: 2076 5469 6c65 2050 4342 2773 2049 442e   vTile PCB's ID.
-00013f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f30: 2020 2020 2020 2020 2027 7674 696c 655f           'vtile_
-00013f40: 6964 273a 2033 2c0a 2020 2020 2020 2020  id': 3,.        
-00013f50: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00013f60: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00013ec0: 2020 2020 2773 6f6c 6465 725f 6d61 7373      'solder_mass
+00013ed0: 273a 2031 382e 312c 0a20 2020 2020 2020  ': 18.1,.       
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2023 2074 6869 7320 7265 6665 7273 2074   # this refers t
+00013f00: 6f20 7468 6520 6f72 6967 696e 616c 2062  o the original b
+00013f10: 6172 6520 7654 696c 6520 5043 4227 7320  are vTile PCB's 
+00013f20: 4944 2e0a 2020 2020 2020 2020 2020 2020  ID..            
+00013f30: 2020 2020 2020 2020 2020 2020 2776 7469              'vti
+00013f40: 6c65 5f69 6427 3a20 332c 0a20 2020 2020  le_id': 3,.     
+00013f50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00013f60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
 00013f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00013f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00013fb0: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
-00013fc0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00013fd0: 5375 6363 6573 7320 6f66 2050 4f53 5420  Success of POST 
-00013fe0: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
-00013ff0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00013fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00013fb0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+00013fc0: 3a20 626f 6f6c 0a20 2020 2020 2020 2020  : bool.         
+00013fd0: 2020 2053 7563 6365 7373 206f 6620 504f     Success of PO
+00013fe0: 5354 206f 7065 7261 7469 6f6e 2e0a 2020  ST operation..  
+00013ff0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 00014000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014030: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00014040: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00014050: 7475 726e 2073 656c 662e 706f 7374 5f69  turn self.post_i
-00014060: 7465 6d28 7461 626c 652c 2027 7670 6362  tem(table, 'vpcb
-00014070: 5f61 7369 6327 290a 0a20 2020 2064 6566  _asic')..    def
-00014080: 2070 6f73 745f 7670 6475 2873 656c 662c   post_vpdu(self,
-00014090: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
-000140a0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
-000140b0: 5420 7461 626c 653a 2076 7064 750a 0a20  T table: vpdu.. 
-000140c0: 2020 2020 2020 2054 6869 7320 6973 2066         This is f
-000140d0: 6f72 2061 2056 6574 6f20 5044 5520 7769  or a Veto PDU wi
-000140e0: 7468 2031 3620 7674 696c 6573 2069 6e73  th 16 vtiles ins
-000140f0: 7461 6c6c 6564 2e0a 0a20 2020 2020 2020  talled...       
-00014100: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00014030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00014040: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014050: 2072 6574 7572 6e20 7365 6c66 2e70 6f73   return self.pos
+00014060: 745f 6974 656d 2874 6162 6c65 2c20 2776  t_item(table, 'v
+00014070: 7063 625f 6173 6963 2729 0a0a 2020 2020  pcb_asic')..    
+00014080: 6465 6620 706f 7374 5f76 7064 7528 7365  def post_vpdu(se
+00014090: 6c66 2c20 7461 626c 6529 3a0a 2020 2020  lf, table):.    
+000140a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000140b0: 504f 5354 2074 6162 6c65 3a20 7670 6475  POST table: vpdu
+000140c0: 0a0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
+000140d0: 7320 666f 7220 6120 5665 746f 2050 4455  s for a Veto PDU
+000140e0: 2077 6974 6820 3136 2076 7469 6c65 7320   with 16 vtiles 
+000140f0: 696e 7374 616c 6c65 642e 0a0a 2020 2020  installed...    
+00014100: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
 00014110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014140: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00014150: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-00014160: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
-00014170: 2020 2020 2020 2020 2020 2020 2020 652e                e.
-00014180: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
-00014190: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00014140: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00014150: 2020 2061 7267 730a 2020 2020 2020 2020     args.        
+00014160: 2020 2020 7461 626c 6520 3a20 6469 6374      table : dict
+00014170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014180: 2065 2e67 2e0a 2020 2020 2020 2020 2020   e.g..          
+00014190: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
 000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141b0: 2027 7072 6f64 7563 7469 6f6e 5f64 6174   'production_dat
-000141c0: 6527 3a20 2732 3032 322d 3039 2d30 3620  e': '2022-09-06 
-000141d0: 3135 3a33 303a 3134 272c 0a20 2020 2020  15:30:14',.     
+000141b0: 2020 2020 2770 726f 6475 6374 696f 6e5f      'production_
+000141c0: 6461 7465 273a 2027 3230 3232 2d30 392d  date': '2022-09-
+000141d0: 3036 2031 353a 3330 3a31 3427 2c0a 2020  06 15:30:14',.  
 000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141f0: 2020 2027 6d61 6e75 6661 6374 7572 6572     'manufacturer
-00014200: 273a 2037 2c0a 2020 2020 2020 2020 2020  ': 7,.          
-00014210: 2020 2020 2020 2020 2020 2020 2020 2772                'r
-00014220: 756e 5f6e 756d 6265 7227 3a20 3233 342c  un_number': 234,
-00014230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014240: 2020 2020 2020 2020 2027 7365 7269 616c           'serial
-00014250: 273a 2027 3132 3334 3536 3741 270a 2020  ': '1234567A'.  
-00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2020 2020 2020 2776 6d6f 7468 6572 626f        'vmotherbo
-00014280: 6172 645f 6964 273a 2035 2c0a 2020 2020  ard_id': 5,.    
+000141f0: 2020 2020 2020 276d 616e 7566 6163 7475        'manufactu
+00014200: 7265 7227 3a20 372c 0a20 2020 2020 2020  rer': 7,.       
+00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014220: 2027 7275 6e5f 6e75 6d62 6572 273a 2032   'run_number': 2
+00014230: 3334 2c0a 2020 2020 2020 2020 2020 2020  34,.            
+00014240: 2020 2020 2020 2020 2020 2020 2773 6572              'ser
+00014250: 6961 6c27 3a20 2731 3233 3435 3637 4127  ial': '1234567A'
+00014260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014270: 2020 2020 2020 2020 2027 766d 6f74 6865           'vmothe
+00014280: 7262 6f61 7264 5f69 6427 3a20 352c 0a20  rboard_id': 5,. 
 00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142a0: 2020 2020 2320 3136 7820 7674 696c 655f      # 16x vtile_
-000142b0: 7069 640a 2020 2020 2020 2020 2020 2020  pid.            
-000142c0: 2020 2020 2020 2020 2020 2020 2776 7469              'vti
-000142d0: 6c65 5f31 273a 2031 372c 0a20 2020 2020  le_1': 17,.     
+000142a0: 2020 2020 2020 2023 2031 3678 2076 7469         # 16x vti
+000142b0: 6c65 5f70 6964 0a20 2020 2020 2020 2020  le_pid.         
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000142d0: 7674 696c 655f 3127 3a20 3137 2c0a 2020  vtile_1': 17,.  
 000142e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142f0: 2020 2027 7674 696c 655f 3227 3a20 3138     'vtile_2': 18
-00014300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014310: 2020 2020 2020 2020 2020 2776 7469 6c65            'vtile
-00014320: 5f33 273a 2031 392c 0a20 2020 2020 2020  _3': 19,.       
+000142f0: 2020 2020 2020 2776 7469 6c65 5f32 273a        'vtile_2':
+00014300: 2031 382c 0a20 2020 2020 2020 2020 2020   18,.           
+00014310: 2020 2020 2020 2020 2020 2020 2027 7674               'vt
+00014320: 696c 655f 3327 3a20 3139 2c0a 2020 2020  ile_3': 19,.    
 00014330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014340: 2027 7674 696c 655f 3427 3a20 3230 2c0a   'vtile_4': 20,.
-00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014360: 2020 2020 2020 2020 2776 7469 6c65 5f35          'vtile_5
-00014370: 273a 2032 312c 0a20 2020 2020 2020 2020  ': 21,.         
-00014380: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014390: 7674 696c 655f 3627 3a20 3232 2c0a 2020  vtile_6': 22,.  
-000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143b0: 2020 2020 2020 2776 7469 6c65 5f37 273a        'vtile_7':
-000143c0: 2032 332c 0a20 2020 2020 2020 2020 2020   23,.           
-000143d0: 2020 2020 2020 2020 2020 2020 2027 7674               'vt
-000143e0: 696c 655f 3827 3a20 3234 2c0a 2020 2020  ile_8': 24,.    
+00014340: 2020 2020 2776 7469 6c65 5f34 273a 2032      'vtile_4': 2
+00014350: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00014360: 2020 2020 2020 2020 2020 2027 7674 696c             'vtil
+00014370: 655f 3527 3a20 3231 2c0a 2020 2020 2020  e_5': 21,.      
+00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014390: 2020 2776 7469 6c65 5f36 273a 2032 322c    'vtile_6': 22,
+000143a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000143b0: 2020 2020 2020 2020 2027 7674 696c 655f           'vtile_
+000143c0: 3727 3a20 3233 2c0a 2020 2020 2020 2020  7': 23,.        
+000143d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143e0: 2776 7469 6c65 5f38 273a 2032 342c 0a20  'vtile_8': 24,. 
 000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 2020 2020 2776 7469 6c65 5f39 273a 2032      'vtile_9': 2
-00014410: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00014420: 2020 2020 2020 2020 2020 2027 7674 696c             'vtil
-00014430: 655f 3130 273a 2032 362c 0a20 2020 2020  e_10': 26,.     
+00014400: 2020 2020 2020 2027 7674 696c 655f 3927         'vtile_9'
+00014410: 3a20 3235 2c0a 2020 2020 2020 2020 2020  : 25,.          
+00014420: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+00014430: 7469 6c65 5f31 3027 3a20 3236 2c0a 2020  tile_10': 26,.  
 00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 2020 2027 7674 696c 655f 3131 273a 2032     'vtile_11': 2
-00014460: 372c 0a20 2020 2020 2020 2020 2020 2020  7,.             
-00014470: 2020 2020 2020 2020 2020 2027 7674 696c             'vtil
-00014480: 655f 3132 273a 2032 382c 0a20 2020 2020  e_12': 28,.     
+00014450: 2020 2020 2020 2776 7469 6c65 5f31 3127        'vtile_11'
+00014460: 3a20 3237 2c0a 2020 2020 2020 2020 2020  : 27,.          
+00014470: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+00014480: 7469 6c65 5f31 3227 3a20 3238 2c0a 2020  tile_12': 28,.  
 00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144a0: 2020 2027 7674 696c 655f 3133 273a 2032     'vtile_13': 2
-000144b0: 392c 0a20 2020 2020 2020 2020 2020 2020  9,.             
-000144c0: 2020 2020 2020 2020 2020 2027 7674 696c             'vtil
-000144d0: 655f 3134 273a 2033 302c 0a20 2020 2020  e_14': 30,.     
+000144a0: 2020 2020 2020 2776 7469 6c65 5f31 3327        'vtile_13'
+000144b0: 3a20 3239 2c0a 2020 2020 2020 2020 2020  : 29,.          
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+000144d0: 7469 6c65 5f31 3427 3a20 3330 2c0a 2020  tile_14': 30,.  
 000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144f0: 2020 2027 7674 696c 655f 3135 273a 2033     'vtile_15': 3
-00014500: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00014510: 2020 2020 2020 2020 2020 2027 7674 696c             'vtil
-00014520: 655f 3136 273a 2033 322c 0a20 2020 2020  e_16': 32,.     
+000144f0: 2020 2020 2020 2776 7469 6c65 5f31 3527        'vtile_15'
+00014500: 3a20 3331 2c0a 2020 2020 2020 2020 2020  : 31,.          
+00014510: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+00014520: 7469 6c65 5f31 3627 3a20 3332 2c0a 2020  tile_16': 32,.  
 00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014540: 2020 2027 6465 7465 6374 6f72 5f69 6427     'detector_id'
-00014550: 3a20 332c 0a20 2020 2020 2020 2020 2020  : 3,.           
-00014560: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00014570: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00014540: 2020 2020 2020 2764 6574 6563 746f 725f        'detector_
+00014550: 6964 273a 2033 2c0a 2020 2020 2020 2020  id': 3,.        
+00014560: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00014570: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 00014580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000145a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000145b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000145c0: 2020 7265 7475 726e 7320 3a20 626f 6f6c    returns : bool
-000145d0: 0a20 2020 2020 2020 2020 2020 2053 7563  .            Suc
-000145e0: 6365 7373 206f 6620 504f 5354 206f 7065  cess of POST ope
-000145f0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-00014600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000145b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000145c0: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
+000145d0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000145e0: 5375 6363 6573 7320 6f66 2050 4f53 5420  Success of POST 
+000145f0: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
+00014600: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 00014610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014640: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2022  ------.        "
-00014650: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00014660: 6e20 7365 6c66 2e70 6f73 745f 6974 656d  n self.post_item
-00014670: 2874 6162 6c65 2c20 2776 7064 7527 290a  (table, 'vpdu').
-00014680: 0a20 2020 2064 6566 2070 6f73 745f 7674  .    def post_vt
-00014690: 696c 6528 7365 6c66 2c20 7461 626c 6529  ile(self, table)
-000146a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000146b0: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-000146c0: 3a20 7674 696c 650a 0a20 2020 2020 2020  : vtile..       
-000146d0: 2054 6869 7320 6973 2066 6f72 2061 2056   This is for a V
-000146e0: 6574 6f20 5043 4220 7769 7468 2062 6163  eto PCB with bac
-000146f0: 6b2d 7369 6465 2063 6f6d 706f 6e65 6e74  k-side component
-00014700: 732c 2041 5349 4320 616e 6420 5369 504d  s, ASIC and SiPM
-00014710: 730a 2020 2020 2020 2020 696e 7374 616c  s.        instal
-00014720: 6c65 642e 0a0a 2020 2020 2020 2020 5468  led...        Th
-00014730: 6520 5369 504d 206e 756d 6265 7269 6e67  e SiPM numbering
-00014740: 2069 7320 7368 6f77 6e20 6c6f 6f6b 696e   is shown lookin
-00014750: 6720 6174 2074 6865 2050 4342 2077 6974  g at the PCB wit
-00014760: 6820 5369 504d 7320 7669 7369 626c 6520  h SiPMs visible 
-00014770: 616e 640a 2020 2020 2020 2020 746f 7761  and.        towa
-00014780: 7264 7320 7468 6520 7669 6577 6572 2c20  rds the viewer, 
-00014790: 616e 6420 7468 6520 6261 636b 7369 6465  and the backside
-000147a0: 2063 6f6d 706f 6e65 6e74 730a 2020 2020   components.    
-000147b0: 2020 2020 2872 6573 6973 746f 7273 2c20      (resistors, 
-000147c0: 6361 7061 6369 746f 7273 2c20 4153 4943  capacitors, ASIC
-000147d0: 2065 7463 2e29 2066 6163 696e 6720 6177   etc.) facing aw
-000147e0: 6179 2066 726f 6d20 7468 6520 7669 6577  ay from the view
-000147f0: 6572 2e20 5468 650a 2020 2020 2020 2020  er. The.        
-00014800: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
-00014810: 5152 2063 6f64 6520 616e 6420 4153 4943  QR code and ASIC
-00014820: 206f 6e20 7468 6520 6261 636b 2d73 6964   on the back-sid
-00014830: 6520 6f66 2074 6865 2050 4342 2061 7265  e of the PCB are
-00014840: 2061 6c73 6f0a 2020 2020 2020 2020 7368   also.        sh
-00014850: 6f77 6e20 746f 2070 726f 7669 6465 206f  own to provide o
-00014860: 7269 656e 7461 7469 6f6e 2e0a 0a20 2020  rientation...   
-00014870: 2020 2020 202b 2d2d 2d2d 2b2d 2d2d 2d2b       +----+----+
-00014880: 2d2d 2d2d 2b2d 2d2d 2d2b 0a20 2020 2020  ----+----+.     
-00014890: 2020 207c 2031 3920 7c20 3133 207c 2020     | 19 | 13 |  
-000148a0: 3720 7c20 2031 207c 0a20 2020 2020 2020  7 |  1 |.       
-000148b0: 202b 2d2d 2d2d 2b2d 2d2d 5152 2d2d 2d2d   +----+---QR----
-000148c0: 2b2d 2d2d 2d2b 0a20 2020 2020 2020 207c  +----+.        |
-000148d0: 2032 3020 7c20 3134 207c 2020 3820 7c20   20 | 14 |  8 | 
-000148e0: 2032 207c 0a20 2020 2020 2020 202b 2d2d   2 |.        +--
-000148f0: 2d2d 2b2d 2d2d 2d2b 2d2d 2d2d 2b2d 2d2d  --+----+----+---
-00014900: 2d2b 0a20 2020 2020 2020 207c 2032 3120  -+.        | 21 
-00014910: 7c20 3135 207c 2020 3920 7c20 2033 207c  | 15 |  9 |  3 |
-00014920: 0a20 2020 2020 2020 202b 2d2d 2d2d 2b2d  .        +----+-
-00014930: 2d2d 2d2b 2d2d 2d2d 2b2d 2d2d 2d2b 0a20  ---+----+----+. 
-00014940: 2020 2020 2020 207c 2032 3220 7c20 3136         | 22 | 16
-00014950: 207c 2031 3020 7c20 2034 207c 0a20 2020   | 10 |  4 |.   
-00014960: 2020 2020 202b 2d2d 2d2d 2b2d 2d2d 4153       +----+---AS
-00014970: 4943 2d2d 2b2d 2d2d 2d2b 0a20 2020 2020  IC--+----+.     
-00014980: 2020 207c 2032 3320 7c20 3137 207c 2031     | 23 | 17 | 1
-00014990: 3120 7c20 2035 207c 0a20 2020 2020 2020  1 |  5 |.       
-000149a0: 202b 2d2d 2d2d 2b2d 2d2d 2d2b 2d2d 2d2d   +----+----+----
-000149b0: 2b2d 2d2d 2d2b 0a20 2020 2020 2020 207c  +----+.        |
-000149c0: 2032 3420 7c20 3138 207c 2031 3220 7c20   24 | 18 | 12 | 
-000149d0: 2036 207c 0a20 2020 2020 2020 202b 2d2d   6 |.        +--
-000149e0: 2d2d 2b2d 2d2d 2d2b 2d2d 2d2d 2b2d 2d2d  --+----+----+---
-000149f0: 2d2b 0a0a 2020 2020 2020 2020 2d2d 2d2d  -+..        ----
+00014640: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00014650: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00014660: 7475 726e 2073 656c 662e 706f 7374 5f69  turn self.post_i
+00014670: 7465 6d28 7461 626c 652c 2027 7670 6475  tem(table, 'vpdu
+00014680: 2729 0a0a 2020 2020 6465 6620 706f 7374  ')..    def post
+00014690: 5f76 7469 6c65 2873 656c 662c 2074 6162  _vtile(self, tab
+000146a0: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+000146b0: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+000146c0: 626c 653a 2076 7469 6c65 0a0a 2020 2020  ble: vtile..    
+000146d0: 2020 2020 5468 6973 2069 7320 666f 7220      This is for 
+000146e0: 6120 5665 746f 2050 4342 2077 6974 6820  a Veto PCB with 
+000146f0: 6261 636b 2d73 6964 6520 636f 6d70 6f6e  back-side compon
+00014700: 656e 7473 2c20 4153 4943 2061 6e64 2053  ents, ASIC and S
+00014710: 6950 4d73 0a20 2020 2020 2020 2069 6e73  iPMs.        ins
+00014720: 7461 6c6c 6564 2e0a 0a20 2020 2020 2020  talled...       
+00014730: 2054 6865 2053 6950 4d20 6e75 6d62 6572   The SiPM number
+00014740: 696e 6720 6973 2073 686f 776e 206c 6f6f  ing is shown loo
+00014750: 6b69 6e67 2061 7420 7468 6520 5043 4220  king at the PCB 
+00014760: 7769 7468 2053 6950 4d73 2076 6973 6962  with SiPMs visib
+00014770: 6c65 2061 6e64 0a20 2020 2020 2020 2074  le and.        t
+00014780: 6f77 6172 6473 2074 6865 2076 6965 7765  owards the viewe
+00014790: 722c 2061 6e64 2074 6865 2062 6163 6b73  r, and the backs
+000147a0: 6964 6520 636f 6d70 6f6e 656e 7473 0a20  ide components. 
+000147b0: 2020 2020 2020 2028 7265 7369 7374 6f72         (resistor
+000147c0: 732c 2063 6170 6163 6974 6f72 732c 2041  s, capacitors, A
+000147d0: 5349 4320 6574 632e 2920 6661 6369 6e67  SIC etc.) facing
+000147e0: 2061 7761 7920 6672 6f6d 2074 6865 2076   away from the v
+000147f0: 6965 7765 722e 2054 6865 0a20 2020 2020  iewer. The.     
+00014800: 2020 206c 6f63 6174 696f 6e20 6f66 2074     location of t
+00014810: 6865 2051 5220 636f 6465 2061 6e64 2041  he QR code and A
+00014820: 5349 4320 6f6e 2074 6865 2062 6163 6b2d  SIC on the back-
+00014830: 7369 6465 206f 6620 7468 6520 5043 4220  side of the PCB 
+00014840: 6172 6520 616c 736f 0a20 2020 2020 2020  are also.       
+00014850: 2073 686f 776e 2074 6f20 7072 6f76 6964   shown to provid
+00014860: 6520 6f72 6965 6e74 6174 696f 6e2e 0a0a  e orientation...
+00014870: 2020 2020 2020 2020 2b2d 2d2d 2d2b 2d2d          +----+--
+00014880: 2d2d 2b2d 2d2d 2d2b 2d2d 2d2d 2b0a 2020  --+----+----+.  
+00014890: 2020 2020 2020 7c20 3139 207c 2031 3320        | 19 | 13 
+000148a0: 7c20 2037 207c 2020 3120 7c0a 2020 2020  |  7 |  1 |.    
+000148b0: 2020 2020 2b2d 2d2d 2d2b 2d2d 2d51 522d      +----+---QR-
+000148c0: 2d2d 2d2b 2d2d 2d2d 2b0a 2020 2020 2020  ---+----+.      
+000148d0: 2020 7c20 3230 207c 2031 3420 7c20 2038    | 20 | 14 |  8
+000148e0: 207c 2020 3220 7c0a 2020 2020 2020 2020   |  2 |.        
+000148f0: 2b2d 2d2d 2d2b 2d2d 2d2d 2b2d 2d2d 2d2b  +----+----+----+
+00014900: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
+00014910: 3231 207c 2031 3520 7c20 2039 207c 2020  21 | 15 |  9 |  
+00014920: 3320 7c0a 2020 2020 2020 2020 2b2d 2d2d  3 |.        +---
+00014930: 2d2b 2d2d 2d2d 2b2d 2d2d 2d2b 2d2d 2d2d  -+----+----+----
+00014940: 2b0a 2020 2020 2020 2020 7c20 3232 207c  +.        | 22 |
+00014950: 2031 3620 7c20 3130 207c 2020 3420 7c0a   16 | 10 |  4 |.
+00014960: 2020 2020 2020 2020 2b2d 2d2d 2d2b 2d2d          +----+--
+00014970: 2d41 5349 432d 2d2b 2d2d 2d2d 2b0a 2020  -ASIC--+----+.  
+00014980: 2020 2020 2020 7c20 3233 207c 2031 3720        | 23 | 17 
+00014990: 7c20 3131 207c 2020 3520 7c0a 2020 2020  | 11 |  5 |.    
+000149a0: 2020 2020 2b2d 2d2d 2d2b 2d2d 2d2d 2b2d      +----+----+-
+000149b0: 2d2d 2d2b 2d2d 2d2d 2b0a 2020 2020 2020  ---+----+.      
+000149c0: 2020 7c20 3234 207c 2031 3820 7c20 3132    | 24 | 18 | 12
+000149d0: 207c 2020 3620 7c0a 2020 2020 2020 2020   |  6 |.        
+000149e0: 2b2d 2d2d 2d2b 2d2d 2d2d 2b2d 2d2d 2d2b  +----+----+----+
+000149f0: 2d2d 2d2d 2b0a 0a20 2020 2020 2020 202d  ----+..        -
 00014a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00014a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00014a40: 2d2d 0a20 2020 2020 2020 2061 7267 730a  --.        args.
-00014a50: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00014a60: 6520 3a20 6469 6374 0a20 2020 2020 2020  e : dict.       
-00014a70: 2020 2020 2020 2020 2065 2e67 2e0a 2020           e.g..  
-00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00014aa0: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-00014ab0: 6475 6374 696f 6e5f 6461 7465 273a 2027  duction_date': '
-00014ac0: 3230 3232 2d30 392d 3036 2031 353a 3330  2022-09-06 15:30
-00014ad0: 3a31 3427 2c0a 2020 2020 2020 2020 2020  :14',.          
-00014ae0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00014af0: 616e 7566 6163 7475 7265 7227 3a20 372c  anufacturer': 7,
-00014b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014b10: 2020 2020 2020 2020 2027 7275 6e5f 6e75           'run_nu
-00014b20: 6d62 6572 273a 2032 3334 2c0a 2020 2020  mber': 234,.    
+00014a40: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6172  -----.        ar
+00014a50: 6773 0a20 2020 2020 2020 2020 2020 2074  gs.            t
+00014a60: 6162 6c65 203a 2064 6963 740a 2020 2020  able : dict.    
+00014a70: 2020 2020 2020 2020 2020 2020 652e 672e              e.g.
+00014a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014a90: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014ab0: 7072 6f64 7563 7469 6f6e 5f64 6174 6527  production_date'
+00014ac0: 3a20 2732 3032 322d 3039 2d30 3620 3135  : '2022-09-06 15
+00014ad0: 3a33 303a 3134 272c 0a20 2020 2020 2020  :30:14',.       
+00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014af0: 2027 6d61 6e75 6661 6374 7572 6572 273a   'manufacturer':
+00014b00: 2037 2c0a 2020 2020 2020 2020 2020 2020   7,.            
+00014b10: 2020 2020 2020 2020 2020 2020 2772 756e              'run
+00014b20: 5f6e 756d 6265 7227 3a20 3233 342c 0a20  _number': 234,. 
 00014b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b40: 2020 2020 2773 6572 6961 6c27 3a20 2731      'serial': '1
-00014b50: 3233 3435 3637 4127 0a20 2020 2020 2020  234567A'.       
+00014b40: 2020 2020 2020 2027 7365 7269 616c 273a         'serial':
+00014b50: 2027 3132 3334 3536 3741 270a 2020 2020   '1234567A'.    
 00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b70: 2027 7670 6362 5f61 7369 635f 6964 273a   'vpcb_asic_id':
-00014b80: 2035 2c0a 2020 2020 2020 2020 2020 2020   5,.            
-00014b90: 2020 2020 2020 2020 2020 2020 2773 6f6c              'sol
-00014ba0: 6465 725f 6964 273a 2032 2c0a 2020 2020  der_id': 2,.    
+00014b70: 2020 2020 2776 7063 625f 6173 6963 5f69      'vpcb_asic_i
+00014b80: 6427 3a20 352c 0a20 2020 2020 2020 2020  d': 5,.         
+00014b90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014ba0: 736f 6c64 6572 5f69 6427 3a20 322c 0a20  solder_id': 2,. 
 00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 2020 2020 2320 3234 7820 7369 706d 5f70      # 24x sipm_p
-00014bd0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-00014be0: 2020 2020 2020 2020 2020 2027 7369 706d             'sipm
-00014bf0: 5f31 273a 2031 372c 0a20 2020 2020 2020  _1': 17,.       
+00014bc0: 2020 2020 2020 2023 2032 3478 2073 6970         # 24x sip
+00014bd0: 6d5f 7069 640a 2020 2020 2020 2020 2020  m_pid.          
+00014be0: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00014bf0: 6970 6d5f 3127 3a20 3137 2c0a 2020 2020  ipm_1': 17,.    
 00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c10: 2027 7369 706d 5f32 273a 2031 382c 0a20   'sipm_2': 18,. 
-00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c30: 2020 2020 2020 2027 7369 706d 5f33 273a         'sipm_3':
-00014c40: 2031 392c 0a20 2020 2020 2020 2020 2020   19,.           
-00014c50: 2020 2020 2020 2020 2020 2020 2027 7369               'si
-00014c60: 706d 5f34 273a 2032 302c 0a20 2020 2020  pm_4': 20,.     
+00014c10: 2020 2020 2773 6970 6d5f 3227 3a20 3138      'sipm_2': 18
+00014c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014c30: 2020 2020 2020 2020 2020 2773 6970 6d5f            'sipm_
+00014c40: 3327 3a20 3139 2c0a 2020 2020 2020 2020  3': 19,.        
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 2773 6970 6d5f 3427 3a20 3230 2c0a 2020  'sipm_4': 20,.  
 00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c80: 2020 2027 7369 706d 5f35 273a 2032 312c     'sipm_5': 21,
-00014c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ca0: 2020 2020 2020 2020 2027 7369 706d 5f36           'sipm_6
-00014cb0: 273a 2032 322c 0a20 2020 2020 2020 2020  ': 22,.         
-00014cc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014cd0: 7369 706d 5f37 273a 2032 332c 0a20 2020  sipm_7': 23,.   
+00014c80: 2020 2020 2020 2773 6970 6d5f 3527 3a20        'sipm_5': 
+00014c90: 3231 2c0a 2020 2020 2020 2020 2020 2020  21,.            
+00014ca0: 2020 2020 2020 2020 2020 2020 2773 6970              'sip
+00014cb0: 6d5f 3627 3a20 3232 2c0a 2020 2020 2020  m_6': 22,.      
+00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cd0: 2020 2773 6970 6d5f 3727 3a20 3233 2c0a    'sipm_7': 23,.
 00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cf0: 2020 2020 2027 7369 706d 5f38 273a 2032       'sipm_8': 2
-00014d00: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-00014d10: 2020 2020 2020 2020 2020 2027 7369 706d             'sipm
-00014d20: 5f39 273a 2032 352c 0a20 2020 2020 2020  _9': 25,.       
+00014cf0: 2020 2020 2020 2020 2773 6970 6d5f 3827          'sipm_8'
+00014d00: 3a20 3234 2c0a 2020 2020 2020 2020 2020  : 24,.          
+00014d10: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00014d20: 6970 6d5f 3927 3a20 3235 2c0a 2020 2020  ipm_9': 25,.    
 00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d40: 2027 7369 706d 5f31 3027 3a20 3236 2c0a   'sipm_10': 26,.
-00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2020 2020 2020 2020 2773 6970 6d5f 3131          'sipm_11
-00014d70: 273a 2032 372c 0a20 2020 2020 2020 2020  ': 27,.         
-00014d80: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00014d90: 7369 706d 5f31 3227 3a20 3238 2c0a 2020  sipm_12': 28,.  
-00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014db0: 2020 2020 2020 2773 6970 6d5f 3133 273a        'sipm_13':
-00014dc0: 2032 392c 0a20 2020 2020 2020 2020 2020   29,.           
-00014dd0: 2020 2020 2020 2020 2020 2020 2027 7369               'si
-00014de0: 706d 5f31 3427 3a20 3330 2c0a 2020 2020  pm_14': 30,.    
+00014d40: 2020 2020 2773 6970 6d5f 3130 273a 2032      'sipm_10': 2
+00014d50: 362c 0a20 2020 2020 2020 2020 2020 2020  6,.             
+00014d60: 2020 2020 2020 2020 2020 2027 7369 706d             'sipm
+00014d70: 5f31 3127 3a20 3237 2c0a 2020 2020 2020  _11': 27,.      
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 2020 2773 6970 6d5f 3132 273a 2032 382c    'sipm_12': 28,
+00014da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014db0: 2020 2020 2020 2020 2027 7369 706d 5f31           'sipm_1
+00014dc0: 3327 3a20 3239 2c0a 2020 2020 2020 2020  3': 29,.        
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014de0: 2773 6970 6d5f 3134 273a 2033 302c 0a20  'sipm_14': 30,. 
 00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e00: 2020 2020 2773 6970 6d5f 3135 273a 2033      'sipm_15': 3
-00014e10: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00014e20: 2020 2020 2020 2020 2020 2027 7369 706d             'sipm
-00014e30: 5f31 3627 3a20 3332 2c0a 2020 2020 2020  _16': 32,.      
+00014e00: 2020 2020 2020 2027 7369 706d 5f31 3527         'sipm_15'
+00014e10: 3a20 3331 2c0a 2020 2020 2020 2020 2020  : 31,.          
+00014e20: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00014e30: 6970 6d5f 3136 273a 2033 322c 0a20 2020  ipm_16': 32,.   
 00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e50: 2020 2773 6970 6d5f 3137 273a 2033 332c    'sipm_17': 33,
-00014e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e70: 2020 2020 2020 2020 2027 7369 706d 5f31           'sipm_1
-00014e80: 3827 3a20 3334 2c0a 2020 2020 2020 2020  8': 34,.        
+00014e50: 2020 2020 2027 7369 706d 5f31 3727 3a20       'sipm_17': 
+00014e60: 3333 2c0a 2020 2020 2020 2020 2020 2020  33,.            
+00014e70: 2020 2020 2020 2020 2020 2020 2773 6970              'sip
+00014e80: 6d5f 3138 273a 2033 342c 0a20 2020 2020  m_18': 34,.     
 00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ea0: 2773 6970 6d5f 3139 273a 2033 352c 0a20  'sipm_19': 35,. 
-00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ec0: 2020 2020 2020 2027 7369 706d 5f32 3027         'sipm_20'
-00014ed0: 3a20 3336 2c0a 2020 2020 2020 2020 2020  : 36,.          
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00014ef0: 6970 6d5f 3231 273a 2033 372c 0a20 2020  ipm_21': 37,.   
+00014ea0: 2020 2027 7369 706d 5f31 3927 3a20 3335     'sipm_19': 35
+00014eb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014ec0: 2020 2020 2020 2020 2020 2773 6970 6d5f            'sipm_
+00014ed0: 3230 273a 2033 362c 0a20 2020 2020 2020  20': 36,.       
+00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ef0: 2027 7369 706d 5f32 3127 3a20 3337 2c0a   'sipm_21': 37,.
 00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f10: 2020 2020 2027 7369 706d 5f32 3227 3a20       'sipm_22': 
-00014f20: 3338 2c0a 2020 2020 2020 2020 2020 2020  38,.            
-00014f30: 2020 2020 2020 2020 2020 2020 2773 6970              'sip
-00014f40: 6d5f 3233 273a 2033 392c 0a20 2020 2020  m_23': 39,.     
+00014f10: 2020 2020 2020 2020 2773 6970 6d5f 3232          'sipm_22
+00014f20: 273a 2033 382c 0a20 2020 2020 2020 2020  ': 38,.         
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014f40: 7369 706d 5f32 3327 3a20 3339 2c0a 2020  sipm_23': 39,.  
 00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f60: 2020 2027 7369 706d 5f32 3427 3a20 3430     'sipm_24': 40
-00014f70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014f80: 2020 2020 2020 2020 2020 2320 4f6d 6974            # Omit
-00014f90: 2074 6869 7320 6669 656c 6420 6966 2073   this field if s
-00014fa0: 7562 6d69 7474 696e 6720 7468 6520 7469  ubmitting the ti
-00014fb0: 6c65 2066 6f72 2074 6865 0a20 2020 2020  le for the.     
+00014f60: 2020 2020 2020 2773 6970 6d5f 3234 273a        'sipm_24':
+00014f70: 2034 302c 0a20 2020 2020 2020 2020 2020   40,.           
+00014f80: 2020 2020 2020 2020 2020 2020 2023 204f               # O
+00014f90: 6d69 7420 7468 6973 2066 6965 6c64 2069  mit this field i
+00014fa0: 6620 7375 626d 6974 7469 6e67 2074 6865  f submitting the
+00014fb0: 2074 696c 6520 666f 7220 7468 650a 2020   tile for the.  
 00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2023 2066 6972 7374 2074 696d 652e     # first time.
-00014fe0: 2057 6865 6e20 7468 6973 2074 696c 6520   When this tile 
-00014ff0: 6973 2061 7373 656d 626c 6564 206f 6e74  is assembled ont
-00015000: 6f20 6120 7650 4455 0a20 2020 2020 2020  o a vPDU.       
+00014fd0: 2020 2020 2020 2320 6669 7273 7420 7469        # first ti
+00014fe0: 6d65 2e20 5768 656e 2074 6869 7320 7469  me. When this ti
+00014ff0: 6c65 2069 7320 6173 7365 6d62 6c65 6420  le is assembled 
+00015000: 6f6e 746f 2061 2076 5044 550a 2020 2020  onto a vPDU.    
 00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015020: 2023 206c 6174 6572 2c20 7468 6973 2049   # later, this I
-00015030: 4420 6361 6e20 6265 2061 6464 6564 2074  D can be added t
-00015040: 6f20 706f 696e 7420 746f 2074 6861 742e  o point to that.
-00015050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015060: 2020 2020 2020 2020 2027 7670 6475 5f69           'vpdu_i
-00015070: 6427 3a20 332c 0a20 2020 2020 2020 2020  d': 3,.         
-00015080: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00015090: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+00015020: 2020 2020 2320 6c61 7465 722c 2074 6869      # later, thi
+00015030: 7320 4944 2063 616e 2062 6520 6164 6465  s ID can be adde
+00015040: 6420 746f 2070 6f69 6e74 2074 6f20 7468  d to point to th
+00015050: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
+00015060: 2020 2020 2020 2020 2020 2020 2776 7064              'vpd
+00015070: 755f 6964 273a 2033 2c0a 2020 2020 2020  u_id': 3,.      
+00015080: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00015090: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
 000150a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000150b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000150c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000150d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000150e0: 2020 2020 7265 7475 726e 7320 3a20 626f      returns : bo
-000150f0: 6f6c 0a20 2020 2020 2020 2020 2020 2053  ol.            S
-00015100: 7563 6365 7373 206f 6620 504f 5354 206f  uccess of POST o
-00015110: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
-00015120: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000150d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000150e0: 2020 2020 2020 2072 6574 7572 6e73 203a         returns :
+000150f0: 2062 6f6f 6c0a 2020 2020 2020 2020 2020   bool.          
+00015100: 2020 5375 6363 6573 7320 6f66 2050 4f53    Success of POS
+00015110: 5420 6f70 6572 6174 696f 6e2e 0a20 2020  T operation..   
+00015120: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 00015130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00015160: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00015170: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00015180: 7572 6e20 7365 6c66 2e70 6f73 745f 6974  urn self.post_it
-00015190: 656d 2874 6162 6c65 2c20 2776 7469 6c65  em(table, 'vtile
-000151a0: 2729 0a0a 2020 2020 6465 6620 706f 7374  ')..    def post
-000151b0: 5f77 6166 6572 2873 656c 662c 2074 6162  _wafer(self, tab
-000151c0: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
-000151d0: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
-000151e0: 626c 653a 2077 6166 6572 0a0a 2020 2020  ble: wafer..    
-000151f0: 2020 2020 4164 6420 6120 5369 504d 2077      Add a SiPM w
-00015200: 6166 6572 2074 6162 6c65 2074 6f20 7468  afer table to th
-00015210: 6520 6461 7461 6261 7365 2e0a 0a20 2020  e database...   
-00015220: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+00015160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00015170: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015180: 7265 7475 726e 2073 656c 662e 706f 7374  return self.post
+00015190: 5f69 7465 6d28 7461 626c 652c 2027 7674  _item(table, 'vt
+000151a0: 696c 6527 290a 0a20 2020 2064 6566 2070  ile')..    def p
+000151b0: 6f73 745f 7761 6665 7228 7365 6c66 2c20  ost_wafer(self, 
+000151c0: 7461 626c 6529 3a0a 2020 2020 2020 2020  table):.        
+000151d0: 2222 220a 2020 2020 2020 2020 504f 5354  """.        POST
+000151e0: 2074 6162 6c65 3a20 7761 6665 720a 0a20   table: wafer.. 
+000151f0: 2020 2020 2020 2041 6464 2061 2053 6950         Add a SiP
+00015200: 4d20 7761 6665 7220 7461 626c 6520 746f  M wafer table to
+00015210: 2074 6865 2064 6174 6162 6173 652e 0a0a   the database...
+00015220: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
 00015230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00015260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00015270: 2020 2020 6172 6773 0a20 2020 2020 2020      args.       
-00015280: 2020 2020 2074 6162 6c65 203a 2064 6963       table : dic
-00015290: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000152a0: 2020 652e 672e 0a20 2020 2020 2020 2020    e.g..         
-000152b0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00015260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00015270: 2020 2020 2020 2061 7267 730a 2020 2020         args.    
+00015280: 2020 2020 2020 2020 7461 626c 6520 3a20          table : 
+00015290: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+000152a0: 2020 2020 2065 2e67 2e0a 2020 2020 2020       e.g..      
+000152b0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
 000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152d0: 2020 2020 2027 6d61 6e75 6661 6374 7572       'manufactur
-000152e0: 6572 273a 2032 2c0a 2020 2020 2020 2020  er': 2,.        
+000152d0: 2020 2020 2020 2020 276d 616e 7566 6163          'manufac
+000152e0: 7475 7265 7227 3a20 322c 0a20 2020 2020  turer': 2,.     
 000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015300: 276c 6f74 273a 2033 2c0a 2020 2020 2020  'lot': 3,.      
+00015300: 2020 2027 6c6f 7427 3a20 332c 0a20 2020     'lot': 3,.   
 00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015320: 2020 2777 6166 6572 5f6e 756d 6265 7227    'wafer_number'
-00015330: 3a20 362c 0a20 2020 2020 2020 2020 2020  : 6,.           
-00015340: 2020 2020 2020 2020 2020 2020 2027 7370               'sp
-00015350: 6164 5f73 697a 6527 3a20 3330 2c0a 2020  ad_size': 30,.  
-00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015370: 2020 2020 2020 2764 6f73 6527 3a20 332c        'dose': 3,
-00015380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015390: 2020 2020 2020 2020 2027 7072 6f64 7563           'produc
-000153a0: 7469 6f6e 5f64 6174 6527 3a20 2732 3032  tion_date': '202
-000153b0: 322d 3039 2d30 3620 3135 3a33 303a 3134  2-09-06 15:30:14
-000153c0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000153d0: 2020 2020 2020 2020 2020 2027 6465 7363             'desc
-000153e0: 7269 7074 696f 6e27 3a20 352c 0a20 2020  ription': 5,.   
+00015320: 2020 2020 2027 7761 6665 725f 6e75 6d62       'wafer_numb
+00015330: 6572 273a 2036 2c0a 2020 2020 2020 2020  er': 6,.        
+00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015350: 2773 7061 645f 7369 7a65 273a 2033 302c  'spad_size': 30,
+00015360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015370: 2020 2020 2020 2020 2027 646f 7365 273a           'dose':
+00015380: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
+00015390: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
+000153a0: 6475 6374 696f 6e5f 6461 7465 273a 2027  duction_date': '
+000153b0: 3230 3232 2d30 392d 3036 2031 353a 3330  2022-09-06 15:30
+000153c0: 3a31 3427 2c0a 2020 2020 2020 2020 2020  :14',.          
+000153d0: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+000153e0: 6573 6372 6970 7469 6f6e 273a 2035 2c0a  escription': 5,.
 000153f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015400: 207d 0a20 2020 2020 2020 202d 2d2d 2d2d   }.        -----
+00015400: 2020 2020 7d0a 2020 2020 2020 2020 2d2d      }.        --
 00015410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00015450: 2d0a 2020 2020 2020 2020 7265 7475 726e  -.        return
-00015460: 7320 3a20 626f 6f6c 0a20 2020 2020 2020  s : bool.       
-00015470: 2020 2020 2053 7563 6365 7373 206f 6620       Success of 
-00015480: 504f 5354 206f 7065 7261 7469 6f6e 2e0a  POST operation..
-00015490: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00015450: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
+00015460: 7572 6e73 203a 2062 6f6f 6c0a 2020 2020  urns : bool.    
+00015470: 2020 2020 2020 2020 5375 6363 6573 7320          Success 
+00015480: 6f66 2050 4f53 5420 6f70 6572 6174 696f  of POST operatio
+00015490: 6e2e 0a20 2020 2020 2020 202d 2d2d 2d2d  n..        -----
 000154a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000154b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000154c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000154d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-000154e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000154f0: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-00015500: 6f73 745f 6974 656d 2874 6162 6c65 2c20  ost_item(table, 
-00015510: 2777 6166 6572 2729 0a0a 2020 2020 6465  'wafer')..    de
-00015520: 6620 706f 7374 5f77 6166 6572 5f64 6566  f post_wafer_def
-00015530: 6563 7473 2873 656c 662c 2074 6162 6c65  ects(self, table
-00015540: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00015550: 2020 2020 2020 2050 4f53 5420 7461 626c         POST tabl
-00015560: 653a 2077 6166 6572 5f64 6566 6563 7473  e: wafer_defects
-00015570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015580: 2020 2020 2023 2072 6574 7572 6e20 7365       # return se
-00015590: 6c66 2e70 6f73 745f 6974 656d 2874 6162  lf.post_item(tab
-000155a0: 6c65 2c20 2777 6166 6572 5f64 6566 6563  le, 'wafer_defec
-000155b0: 7473 2729 0a20 2020 2020 2020 2072 6169  ts').        rai
-000155c0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000155d0: 6445 7272 6f72 0a0a 2020 2020 6465 6620  dError..    def 
-000155e0: 706f 7374 5f77 6166 6572 5f73 7461 7475  post_wafer_statu
-000155f0: 7328 7365 6c66 2c20 7461 626c 6529 3a0a  s(self, table):.
-00015600: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015610: 2020 2020 504f 5354 2074 6162 6c65 3a20      POST table: 
-00015620: 7761 6665 725f 7374 6174 7573 0a20 2020  wafer_status.   
-00015630: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015640: 2023 2072 6574 7572 6e20 7365 6c66 2e70   # return self.p
-00015650: 6f73 745f 6974 656d 2874 6162 6c65 2c20  ost_item(table, 
-00015660: 2777 6166 6572 5f73 7461 7475 7327 290a  'wafer_status').
-00015670: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00015680: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00015690: 720a 0a20 2020 2023 2323 2323 2323 2323  r..    #########
+000154d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000154e0: 2d0a 2020 2020 2020 2020 2222 220a 2020  -.        """.  
+000154f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00015500: 662e 706f 7374 5f69 7465 6d28 7461 626c  f.post_item(tabl
+00015510: 652c 2027 7761 6665 7227 290a 0a20 2020  e, 'wafer')..   
+00015520: 2064 6566 2070 6f73 745f 7761 6665 725f   def post_wafer_
+00015530: 6465 6665 6374 7328 7365 6c66 2c20 7461  defects(self, ta
+00015540: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
+00015550: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
+00015560: 6162 6c65 3a20 7761 6665 725f 6465 6665  able: wafer_defe
+00015570: 6374 730a 2020 2020 2020 2020 2222 220a  cts.        """.
+00015580: 2020 2020 2020 2020 2320 7265 7475 726e          # return
+00015590: 2073 656c 662e 706f 7374 5f69 7465 6d28   self.post_item(
+000155a0: 7461 626c 652c 2027 7761 6665 725f 6465  table, 'wafer_de
+000155b0: 6665 6374 7327 290a 2020 2020 2020 2020  fects').        
+000155c0: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+000155d0: 6e74 6564 4572 726f 720a 0a20 2020 2064  ntedError..    d
+000155e0: 6566 2070 6f73 745f 7761 6665 725f 7374  ef post_wafer_st
+000155f0: 6174 7573 2873 656c 662c 2074 6162 6c65  atus(self, table
+00015600: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00015610: 2020 2020 2020 2050 4f53 5420 7461 626c         POST tabl
+00015620: 653a 2077 6166 6572 5f73 7461 7475 730a  e: wafer_status.
+00015630: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015640: 2020 2020 2320 7265 7475 726e 2073 656c      # return sel
+00015650: 662e 706f 7374 5f69 7465 6d28 7461 626c  f.post_item(tabl
+00015660: 652c 2027 7761 6665 725f 7374 6174 7573  e, 'wafer_status
+00015670: 2729 0a20 2020 2020 2020 2072 6169 7365  ').        raise
+00015680: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00015690: 7272 6f72 0a0a 2020 2020 2323 2323 2323  rror..    ######
 000156a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000156b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000156c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000156d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000156e0: 230a 2020 2020 2320 7370 6563 6966 6963  #.    # specific
-000156f0: 2074 6573 7420 7265 7375 6c74 730a 2020   test results.  
-00015700: 2020 230a 2020 2020 2320 5468 6573 6520    #.    # These 
-00015710: 6d65 7468 6f64 7320 6172 6520 7369 6d70  methods are simp
-00015720: 6c79 2077 7261 7070 6572 7320 666f 7220  ly wrappers for 
-00015730: 7468 6520 6765 6e65 7269 6320 706f 7374  the generic post
-00015740: 5f6d 6561 7375 7265 6d65 6e74 2063 616c  _measurement cal
-00015750: 6c2e 0a20 2020 2023 0a20 2020 2023 2054  l..    #.    # T
-00015760: 6865 7920 6172 6520 6f6e 6c79 2064 6566  hey are only def
-00015770: 696e 6564 2074 6f20 6769 7665 2061 6e20  ined to give an 
-00015780: 696e 7465 7261 6374 6976 6520 7573 6572  interactive user
-00015790: 2061 2063 6861 6e63 6520 746f 2067 6574   a chance to get
-000157a0: 2074 6865 0a20 2020 2023 2064 6174 6162   the.    # datab
-000157b0: 6173 6520 7375 626d 6973 7369 6f6e 2072  ase submission r
-000157c0: 6967 6874 2062 7920 7265 6665 7272 696e  ight by referrin
-000157d0: 6720 746f 2074 6865 206d 6574 686f 6420  g to the method 
-000157e0: 646f 6375 6d65 6e74 6174 696f 6e0a 2020  documentation.  
-000157f0: 2020 2320 7573 696e 6720 7468 6520 5079    # using the Py
-00015800: 7468 6f6e 2069 6e74 6572 7072 6574 6572  thon interpreter
-00015810: 2773 2027 6865 6c70 2829 2720 636f 6d6d  's 'help()' comm
-00015820: 616e 642e 0a20 2020 2023 0a0a 2020 2020  and..    #..    
-00015830: 6465 6620 706f 7374 5f64 756d 6d79 6c6f  def post_dummylo
-00015840: 6164 5f74 6573 7428 7365 6c66 2c20 7461  ad_test(self, ta
-00015850: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
-00015860: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
-00015870: 6162 6c65 3a20 6475 6d6d 796c 6f61 645f  able: dummyload_
-00015880: 7465 7374 0a20 2020 2020 2020 2022 2222  test.        """
-00015890: 0a20 2020 2020 2020 2023 2072 6574 7572  .        # retur
-000158a0: 6e20 7365 6c66 2e70 6f73 745f 6d65 6173  n self.post_meas
-000158b0: 7572 656d 656e 7428 7461 626c 652c 2027  urement(table, '
-000158c0: 6475 6d6d 796c 6f61 645f 7465 7374 2729  dummyload_test')
-000158d0: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-000158e0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-000158f0: 6f72 0a0a 2020 2020 6465 6620 706f 7374  or..    def post
-00015900: 5f70 6475 5f70 756c 7365 5f74 6573 7428  _pdu_pulse_test(
-00015910: 7365 6c66 2c20 7461 626c 6529 3a0a 2020  self, table):.  
-00015920: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00015930: 2020 504f 5354 2074 6162 6c65 3a20 7064    POST table: pd
-00015940: 755f 7075 6c73 655f 7465 7374 0a20 2020  u_pulse_test.   
-00015950: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015960: 2023 2072 6574 7572 6e20 7365 6c66 2e70   # return self.p
-00015970: 6f73 745f 6d65 6173 7572 656d 656e 7428  ost_measurement(
-00015980: 7461 626c 652c 2027 7064 755f 7075 6c73  table, 'pdu_puls
-00015990: 655f 7465 7374 2729 0a20 2020 2020 2020  e_test').       
-000159a0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-000159b0: 656e 7465 6445 7272 6f72 0a0a 2020 2020  entedError..    
-000159c0: 6465 6620 706f 7374 5f74 696c 655f 636f  def post_tile_co
-000159d0: 6c64 5f74 6573 7428 7365 6c66 2c20 7461  ld_test(self, ta
-000159e0: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
-000159f0: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
-00015a00: 6162 6c65 3a20 7469 6c65 5f63 6f6c 645f  able: tile_cold_
-00015a10: 7465 7374 0a20 2020 2020 2020 2022 2222  test.        """
-00015a20: 0a20 2020 2020 2020 2023 2072 6574 7572  .        # retur
-00015a30: 6e20 7365 6c66 2e70 6f73 745f 6d65 6173  n self.post_meas
-00015a40: 7572 656d 656e 7428 7461 626c 652c 2027  urement(table, '
-00015a50: 7469 6c65 5f63 6f6c 645f 7465 7374 2729  tile_cold_test')
-00015a60: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-00015a70: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00015a80: 6f72 0a0a 2020 2020 6465 6620 706f 7374  or..    def post
-00015a90: 5f74 696c 655f 7761 726d 5f74 6573 7428  _tile_warm_test(
-00015aa0: 7365 6c66 2c20 7461 626c 6529 3a0a 2020  self, table):.  
-00015ab0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00015ac0: 2020 504f 5354 2074 6162 6c65 3a20 7469    POST table: ti
-00015ad0: 6c65 5f77 6172 6d5f 7465 7374 0a20 2020  le_warm_test.   
-00015ae0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015af0: 2023 2072 6574 7572 6e20 7365 6c66 2e70   # return self.p
-00015b00: 6f73 745f 6d65 6173 7572 656d 656e 7428  ost_measurement(
-00015b10: 7461 626c 652c 2027 7469 6c65 5f77 6172  table, 'tile_war
-00015b20: 6d5f 7465 7374 2729 0a20 2020 2020 2020  m_test').       
-00015b30: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-00015b40: 656e 7465 6445 7272 6f72 0a0a 2020 2020  entedError..    
-00015b50: 6465 6620 706f 7374 5f75 7365 725f 7465  def post_user_te
-00015b60: 7374 2873 656c 662c 2074 6162 6c65 293a  st(self, table):
-00015b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015b80: 2020 2020 2050 4f53 5420 7461 626c 653a       POST table:
-00015b90: 2075 7365 725f 7465 7374 0a20 2020 2020   user_test.     
-00015ba0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00015bb0: 2072 6574 7572 6e20 7365 6c66 2e70 6f73   return self.pos
-00015bc0: 745f 6d65 6173 7572 656d 656e 7428 7461  t_measurement(ta
-00015bd0: 626c 652c 2027 7573 6572 5f74 6573 7427  ble, 'user_test'
-00015be0: 290a 2020 2020 2020 2020 7261 6973 6520  ).        raise 
-00015bf0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-00015c00: 726f 720a 0a20 2020 2064 6566 2070 6f73  ror..    def pos
-00015c10: 745f 7661 7369 635f 7465 7374 2873 656c  t_vasic_test(sel
-00015c20: 662c 2074 6162 6c65 293a 0a20 2020 2020  f, table):.     
-00015c30: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-00015c40: 4f53 5420 7461 626c 653a 2076 6173 6963  OST table: vasic
-00015c50: 5f74 6573 740a 2020 2020 2020 2020 2222  _test.        ""
-00015c60: 220a 2020 2020 2020 2020 2320 7265 7475  ".        # retu
-00015c70: 726e 2073 656c 662e 706f 7374 5f6d 6561  rn self.post_mea
-00015c80: 7375 7265 6d65 6e74 2874 6162 6c65 2c20  surement(table, 
-00015c90: 2776 6173 6963 5f74 6573 7427 290a 2020  'vasic_test').  
-00015ca0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-00015cb0: 6d70 6c65 6d65 6e74 6564 4572 726f 720a  mplementedError.
-00015cc0: 0a20 2020 2064 6566 2070 6f73 745f 7369  .    def post_si
-00015cd0: 706d 5f74 6573 7428 7365 6c66 2c20 7461  pm_test(self, ta
-00015ce0: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
-00015cf0: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
-00015d00: 6162 6c65 3a20 7369 706d 5f74 6573 740a  able: sipm_test.
-00015d10: 0a20 2020 2020 2020 2041 6464 2061 2074  .        Add a t
-00015d20: 6573 7420 7265 7375 6c74 2066 6f72 2061  est result for a
-00015d30: 2053 6950 4d20 7468 6174 2065 7869 7374   SiPM that exist
-00015d40: 7320 696e 2074 6865 2064 6174 6162 6173  s in the databas
-00015d50: 652e 0a0a 2020 2020 2020 2020 2d2d 2d2d  e...        ----
+000156e0: 2323 2323 0a20 2020 2023 2073 7065 6369  ####.    # speci
+000156f0: 6669 6320 7465 7374 2072 6573 756c 7473  fic test results
+00015700: 0a20 2020 2023 0a20 2020 2023 2054 6865  .    #.    # The
+00015710: 7365 206d 6574 686f 6473 2061 7265 2073  se methods are s
+00015720: 696d 706c 7920 7772 6170 7065 7273 2066  imply wrappers f
+00015730: 6f72 2074 6865 2067 656e 6572 6963 2070  or the generic p
+00015740: 6f73 745f 6d65 6173 7572 656d 656e 7420  ost_measurement 
+00015750: 6361 6c6c 2e0a 2020 2020 230a 2020 2020  call..    #.    
+00015760: 2320 5468 6579 2061 7265 206f 6e6c 7920  # They are only 
+00015770: 6465 6669 6e65 6420 746f 2067 6976 6520  defined to give 
+00015780: 616e 2069 6e74 6572 6163 7469 7665 2075  an interactive u
+00015790: 7365 7220 6120 6368 616e 6365 2074 6f20  ser a chance to 
+000157a0: 6765 7420 7468 650a 2020 2020 2320 6461  get the.    # da
+000157b0: 7461 6261 7365 2073 7562 6d69 7373 696f  tabase submissio
+000157c0: 6e20 7269 6768 7420 6279 2072 6566 6572  n right by refer
+000157d0: 7269 6e67 2074 6f20 7468 6520 6d65 7468  ring to the meth
+000157e0: 6f64 2064 6f63 756d 656e 7461 7469 6f6e  od documentation
+000157f0: 0a20 2020 2023 2075 7369 6e67 2074 6865  .    # using the
+00015800: 2050 7974 686f 6e20 696e 7465 7270 7265   Python interpre
+00015810: 7465 7227 7320 2768 656c 7028 2927 2063  ter's 'help()' c
+00015820: 6f6d 6d61 6e64 2e0a 2020 2020 230a 0a20  ommand..    #.. 
+00015830: 2020 2064 6566 2070 6f73 745f 6475 6d6d     def post_dumm
+00015840: 796c 6f61 645f 7465 7374 2873 656c 662c  yload_test(self,
+00015850: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
+00015860: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
+00015870: 5420 7461 626c 653a 2064 756d 6d79 6c6f  T table: dummylo
+00015880: 6164 5f74 6573 740a 2020 2020 2020 2020  ad_test.        
+00015890: 2222 220a 2020 2020 2020 2020 2320 7265  """.        # re
+000158a0: 7475 726e 2073 656c 662e 706f 7374 5f6d  turn self.post_m
+000158b0: 6561 7375 7265 6d65 6e74 2874 6162 6c65  easurement(table
+000158c0: 2c20 2764 756d 6d79 6c6f 6164 5f74 6573  , 'dummyload_tes
+000158d0: 7427 290a 2020 2020 2020 2020 7261 6973  t').        rais
+000158e0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+000158f0: 4572 726f 720a 0a20 2020 2064 6566 2070  Error..    def p
+00015900: 6f73 745f 7064 755f 7075 6c73 655f 7465  ost_pdu_pulse_te
+00015910: 7374 2873 656c 662c 2074 6162 6c65 293a  st(self, table):
+00015920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015930: 2020 2020 2050 4f53 5420 7461 626c 653a       POST table:
+00015940: 2070 6475 5f70 756c 7365 5f74 6573 740a   pdu_pulse_test.
+00015950: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015960: 2020 2020 2320 7265 7475 726e 2073 656c      # return sel
+00015970: 662e 706f 7374 5f6d 6561 7375 7265 6d65  f.post_measureme
+00015980: 6e74 2874 6162 6c65 2c20 2770 6475 5f70  nt(table, 'pdu_p
+00015990: 756c 7365 5f74 6573 7427 290a 2020 2020  ulse_test').    
+000159a0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+000159b0: 6c65 6d65 6e74 6564 4572 726f 720a 0a20  lementedError.. 
+000159c0: 2020 2064 6566 2070 6f73 745f 7469 6c65     def post_tile
+000159d0: 5f63 6f6c 645f 7465 7374 2873 656c 662c  _cold_test(self,
+000159e0: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
+000159f0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
+00015a00: 5420 7461 626c 653a 2074 696c 655f 636f  T table: tile_co
+00015a10: 6c64 5f74 6573 740a 2020 2020 2020 2020  ld_test.        
+00015a20: 2222 220a 2020 2020 2020 2020 2320 7265  """.        # re
+00015a30: 7475 726e 2073 656c 662e 706f 7374 5f6d  turn self.post_m
+00015a40: 6561 7375 7265 6d65 6e74 2874 6162 6c65  easurement(table
+00015a50: 2c20 2774 696c 655f 636f 6c64 5f74 6573  , 'tile_cold_tes
+00015a60: 7427 290a 2020 2020 2020 2020 7261 6973  t').        rais
+00015a70: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00015a80: 4572 726f 720a 0a20 2020 2064 6566 2070  Error..    def p
+00015a90: 6f73 745f 7469 6c65 5f77 6172 6d5f 7465  ost_tile_warm_te
+00015aa0: 7374 2873 656c 662c 2074 6162 6c65 293a  st(self, table):
+00015ab0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015ac0: 2020 2020 2050 4f53 5420 7461 626c 653a       POST table:
+00015ad0: 2074 696c 655f 7761 726d 5f74 6573 740a   tile_warm_test.
+00015ae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00015af0: 2020 2020 2320 7265 7475 726e 2073 656c      # return sel
+00015b00: 662e 706f 7374 5f6d 6561 7375 7265 6d65  f.post_measureme
+00015b10: 6e74 2874 6162 6c65 2c20 2774 696c 655f  nt(table, 'tile_
+00015b20: 7761 726d 5f74 6573 7427 290a 2020 2020  warm_test').    
+00015b30: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00015b40: 6c65 6d65 6e74 6564 4572 726f 720a 0a20  lementedError.. 
+00015b50: 2020 2064 6566 2070 6f73 745f 7573 6572     def post_user
+00015b60: 5f74 6573 7428 7365 6c66 2c20 7461 626c  _test(self, tabl
+00015b70: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00015b80: 2020 2020 2020 2020 504f 5354 2074 6162          POST tab
+00015b90: 6c65 3a20 7573 6572 5f74 6573 740a 2020  le: user_test.  
+00015ba0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015bb0: 2020 2320 7265 7475 726e 2073 656c 662e    # return self.
+00015bc0: 706f 7374 5f6d 6561 7375 7265 6d65 6e74  post_measurement
+00015bd0: 2874 6162 6c65 2c20 2775 7365 725f 7465  (table, 'user_te
+00015be0: 7374 2729 0a20 2020 2020 2020 2072 6169  st').        rai
+00015bf0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+00015c00: 6445 7272 6f72 0a0a 2020 2020 6465 6620  dError..    def 
+00015c10: 706f 7374 5f76 6173 6963 5f74 6573 7428  post_vasic_test(
+00015c20: 7365 6c66 2c20 7461 626c 6529 3a0a 2020  self, table):.  
+00015c30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015c40: 2020 504f 5354 2074 6162 6c65 3a20 7661    POST table: va
+00015c50: 7369 635f 7465 7374 0a20 2020 2020 2020  sic_test.       
+00015c60: 2022 2222 0a20 2020 2020 2020 2023 2072   """.        # r
+00015c70: 6574 7572 6e20 7365 6c66 2e70 6f73 745f  eturn self.post_
+00015c80: 6d65 6173 7572 656d 656e 7428 7461 626c  measurement(tabl
+00015c90: 652c 2027 7661 7369 635f 7465 7374 2729  e, 'vasic_test')
+00015ca0: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
+00015cb0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+00015cc0: 6f72 0a0a 2020 2020 6465 6620 706f 7374  or..    def post
+00015cd0: 5f73 6970 6d5f 7465 7374 2873 656c 662c  _sipm_test(self,
+00015ce0: 2074 6162 6c65 293a 0a20 2020 2020 2020   table):.       
+00015cf0: 2022 2222 0a20 2020 2020 2020 2050 4f53   """.        POS
+00015d00: 5420 7461 626c 653a 2073 6970 6d5f 7465  T table: sipm_te
+00015d10: 7374 0a0a 2020 2020 2020 2020 4164 6420  st..        Add 
+00015d20: 6120 7465 7374 2072 6573 756c 7420 666f  a test result fo
+00015d30: 7220 6120 5369 504d 2074 6861 7420 6578  r a SiPM that ex
+00015d40: 6973 7473 2069 6e20 7468 6520 6461 7461  ists in the data
+00015d50: 6261 7365 2e0a 0a20 2020 2020 2020 202d  base...        -
 00015d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00015da0: 2d2d 0a20 2020 2020 2020 2061 7267 730a  --.        args.
-00015db0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
-00015dc0: 6520 3a20 6469 6374 0a20 2020 2020 2020  e : dict.       
-00015dd0: 2020 2020 2020 2020 2065 2e67 2e0a 2020           e.g..  
-00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015df0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00015e00: 2020 2020 2020 2020 2020 2020 2774 696d              'tim
-00015e10: 6573 7461 6d70 273a 2027 3230 3232 2d30  estamp': '2022-0
-00015e20: 392d 3036 2031 353a 3330 3a31 3427 2c0a  9-06 15:30:14',.
-00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e40: 2020 2020 2020 2020 2320 696e 6974 6961          # initia
-00015e50: 6c73 206f 6620 7065 7273 6f6e 2061 6464  ls of person add
-00015e60: 696e 6720 7468 6973 2074 6573 7420 7265  ing this test re
-00015e70: 7375 6c74 0a20 2020 2020 2020 2020 2020  sult.           
-00015e80: 2020 2020 2020 2020 2020 2020 2027 6f70               'op
-00015e90: 6572 6174 6f72 273a 2027 6170 272c 0a20  erator': 'ap',. 
-00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015eb0: 2020 2020 2020 2027 7369 706d 5f69 6427         'sipm_id'
-00015ec0: 3a20 3133 372c 0a20 2020 2020 2020 2020  : 137,.         
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00015ee0: 2031 3d70 6173 732c 2030 3d66 6169 6c0a   1=pass, 0=fail.
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f00: 2020 2020 2020 2020 2767 6f6f 6427 3a20          'good': 
-00015f10: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00015f20: 2020 2020 2020 2020 2020 2027 636f 6d6d             'comm
-00015f30: 656e 7427 3a20 2767 6f6f 642f 6261 6420  ent': 'good/bad 
-00015f40: 7374 6174 7573 2062 6173 6564 2073 6f6c  status based sol
-00015f50: 656c 7920 6f6e 2077 6166 6572 2e2e 2e27  ely on wafer...'
-00015f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015f70: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00015f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00015da0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6172  -----.        ar
+00015db0: 6773 0a20 2020 2020 2020 2020 2020 2074  gs.            t
+00015dc0: 6162 6c65 203a 2064 6963 740a 2020 2020  able : dict.    
+00015dd0: 2020 2020 2020 2020 2020 2020 652e 672e              e.g.
+00015de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015df0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00015e00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00015e10: 7469 6d65 7374 616d 7027 3a20 2732 3032  timestamp': '202
+00015e20: 322d 3039 2d30 3620 3135 3a33 303a 3134  2-09-06 15:30:14
+00015e30: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00015e40: 2020 2020 2020 2020 2020 2023 2069 6e69             # ini
+00015e50: 7469 616c 7320 6f66 2070 6572 736f 6e20  tials of person 
+00015e60: 6164 6469 6e67 2074 6869 7320 7465 7374  adding this test
+00015e70: 2072 6573 756c 740a 2020 2020 2020 2020   result.        
+00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e90: 276f 7065 7261 746f 7227 3a20 2761 7027  'operator': 'ap'
+00015ea0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015eb0: 2020 2020 2020 2020 2020 2773 6970 6d5f            'sipm_
+00015ec0: 6964 273a 2031 3337 2c0a 2020 2020 2020  id': 137,.      
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ee0: 2020 2320 313d 7061 7373 2c20 303d 6661    # 1=pass, 0=fa
+00015ef0: 696c 0a20 2020 2020 2020 2020 2020 2020  il.             
+00015f00: 2020 2020 2020 2020 2020 2027 676f 6f64             'good
+00015f10: 273a 2031 2c0a 2020 2020 2020 2020 2020  ': 1,.          
+00015f20: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00015f30: 6f6d 6d65 6e74 273a 2027 676f 6f64 2f62  omment': 'good/b
+00015f40: 6164 2073 7461 7475 7320 6261 7365 6420  ad status based 
+00015f50: 736f 6c65 6c79 206f 6e20 7761 6665 722e  solely on wafer.
+00015f60: 2e2e 272c 0a20 2020 2020 2020 2020 2020  ..',.           
+00015f70: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00015f80: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 00015f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00015fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00015fc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2072  ------.        r
-00015fd0: 6574 7572 6e73 203a 2062 6f6f 6c0a 2020  eturns : bool.  
-00015fe0: 2020 2020 2020 2020 2020 5375 6363 6573            Succes
-00015ff0: 7320 6f66 2050 4f53 5420 6f70 6572 6174  s of POST operat
-00016000: 696f 6e2e 0a20 2020 2020 2020 202d 2d2d  ion..        ---
+00015fc0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00015fd0: 2020 7265 7475 726e 7320 3a20 626f 6f6c    returns : bool
+00015fe0: 0a20 2020 2020 2020 2020 2020 2053 7563  .            Suc
+00015ff0: 6365 7373 206f 6620 504f 5354 206f 7065  cess of POST ope
+00016000: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
 00016010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016050: 2d2d 2d0a 2020 2020 2020 2020 2222 220a  ---.        """.
-00016060: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00016070: 656c 662e 706f 7374 5f6d 6561 7375 7265  elf.post_measure
-00016080: 6d65 6e74 2874 6162 6c65 2c20 2773 6970  ment(table, 'sip
-00016090: 6d27 290a 0a20 2020 2064 6566 2070 6f73  m')..    def pos
-000160a0: 745f 7670 6362 5f61 7369 635f 7465 7374  t_vpcb_asic_test
-000160b0: 2873 656c 662c 2074 6162 6c65 293a 0a20  (self, table):. 
-000160c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000160d0: 2020 2050 4f53 5420 7461 626c 653a 2076     POST table: v
-000160e0: 7063 625f 6173 6963 5f74 6573 740a 0a20  pcb_asic_test.. 
-000160f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00016050: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2022  ------.        "
+00016060: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00016070: 6e20 7365 6c66 2e70 6f73 745f 6d65 6173  n self.post_meas
+00016080: 7572 656d 656e 7428 7461 626c 652c 2027  urement(table, '
+00016090: 7369 706d 2729 0a0a 2020 2020 6465 6620  sipm')..    def 
+000160a0: 706f 7374 5f76 7063 625f 6173 6963 5f74  post_vpcb_asic_t
+000160b0: 6573 7428 7365 6c66 2c20 7461 626c 6529  est(self, table)
+000160c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000160d0: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
+000160e0: 3a20 7670 6362 5f61 7369 635f 7465 7374  : vpcb_asic_test
+000160f0: 0a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
 00016100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00016140: 2020 2020 2020 6172 6773 0a20 2020 2020        args.     
-00016150: 2020 2020 2020 2074 6162 6c65 203a 2064         table : d
-00016160: 6963 740a 2020 2020 2020 2020 2d2d 2d2d  ict.        ----
+00016130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016140: 0a20 2020 2020 2020 2061 7267 730a 2020  .        args.  
+00016150: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00016160: 3a20 6469 6374 0a20 2020 2020 2020 202d  : dict.        -
 00016170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000161a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000161b0: 2d2d 0a20 2020 2020 2020 2072 6574 7572  --.        retur
-000161c0: 6e73 203a 2062 6f6f 6c0a 2020 2020 2020  ns : bool.      
-000161d0: 2020 2020 2020 5375 6363 6573 7320 6f66        Success of
-000161e0: 2050 4f53 5420 6f70 6572 6174 696f 6e2e   POST operation.
-000161f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000161b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
+000161c0: 7475 726e 7320 3a20 626f 6f6c 0a20 2020  turns : bool.   
+000161d0: 2020 2020 2020 2020 2053 7563 6365 7373           Success
+000161e0: 206f 6620 504f 5354 206f 7065 7261 7469   of POST operati
+000161f0: 6f6e 2e0a 2020 2020 2020 2020 2d2d 2d2d  on..        ----
 00016200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00016240: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016250: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00016260: 706f 7374 5f6d 6561 7375 7265 6d65 6e74  post_measurement
-00016270: 2874 6162 6c65 2c20 2776 7063 625f 6173  (table, 'vpcb_as
-00016280: 6963 2729 0a0a 2020 2020 6465 6620 706f  ic')..    def po
-00016290: 7374 5f76 7063 625f 7465 7374 2873 656c  st_vpcb_test(sel
-000162a0: 662c 2074 6162 6c65 293a 0a20 2020 2020  f, table):.     
-000162b0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
-000162c0: 4f53 5420 7461 626c 653a 2076 7063 625f  OST table: vpcb_
-000162d0: 7465 7374 0a0a 2020 2020 2020 2020 2d2d  test..        --
-000162e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016240: 2d2d 0a20 2020 2020 2020 2022 2222 0a20  --.        """. 
+00016250: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00016260: 6c66 2e70 6f73 745f 6d65 6173 7572 656d  lf.post_measurem
+00016270: 656e 7428 7461 626c 652c 2027 7670 6362  ent(table, 'vpcb
+00016280: 5f61 7369 6327 290a 0a20 2020 2064 6566  _asic')..    def
+00016290: 2070 6f73 745f 7670 6362 5f74 6573 7428   post_vpcb_test(
+000162a0: 7365 6c66 2c20 7461 626c 6529 3a0a 2020  self, table):.  
+000162b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000162c0: 2020 504f 5354 2074 6162 6c65 3a20 7670    POST table: vp
+000162d0: 6362 5f74 6573 740a 0a20 2020 2020 2020  cb_test..       
+000162e0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 000162f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016320: 2d2d 2d2d 0a20 2020 2020 2020 2061 7267  ----.        arg
-00016330: 730a 2020 2020 2020 2020 2020 2020 7461  s.            ta
-00016340: 626c 6520 3a20 6469 6374 0a20 2020 2020  ble : dict.     
-00016350: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00016320: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016330: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
+00016340: 2074 6162 6c65 203a 2064 6963 740a 2020   table : dict.  
+00016350: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
 00016360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016390: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000163a0: 2020 7265 7475 726e 7320 3a20 626f 6f6c    returns : bool
-000163b0: 0a20 2020 2020 2020 2020 2020 2053 7563  .            Suc
-000163c0: 6365 7373 206f 6620 504f 5354 206f 7065  cess of POST ope
-000163d0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
-000163e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000163a0: 2020 2020 2072 6574 7572 6e73 203a 2062       returns : b
+000163b0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
+000163c0: 5375 6363 6573 7320 6f66 2050 4f53 5420  Success of POST 
+000163d0: 6f70 6572 6174 696f 6e2e 0a20 2020 2020  operation..     
+000163e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
 000163f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016420: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2022  ------.        "
-00016430: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00016440: 6e20 7365 6c66 2e70 6f73 745f 6d65 6173  n self.post_meas
-00016450: 7572 656d 656e 7428 7461 626c 652c 2027  urement(table, '
-00016460: 7670 6362 2729 0a0a 2020 2020 6465 6620  vpcb')..    def 
-00016470: 706f 7374 5f76 7064 755f 636f 6c64 5f74  post_vpdu_cold_t
-00016480: 6573 7428 7365 6c66 2c20 7461 626c 6529  est(self, table)
-00016490: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000164a0: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-000164b0: 3a20 7670 6475 5f63 6f6c 645f 7465 7374  : vpdu_cold_test
-000164c0: 0a0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00016420: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00016430: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00016440: 7475 726e 2073 656c 662e 706f 7374 5f6d  turn self.post_m
+00016450: 6561 7375 7265 6d65 6e74 2874 6162 6c65  easurement(table
+00016460: 2c20 2776 7063 6227 290a 0a20 2020 2064  , 'vpcb')..    d
+00016470: 6566 2070 6f73 745f 7670 6475 5f63 6f6c  ef post_vpdu_col
+00016480: 645f 7465 7374 2873 656c 662c 2074 6162  d_test(self, tab
+00016490: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+000164a0: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+000164b0: 626c 653a 2076 7064 755f 636f 6c64 5f74  ble: vpdu_cold_t
+000164c0: 6573 740a 0a20 2020 2020 2020 202d 2d2d  est..        ---
 000164d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000164e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000164f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016510: 0a20 2020 2020 2020 2061 7267 730a 2020  .        args.  
-00016520: 2020 2020 2020 2020 2020 7461 626c 6520            table 
-00016530: 3a20 6469 6374 0a20 2020 2020 2020 202d  : dict.        -
-00016540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016510: 2d2d 2d0a 2020 2020 2020 2020 6172 6773  ---.        args
+00016520: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
+00016530: 6c65 203a 2064 6963 740a 2020 2020 2020  le : dict.      
+00016540: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
 00016550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016580: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7265  -----.        re
-00016590: 7475 726e 7320 3a20 626f 6f6c 0a20 2020  turns : bool.   
-000165a0: 2020 2020 2020 2020 2053 7563 6365 7373           Success
-000165b0: 206f 6620 504f 5354 206f 7065 7261 7469   of POST operati
-000165c0: 6f6e 2e0a 2020 2020 2020 2020 2d2d 2d2d  on..        ----
+00016580: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00016590: 2072 6574 7572 6e73 203a 2062 6f6f 6c0a   returns : bool.
+000165a0: 2020 2020 2020 2020 2020 2020 5375 6363              Succ
+000165b0: 6573 7320 6f66 2050 4f53 5420 6f70 6572  ess of POST oper
+000165c0: 6174 696f 6e2e 0a20 2020 2020 2020 202d  ation..        -
 000165d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000165e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000165f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016610: 2d2d 0a20 2020 2020 2020 2022 2222 0a20  --.        """. 
-00016620: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00016630: 6c66 2e70 6f73 745f 6d65 6173 7572 656d  lf.post_measurem
-00016640: 656e 7428 7461 626c 652c 2027 7670 6475  ent(table, 'vpdu
-00016650: 5f63 6f6c 645f 7465 7374 2729 0a0a 2020  _cold_test')..  
-00016660: 2020 6465 6620 706f 7374 5f76 7064 755f    def post_vpdu_
-00016670: 7465 7374 2873 656c 662c 2074 6162 6c65  test(self, table
-00016680: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00016690: 2020 2020 2020 2050 4f53 5420 7461 626c         POST tabl
-000166a0: 653a 2076 7064 755f 7465 7374 0a0a 2020  e: vpdu_test..  
-000166b0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00016610: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
+00016620: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00016630: 2073 656c 662e 706f 7374 5f6d 6561 7375   self.post_measu
+00016640: 7265 6d65 6e74 2874 6162 6c65 2c20 2776  rement(table, 'v
+00016650: 7064 755f 636f 6c64 5f74 6573 7427 290a  pdu_cold_test').
+00016660: 0a20 2020 2064 6566 2070 6f73 745f 7670  .    def post_vp
+00016670: 6475 5f74 6573 7428 7365 6c66 2c20 7461  du_test(self, ta
+00016680: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
+00016690: 220a 2020 2020 2020 2020 504f 5354 2074  ".        POST t
+000166a0: 6162 6c65 3a20 7670 6475 5f74 6573 740a  able: vpdu_test.
+000166b0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
 000166c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000166d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000166e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000166f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00016700: 2020 2020 2061 7267 730a 2020 2020 2020       args.      
-00016710: 2020 2020 2020 7461 626c 6520 3a20 6469        table : di
-00016720: 6374 0a20 2020 2020 2020 202d 2d2d 2d2d  ct.        -----
+000166f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00016700: 2020 2020 2020 2020 6172 6773 0a20 2020          args.   
+00016710: 2020 2020 2020 2020 2074 6162 6c65 203a           table :
+00016720: 2064 6963 740a 2020 2020 2020 2020 2d2d   dict.        --
 00016730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016770: 2d0a 2020 2020 2020 2020 7265 7475 726e  -.        return
-00016780: 7320 3a20 626f 6f6c 0a20 2020 2020 2020  s : bool.       
-00016790: 2020 2020 2053 7563 6365 7373 206f 6620       Success of 
-000167a0: 504f 5354 206f 7065 7261 7469 6f6e 2e0a  POST operation..
-000167b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00016770: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
+00016780: 7572 6e73 203a 2062 6f6f 6c0a 2020 2020  urns : bool.    
+00016790: 2020 2020 2020 2020 5375 6363 6573 7320          Success 
+000167a0: 6f66 2050 4f53 5420 6f70 6572 6174 696f  of POST operatio
+000167b0: 6e2e 0a20 2020 2020 2020 202d 2d2d 2d2d  n..        -----
 000167c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000167d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000167e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000167f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00016800: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016810: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-00016820: 6f73 745f 6d65 6173 7572 656d 656e 7428  ost_measurement(
-00016830: 7461 626c 652c 2027 7670 6475 5f74 6573  table, 'vpdu_tes
-00016840: 7427 290a 0a20 2020 2064 6566 2070 6f73  t')..    def pos
-00016850: 745f 766d 6f74 6865 7262 6f61 7264 5f74  t_vmotherboard_t
-00016860: 6573 7428 7365 6c66 2c20 7461 626c 6529  est(self, table)
-00016870: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00016880: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
-00016890: 3a20 766d 6f74 6865 7262 6f61 7264 5f74  : vmotherboard_t
-000168a0: 6573 740a 0a20 2020 2020 2020 202d 2d2d  est..        ---
+000167f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016800: 2d0a 2020 2020 2020 2020 2222 220a 2020  -.        """.  
+00016810: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00016820: 662e 706f 7374 5f6d 6561 7375 7265 6d65  f.post_measureme
+00016830: 6e74 2874 6162 6c65 2c20 2776 7064 755f  nt(table, 'vpdu_
+00016840: 7465 7374 2729 0a0a 2020 2020 6465 6620  test')..    def 
+00016850: 706f 7374 5f76 6d6f 7468 6572 626f 6172  post_vmotherboar
+00016860: 645f 7465 7374 2873 656c 662c 2074 6162  d_test(self, tab
+00016870: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
+00016880: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
+00016890: 626c 653a 2076 6d6f 7468 6572 626f 6172  ble: vmotherboar
+000168a0: 645f 7465 7374 0a0a 2020 2020 2020 2020  d_test..        
 000168b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000168c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000168d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000168e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000168f0: 2d2d 2d0a 2020 2020 2020 2020 6172 6773  ---.        args
-00016900: 0a20 2020 2020 2020 2020 2020 2074 6162  .            tab
-00016910: 6c65 203a 2064 6963 740a 2020 2020 2020  le : dict.      
-00016920: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000168f0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2061  ------.        a
+00016900: 7267 730a 2020 2020 2020 2020 2020 2020  rgs.            
+00016910: 7461 626c 6520 3a20 6469 6374 0a20 2020  table : dict.   
+00016920: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
 00016930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016960: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00016970: 2072 6574 7572 6e73 203a 2062 6f6f 6c0a   returns : bool.
-00016980: 2020 2020 2020 2020 2020 2020 5375 6363              Succ
-00016990: 6573 7320 6f66 2050 4f53 5420 6f70 6572  ess of POST oper
-000169a0: 6174 696f 6e2e 0a20 2020 2020 2020 202d  ation..        -
-000169b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00016970: 2020 2020 7265 7475 726e 7320 3a20 626f      returns : bo
+00016980: 6f6c 0a20 2020 2020 2020 2020 2020 2053  ol.            S
+00016990: 7563 6365 7373 206f 6620 504f 5354 206f  uccess of POST o
+000169a0: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
+000169b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
 000169c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000169d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000169e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000169f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2222  -----.        ""
-00016a00: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00016a10: 2073 656c 662e 706f 7374 5f6d 6561 7375   self.post_measu
-00016a20: 7265 6d65 6e74 2874 6162 6c65 2c20 2776  rement(table, 'v
-00016a30: 6d6f 7468 6572 626f 6172 6427 290a 0a20  motherboard').. 
-00016a40: 2020 2064 6566 2070 6f73 745f 7674 696c     def post_vtil
-00016a50: 655f 7465 7374 2873 656c 662c 2074 6162  e_test(self, tab
-00016a60: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
-00016a70: 0a20 2020 2020 2020 2050 4f53 5420 7461  .        POST ta
-00016a80: 626c 653a 2076 7469 6c65 5f74 6573 740a  ble: vtile_test.
-00016a90: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+000169f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00016a00: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00016a10: 7572 6e20 7365 6c66 2e70 6f73 745f 6d65  urn self.post_me
+00016a20: 6173 7572 656d 656e 7428 7461 626c 652c  asurement(table,
+00016a30: 2027 766d 6f74 6865 7262 6f61 7264 2729   'vmotherboard')
+00016a40: 0a0a 2020 2020 6465 6620 706f 7374 5f76  ..    def post_v
+00016a50: 7469 6c65 5f74 6573 7428 7365 6c66 2c20  tile_test(self, 
+00016a60: 7461 626c 6529 3a0a 2020 2020 2020 2020  table):.        
+00016a70: 2222 220a 2020 2020 2020 2020 504f 5354  """.        POST
+00016a80: 2074 6162 6c65 3a20 7674 696c 655f 7465   table: vtile_te
+00016a90: 7374 0a0a 2020 2020 2020 2020 2d2d 2d2d  st..        ----
 00016aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00016ae0: 2020 2020 2020 2020 6172 6773 0a20 2020          args.   
-00016af0: 2020 2020 2020 2020 2074 6162 6c65 203a           table :
-00016b00: 2064 6963 740a 2020 2020 2020 2020 2d2d   dict.        --
-00016b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016ae0: 2d2d 0a20 2020 2020 2020 2061 7267 730a  --.        args.
+00016af0: 2020 2020 2020 2020 2020 2020 7461 626c              tabl
+00016b00: 6520 3a20 6469 6374 0a20 2020 2020 2020  e : dict.       
+00016b10: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
 00016b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016b50: 2d2d 2d2d 0a20 2020 2020 2020 2072 6574  ----.        ret
-00016b60: 7572 6e73 203a 2062 6f6f 6c0a 2020 2020  urns : bool.    
-00016b70: 2020 2020 2020 2020 5375 6363 6573 7320          Success 
-00016b80: 6f66 2050 4f53 5420 6f70 6572 6174 696f  of POST operatio
-00016b90: 6e2e 0a20 2020 2020 2020 202d 2d2d 2d2d  n..        -----
+00016b50: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00016b60: 7265 7475 726e 7320 3a20 626f 6f6c 0a20  returns : bool. 
+00016b70: 2020 2020 2020 2020 2020 2053 7563 6365             Succe
+00016b80: 7373 206f 6620 504f 5354 206f 7065 7261  ss of POST opera
+00016b90: 7469 6f6e 2e0a 2020 2020 2020 2020 2d2d  tion..        --
 00016ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00016bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016be0: 2d0a 2020 2020 2020 2020 2222 220a 2020  -.        """.  
-00016bf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00016c00: 662e 706f 7374 5f6d 6561 7375 7265 6d65  f.post_measureme
-00016c10: 6e74 2874 6162 6c65 2c20 2776 7469 6c65  nt(table, 'vtile
-00016c20: 2729 0a0a 2020 2020 6465 6620 706f 7374  ')..    def post
-00016c30: 5f76 7469 6c65 5f63 6f6c 645f 7465 7374  _vtile_cold_test
-00016c40: 2873 656c 662c 2074 6162 6c65 293a 0a20  (self, table):. 
-00016c50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016c60: 2020 2050 4f53 5420 7461 626c 653a 2076     POST table: v
-00016c70: 7469 6c65 5f63 6f6c 645f 7465 7374 0a20  tile_cold_test. 
-00016c80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016c90: 2020 2023 2072 6574 7572 6e20 7365 6c66     # return self
-00016ca0: 2e70 6f73 745f 6d65 6173 7572 656d 656e  .post_measuremen
-00016cb0: 7428 7461 626c 652c 2027 7674 696c 655f  t(table, 'vtile_
-00016cc0: 636f 6c64 5f74 6573 7427 290a 2020 2020  cold_test').    
-00016cd0: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-00016ce0: 6c65 6d65 6e74 6564 4572 726f 720a       lementedError.
+00016be0: 2d2d 2d2d 0a20 2020 2020 2020 2022 2222  ----.        """
+00016bf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016c00: 7365 6c66 2e70 6f73 745f 6d65 6173 7572  self.post_measur
+00016c10: 656d 656e 7428 7461 626c 652c 2027 7674  ement(table, 'vt
+00016c20: 696c 6527 290a 0a20 2020 2064 6566 2070  ile')..    def p
+00016c30: 6f73 745f 7674 696c 655f 636f 6c64 5f74  ost_vtile_cold_t
+00016c40: 6573 7428 7365 6c66 2c20 7461 626c 6529  est(self, table)
+00016c50: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00016c60: 2020 2020 2020 504f 5354 2074 6162 6c65        POST table
+00016c70: 3a20 7674 696c 655f 636f 6c64 5f74 6573  : vtile_cold_tes
+00016c80: 740a 2020 2020 2020 2020 2222 220a 2020  t.        """.  
+00016c90: 2020 2020 2020 2320 7265 7475 726e 2073        # return s
+00016ca0: 656c 662e 706f 7374 5f6d 6561 7375 7265  elf.post_measure
+00016cb0: 6d65 6e74 2874 6162 6c65 2c20 2776 7469  ment(table, 'vti
+00016cc0: 6c65 5f63 6f6c 645f 7465 7374 2729 0a20  le_cold_test'). 
+00016cd0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
+00016ce0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00016cf0: 0a                                       .
```

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/qr.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/qrgen.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/scanner_auto.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/scanner_auto.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile.py`

 * *Files 0% similar despite different names*

```diff
@@ -2884,15 +2884,15 @@
             dt_rtd = datetime.datetime.strptime(
                 sold['room_temperature_date'],
                 '%Y-%m-%d %H:%M:%S'
             )
             dt_rtd_p30 = dt_rtd + datetime.timedelta(days=30)
 
             solder_fail = False
-            if dt_now >= dt_exp:
+            if dt_now > dt_exp:
                 self.print_to_console(f'{cluster}: check expiry date')
                 solder_fail = True
             if dt_now > dt_rtd_p30:
                 self.print_to_console(
                     f'{cluster}: check duration at room temperature'
                 )
                 solder_fail = True
@@ -3159,14 +3159,25 @@
 
         button_submit_widget = next(
             w.instance for w in self.widgets
             if w.cluster == 'submit' and w.itype == Itype.BUTTON
         )
         self.set_button_state(button_submit_widget, disabled=len(table) != 30)
 
+        ######################################################################
+        # Issue reminder for Liverpool
+
+        # Liverpool uses version control for SiPM tray files. It's easy to
+        # forget to use git pull to ensure the latest files are being used, so
+        # remind the user before they press the SUBMIT button.
+        if 'Liverpool' in other_definitions['institute']:
+            self.print_to_console(
+                f'WARNING: is this tray file up to date? Remember to use "git pull".\n'
+            )
+
     def submit(self):
         """
         POST vTile to the pre-production database.
 
         ----------------------------------------------------------------------
         args : none
         ----------------------------------------------------------------------
```

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/submit_vtile_json.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/submit_vtile_json.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/veto_location.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/veto_location.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/veto_location_gui.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/veto_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/visual.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     args
         val : string
             filename, e.g. '20221031_135532_22061703000021001.csv'
     --------------------------------------------------------------------------
     returns : string
     --------------------------------------------------------------------------
     """
-    if not os.path.exists(filename):
-        raise argparse.ArgumentTypeError(f'{filename}: file does not exist')
+    if not os.path.isfile(filename):
+        raise argparse.ArgumentTypeError(f'{filename}: is not a file')
 
     return filename
 
 
 def check_arguments(settings):
     """
     Handle command line options.
@@ -159,20 +159,24 @@
                 # Freq:,10KHz,Amp:,100mV,MM:,CSRS,Operator:,A,S/N:,22061703000021001_dark,
                 *_, operator, _, sno, _ = row
 
                 # The DarkSide-20k database requires UTC date/time in this format:
                 # YYYY-MM-DD hh:mm:ss, e.g. 2022-07-19 07:00:00
 
                 # filename: 20221031_135532_22061703000021001_dark.csv
-                datetime_from_string = datetime.strptime(
-                    os.path.basename(filename)[:15], '%Y%m%d_%H%M%S'
-                )
-                timestamp = datetime_from_string.strftime('%Y-%m-%d %H:%M:%S')
+                try:
+                    datetime_from_string = datetime.strptime(
+                        os.path.basename(filename)[:15], '%Y%m%d_%H%M%S'
+                    )
+                except ValueError:
+                    continue
+                else:
+                    timestamp = datetime_from_string.strftime('%Y-%m-%d %H:%M:%S')
 
-                qrcode = sno[:17]
+                    qrcode = sno[:17]
 
     try:
         return {
             'timestamp': timestamp,
             'operator': operator,
             'qrcode': qrcode,
             'capacitance_1': float(cap1),
```

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_location_gui.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb/wafer_map_from_db.py` & `ds20kdb-avt-1.0.4/src/ds20kdb/wafer_map_from_db.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.3
+Version: 1.0.4
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.3/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb-avt-1.0.4/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

