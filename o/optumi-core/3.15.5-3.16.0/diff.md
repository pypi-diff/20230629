# Comparing `tmp/optumi-core-3.15.5.tar.gz` & `tmp/optumi_core-3.16.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-core-3.15.5.tar", last modified: Fri Apr 28 23:43:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

