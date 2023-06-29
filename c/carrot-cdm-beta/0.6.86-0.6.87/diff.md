# Comparing `tmp/carrot-cdm-beta-0.6.86.tar.gz` & `tmp/carrot_cdm_beta-0.6.87-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-beta-0.6.86.tar", last modified: Mon Jun 12 13:39:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

