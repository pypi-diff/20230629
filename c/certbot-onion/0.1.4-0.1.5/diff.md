# Comparing `tmp/certbot-onion-0.1.4.tar.gz` & `tmp/certbot_onion-0.1.5-cp310-cp310-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.4.tar", last modified: Fri May 26 09:07:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

