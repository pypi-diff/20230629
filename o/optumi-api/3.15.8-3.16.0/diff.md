# Comparing `tmp/optumi-api-3.15.8.tar.gz` & `tmp/optumi_api-3.16.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.15.8.tar", last modified: Tue May 16 18:59:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

