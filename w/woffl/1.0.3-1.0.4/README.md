# Comparing `tmp/woffl-1.0.3.tar.gz` & `tmp/woffl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woffl-1.0.3.tar", last modified: Fri Apr 12 17:05:05 2024, max compression
+gzip compressed data, was "woffl-1.0.4.tar", last modified: Sat Apr 13 00:21:28 2024, max compression
```

## Comparing `woffl-1.0.3.tar` & `woffl-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.132566 woffl-1.0.3/
--rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4028 2024-04-12 17:05:05.132566 woffl-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.3/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-12 17:04:14.000000 woffl-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 17:05:05.134901 woffl-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.052110 woffl-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.3/tests/boil_test.py
--rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.3/tests/e41_test.py
--rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.3/tests/fgas_test.py
--rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.3/tests/flow_test.py
--rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.3/tests/jpump_test.py
--rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.3/tests/outflow_test.py
--rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.3/tests/pvt_test.py
--rw-rw-rw-   0        0        0     2375 2024-04-12 01:33:15.000000 woffl-1.0.3/tests/rmix_test.py
--rw-rw-rw-   0        0        0      358 2024-04-11 21:40:46.000000 woffl-1.0.3/tests/wprof_test.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.053622 woffl-1.0.3/woffl/
--rw-rw-rw-   0        0        0       56 2024-04-12 17:04:14.000000 woffl-1.0.3/woffl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.077712 woffl-1.0.3/woffl/assembly/
--rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.3/woffl/assembly/__init__.py
--rw-rw-rw-   0        0        0     2313 2024-04-11 21:31:27.000000 woffl-1.0.3/woffl/assembly/batchrun.py
--rw-rw-rw-   0        0        0     3756 2024-04-12 15:24:00.000000 woffl-1.0.3/woffl/assembly/easypump.py
--rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.3/woffl/assembly/sysops.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.099772 woffl-1.0.3/woffl/flow/
--rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.3/woffl/flow/__init__.py
--rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.3/woffl/flow/annflow.py
--rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.3/woffl/flow/inflow.py
--rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.3/woffl/flow/jetcheck.py
--rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.3/woffl/flow/jetflow.py
--rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.3/woffl/flow/jetplot.py
--rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.3/woffl/flow/outflow.py
--rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.3/woffl/flow/singlephase.py
--rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.3/woffl/flow/twophase.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.111478 woffl-1.0.3/woffl/geometry/
--rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.3/woffl/geometry/__init__.py
--rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.3/woffl/geometry/forms.py
--rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.3/woffl/geometry/jetpump.py
--rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.3/woffl/geometry/pipe.py
--rw-rw-rw-   0        0        0    26650 2024-04-12 15:30:05.000000 woffl-1.0.3/woffl/geometry/wellprofile.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.126874 woffl-1.0.3/woffl/pvt/
--rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.3/woffl/pvt/__init__.py
--rw-rw-rw-   0        0        0    23100 2024-04-12 16:12:06.000000 woffl-1.0.3/woffl/pvt/blackoil.py
--rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.3/woffl/pvt/deadoil.py
--rw-rw-rw-   0        0        0    13803 2024-04-12 15:28:33.000000 woffl-1.0.3/woffl/pvt/formgas.py
--rw-rw-rw-   0        0        0     4192 2024-04-12 17:03:55.000000 woffl-1.0.3/woffl/pvt/formwat.py
--rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.3/woffl/pvt/resmix.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:05:05.130124 woffl-1.0.3/woffl.egg-info/
--rw-rw-rw-   0        0        0     4028 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2024-04-12 17:05:05.000000 woffl-1.0.3/woffl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-12 17:05:04.000000 woffl-1.0.3/woffl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.581800 woffl-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2024-01-10 03:00:27.000000 woffl-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4069 2024-04-13 00:21:28.579712 woffl-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1926 2024-01-11 23:52:57.000000 woffl-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1622 2024-04-13 00:08:41.000000 woffl-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 00:21:28.581800 woffl-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.498362 woffl-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-10 03:00:27.000000 woffl-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-04-11 21:37:06.000000 woffl-1.0.4/tests/boil_test.py
+-rw-rw-rw-   0        0        0     1853 2024-04-11 21:38:00.000000 woffl-1.0.4/tests/e41_test.py
+-rw-rw-rw-   0        0        0     2010 2024-04-11 21:38:27.000000 woffl-1.0.4/tests/fgas_test.py
+-rw-rw-rw-   0        0        0     3080 2024-04-11 21:39:03.000000 woffl-1.0.4/tests/flow_test.py
+-rw-rw-rw-   0        0        0     2697 2024-04-11 21:39:58.000000 woffl-1.0.4/tests/jpump_test.py
+-rw-rw-rw-   0        0        0     1628 2024-04-11 21:40:16.000000 woffl-1.0.4/tests/outflow_test.py
+-rw-rw-rw-   0        0        0      932 2024-04-12 01:06:46.000000 woffl-1.0.4/tests/pvt_test.py
+-rw-rw-rw-   0        0        0     2375 2024-04-12 01:33:15.000000 woffl-1.0.4/tests/rmix_test.py
+-rw-rw-rw-   0        0        0      358 2024-04-12 20:42:07.000000 woffl-1.0.4/tests/wprof_test.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.500503 woffl-1.0.4/woffl/
+-rw-rw-rw-   0        0        0       56 2024-04-13 00:08:41.000000 woffl-1.0.4/woffl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.524402 woffl-1.0.4/woffl/assembly/
+-rw-rw-rw-   0        0        0      324 2024-03-27 23:41:15.000000 woffl-1.0.4/woffl/assembly/__init__.py
+-rw-rw-rw-   0        0        0     2246 2024-04-12 18:49:52.000000 woffl-1.0.4/woffl/assembly/batchrun.py
+-rw-rw-rw-   0        0        0     3756 2024-04-12 15:24:00.000000 woffl-1.0.4/woffl/assembly/easypump.py
+-rw-rw-rw-   0        0        0     6051 2024-04-11 21:47:40.000000 woffl-1.0.4/woffl/assembly/sysops.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.548608 woffl-1.0.4/woffl/flow/
+-rw-rw-rw-   0        0        0      202 2024-03-14 00:29:33.000000 woffl-1.0.4/woffl/flow/__init__.py
+-rw-rw-rw-   0        0        0     1359 2024-04-11 21:44:39.000000 woffl-1.0.4/woffl/flow/annflow.py
+-rw-rw-rw-   0        0        0     3213 2024-01-10 03:00:27.000000 woffl-1.0.4/woffl/flow/inflow.py
+-rw-rw-rw-   0        0        0     6639 2024-04-11 21:45:21.000000 woffl-1.0.4/woffl/flow/jetcheck.py
+-rw-rw-rw-   0        0        0    18742 2024-04-11 21:45:56.000000 woffl-1.0.4/woffl/flow/jetflow.py
+-rw-rw-rw-   0        0        0    18559 2024-04-11 21:46:16.000000 woffl-1.0.4/woffl/flow/jetplot.py
+-rw-rw-rw-   0        0        0     8850 2024-04-11 21:46:30.000000 woffl-1.0.4/woffl/flow/outflow.py
+-rw-rw-rw-   0        0        0     6306 2024-02-12 23:51:08.000000 woffl-1.0.4/woffl/flow/singlephase.py
+-rw-rw-rw-   0        0        0    16499 2024-04-11 21:46:45.000000 woffl-1.0.4/woffl/flow/twophase.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.560696 woffl-1.0.4/woffl/geometry/
+-rw-rw-rw-   0        0        0      113 2024-02-18 01:31:16.000000 woffl-1.0.4/woffl/geometry/__init__.py
+-rw-rw-rw-   0        0        0     1786 2024-02-13 20:25:30.000000 woffl-1.0.4/woffl/geometry/forms.py
+-rw-rw-rw-   0        0        0     3388 2024-01-31 19:16:45.000000 woffl-1.0.4/woffl/geometry/jetpump.py
+-rw-rw-rw-   0        0        0     2674 2024-02-19 03:49:34.000000 woffl-1.0.4/woffl/geometry/pipe.py
+-rw-rw-rw-   0        0        0    26650 2024-04-12 15:30:05.000000 woffl-1.0.4/woffl/geometry/wellprofile.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.574438 woffl-1.0.4/woffl/pvt/
+-rw-rw-rw-   0        0        0      330 2024-04-12 01:14:17.000000 woffl-1.0.4/woffl/pvt/__init__.py
+-rw-rw-rw-   0        0        0    23100 2024-04-12 16:12:06.000000 woffl-1.0.4/woffl/pvt/blackoil.py
+-rw-rw-rw-   0        0        0      609 2024-01-10 03:00:27.000000 woffl-1.0.4/woffl/pvt/deadoil.py
+-rw-rw-rw-   0        0        0    13803 2024-04-12 15:28:33.000000 woffl-1.0.4/woffl/pvt/formgas.py
+-rw-rw-rw-   0        0        0     4192 2024-04-12 17:05:54.000000 woffl-1.0.4/woffl/pvt/formwat.py
+-rw-rw-rw-   0        0        0    19555 2024-04-11 22:34:02.000000 woffl-1.0.4/woffl/pvt/resmix.py
+drwxrwxrwx   0        0        0        0 2024-04-13 00:21:28.576694 woffl-1.0.4/woffl.egg-info/
+-rw-rw-rw-   0        0        0     4069 2024-04-13 00:21:28.000000 woffl-1.0.4/woffl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2024-04-13 00:21:28.000000 woffl-1.0.4/woffl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 00:21:28.000000 woffl-1.0.4/woffl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-04-13 00:21:28.000000 woffl-1.0.4/woffl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-13 00:21:28.000000 woffl-1.0.4/woffl.egg-info/top_level.txt
```

### Comparing `woffl-1.0.3/LICENSE` & `woffl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/PKG-INFO` & `woffl-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.3
-Summary: Numerically solve jet pump equations in multiphase oil wells
+Version: 1.0.4
+Summary: Water Optimization For Fluid Lift. Numerical solver for liquid powered jet pumps with multiphase flow
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `woffl-1.0.3/README.md` & `woffl-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/pyproject.toml` & `woffl-1.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,96 +5,98 @@
 00000040: 6174 6573 2074 6865 2022 6368 6565 7365  ates the "cheese
 00000050: 2077 6865 656c 220d 0a62 7569 6c64 2d62   wheel"..build-b
 00000060: 6163 6b65 6e64 203d 2022 7365 7475 7074  ackend = "setupt
 00000070: 6f6f 6c73 2e62 7569 6c64 5f6d 6574 6122  ools.build_meta"
 00000080: 0d0a 0d0a 5b74 6f6f 6c2e 7365 7475 7074  ....[tool.setupt
 00000090: 6f6f 6c73 2e70 6163 6b61 6765 732e 6669  ools.packages.fi
 000000a0: 6e64 5d0d 0a65 7863 6c75 6465 203d 205b  nd]..exclude = [
-000000b0: 2264 6174 6122 5d20 2023 2061 6c74 6572  "data"]  # alter
-000000c0: 6e61 7469 7665 6c79 3a20 6065 7863 6c75  natively: `exclu
-000000d0: 6465 203d 205b 2261 6464 6974 696f 6e61  de = ["additiona
-000000e0: 6c2a 225d 600d 0a0d 0a5b 7072 6f6a 6563  l*"]`....[projec
-000000f0: 745d 0d0a 6e61 6d65 203d 2022 776f 6666  t]..name = "woff
-00000100: 6c22 0d0a 7665 7273 696f 6e20 3d20 2231  l"..version = "1
-00000110: 2e30 2e33 2220 2320 6275 6d70 7665 7220  .0.3" # bumpver 
-00000120: 6175 746f 6d61 7469 6361 6c6c 7920 7570  automatically up
-00000130: 6461 7465 730d 0a64 6573 6372 6970 7469  dates..descripti
-00000140: 6f6e 203d 2022 4e75 6d65 7269 6361 6c6c  on = "Numericall
-00000150: 7920 736f 6c76 6520 6a65 7420 7075 6d70  y solve jet pump
-00000160: 2065 7175 6174 696f 6e73 2069 6e20 6d75   equations in mu
-00000170: 6c74 6970 6861 7365 206f 696c 2077 656c  ltiphase oil wel
-00000180: 6c73 220d 0a72 6561 646d 6520 3d20 2252  ls"..readme = "R
-00000190: 4541 444d 452e 6d64 220d 0a6c 6963 656e  EADME.md"..licen
-000001a0: 7365 203d 207b 2066 696c 6520 3d20 224c  se = { file = "L
-000001b0: 4943 454e 5345 2220 7d0d 0a63 6c61 7373  ICENSE" }..class
-000001c0: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
-000001d0: 2244 6576 656c 6f70 6d65 6e74 2053 7461  "Development Sta
-000001e0: 7475 7320 3a3a 2033 202d 2041 6c70 6861  tus :: 3 - Alpha
-000001f0: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
-00000200: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000210: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
-00000220: 2020 2020 2249 6e74 656e 6465 6420 4175      "Intended Au
-00000230: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-00000240: 652f 5265 7365 6172 6368 222c 0d0a 2020  e/Research",..  
-00000250: 2020 2254 6f70 6963 203a 3a20 5363 6965    "Topic :: Scie
-00000260: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-00000270: 6e67 203a 3a20 5068 7973 6963 7322 2c0d  ng :: Physics",.
-00000280: 0a20 2020 2022 4c69 6365 6e73 6520 3a3a  .    "License ::
-00000290: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000002a0: 204d 4954 204c 6963 656e 7365 220d 0a20   MIT License".. 
-000002b0: 2020 205d 0d0a 6b65 7977 6f72 6473 203d     ]..keywords =
-000002c0: 205b 226a 6574 2070 756d 7022 2c20 2273   ["jet pump", "s
-000002d0: 6f6c 7665 7222 2c20 226e 756d 6572 6963  olver", "numeric
-000002e0: 616c 222c 2022 6d75 6c74 6970 6861 7365  al", "multiphase
-000002f0: 225d 0d0a 6465 7065 6e64 656e 6369 6573  "]..dependencies
-00000300: 203d 205b 0d0a 2020 2020 226d 6174 706c   = [..    "matpl
-00000310: 6f74 6c69 623e 3d33 2e38 2e32 222c 2023  otlib>=3.8.2", #
-00000320: 2079 6172 0d0a 2020 2020 226e 756d 7079   yar..    "numpy
-00000330: 3e3d 312e 3236 2e33 222c 2023 2079 6172  >=1.26.3", # yar
-00000340: 0d0a 2020 2020 2270 616e 6461 733e 3d32  ..    "pandas>=2
-00000350: 2e31 2e34 222c 2023 2079 6172 0d0a 2020  .1.4", # yar..  
-00000360: 2020 2273 6369 7079 3e3d 312e 3131 2e34    "scipy>=1.11.4
-00000370: 222c 2023 2079 6172 0d0a 5d0d 0a72 6571  ", # yar..]..req
-00000380: 7569 7265 732d 7079 7468 6f6e 203d 2022  uires-python = "
-00000390: 3e3d 332e 3130 2220 2320 6e6f 7420 7375  >=3.10" # not su
-000003a0: 7265 2077 6865 6e20 7479 7065 2068 696e  re when type hin
-000003b0: 7469 6e67 2077 6173 2072 656c 6561 7365  ting was release
-000003c0: 640d 0a0d 0a5b 7072 6f6a 6563 742e 6f70  d....[project.op
-000003d0: 7469 6f6e 616c 2d64 6570 656e 6465 6e63  tional-dependenc
-000003e0: 6965 735d 0d0a 6465 7620 3d20 5b22 6275  ies]..dev = ["bu
-000003f0: 6d70 7665 7222 2c20 2269 736f 7274 222c  mpver", "isort",
-00000400: 2022 626c 6163 6b22 5d0d 0a0d 0a5b 7072   "black"]....[pr
-00000410: 6f6a 6563 742e 7572 6c73 5d0d 0a48 6f6d  oject.urls]..Hom
-00000420: 6570 6167 6520 3d20 2268 7474 7073 3a2f  epage = "https:/
-00000430: 2f67 6974 6875 622e 636f 6d2f 6b77 656c  /github.com/kwel
-00000440: 6c69 732f 776f 6666 6c22 0d0a 0d0a 0d0a  lis/woffl"......
-00000450: 5b74 6f6f 6c2e 6275 6d70 7665 725d 0d0a  [tool.bumpver]..
-00000460: 6375 7272 656e 745f 7665 7273 696f 6e20  current_version 
-00000470: 3d20 2231 2e30 2e33 2220 2320 6275 6d70  = "1.0.3" # bump
-00000480: 7665 7220 7570 6461 7465 2070 6174 6368  ver update patch
-00000490: 0d0a 7665 7273 696f 6e5f 7061 7474 6572  ..version_patter
-000004a0: 6e20 3d20 224d 414a 4f52 2e4d 494e 4f52  n = "MAJOR.MINOR
-000004b0: 2e50 4154 4348 220d 0a23 2063 6f6d 6d69  .PATCH"..# commi
-000004c0: 745f 6d65 7373 6167 6520 3d20 2262 756d  t_message = "bum
-000004d0: 7020 7665 7273 696f 6e20 7b6f 6c64 5f76  p version {old_v
-000004e0: 6572 7369 6f6e 7d20 2d3e 207b 6e65 775f  ersion} -> {new_
-000004f0: 7665 7273 696f 6e7d 220d 0a23 2074 6167  version}"..# tag
-00000500: 5f6d 6573 7361 6765 203d 2022 7b6e 6577  _message = "{new
-00000510: 5f76 6572 7369 6f6e 7d22 0d0a 2320 7461  _version}"..# ta
-00000520: 675f 7363 6f70 6520 3d20 2264 6566 6175  g_scope = "defau
-00000530: 6c74 220d 0a23 2070 7265 5f63 6f6d 6d69  lt"..# pre_commi
-00000540: 745f 686f 6f6b 203d 2022 220d 0a23 2070  t_hook = ""..# p
-00000550: 6f73 745f 636f 6d6d 6974 5f68 6f6f 6b20  ost_commit_hook 
-00000560: 3d20 2222 0d0a 2320 636f 6d6d 6974 203d  = ""..# commit =
-00000570: 2074 7275 650d 0a23 2074 6167 203d 2074   true..# tag = t
-00000580: 7275 650d 0a23 2070 7573 6820 3d20 6661  rue..# push = fa
-00000590: 6c73 650d 0a0d 0a5b 746f 6f6c 2e62 756d  lse....[tool.bum
-000005a0: 7076 6572 2e66 696c 655f 7061 7474 6572  pver.file_patter
-000005b0: 6e73 5d0d 0a22 7079 7072 6f6a 6563 742e  ns].."pyproject.
-000005c0: 746f 6d6c 2220 3d20 5b0d 0a20 2020 2027  toml" = [..    '
-000005d0: 6375 7272 656e 745f 7665 7273 696f 6e20  current_version 
-000005e0: 3d20 227b 7665 7273 696f 6e7d 2227 2c0d  = "{version}"',.
-000005f0: 0a20 2020 2027 7665 7273 696f 6e20 3d20  .    'version = 
-00000600: 227b 7665 7273 696f 6e7d 2227 0d0a 5d0d  "{version}"'..].
-00000610: 0a22 776f 6666 6c2f 5f5f 696e 6974 5f5f  ."woffl/__init__
-00000620: 2e70 7922 203d 205b 227b 7665 7273 696f  .py" = ["{versio
-00000630: 6e7d 225d 0d0a 0d0a                      n}"]....
+000000b0: 2264 6174 6122 5d0d 0a0d 0a5b 7072 6f6a  "data"]....[proj
+000000c0: 6563 745d 0d0a 6e61 6d65 203d 2022 776f  ect]..name = "wo
+000000d0: 6666 6c22 0d0a 7665 7273 696f 6e20 3d20  ffl"..version = 
+000000e0: 2231 2e30 2e34 2220 2320 6275 6d70 7665  "1.0.4" # bumpve
+000000f0: 7220 6175 746f 6d61 7469 6361 6c6c 7920  r automatically 
+00000100: 7570 6461 7465 730d 0a64 6573 6372 6970  updates..descrip
+00000110: 7469 6f6e 203d 2022 5761 7465 7220 4f70  tion = "Water Op
+00000120: 7469 6d69 7a61 7469 6f6e 2046 6f72 2046  timization For F
+00000130: 6c75 6964 204c 6966 742e 204e 756d 6572  luid Lift. Numer
+00000140: 6963 616c 2073 6f6c 7665 7220 666f 7220  ical solver for 
+00000150: 6c69 7175 6964 2070 6f77 6572 6564 206a  liquid powered j
+00000160: 6574 2070 756d 7073 2077 6974 6820 6d75  et pumps with mu
+00000170: 6c74 6970 6861 7365 2066 6c6f 7722 0d0a  ltiphase flow"..
+00000180: 7265 6164 6d65 203d 2022 5245 4144 4d45  readme = "README
+00000190: 2e6d 6422 0d0a 6c69 6365 6e73 6520 3d20  .md"..license = 
+000001a0: 7b20 6669 6c65 203d 2022 4c49 4345 4e53  { file = "LICENS
+000001b0: 4522 207d 0d0a 636c 6173 7369 6669 6572  E" }..classifier
+000001c0: 7320 3d20 5b0d 0a20 2020 2022 4465 7665  s = [..    "Deve
+000001d0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+000001e0: 3a20 3320 2d20 416c 7068 6122 2c0d 0a20  : 3 - Alpha",.. 
+000001f0: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000210: 6f6e 203a 3a20 3322 2c0d 0a20 2020 2022  on :: 3",..    "
+00000220: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000230: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+00000240: 6561 7263 6822 2c0d 0a20 2020 2022 546f  earch",..    "To
+00000250: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+00000260: 632f 456e 6769 6e65 6572 696e 6720 3a3a  c/Engineering ::
+00000270: 2050 6879 7369 6373 222c 0d0a 2020 2020   Physics",..    
+00000280: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
+00000290: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000002a0: 4c69 6365 6e73 6522 0d0a 2020 2020 5d0d  License"..    ].
+000002b0: 0a6b 6579 776f 7264 7320 3d20 5b22 6a65  .keywords = ["je
+000002c0: 7420 7075 6d70 222c 2022 736f 6c76 6572  t pump", "solver
+000002d0: 222c 2022 6e75 6d65 7269 6361 6c22 2c20  ", "numerical", 
+000002e0: 226d 756c 7469 7068 6173 6522 5d0d 0a64  "multiphase"]..d
+000002f0: 6570 656e 6465 6e63 6965 7320 3d20 5b0d  ependencies = [.
+00000300: 0a20 2020 2022 6d61 7470 6c6f 746c 6962  .    "matplotlib
+00000310: 3e3d 332e 382e 3222 2c0d 0a20 2020 2022  >=3.8.2",..    "
+00000320: 6e75 6d70 793e 3d31 2e32 362e 3322 2c20  numpy>=1.26.3", 
+00000330: 0d0a 2020 2020 2270 616e 6461 733e 3d32  ..    "pandas>=2
+00000340: 2e31 2e34 222c 2023 2070 616e 6461 7320  .1.4", # pandas 
+00000350: 696e 7374 616c 6c73 206e 756d 7079 2c20  installs numpy, 
+00000360: 6275 7420 4920 6d69 6768 7420 6765 7420  but I might get 
+00000370: 7269 6420 6f66 2070 616e 6461 730d 0a20  rid of pandas.. 
+00000380: 2020 2022 7363 6970 793e 3d31 2e31 312e     "scipy>=1.11.
+00000390: 3422 2c20 0d0a 5d0d 0a0d 0a72 6571 7569  4", ..]....requi
+000003a0: 7265 732d 7079 7468 6f6e 203d 2022 3e3d  res-python = ">=
+000003b0: 332e 3130 2220 2320 6e6f 7420 7375 7265  3.10" # not sure
+000003c0: 2077 6865 6e20 7479 7065 2068 696e 7469   when type hinti
+000003d0: 6e67 2077 6173 2072 656c 6561 7365 640d  ng was released.
+000003e0: 0a0d 0a5b 7072 6f6a 6563 742e 6f70 7469  ...[project.opti
+000003f0: 6f6e 616c 2d64 6570 656e 6465 6e63 6965  onal-dependencie
+00000400: 735d 0d0a 6465 7620 3d20 5b22 6275 6d70  s]..dev = ["bump
+00000410: 7665 7222 2c20 2269 736f 7274 222c 2022  ver", "isort", "
+00000420: 626c 6163 6b22 5d0d 0a0d 0a5b 7072 6f6a  black"]....[proj
+00000430: 6563 742e 7572 6c73 5d0d 0a48 6f6d 6570  ect.urls]..Homep
+00000440: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
+00000450: 6974 6875 622e 636f 6d2f 6b77 656c 6c69  ithub.com/kwelli
+00000460: 732f 776f 6666 6c22 0d0a 0d0a 0d0a 5b74  s/woffl"......[t
+00000470: 6f6f 6c2e 6275 6d70 7665 725d 0d0a 6375  ool.bumpver]..cu
+00000480: 7272 656e 745f 7665 7273 696f 6e20 3d20  rrent_version = 
+00000490: 2231 2e30 2e34 2220 2320 6275 6d70 7665  "1.0.4" # bumpve
+000004a0: 7220 7570 6461 7465 2070 6174 6368 0d0a  r update patch..
+000004b0: 7665 7273 696f 6e5f 7061 7474 6572 6e20  version_pattern 
+000004c0: 3d20 224d 414a 4f52 2e4d 494e 4f52 2e50  = "MAJOR.MINOR.P
+000004d0: 4154 4348 220d 0a23 2063 6f6d 6d69 745f  ATCH"..# commit_
+000004e0: 6d65 7373 6167 6520 3d20 2262 756d 7020  message = "bump 
+000004f0: 7665 7273 696f 6e20 7b6f 6c64 5f76 6572  version {old_ver
+00000500: 7369 6f6e 7d20 2d3e 207b 6e65 775f 7665  sion} -> {new_ve
+00000510: 7273 696f 6e7d 220d 0a23 2074 6167 5f6d  rsion}"..# tag_m
+00000520: 6573 7361 6765 203d 2022 7b6e 6577 5f76  essage = "{new_v
+00000530: 6572 7369 6f6e 7d22 0d0a 2320 7461 675f  ersion}"..# tag_
+00000540: 7363 6f70 6520 3d20 2264 6566 6175 6c74  scope = "default
+00000550: 220d 0a23 2070 7265 5f63 6f6d 6d69 745f  "..# pre_commit_
+00000560: 686f 6f6b 203d 2022 220d 0a23 2070 6f73  hook = ""..# pos
+00000570: 745f 636f 6d6d 6974 5f68 6f6f 6b20 3d20  t_commit_hook = 
+00000580: 2222 0d0a 2320 636f 6d6d 6974 203d 2074  ""..# commit = t
+00000590: 7275 650d 0a23 2074 6167 203d 2074 7275  rue..# tag = tru
+000005a0: 650d 0a23 2070 7573 6820 3d20 6661 6c73  e..# push = fals
+000005b0: 650d 0a0d 0a5b 746f 6f6c 2e62 756d 7076  e....[tool.bumpv
+000005c0: 6572 2e66 696c 655f 7061 7474 6572 6e73  er.file_patterns
+000005d0: 5d0d 0a22 7079 7072 6f6a 6563 742e 746f  ].."pyproject.to
+000005e0: 6d6c 2220 3d20 5b0d 0a20 2020 2027 6375  ml" = [..    'cu
+000005f0: 7272 656e 745f 7665 7273 696f 6e20 3d20  rrent_version = 
+00000600: 227b 7665 7273 696f 6e7d 2227 2c0d 0a20  "{version}"',.. 
+00000610: 2020 2027 7665 7273 696f 6e20 3d20 227b     'version = "{
+00000620: 7665 7273 696f 6e7d 2227 0d0a 5d0d 0a22  version}"'..].."
+00000630: 776f 6666 6c2f 5f5f 696e 6974 5f5f 2e70  woffl/__init__.p
+00000640: 7922 203d 205b 227b 7665 7273 696f 6e7d  y" = ["{version}
+00000650: 225d 0d0a 0d0a                           "]....
```

### Comparing `woffl-1.0.3/tests/boil_test.py` & `woffl-1.0.4/tests/boil_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/e41_test.py` & `woffl-1.0.4/tests/e41_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/fgas_test.py` & `woffl-1.0.4/tests/fgas_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/flow_test.py` & `woffl-1.0.4/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/jpump_test.py` & `woffl-1.0.4/tests/jpump_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/outflow_test.py` & `woffl-1.0.4/tests/outflow_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/pvt_test.py` & `woffl-1.0.4/tests/pvt_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/tests/rmix_test.py` & `woffl-1.0.4/tests/rmix_test.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/assembly/batchrun.py` & `woffl-1.0.4/woffl/assembly/batchrun.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 """Batch Jet Pump Runs
 
 Contains code that is used to run multiple pumps at once to understand the
-current conditions.
+current conditions. Currently Scott's code is here with a simple nested for
+loop. Will eventually update this to more of a class style system. Runs the
+analysis and sends the results to a .csv file.
 """
 
 import pandas as pd
 
 from woffl.assembly.easypump import jetpump_wrapper
 
-"""
-This is a file to call the run_pump file from Assembly folder
-
-Loops through a list of jet pump nozzle and throat sizes and returns a csv file with the results
-Update well characterisitics in the call to the model pump function
-
-"""
-
-
 nozzles = ["9", "10", "11", "12", "13", "14"]
 throats = ["X", "A", "B", "C", "D", "E"]
 
 results = []
 
 for nozzle in nozzles:
     for throat in throats:
```

### Comparing `woffl-1.0.3/woffl/assembly/easypump.py` & `woffl-1.0.4/woffl/assembly/easypump.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/assembly/sysops.py` & `woffl-1.0.4/woffl/assembly/sysops.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/annflow.py` & `woffl-1.0.4/woffl/flow/annflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/inflow.py` & `woffl-1.0.4/woffl/flow/inflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/jetcheck.py` & `woffl-1.0.4/woffl/flow/jetcheck.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/jetflow.py` & `woffl-1.0.4/woffl/flow/jetflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/jetplot.py` & `woffl-1.0.4/woffl/flow/jetplot.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/outflow.py` & `woffl-1.0.4/woffl/flow/outflow.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/singlephase.py` & `woffl-1.0.4/woffl/flow/singlephase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/flow/twophase.py` & `woffl-1.0.4/woffl/flow/twophase.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/geometry/forms.py` & `woffl-1.0.4/woffl/geometry/forms.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/geometry/jetpump.py` & `woffl-1.0.4/woffl/geometry/jetpump.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/geometry/pipe.py` & `woffl-1.0.4/woffl/geometry/pipe.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/geometry/wellprofile.py` & `woffl-1.0.4/woffl/geometry/wellprofile.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/pvt/blackoil.py` & `woffl-1.0.4/woffl/pvt/blackoil.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/pvt/deadoil.py` & `woffl-1.0.4/woffl/pvt/deadoil.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/pvt/formgas.py` & `woffl-1.0.4/woffl/pvt/formgas.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/pvt/formwat.py` & `woffl-1.0.4/woffl/pvt/formwat.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl/pvt/resmix.py` & `woffl-1.0.4/woffl/pvt/resmix.py`

 * *Files identical despite different names*

### Comparing `woffl-1.0.3/woffl.egg-info/PKG-INFO` & `woffl-1.0.4/woffl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: woffl
-Version: 1.0.3
-Summary: Numerically solve jet pump equations in multiphase oil wells
+Version: 1.0.4
+Summary: Water Optimization For Fluid Lift. Numerical solver for liquid powered jet pumps with multiphase flow
 License: MIT License
         
         Copyright (c) 2023 Kaelin Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `woffl-1.0.3/woffl.egg-info/SOURCES.txt` & `woffl-1.0.4/woffl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

