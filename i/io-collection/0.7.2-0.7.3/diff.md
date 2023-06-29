# Comparing `tmp/io_collection-0.7.2.tar.gz` & `tmp/io_collection-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_collection-0.7.2.tar", max compression
+gzip compressed data, was "io_collection-0.7.3.tar", max compression
```

## Comparing `io_collection-0.7.2.tar` & `io_collection-0.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1519 2023-03-30 00:46:40.079913 io_collection-0.7.2/LICENSE
--rw-r--r--   0        0        0      788 2023-03-30 00:46:40.079913 io_collection-0.7.2/README.md
--rw-r--r--   0        0        0     1899 2023-03-30 00:46:40.083913 io_collection-0.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/__main__.py
--rw-r--r--   0        0        0      389 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/__init__.py
--rw-r--r--   0        0        0      709 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/change_key.py
--rw-r--r--   0        0        0      525 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/check_key.py
--rw-r--r--   0        0        0      726 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/copy_key.py
--rw-r--r--   0        0        0     1302 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/get_keys.py
--rw-r--r--   0        0        0      297 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/make_key.py
--rw-r--r--   0        0        0      461 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/keys/remove_key.py
--rw-r--r--   0        0        0      429 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/__init__.py
--rw-r--r--   0        0        0     1028 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_buffer.py
--rw-r--r--   0        0        0      705 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_dataframe.py
--rw-r--r--   0        0        0      953 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_image.py
--rw-r--r--   0        0        0      223 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_pickle.py
--rw-r--r--   0        0        0      606 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_tar.py
--rw-r--r--   0        0        0      561 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/load/load_text.py
--rw-r--r--   0        0        0        0 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/py.typed
--rw-r--r--   0        0        0      209 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/quilt/__init__.py
--rw-r--r--   0        0        0      185 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/quilt/load_quilt_package.py
--rw-r--r--   0        0        0      287 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/quilt/save_quilt_item.py
--rw-r--r--   0        0        0      616 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/__init__.py
--rw-r--r--   0        0        0      745 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_buffer.py
--rw-r--r--   0        0        0      920 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_dataframe.py
--rw-r--r--   0        0        0      889 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_figure.py
--rw-r--r--   0        0        0      514 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_gif.py
--rw-r--r--   0        0        0      902 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_image.py
--rw-r--r--   0        0        0      587 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_json.py
--rw-r--r--   0        0        0      274 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_pickle.py
--rw-r--r--   0        0        0     1018 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_tar.py
--rw-r--r--   0        0        0      712 2023-03-30 00:46:40.083913 io_collection-0.7.2/src/io_collection/save/save_text.py
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 io_collection-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-06-29 20:45:22.718034 io_collection-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2506 2023-06-29 20:45:22.718034 io_collection-0.7.3/README.md
+-rw-r--r--   0        0        0     1915 2023-06-29 20:45:22.722034 io_collection-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/__main__.py
+-rw-r--r--   0        0        0      389 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/__init__.py
+-rw-r--r--   0        0        0      709 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/change_key.py
+-rw-r--r--   0        0        0      525 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/check_key.py
+-rw-r--r--   0        0        0      726 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/copy_key.py
+-rw-r--r--   0        0        0     1365 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/get_keys.py
+-rw-r--r--   0        0        0      297 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/make_key.py
+-rw-r--r--   0        0        0      461 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/keys/remove_key.py
+-rw-r--r--   0        0        0      429 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/__init__.py
+-rw-r--r--   0        0        0     1028 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_buffer.py
+-rw-r--r--   0        0        0      705 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_dataframe.py
+-rw-r--r--   0        0        0      953 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_image.py
+-rw-r--r--   0        0        0      223 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_pickle.py
+-rw-r--r--   0        0        0      606 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_tar.py
+-rw-r--r--   0        0        0      561 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/load/load_text.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/py.typed
+-rw-r--r--   0        0        0      209 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/__init__.py
+-rw-r--r--   0        0        0      185 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/load_quilt_package.py
+-rw-r--r--   0        0        0      287 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/quilt/save_quilt_item.py
+-rw-r--r--   0        0        0      616 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/__init__.py
+-rw-r--r--   0        0        0      745 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_buffer.py
+-rw-r--r--   0        0        0      920 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_dataframe.py
+-rw-r--r--   0        0        0      889 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_figure.py
+-rw-r--r--   0        0        0      514 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_gif.py
+-rw-r--r--   0        0        0      902 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_image.py
+-rw-r--r--   0        0        0      587 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_json.py
+-rw-r--r--   0        0        0      274 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_pickle.py
+-rw-r--r--   0        0        0     1018 2023-06-29 20:45:22.722034 io_collection-0.7.3/src/io_collection/save/save_tar.py
+-rw-r--r--   0        0        0      712 2023-06-29 20:45:22.726034 io_collection-0.7.3/src/io_collection/save/save_text.py
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 io_collection-0.7.3/PKG-INFO
```

### Comparing `io_collection-0.7.2/LICENSE` & `io_collection-0.7.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Bagheri Lab
+Copyright (c) 2023, Allen Institute for Cell Science
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `io_collection-0.7.2/pyproject.toml` & `io_collection-0.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "io-collection"
-version = "0.7.2"
+version = "0.7.3"
 description = "Collection of tasks for I/O."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -18,23 +18,24 @@
 aicsimageio = "^4.9.4"
 matplotlib = "^3.7.0"
 s3fs = "^2023.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
-mypy = "^0.991"
+mypy = "^1.3.0"
 pylint = "^2.16.2"
-pytest = "^7.2.0"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
-pytest-subtests = "^0.8.0"
-Sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.2.0"
-sphinx_mdinclude = "^0.5.3"
-tox = "^3.26.0"
+pytest-subtests = "^0.11.0"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
+myst-parser = "^2.0.0"
+sphinx-copybutton = "^0.5.2"
+tox = "^4.5.1"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `io_collection-0.7.2/src/io_collection/keys/change_key.py` & `io_collection-0.7.3/src/io_collection/keys/change_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/keys/check_key.py` & `io_collection-0.7.3/src/io_collection/keys/check_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/keys/copy_key.py` & `io_collection-0.7.3/src/io_collection/keys/copy_key.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/keys/get_keys.py` & `io_collection-0.7.3/src/io_collection/keys/get_keys.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     if location[:5] == "s3://":
         return get_keys_from_s3(location[5:], prefix)
     else:
         return get_keys_from_fs(location, prefix)
 
 
 def get_keys_from_fs(path: str, prefix: str) -> list[str]:
-    all_files = glob(f"{path}{prefix}/**/*", recursive=True)
+    glob_pattern = f"{path}/{prefix}/**/*".replace("//", "/")
+    all_files = glob(glob_pattern, recursive=True)
     regular_files = [file for file in all_files if not os.path.isdir(file)]
-    keys = [file.replace(path, "") for file in regular_files]
+    keys = [file.replace(path, "").strip("/") for file in regular_files]
     return keys
 
 
 def get_keys_from_s3(bucket: str, prefix: str) -> list[str]:
     s3_client = boto3.client("s3")
 
     bucket = bucket.replace("s3://", "")
```

### Comparing `io_collection-0.7.2/src/io_collection/load/load_buffer.py` & `io_collection-0.7.3/src/io_collection/load/load_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/load/load_dataframe.py` & `io_collection-0.7.3/src/io_collection/load/load_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/load/load_image.py` & `io_collection-0.7.3/src/io_collection/load/load_image.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/load/load_tar.py` & `io_collection-0.7.3/src/io_collection/load/load_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/load/load_text.py` & `io_collection-0.7.3/src/io_collection/load/load_text.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/__init__.py` & `io_collection-0.7.3/src/io_collection/save/__init__.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_buffer.py` & `io_collection-0.7.3/src/io_collection/save/save_buffer.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_dataframe.py` & `io_collection-0.7.3/src/io_collection/save/save_dataframe.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_figure.py` & `io_collection-0.7.3/src/io_collection/save/save_figure.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_gif.py` & `io_collection-0.7.3/src/io_collection/save/save_gif.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_image.py` & `io_collection-0.7.3/src/io_collection/save/save_image.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_json.py` & `io_collection-0.7.3/src/io_collection/save/save_json.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_tar.py` & `io_collection-0.7.3/src/io_collection/save/save_tar.py`

 * *Files identical despite different names*

### Comparing `io_collection-0.7.2/src/io_collection/save/save_text.py` & `io_collection-0.7.3/src/io_collection/save/save_text.py`

 * *Files identical despite different names*

