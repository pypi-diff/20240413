# Comparing `tmp/latk-2.9.1.tar.gz` & `tmp/latk-2.9.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latk-2.9.1.tar", last modified: Fri Nov  3 18:32:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

