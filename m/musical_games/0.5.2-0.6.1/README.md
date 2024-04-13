# Comparing `tmp/musical_games-0.5.2.tar.gz` & `tmp/musical_games-0.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.5.2.tar", last modified: Tue Feb 15 13:40:26 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

