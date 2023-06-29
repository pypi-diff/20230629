# Comparing `tmp/resize_icon-0.1.1.tar.gz` & `tmp/resize_icon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resize_icon-0.1.1.tar", max compression
+gzip compressed data, was "resize_icon-0.1.2.tar", max compression
```

## Comparing `resize_icon-0.1.1.tar` & `resize_icon-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-29 10:19:52.627269 resize_icon-0.1.1/README.md
--rw-r--r--   0        0        0      355 2023-06-29 10:50:04.683551 resize_icon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       51 2023-06-29 10:39:58.108479 resize_icon-0.1.1/resize_icon/__init__.py
--rw-r--r--   0        0        0     4894 2023-06-29 10:48:54.368616 resize_icon-0.1.1/resize_icon/resize.py
--rw-r--r--   0        0        0    13368 2023-06-29 10:32:40.806258 resize_icon-0.1.1/resize_icon/spec.py
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 resize_icon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-29 10:19:52.627269 resize_icon-0.1.2/README.md
+-rw-r--r--   0        0        0      343 2023-06-29 11:19:11.722573 resize_icon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-29 10:39:58.108479 resize_icon-0.1.2/resize_icon/__init__.py
+-rw-r--r--   0        0        0     4894 2023-06-29 10:48:54.368616 resize_icon-0.1.2/resize_icon/resize.py
+-rw-r--r--   0        0        0    13368 2023-06-29 10:32:40.806258 resize_icon-0.1.2/resize_icon/spec.py
+-rw-r--r--   0        0        0      367 1970-01-01 00:00:00.000000 resize_icon-0.1.2/PKG-INFO
```

### Comparing `resize_icon-0.1.1/resize_icon/resize.py` & `resize_icon-0.1.2/resize_icon/resize.py`

 * *Files identical despite different names*

### Comparing `resize_icon-0.1.1/resize_icon/spec.py` & `resize_icon-0.1.2/resize_icon/spec.py`

 * *Files identical despite different names*

