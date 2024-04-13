# Comparing `tmp/gkeepapi-0.9.7-py2.py3-none-any.whl.zip` & `tmp/gkeepapi-0.9.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16015 bytes, number of entries: 10
+Zip file size: 16025 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx    36432 b- defN 17-Dec-10 16:40 gkeepapi/node.py
--rw-rw-r--  2.0 unx    17901 b- defN 17-Dec-12 02:43 gkeepapi/__init__.py
+-rw-rw-r--  2.0 unx    17907 b- defN 17-Dec-12 05:38 gkeepapi/__init__.py
 -rw-rw-r--  2.0 unx     8892 b- defN 17-Nov-12 04:53 test/test_nodes.py
 -rw-rw-r--  2.0 unx        0 b- defN 17-Nov-05 22:16 test/__init__.py
--rw-rw-r--  2.0 unx       10 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      865 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/metadata.json
--rw-rw-r--  2.0 unx       14 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      110 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx      707 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      798 b- defN 17-Dec-12 02:43 gkeepapi-0.9.7.dist-info/RECORD
-10 files, 65729 bytes uncompressed, 14673 bytes compressed:  77.7%
+-rw-rw-r--  2.0 unx       10 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      865 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/metadata.json
+-rw-rw-r--  2.0 unx       14 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      110 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      707 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx      798 b- defN 17-Dec-12 05:38 gkeepapi-0.9.8.dist-info/RECORD
+10 files, 65735 bytes uncompressed, 14683 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: test/test_nodes.py
 Comment: 
 
 Filename: test/__init__.py
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/DESCRIPTION.rst
+Filename: gkeepapi-0.9.8.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/metadata.json
+Filename: gkeepapi-0.9.8.dist-info/metadata.json
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/top_level.txt
+Filename: gkeepapi-0.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/WHEEL
+Filename: gkeepapi-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/METADATA
+Filename: gkeepapi-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: gkeepapi-0.9.7.dist-info/RECORD
+Filename: gkeepapi-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gkeepapi/__init__.py

```diff
@@ -528,15 +528,15 @@
 
         for label_id in self._labels:
             logger.debug('Deleted label: %s', label_id)
 
         self._labels = labels
 
     def _findDirtyNodes(self):
-        for node in self._nodes.values():
+        for node in list(self._nodes.values()):
             for child in node.children:
                 if not child.id in self._nodes:
                     self._nodes[child.id] = child
 
         nodes = []
         for node in self._nodes.values():
             if node.dirty:
```

## Comparing `gkeepapi-0.9.7.dist-info/metadata.json` & `gkeepapi-0.9.8.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.9.8'"}*

```diff
@@ -41,9 +41,9 @@
             "requires": [
                 "gpsoauth (>=0.4.1)",
                 "six (>=1.11.0)"
             ]
         }
     ],
     "summary": "An unofficial Google Keep API client",
-    "version": "0.9.7"
+    "version": "0.9.8"
 }
```

## Comparing `gkeepapi-0.9.7.dist-info/METADATA` & `gkeepapi-0.9.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: gkeepapi
-Version: 0.9.7
+Version: 0.9.8
 Summary: An unofficial Google Keep API client
 Home-page: https://github.com/kiwiz/gkeepapi
 Author: Kai
 Author-email: z@kwi.li
 License: MIT
 Keywords: google keep api
 Platform: UNKNOWN
```

## Comparing `gkeepapi-0.9.7.dist-info/RECORD` & `gkeepapi-0.9.8.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-gkeepapi/__init__.py,sha256=Jrq3dTb43F0h9INrco3W0uNQf8KbhQtF2tC_PNovNO0,17901
+gkeepapi/__init__.py,sha256=KZ8bfe5hn0IMpLE3tRM2iX4DkE0gRcSuAYIv-7KXqO0,17907
 gkeepapi/node.py,sha256=alkZmbwNaFbZ6wQpExekpqDHm8oQRED-CygV5_a-E5Q,36432
-gkeepapi-0.9.7.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
-gkeepapi-0.9.7.dist-info/METADATA,sha256=zKrR0DJURNeefaA4Kzlp8YNUmNXmDFRWH7zif05BTyw,707
-gkeepapi-0.9.7.dist-info/RECORD,,
-gkeepapi-0.9.7.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
-gkeepapi-0.9.7.dist-info/metadata.json,sha256=tUNKsovM6DAY754R70PyNChWDW2RW8ZA4kdm181jic8,865
-gkeepapi-0.9.7.dist-info/top_level.txt,sha256=d3QQ-9H4MBm37EL4JpIdhWb-3lsW8zBpufnVzjtNBVg,14
+gkeepapi-0.9.8.dist-info/DESCRIPTION.rst,sha256=OCTuuN6LcWulhHS3d5rfjdsQtW22n7HENFRh6jC6ego,10
+gkeepapi-0.9.8.dist-info/METADATA,sha256=KYRkBVvCQBkiYGWXxLfuxDWB6Fd1tsL--XoUBrj8bdk,707
+gkeepapi-0.9.8.dist-info/RECORD,,
+gkeepapi-0.9.8.dist-info/WHEEL,sha256=o2k-Qa-RMNIJmUdIc7KU6VWR_ErNRbWNlxDIpl7lm34,110
+gkeepapi-0.9.8.dist-info/metadata.json,sha256=qzubYExgg7lhD7UbPreBK6fBvJ_KUZ2_8Shgl_Abdk4,865
+gkeepapi-0.9.8.dist-info/top_level.txt,sha256=d3QQ-9H4MBm37EL4JpIdhWb-3lsW8zBpufnVzjtNBVg,14
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_nodes.py,sha256=rem82XRwl7pslVKAwmnJx8kkkZVhlxWmvB_RD9dYucA,8892
```

