# Comparing `tmp/whishow-1.3.0-py2.py3-none-any.whl.zip` & `tmp/whishow-1.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9816207 bytes, number of entries: 11
+Zip file size: 9816213 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat 16574124 b- defN 24-Apr-09 14:00 whishow/NotoSansCJKsc-Regular.ttf
 -rw-rw-rw-  2.0 fat      107 b- defN 24-Apr-13 20:05 whishow/__init__.py
 -rw-rw-rw-  2.0 fat     1473 b- defN 24-Apr-13 19:58 whishow/easyplayer.py
 -rw-rw-rw-  2.0 fat     7221 b- defN 24-Apr-13 20:04 whishow/stream.py
 -rw-rw-rw-  2.0 fat     4093 b- defN 24-Apr-13 18:10 whishow/utils.py
 -rw-rw-rw-  2.0 fat     8407 b- defN 24-Apr-13 20:02 whishow/whishow.py
--rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 20:17 whishow-1.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      838 b- defN 24-Apr-13 20:17 whishow-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 20:17 whishow-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-13 20:17 whishow-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      855 b- defN 24-Apr-13 20:17 whishow-1.3.0.dist-info/RECORD
-11 files, 16633057 bytes uncompressed, 9814783 bytes compressed:  41.0%
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 20:25 whishow-1.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      861 b- defN 24-Apr-13 20:25 whishow-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 20:25 whishow-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-13 20:25 whishow-1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      855 b- defN 24-Apr-13 20:25 whishow-1.3.1.dist-info/RECORD
+11 files, 16633080 bytes uncompressed, 9814789 bytes compressed:  41.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: whishow/utils.py
 Comment: 
 
 Filename: whishow/whishow.py
 Comment: 
 
-Filename: whishow-1.3.0.dist-info/LICENSE
+Filename: whishow-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: whishow-1.3.0.dist-info/METADATA
+Filename: whishow-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: whishow-1.3.0.dist-info/WHEEL
+Filename: whishow-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: whishow-1.3.0.dist-info/top_level.txt
+Filename: whishow-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: whishow-1.3.0.dist-info/RECORD
+Filename: whishow-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `whishow-1.3.0.dist-info/LICENSE` & `whishow-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `whishow-1.3.0.dist-info/METADATA` & `whishow-1.3.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whishow
-Version: 1.3.0
+Version: 1.3.1
 Summary: an online player for video stream
 Home-page: https://github.com/coolEphemeroptera/Whishow
 Author: wei.wang
 Author-email: coolephemeroptera@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,9 +17,10 @@
 License-File: LICENSE
 Requires-Dist: pyav
 Requires-Dist: opencv-python
 Requires-Dist: soxr
 Requires-Dist: pillow
 Requires-Dist: pyaudio
 Requires-Dist: numpy
+Requires-Dist: pyyaml
 
 an online player for video stream
```

## Comparing `whishow-1.3.0.dist-info/RECORD` & `whishow-1.3.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 whishow/NotoSansCJKsc-Regular.ttf,sha256=ebHembhhphIpJJouit9XVHPsICNtxNkgBozLl65AojY,16574124
 whishow/__init__.py,sha256=zVRBkKHhqddeUbbh5Vx3ePsgx_NgDbPUQBf0Uji8Z0Y,107
 whishow/easyplayer.py,sha256=-bLFxel35ETugIa5rw3yi-BGxVNU1eTxKufBe7eYcm0,1473
 whishow/stream.py,sha256=ET081-gzYZsp3rbqN1BL4MUMQb2hqUNQCAekzLm59iI,7221
 whishow/utils.py,sha256=1LLUWI5eqM1I7W_CFLII_r-pHdXfLPHQk18apMovcWM,4093
 whishow/whishow.py,sha256=nV_rAqWq847-Vyw5qa7thypMD2L0F_ekaIa1y64pbWg,8407
-whishow-1.3.0.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-whishow-1.3.0.dist-info/METADATA,sha256=oGFpPtjR6OYuk8npmwfXAORfF3OnP-NjrQQ9NA6czD4,838
-whishow-1.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-whishow-1.3.0.dist-info/top_level.txt,sha256=8jiD8NtoF80xztcrrSTXycTZIEMKH3tfUNrJ0wQqZBY,8
-whishow-1.3.0.dist-info/RECORD,,
+whishow-1.3.1.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+whishow-1.3.1.dist-info/METADATA,sha256=ZutFmvExtuzrw-G0JITXTemqLu06bF7PxqajAwVNsbA,861
+whishow-1.3.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+whishow-1.3.1.dist-info/top_level.txt,sha256=8jiD8NtoF80xztcrrSTXycTZIEMKH3tfUNrJ0wQqZBY,8
+whishow-1.3.1.dist-info/RECORD,,
```

