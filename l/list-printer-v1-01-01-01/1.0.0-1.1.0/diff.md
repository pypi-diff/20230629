# Comparing `tmp/list_printer_v1_01_01_01-1.0.0.tar.gz` & `tmp/list_printer_v1_01_01_01-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_printer_v1_01_01_01-1.0.0.tar", last modified: Thu Jun 29 16:41:43 2023, max compression
+gzip compressed data, was "list_printer_v1_01_01_01-1.1.0.tar", last modified: Thu Jun 29 18:16:06 2023, max compression
```

## Comparing `list_printer_v1_01_01_01-1.0.0.tar` & `list_printer_v1_01_01_01-1.1.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 16:41:43.643482 list_printer_v1_01_01_01-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-29 16:41:43.643482 list_printer_v1_01_01_01-1.0.0/PKG-INFO
--rw-rw-r--   0 crackygeek  (1000) crackygeek  (1000)      361 2023-06-29 16:41:12.305249 list_printer_v1_01_01_01-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 18:16:06.778882 list_printer_v1_01_01_01-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-29 18:16:06.778882 list_printer_v1_01_01_01-1.1.0/PKG-INFO
+-rw-rw-r--   0 crackygeek  (1000) crackygeek  (1000)      361 2023-06-29 18:14:28.119385 list_printer_v1_01_01_01-1.1.0/setup.py
```

