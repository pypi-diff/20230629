# Comparing `tmp/tcfetch-0.3.2.tar.gz` & `tmp/tcfetch-0.4.0-cp311-cp311-macosx_10_7_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

