# Comparing `tmp/kt-ds-api-0.0.2.tar.gz` & `tmp/kt_ds_api-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kt-ds-api-0.0.2.tar", last modified: Tue May 30 07:09:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

