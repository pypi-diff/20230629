# Comparing `tmp/outlines-unleashed-0.0.8.tar.gz` & `tmp/outlines_unleashed-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/outlines-unleashed-0.0.8.tar", last modified: Sun Feb 16 14:12:03 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

