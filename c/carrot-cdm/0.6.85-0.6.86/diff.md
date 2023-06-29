# Comparing `tmp/carrot-cdm-0.6.85.tar.gz` & `tmp/carrot_cdm-0.6.86-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-0.6.85.tar", last modified: Mon May  1 14:55:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

