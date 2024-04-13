# Comparing `tmp/whishow-0.1.0-py2.py3-none-any.whl.zip` & `tmp/whishow-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 13713 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 18:11 whishow-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-13 18:11 whishow-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 18:11 whishow-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-13 18:11 whishow-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      386 b- defN 24-Apr-13 18:11 whishow-0.1.0.dist-info/RECORD
-5 files, 37152 bytes uncompressed, 12993 bytes compressed:  65.0%
+Zip file size: 13717 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 18:22 whishow-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      856 b- defN 24-Apr-13 18:22 whishow-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 18:22 whishow-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-13 18:22 whishow-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      386 b- defN 24-Apr-13 18:22 whishow-0.2.0.dist-info/RECORD
+5 files, 37174 bytes uncompressed, 12997 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: whishow-0.1.0.dist-info/LICENSE
+Filename: whishow-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: whishow-0.1.0.dist-info/METADATA
+Filename: whishow-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: whishow-0.1.0.dist-info/WHEEL
+Filename: whishow-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: whishow-0.1.0.dist-info/top_level.txt
+Filename: whishow-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: whishow-0.1.0.dist-info/RECORD
+Filename: whishow-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `whishow-0.1.0.dist-info/LICENSE` & `whishow-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `whishow-0.1.0.dist-info/METADATA` & `whishow-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whishow
-Version: 0.1.0
+Version: 0.2.0
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
 Requires-Dist: queue
 Requires-Dist: PIL
 Requires-Dist: pyaudio
+Requires-Dist: numpy
 
 an online player for video stream
```

