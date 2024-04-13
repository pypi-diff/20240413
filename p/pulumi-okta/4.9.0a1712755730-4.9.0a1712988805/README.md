# Comparing `tmp/pulumi_okta-4.9.0a1712755730.tar.gz` & `tmp/pulumi_okta-4.9.0a1712988805-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1712755730.tar", last modified: Wed Apr 10 13:33:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

