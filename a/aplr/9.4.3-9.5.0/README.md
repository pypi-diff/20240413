# Comparing `tmp/aplr-9.4.3.tar.gz` & `tmp/aplr-9.5.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplr-9.4.3.tar", last modified: Thu Apr 11 15:45:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

