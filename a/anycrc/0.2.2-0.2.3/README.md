# Comparing `tmp/anycrc-0.2.2.tar.gz` & `tmp/anycrc-0.2.3-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.2.2.tar", last modified: Sat Apr 13 19:45:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

