# Comparing `tmp/whishow-0.3.0-py2.py3-none-any.whl.zip` & `tmp/whishow-0.4.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 13714 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 18:27 whishow-0.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-13 18:27 whishow-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 18:27 whishow-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-13 18:27 whishow-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      386 b- defN 24-Apr-13 18:27 whishow-0.3.0.dist-info/RECORD
-5 files, 37152 bytes uncompressed, 12994 bytes compressed:  65.0%
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-Apr-13 18:35 whishow-0.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      837 b- defN 24-Apr-13 18:35 whishow-0.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-13 18:35 whishow-0.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-13 18:35 whishow-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      386 b- defN 24-Apr-13 18:35 whishow-0.4.0.dist-info/RECORD
+5 files, 37155 bytes uncompressed, 12994 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: whishow-0.3.0.dist-info/LICENSE
+Filename: whishow-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: whishow-0.3.0.dist-info/METADATA
+Filename: whishow-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: whishow-0.3.0.dist-info/WHEEL
+Filename: whishow-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: whishow-0.3.0.dist-info/top_level.txt
+Filename: whishow-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: whishow-0.3.0.dist-info/RECORD
+Filename: whishow-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `whishow-0.3.0.dist-info/LICENSE` & `whishow-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `whishow-0.3.0.dist-info/METADATA` & `whishow-0.4.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whishow
-Version: 0.3.0
+Version: 0.4.0
 Summary: an online player for video stream
 Home-page: https://github.com/coolEphemeroptera/Whishow
 Author: wei.wang
 Author-email: coolephemeroptera@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,12 +14,12 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyav
 Requires-Dist: opencv-python
 Requires-Dist: soxr
-Requires-Dist: PIL
+Requires-Dist: pillow
 Requires-Dist: pyaudio
 Requires-Dist: numpy
 
 an online player for video stream
```

