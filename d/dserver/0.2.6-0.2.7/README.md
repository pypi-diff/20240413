# Comparing `tmp/dserver-0.2.6-py3-none-any.whl.zip` & `tmp/dserver-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,24 @@
-Zip file size: 17781 bytes, number of entries: 18
+Zip file size: 180691 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-08 07:45 dserver/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Jan-11 06:36 dserver/__main__.py
 -rw-r--r--  2.0 unx     6215 b- defN 24-Feb-26 03:00 dserver/main.py
 -rw-r--r--  2.0 unx      871 b- defN 24-Jan-11 06:36 dserver/utils.py
 -rw-r--r--  2.0 unx       42 b- defN 24-Jan-08 07:42 sserver/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Jan-11 06:36 sserver/__main__.py
 -rw-r--r--  2.0 unx      914 b- defN 24-Mar-14 08:40 sserver/filters.py
--rw-r--r--  2.0 unx     9928 b- defN 24-Mar-18 06:53 sserver/main.py
+-rw-r--r--  2.0 unx    10100 b- defN 24-Apr-12 15:36 sserver/main.py
 -rw-r--r--  2.0 unx     2891 b- defN 24-Mar-14 08:40 sserver/model.py
 -rw-r--r--  2.0 unx     1309 b- defN 24-Mar-14 09:24 sserver/utils.py
 -rw-r--r--  2.0 unx     9442 b- defN 24-Mar-15 03:34 sserver/templates/index.html
 -rw-r--r--  2.0 unx      956 b- defN 24-Jan-05 09:31 sserver/templates/media.html
 -rw-r--r--  2.0 unx     1485 b- defN 24-Jan-05 09:31 sserver/templates/message.html
+-rw-r--r--  2.0 unx   232855 b- defN 24-Apr-12 15:35 sserver/upload/bootstrap-5.3.1.min.css
+-rw-r--r--  2.0 unx    60582 b- defN 24-Apr-12 15:35 sserver/upload/bootstrap-5.3.1.min.js
 -rw-r--r--  2.0 unx    67646 b- defN 24-Jan-09 02:46 sserver/upload/favicon.ico
--rw-r--r--  2.0 unx      283 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1370 b- defN 24-Apr-12 15:22 dserver-0.2.6.dist-info/RECORD
-18 files, 103798 bytes uncompressed, 15567 bytes compressed:  85.0%
+-rw-r--r--  2.0 unx   285314 b- defN 24-Apr-12 15:35 sserver/upload/jquery-3.7.1.js
+-rw-r--r--  2.0 unx    87533 b- defN 24-Apr-12 15:35 sserver/upload/jquery-3.7.1.min.js
+-rw-r--r--  2.0 unx      283 b- defN 24-Apr-12 15:38 dserver-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 15:38 dserver-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-12 15:38 dserver-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1744 b- defN 24-Apr-12 15:38 dserver-0.2.7.dist-info/RECORD
+22 files, 770628 bytes uncompressed, 177895 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -33,23 +33,35 @@
 
 Filename: sserver/templates/media.html
 Comment: 
 
 Filename: sserver/templates/message.html
 Comment: 
 
+Filename: sserver/upload/bootstrap-5.3.1.min.css
+Comment: 
+
+Filename: sserver/upload/bootstrap-5.3.1.min.js
+Comment: 
+
 Filename: sserver/upload/favicon.ico
 Comment: 
 
-Filename: dserver-0.2.6.dist-info/METADATA
+Filename: sserver/upload/jquery-3.7.1.js
+Comment: 
+
+Filename: sserver/upload/jquery-3.7.1.min.js
+Comment: 
+
+Filename: dserver-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: dserver-0.2.6.dist-info/WHEEL
+Filename: dserver-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: dserver-0.2.6.dist-info/top_level.txt
+Filename: dserver-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dserver-0.2.6.dist-info/RECORD
+Filename: dserver-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sserver/main.py

```diff
@@ -1,9 +1,10 @@
 from functools import partial
 from glob import glob
+from itertools import chain
 import os
 import argparse
 import shutil
 from urllib.parse import unquote
 import aiofiles
 
 from sanic import Blueprint, Sanic, Request, response, app
@@ -201,23 +202,25 @@
     app.config.REQUEST_MAX_SIZE = int(os.environ.get("REQUEST_MAX_SIZE", 10 * 1024 * 1024 * 1024))
     app.blueprint(bp)
 
     @app.listener("before_server_start")
     async def setup(app, loop):
         await get_db()
 
+        static_files = ["favicon.ico", "*.js", "*.css"]
         if not os.path.exists(app.config.UPLOAD_DIR):
             os.makedirs(app.config.UPLOAD_DIR)
-        if not await FileRecord.get("favicon.ico"):
-            await FileRecord("favicon.ico", "favicon.ico", True).save()
-        if not os.path.exists(app.config.UPLOAD_DIR + "/favicon.ico"):
-            shutil.copy(
-                os.path.join(os.path.dirname(__file__), "upload", "favicon.ico"),
-                os.path.join(app.config.UPLOAD_DIR, "favicon.ico"),
-            )
+        src_path = os.path.join(os.path.dirname(__file__), "upload")
+        files = chain(*[glob(os.path.join(src_path, it)) for it in static_files])
+        for file in files:
+            filename = os.path.basename(file)
+            if not await FileRecord.get(filename):
+                await FileRecord(filename, filename, True).save()
+            if not (dst_file:= os.path.exists(app.config.UPLOAD_DIR + f"/{filename}")):
+                shutil.copy(file,dst_file)
 
     return app
 
 
 def parseargs():
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", "-H", type=str, default="0.0.0.0", help="host")
```

## Comparing `dserver-0.2.6.dist-info/RECORD` & `dserver-0.2.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 dserver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dserver/__main__.py,sha256=yZoUXBVZGqRGlyIyPyFo_lhDwopuliF-I81qXQL1phs,169
 dserver/main.py,sha256=1WHlZ_8PJnms4AI5pdqVJfT_4O2Xi-XqCUwWaK8l1bE,6215
 dserver/utils.py,sha256=wWdoB1zA5uzT2WSkrGG6onLIUkU3-pSMSGR9pq0bb3o,871
 sserver/__init__.py,sha256=5qfY42LaeOv41nxPaRZwGtCEe2TR3LnvyC6KpTjDHis,42
 sserver/__main__.py,sha256=yZoUXBVZGqRGlyIyPyFo_lhDwopuliF-I81qXQL1phs,169
 sserver/filters.py,sha256=vi7BQaMjGA6KDksQYa7v6nEcawkR9EeeuEojo8OO0z8,914
-sserver/main.py,sha256=ZIW5nRJb9_1xSmd25eDNbZHl2_kEdRxjXJZfrDikkHs,9928
+sserver/main.py,sha256=i5TO-EvgDJ2-dUU17S7haRDphWIDdKnqQy1Yg95a2B0,10100
 sserver/model.py,sha256=N3zWoSTuSsm_O0Ba3t9YIJJF1nZ_FvG1VH7Mj7JcIEA,2891
 sserver/utils.py,sha256=aZE_gPDK3EQi59m3e6U6EBTxyoc4-qiLEF42Y3m9w_4,1309
 sserver/templates/index.html,sha256=Y_1tucpIBR9p9IiRY3jvCg8HLcE5mMmMd1EJnlipGzM,9442
 sserver/templates/media.html,sha256=XORUp0Wj-kq8L5oNLuLe7VxiVnL4Qn8wHMN5w0GyDI8,956
 sserver/templates/message.html,sha256=sP3TlrScBuH19Nm7WLkLabD4DDmM3Ynk-ZL189NgIvM,1485
+sserver/upload/bootstrap-5.3.1.min.css,sha256=2TnSHycBDAm2wpZmgdi0z81kykGPJAkiUY-Wf97RbvY,232855
+sserver/upload/bootstrap-5.3.1.min.js,sha256=gOQJIa9-K_XdfAuBkg2ONAdw5EnQbokw_s2b8BqsRFg,60582
 sserver/upload/favicon.ico,sha256=Tgs5rN3sYkx3KXC2GfEy5ggUldH-I_nH6bR27A8-CUo,67646
-dserver-0.2.6.dist-info/METADATA,sha256=6ihPIbHdAY2w5XMRRHUEvXqa5XRZQIfZs95XmRsFcGo,283
-dserver-0.2.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-dserver-0.2.6.dist-info/top_level.txt,sha256=N-vaTOxCZp44JisKy4P3VbvVjobIuHmAEBTH706kCvo,16
-dserver-0.2.6.dist-info/RECORD,,
+sserver/upload/jquery-3.7.1.js,sha256=eKhayi8LEQwp4NKxN-CfCh-3qOVUtJn3QNZ0TciWLP4,285314
+sserver/upload/jquery-3.7.1.min.js,sha256=_JqT3SQfawRcv_BIHPThkBvs0OEvtFFmqPF_lYI_Cxo,87533
+dserver-0.2.7.dist-info/METADATA,sha256=6gLAnwM7lB299PStiXOX9cp6Rh2N6Fn8bLQRQ5xIxaU,283
+dserver-0.2.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+dserver-0.2.7.dist-info/top_level.txt,sha256=N-vaTOxCZp44JisKy4P3VbvVjobIuHmAEBTH706kCvo,16
+dserver-0.2.7.dist-info/RECORD,,
```

