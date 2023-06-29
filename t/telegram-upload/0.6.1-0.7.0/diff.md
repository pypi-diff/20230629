# Comparing `tmp/telegram-upload-0.6.1.tar.gz` & `tmp/telegram-upload-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-upload-0.6.1.tar", last modified: Sat Jun 17 14:15:51 2023, max compression
+gzip compressed data, was "telegram-upload-0.7.0.tar", last modified: Thu Jun 29 16:27:54 2023, max compression
```

## Comparing `telegram-upload-0.6.1.tar` & `telegram-upload-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    49610 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9637 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-17 14:15:51.858001 telegram-upload-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/telegram_upload/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/upload_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/telegram_upload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.419312 telegram-upload-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.419312 telegram-upload-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    49610 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/caption_format.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9637 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.423312 telegram-upload-0.7.0/telegram_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/caption_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.427312 telegram-upload-0.7.0/telegram_upload/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_manager_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/client/telegram_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-29 16:27:29.000000 telegram-upload-0.7.0/telegram_upload/upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/telegram_upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/telegram_upload/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.423312 telegram-upload-0.7.0/telegram_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:27:54.000000 telegram-upload-0.7.0/telegram_upload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.427312 telegram-upload-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_caption_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:54.431312 telegram-upload-0.7.0/tests/test_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_manager_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_client/test_telegram_upload_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-29 16:27:30.000000 telegram-upload-0.7.0/tests/test_video.py
```

### Comparing `telegram-upload-0.6.1/CONTRIBUTING.rst` & `telegram-upload-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/HISTORY.rst` & `telegram-upload-0.7.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+0.7.0 (2023-06-29)
+------------------
+
+* Issue #140: Speed up upload & download speed
+* Issue #115: Add support for variables in the caption argument
+* Issue #159: Telegram premium
+* Issue #176: Bug uploading .flv files
+* Issue #198: Improve README
+
 0.6.1 (2023-06-17)
 ------------------
 
 * Issue #197: if to.lstrip("-+").isdigit(): AttributeError: 'int' object has no attribute 'lstrip'
 
 0.6.0 (2023-06-15)
 ------------------
```

### Comparing `telegram-upload-0.6.1/LICENSE` & `telegram-upload-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/PKG-INFO` & `telegram-upload-0.7.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: telegram-upload
-Version: 0.6.1
-Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
-Home-page: https://github.com/Nekmo/telegram-upload/
-Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
-Author: Nekmo
-Author-email: contacto@nekmo.com
-Keywords: telegram-upload,telegram,upload,video
-Platform: linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Natural Language :: English
-Classifier: Development Status :: 5 - Production/Stable
-Provides: tests
-Provides: telegram_upload
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
 
 |
 
 
@@ -47,102 +21,160 @@
   :target: https://codeclimate.com/github/Nekmo/telegram-upload
   :alt: Code Climate
 
 .. image:: https://img.shields.io/codecov/c/github/Nekmo/telegram-upload/master.svg?style=flat-square
   :target: https://codecov.io/github/Nekmo/telegram-upload
   :alt: Test coverage
 
-.. image:: https://img.shields.io/requires/github/Nekmo/telegram-upload.svg?style=flat-square
-     :target: https://requires.io/github/Nekmo/telegram-upload/requirements/?branch=master
-     :alt: Requirements Status
+.. image:: https://img.shields.io/github/stars/Nekmo/telegram-upload?style=flat-square
+     :target: https://github.com/Nekmo/telegram-upload
+     :alt: Github stars
 
 
 ###############
 telegram-upload
 ###############
-Telegram-upload uses your personal Telegram account to upload and download files up to 2GiB (bots are limited to 50
-MiB). Turn Telegram into your personal cloud!
+Telegram-upload uses your **personal Telegram account** to **upload** and **download** files up to **4 GiB** (2 GiB for
+free users). Turn Telegram into your personal ☁ cloud!
 
-To **install telegram-upload**, run this command in your terminal:
+To **install 🔧 telegram-upload**, run this command in your terminal:
 
 .. code-block:: console
 
     $ sudo pip3 install -U telegram-upload
 
 This is the preferred method to install telegram-upload, as it will always install the most recent stable release.
-`More info in the documentation <https://docs.nekmo.org/telegram-upload/installation.html>`_
-
+🐍 **Python 3.7-3.11** are tested and supported. There are other installation ways available like `Docker <#-docker>`_.
+More info in the `📕 documentation <https://docs.nekmo.org/telegram-upload/installation.html>`_
 
-To use this program you need an Telegram account and your *App api_id/api_hash* (get it in
-`my.telegram.org <https://my.telegram.org/>`_). The first time you use telegram-upload it requests your telephone,
-api_id and api_hash. Bot tokens can not be used with this program (bot uploads are limited to 50MB). To **send files**
-(by default it is uploaded to saved messages):
+.. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/telegram-upload-demo.gif
+  :target: https://asciinema.org/a/592098
+  :width: 100%
 
-.. code-block:: console
+❓ Usage
+========
+To use this program you need an Telegram account and your **App api_id & api_hash** (get it in
+`my.telegram.org <https://my.telegram.org/>`_). The first time you use telegram-upload it requests your
+📱 **telephone**, **api_id** and **api_hash**. Bot tokens can not be used with this program (bot uploads are limited to
+50MB).
 
-    $ telegram-upload file1.mp4 /path/to/file2.mkv
+To **send ⬆️ files** (by default it is uploaded to saved messages):
 
-Credentials are saved in ``~/.config/telegram-upload.json`` and ``~/.config/telegram-upload.session``. You must make
-sure that these files are secured. You can copy these files to authenticate ``telegram-upload`` on more machines, but
-it is advisable to create a session file for each machine. Upload options are available
-`in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-upload>`_.
+.. code-block:: console
 
+    $ telegram-upload file1.mp4 file2.mkv
 
-You can **download the files** again from your saved messages (by default) or from a channel. All files will be
+You can **download ⤵️ the files** again from your saved messages (by default) or from a channel. All files will be
 downloaded until the last text message.
 
 .. code-block:: console
 
     $ telegram-download
 
-The ``--delete-on-success`` option allows you to delete the Telegram message after downloading the file. This is
-useful to send files to download to your saved messages and avoid downloading them again. You can use this option to
-download files on your computer away from home.
-
-`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info.
-
+`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info about the
+options availables.
 
 Interactive mode
-================
+----------------
 The **interactive option** (``--interactive``) allows you to choose the dialog and the files to download or upload with
-a **terminal wizard**. It even **supports mouse**!
+a **terminal 🪄 wizard**. It even **supports mouse**!
 
 .. code-block:: console
 
     $ telegram-upload --interactive    # Interactive upload
     $ telegram-download --interactive  # Interactive download
 
+`More info in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#interactive-mode>`_
 
-Features
-========
+Set group or chat
+-----------------
+By default when using telegram-upload without specifying the recipient or sender, telegram-upload will use your personal
+chat. However you can define the 👨 destination. For file upload the argument is ``--to <entity>``. For example:
+
+.. code-block::
+
+    $ telegram-upload --to telegram.me/joinchat/AAAAAEkk2WdoDrB4-Q8-gg video.mkv
+
+You can download files from a specific chat using the --from <entity> parameter. For example:
+
+.. code-block::
+
+    $ telegram-download --from username
+
+You can see all `the possible values for the entity in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#set-recipient-or-sender>`_.
 
-* Upload multiples files (up to 2GiB per file)
-* Download files.
-* Add video thumbs.
-* Delete local or remote file on success.
-* ... And more.
+Split & join files
+------------------
+If you try to upload a file that **exceeds the maximum supported** by Telegram by default, an error will occur. But you
+can enable ✂ **split mode** to upload multiple files:
 
-Docker
-======
+.. code-block:: console
+
+    $ telegram-upload --large-files split large-video.mkv
+
+Files split using split can be rejoined on download using:
+
+.. code-block:: console
+
+    $ telegram-download --split-files join
+
+Find more help in `the telegram-upload documentation <https://docs.nekmo.org/telegram-upload/usage.html#split-files>`_.
+
+Delete on success
+-----------------
+The ``--delete-on-success`` option allows you to ❌ **delete the Telegram message** after downloading the file. This is
+useful to send files to download to your saved messages and avoid downloading them again. You can use this option to
+download files on your computer away from home.
+
+Configuration
+-------------
+Credentials are saved in ``~/.config/telegram-upload.json`` and ``~/.config/telegram-upload.session``. You must make
+sure that these files are secured. You can copy these 📁 files to authenticate ``telegram-upload`` on more machines, but
+it is advisable to create a session file for each machine.
+
+More options
+------------
+Telegram-upload has more options available, like customizing the files thumbnail, set a caption message (including
+variables) or configuring a proxy.
+`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info.
+
+💡 Features
+===========
+
+* **Upload** and **download** multiples files  (up to 4 GiB per file for premium users).
+* **Interactive** mode.
+* Add video **thumbs**.
+* **Split** and **join** large files.
+* **Delete** local or remote file on success.
+* Use **variables** in the **caption** message.
+* ... And **more**.
+
+🐋 Docker
+=========
 Run telegram-upload without installing it on your system using Docker. Instead of ``telegram-upload``
 and ``telegram-download`` you should use ``upload`` and ``download``. Usage::
 
 
-    docker run -v <files_dir>:/files/
-               -v <config_dir>:/config
-               -it nekmo/telegram-upload:master
-               <command> <args>
+    $ docker run -v <files_dir>:/files/
+                 -v <config_dir>:/config
+                 -it nekmo/telegram-upload:master
+                 <command> <args>
 
 * ``<files_dir>``: upload or download directory.
 * ``<config_dir>``: Directory that will be created to store the telegram-upload configuration.
   It is created automatically.
 * ``<command>``: ``upload`` and ``download``.
 * ``<args>``: ``telegram-upload`` and ``telegram-download`` arguments.
 
 For example::
 
-    docker run -v /media/data/:/files/
-               -v $PWD/config:/config
-               -it nekmo/telegram-upload:master
-               upload file_to_upload.txt
-
+    $ docker run -v /media/data/:/files/
+                 -v $PWD/config:/config
+                 -it nekmo/telegram-upload:master
+                 upload file_to_upload.txt
+
+❤️ Thanks
+=========
+This project developed by `Nekmo <https://github.com/Nekmo>`_ & `collaborators <https://github.com/Nekmo/telegram-upload/graphs/contributors>`_ would not be possible without
+`Telethon <https://github.com/LonamiWebs/Telethon>`_, the library used as a Telegram client.
 
+Telegram-upload is licensed under the `MIT license <https://github.com/Nekmo/telegram-upload/blob/master/LICENSE>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `telegram-upload-0.6.1/docs/Makefile` & `telegram-upload-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/docs/_static/logo.png` & `telegram-upload-0.7.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/docs/conf.py` & `telegram-upload-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/docs/index.rst` & `telegram-upload-0.7.0/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. toctree::
    :maxdepth: 2
    :glob:
 
    installation
    readme
    usage
+   caption_format
    troubleshooting
    contributing
    authors
    history
 
 
 ..
```

### Comparing `telegram-upload-0.6.1/docs/installation.rst` & `telegram-upload-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/docs/usage.rst` & `telegram-upload-0.7.0/docs/usage.rst`

 * *Files 14% similar despite different names*

```diff
@@ -140,14 +140,37 @@
 
     http://1.2.3.4:80
 
 An example with credentials::
 
     socks4://user:pass@proxy.my.site:1080
 
+Caption message
+===============
+You can add a caption message to the file to upload using the ``--caption`` parameter::
+
+    $ telegram-upload image.jpg --caption "This is a caption"
+
+This parameter support variables using the ``{}`` syntax. For example::
+
+    $ telegram-upload image.jpg --caption "This is a caption for {file.stem.capitalize}"
+
+The ``{file}`` variable is the file path. The ``{file.stem}`` variable is the file name without extension. The
+``{file.stem.capitalize}`` variable is the file name without extension with the first letter in uppercase. The
+``{file}`` variable has attributes for get info about the file like their size, their creation date, their checksums
+(md5, sha1, sha256...), their media info (width, height, artist...) and more. For example::
+
+    $ telegram-upload image.jpg --caption "{file.media.width}x{file.media.height}px {file.media.duration.for_humans}"
+
+If you want to use the ``{}`` syntax in the caption message, you can escape it using the brace twice. For example::
+
+    $ telegram-upload image.jpg --caption "This is a caption with {{}}"
+
+For get more info about the variables, see the :ref:`caption_format` section.
+
 Split files
 ===========
 By default, when trying to **upload** a file larger than the supported size by Telegram, an error will occur. However,
 *Telegram-upload* has different policies for large files using the ``--large-files`` parameter:
 
 * ``fail`` (default): The execution of telegram-upload is stopped and the uploads are not continued.
 * ``split``: The files are split as parts. For example *myfile.tar.00*, *myfile.tar.01*...
@@ -158,23 +181,23 @@
 
     ~$ telegram-upload --large-files <fail|split>
 
 To join the split files using the *split* option, you can use in GNU/Linux:
 
 .. code-block:: bash
 
-    ~ $ cat myfile.tar.* > myfile.tar
+    $ cat myfile.tar.* > myfile.tar
 
 In windows there are different programs like `7z <https://7-zip.org/>`_ or `GSplit <https://www.gdgsoft.com/gsplit>`_.
 
 *Telegram-upload* when downloading split files by default will download the files without joining them. However, the
 **download** policy can be changed using the ``--split-files`` parameter:
 
 * ``keep`` (default): Files are downloaded without joining.
 * ``join``: Downloaded files are merged after downloading. In case of errors, such as missing files, the keep policy
   is used.
 
 The syntax is:
 
 .. code-block::
 
-    ~ $ telegram-download --split-files <keep|join>
+    $ telegram-download --split-files <keep|join>
```

### Comparing `telegram-upload-0.6.1/setup.py` & `telegram-upload-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/telegram_upload/cli.py` & `telegram-upload-0.7.0/telegram_upload/cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/telegram_upload/config.py` & `telegram-upload-0.7.0/telegram_upload/config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/telegram_upload/download_files.py` & `telegram-upload-0.7.0/telegram_upload/download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/telegram_upload/exceptions.py` & `telegram-upload-0.7.0/telegram_upload/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,18 @@
     error_code = 29
 
 
 class TelegramProxyError(TelegramUploadError):
     error_code = 30
 
 
+class TelegramEnvironmentError(TelegramUploadError):
+    error_code = 31
+
+
 def catch(fn):
     def wrap(*args, **kwargs):
         try:
             return fn(*args, **kwargs)
         except InvalidApiFileError as e:
             click.echo('The api_id/api_hash combination is invalid. Re-enter both values.')
             prompt_config(e.config_file)
```

### Comparing `telegram-upload-0.6.1/telegram_upload/management.py` & `telegram-upload-0.7.0/telegram_upload/management.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Console script for telegram-upload."""
 import os
 
 import click
 from telethon.tl.types import User
 
 from telegram_upload.cli import show_checkboxlist, show_radiolist
-from telegram_upload.client import Client, get_message_file_attribute
+from telegram_upload.client import TelegramManagerClient, get_message_file_attribute
 from telegram_upload.config import default_config, CONFIG_FILE
 from telegram_upload.download_files import KeepDownloadSplitFiles, JoinDownloadSplitFiles
 from telegram_upload.exceptions import catch
 from telegram_upload.upload_files import NoDirectoriesFiles, RecursiveFiles, NoLargeFiles, SplitFiles, is_valid_file
 from telegram_upload.utils import async_to_sync, amap, sync_to_async_iterator
 
 
@@ -144,15 +144,15 @@
               help='Sort files by name before upload it. Install the natsort Python package for natural sorting.')
 def upload(files, to, config, delete_on_success, print_file_id, force_file, forward, directories, large_files, caption,
            no_thumbnail, thumbnail_file, proxy, album, interactive, sort):
     """Upload one or more files to Telegram using your personal account.
     The maximum file size is 2 GiB and by default they will be saved in
     your saved messages.
     """
-    client = Client(config or default_config(), proxy=proxy)
+    client = TelegramManagerClient(config or default_config(), proxy=proxy)
     client.start()
     if interactive and not files:
         click.echo('Select the local files to upload:')
         click.echo('[SPACE] Select file [ENTER] Next step')
         files = async_to_sync(interactive_select_local_files())
     if interactive and not files:
         # No files selected. Exiting.
@@ -160,26 +160,26 @@
     if interactive and to is None:
         click.echo('Select the recipient dialog of the files:')
         click.echo('[SPACE] Select dialog [ENTER] Next step')
         to = async_to_sync(interactive_select_dialog(client))
     elif to is None:
         to = 'me'
     files = filter(lambda file: is_valid_file(file, lambda message: click.echo(message, err=True)), files)
-    files = DIRECTORY_MODES[directories](files)
+    files = DIRECTORY_MODES[directories](client, files)
     if directories == 'fail':
         # Validate now
         files = list(files)
     if no_thumbnail:
         thumbnail = False
     elif thumbnail_file:
         thumbnail = thumbnail_file
     else:
         thumbnail = None
     files_cls = LARGE_FILE_MODES[large_files]
-    files = files_cls(files, caption=caption, thumbnail=thumbnail, force_file=force_file)
+    files = files_cls(client, files, caption=caption, thumbnail=thumbnail, force_file=force_file)
     if large_files == 'fail':
         # Validate now
         files = list(files)
     if isinstance(to, str) and to.lstrip("-+").isdigit():
         to = int(to)
     if sort and natsorted:
         files = natsorted(files, key=lambda x: x.name)
@@ -206,15 +206,15 @@
               help='Use interactive mode.')
 def download(from_, config, delete_on_success, proxy, split_files, interactive):
     """Download all the latest messages that are files in a chat, by default download
     from "saved messages". It is recommended to forward the files to download to
     "saved messages" and use parameter ``--delete-on-success``. Forwarded messages will
     be removed from the chat after downloading, such as a download queue.
     """
-    client = Client(config or default_config(), proxy=proxy)
+    client = TelegramManagerClient(config or default_config(), proxy=proxy)
     client.start()
     if not interactive and not from_:
         from_ = 'me'
     elif isinstance(from_, str)  and from_.lstrip("-+").isdigit():
         from_ = int(from_)
     elif interactive and not from_:
         click.echo('Select the dialog of the files to download:')
```

### Comparing `telegram-upload-0.6.1/telegram_upload/upload_files.py` & `telegram-upload-0.7.0/telegram_upload/upload_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import datetime
 import math
 import os
 
 
 import mimetypes
 from io import FileIO, SEEK_SET
-from typing import Union
+from typing import Union, TYPE_CHECKING
 
 import click
+from hachoir.metadata.metadata import RootMetadata
 from hachoir.metadata.video import MP4Metadata
 from telethon.tl.types import DocumentAttributeVideo, DocumentAttributeFilename
 
+from telegram_upload.caption_formatter import CaptionFormatter, FilePath
 from telegram_upload.exceptions import TelegramInvalidFile, ThumbError
 from telegram_upload.utils import scantree, truncate
 from telegram_upload.video import get_video_thumb, video_metadata
 
 mimetypes.init()
 
 
-MAX_FILE_SIZE = 2097152000
-CAPTION_MAX_LENGTH = 1024
+if TYPE_CHECKING:
+    from telegram_upload.client import TelegramManagerClient
 
 
 def is_valid_file(file, error_logger=None):
     error_message = None
     if not os.path.lexists(file):
         error_message = 'File "{}" does not exist.'.format(file)
     elif not os.path.getsize(file):
@@ -32,14 +35,21 @@
     return error_message is None
 
 
 def get_file_mime(file):
     return (mimetypes.guess_type(file)[0] or ('')).split('/')[0]
 
 
+def metadata_has(metadata: RootMetadata, key: str):
+    try:
+        return metadata.has(key)
+    except ValueError:
+        return False
+
+
 def get_file_attributes(file):
     attrs = []
     mime = get_file_mime(file)
     if mime == 'video':
         metadata = video_metadata(file)
         video_meta = metadata
         meta_groups = None
@@ -47,32 +57,33 @@
             # Is mkv
             meta_groups = metadata._MultipleMetadata__groups
         if metadata is not None and not metadata.has('width') and meta_groups:
             video_meta = meta_groups[next(filter(lambda x: x.startswith('video'), meta_groups._key_list))]
         if metadata is not None:
             supports_streaming = isinstance(video_meta, MP4Metadata)
             attrs.append(DocumentAttributeVideo(
-                (0, metadata.get('duration').seconds)[metadata.has('duration')],
-                (0, video_meta.get('width'))[video_meta.has('width')],
-                (0, video_meta.get('height'))[video_meta.has('height')],
+                (0, metadata.get('duration').seconds)[metadata_has(metadata, 'duration')],
+                (0, video_meta.get('width'))[metadata_has(video_meta, 'width')],
+                (0, video_meta.get('height'))[metadata_has(video_meta, 'height')],
                 False,
                 supports_streaming,
             ))
     return attrs
 
 
 def get_file_thumb(file):
     if get_file_mime(file) == 'video':
         return get_video_thumb(file)
 
 
 class UploadFilesBase:
-    def __init__(self, files, thumbnail: Union[str, bool, None] = None, force_file: bool = False,
-                 caption: Union[str, None] = None):
+    def __init__(self, client: 'TelegramManagerClient', files, thumbnail: Union[str, bool, None] = None,
+                 force_file: bool = False, caption: Union[str, None] = None):
         self._iterator = None
+        self.client = client
         self.files = files
         self.thumbnail = thumbnail
         self.force_file = force_file
         self.caption = caption
 
     def get_iterator(self):
         raise NotImplementedError
@@ -106,37 +117,38 @@
             else:
                 yield file
 
 
 class LargeFilesBase(UploadFilesBase):
     def get_iterator(self):
         for file in self.files:
-            if os.path.getsize(file) > MAX_FILE_SIZE:
+            if os.path.getsize(file) > self.client.max_file_size:
                 yield from self.process_large_file(file)
             else:
                 yield self.process_normal_file(file)
 
     def process_normal_file(self, file: str) -> 'File':
-        return File(file, force_file=self.force_file, thumbnail=self.thumbnail, caption=self.caption)
+        return File(self.client, file, force_file=self.force_file, thumbnail=self.thumbnail, caption=self.caption)
 
     def process_large_file(self, file):
         raise NotImplementedError
 
 
 class NoLargeFiles(LargeFilesBase):
     def process_large_file(self, file):
         raise TelegramInvalidFile('"{}" file is too large for Telegram.'.format(file))
 
 
 class File(FileIO):
     force_file = False
 
-    def __init__(self, path: str, force_file: Union[bool, None] = None, thumbnail: Union[str, bool, None] = None,
-                 caption: Union[str, None] = None):
+    def __init__(self, client: 'TelegramManagerClient', path: str, force_file: Union[bool, None] = None,
+                 thumbnail: Union[str, bool, None] = None, caption: Union[str, None] = None):
         super().__init__(path)
+        self.client = client
         self.path = path
         self.force_file = self.force_file if force_file is None else force_file
         self._thumbnail = thumbnail
         self._caption = caption
 
     @property
     def file_name(self):
@@ -152,15 +164,24 @@
 
     @property
     def is_custom_thumbnail(self):
         return self._thumbnail is not False and self._thumbnail is not None
 
     @property
     def file_caption(self) -> str:
-        return truncate(self._caption if self._caption is not None else self.short_name, CAPTION_MAX_LENGTH)
+        """Get file caption. If caption parameter is not set, return file name.
+        If caption is set, format it with CaptionFormatter.
+        Anyways, truncate caption to max_caption_length.
+        """
+        if self._caption is not None:
+            formatter = CaptionFormatter()
+            caption = formatter.format(self._caption, file=FilePath(self.path), now=datetime.datetime.now())
+        else:
+            caption = self.short_name
+        return truncate(caption, self.client.max_caption_length)
 
     def get_thumbnail(self):
         thumb = None
         if self._thumbnail is None and not self.force_file:
             try:
                 thumb = get_file_thumb(self.path)
             except ThumbError as e:
@@ -180,16 +201,16 @@
         else:
             return get_file_attributes(self.path)
 
 
 class SplitFile(File, FileIO):
     force_file = True
 
-    def __init__(self, file: Union[str, bytes, int], max_read_size: int, name: str):
-        super().__init__(file)
+    def __init__(self, client: 'TelegramManagerClient', file: Union[str, bytes, int], max_read_size: int, name: str):
+        super().__init__(client, file)
         self.max_read_size = max_read_size
         self.remaining_size = max_read_size
         self._name = name
 
     def read(self, size: int = -1) -> bytes:
         if size == -1:
             size = self.remaining_size
@@ -220,14 +241,14 @@
         return self.file_name.split('/')[-1]
 
 
 class SplitFiles(LargeFilesBase):
     def process_large_file(self, file):
         file_name = os.path.basename(file)
         total_size = os.path.getsize(file)
-        parts = math.ceil(total_size / MAX_FILE_SIZE)
+        parts = math.ceil(total_size / self.client.max_file_size)
         zfill = int(math.log10(10)) + 1
         for part in range(parts):
-            size = total_size - (part * MAX_FILE_SIZE) if part >= parts - 1 else MAX_FILE_SIZE
-            splitted_file = SplitFile(file, size, '{}.{}'.format(file_name, str(part).zfill(zfill)))
-            splitted_file.seek(MAX_FILE_SIZE * part, split_seek=True)
+            size = total_size - (part * self.client.max_file_size) if part >= parts - 1 else self.client.max_file_size
+            splitted_file = SplitFile(self.client, file, size, '{}.{}'.format(file_name, str(part).zfill(zfill)))
+            splitted_file.seek(self.client.max_file_size * part, split_seek=True)
             yield splitted_file
```

### Comparing `telegram-upload-0.6.1/telegram_upload/video.py` & `telegram-upload-0.7.0/telegram_upload/video.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/telegram_upload.egg-info/PKG-INFO` & `telegram-upload-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: telegram-upload
-Version: 0.6.1
+Version: 0.7.0
 Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
 Home-page: https://github.com/Nekmo/telegram-upload/
 Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
 Author: Nekmo
 Author-email: contacto@nekmo.com
 Keywords: telegram-upload,telegram,upload,video
 Platform: linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
-Provides: tests
 Provides: telegram_upload
+Provides: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
 
@@ -47,102 +47,160 @@
   :target: https://codeclimate.com/github/Nekmo/telegram-upload
   :alt: Code Climate
 
 .. image:: https://img.shields.io/codecov/c/github/Nekmo/telegram-upload/master.svg?style=flat-square
   :target: https://codecov.io/github/Nekmo/telegram-upload
   :alt: Test coverage
 
-.. image:: https://img.shields.io/requires/github/Nekmo/telegram-upload.svg?style=flat-square
-     :target: https://requires.io/github/Nekmo/telegram-upload/requirements/?branch=master
-     :alt: Requirements Status
+.. image:: https://img.shields.io/github/stars/Nekmo/telegram-upload?style=flat-square
+     :target: https://github.com/Nekmo/telegram-upload
+     :alt: Github stars
 
 
 ###############
 telegram-upload
 ###############
-Telegram-upload uses your personal Telegram account to upload and download files up to 2GiB (bots are limited to 50
-MiB). Turn Telegram into your personal cloud!
+Telegram-upload uses your **personal Telegram account** to **upload** and **download** files up to **4 GiB** (2 GiB for
+free users). Turn Telegram into your personal ☁ cloud!
 
-To **install telegram-upload**, run this command in your terminal:
+To **install 🔧 telegram-upload**, run this command in your terminal:
 
 .. code-block:: console
 
     $ sudo pip3 install -U telegram-upload
 
 This is the preferred method to install telegram-upload, as it will always install the most recent stable release.
-`More info in the documentation <https://docs.nekmo.org/telegram-upload/installation.html>`_
-
+🐍 **Python 3.7-3.11** are tested and supported. There are other installation ways available like `Docker <#-docker>`_.
+More info in the `📕 documentation <https://docs.nekmo.org/telegram-upload/installation.html>`_
 
-To use this program you need an Telegram account and your *App api_id/api_hash* (get it in
-`my.telegram.org <https://my.telegram.org/>`_). The first time you use telegram-upload it requests your telephone,
-api_id and api_hash. Bot tokens can not be used with this program (bot uploads are limited to 50MB). To **send files**
-(by default it is uploaded to saved messages):
+.. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/telegram-upload-demo.gif
+  :target: https://asciinema.org/a/592098
+  :width: 100%
 
-.. code-block:: console
+❓ Usage
+========
+To use this program you need an Telegram account and your **App api_id & api_hash** (get it in
+`my.telegram.org <https://my.telegram.org/>`_). The first time you use telegram-upload it requests your
+📱 **telephone**, **api_id** and **api_hash**. Bot tokens can not be used with this program (bot uploads are limited to
+50MB).
 
-    $ telegram-upload file1.mp4 /path/to/file2.mkv
+To **send ⬆️ files** (by default it is uploaded to saved messages):
 
-Credentials are saved in ``~/.config/telegram-upload.json`` and ``~/.config/telegram-upload.session``. You must make
-sure that these files are secured. You can copy these files to authenticate ``telegram-upload`` on more machines, but
-it is advisable to create a session file for each machine. Upload options are available
-`in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-upload>`_.
+.. code-block:: console
 
+    $ telegram-upload file1.mp4 file2.mkv
 
-You can **download the files** again from your saved messages (by default) or from a channel. All files will be
+You can **download ⤵️ the files** again from your saved messages (by default) or from a channel. All files will be
 downloaded until the last text message.
 
 .. code-block:: console
 
     $ telegram-download
 
-The ``--delete-on-success`` option allows you to delete the Telegram message after downloading the file. This is
-useful to send files to download to your saved messages and avoid downloading them again. You can use this option to
-download files on your computer away from home.
-
-`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info.
-
+`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info about the
+options availables.
 
 Interactive mode
-================
+----------------
 The **interactive option** (``--interactive``) allows you to choose the dialog and the files to download or upload with
-a **terminal wizard**. It even **supports mouse**!
+a **terminal 🪄 wizard**. It even **supports mouse**!
 
 .. code-block:: console
 
     $ telegram-upload --interactive    # Interactive upload
     $ telegram-download --interactive  # Interactive download
 
+`More info in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#interactive-mode>`_
 
-Features
-========
+Set group or chat
+-----------------
+By default when using telegram-upload without specifying the recipient or sender, telegram-upload will use your personal
+chat. However you can define the 👨 destination. For file upload the argument is ``--to <entity>``. For example:
+
+.. code-block::
+
+    $ telegram-upload --to telegram.me/joinchat/AAAAAEkk2WdoDrB4-Q8-gg video.mkv
+
+You can download files from a specific chat using the --from <entity> parameter. For example:
 
-* Upload multiples files (up to 2GiB per file)
-* Download files.
-* Add video thumbs.
-* Delete local or remote file on success.
-* ... And more.
+.. code-block::
 
-Docker
-======
+    $ telegram-download --from username
+
+You can see all `the possible values for the entity in the documentation <https://docs.nekmo.org/telegram-upload/usage.html#set-recipient-or-sender>`_.
+
+Split & join files
+------------------
+If you try to upload a file that **exceeds the maximum supported** by Telegram by default, an error will occur. But you
+can enable ✂ **split mode** to upload multiple files:
+
+.. code-block:: console
+
+    $ telegram-upload --large-files split large-video.mkv
+
+Files split using split can be rejoined on download using:
+
+.. code-block:: console
+
+    $ telegram-download --split-files join
+
+Find more help in `the telegram-upload documentation <https://docs.nekmo.org/telegram-upload/usage.html#split-files>`_.
+
+Delete on success
+-----------------
+The ``--delete-on-success`` option allows you to ❌ **delete the Telegram message** after downloading the file. This is
+useful to send files to download to your saved messages and avoid downloading them again. You can use this option to
+download files on your computer away from home.
+
+Configuration
+-------------
+Credentials are saved in ``~/.config/telegram-upload.json`` and ``~/.config/telegram-upload.session``. You must make
+sure that these files are secured. You can copy these 📁 files to authenticate ``telegram-upload`` on more machines, but
+it is advisable to create a session file for each machine.
+
+More options
+------------
+Telegram-upload has more options available, like customizing the files thumbnail, set a caption message (including
+variables) or configuring a proxy.
+`Read the documentation <https://docs.nekmo.org/telegram-upload/usage.html#telegram-download>`_ for more info.
+
+💡 Features
+===========
+
+* **Upload** and **download** multiples files  (up to 4 GiB per file for premium users).
+* **Interactive** mode.
+* Add video **thumbs**.
+* **Split** and **join** large files.
+* **Delete** local or remote file on success.
+* Use **variables** in the **caption** message.
+* ... And **more**.
+
+🐋 Docker
+=========
 Run telegram-upload without installing it on your system using Docker. Instead of ``telegram-upload``
 and ``telegram-download`` you should use ``upload`` and ``download``. Usage::
 
 
-    docker run -v <files_dir>:/files/
-               -v <config_dir>:/config
-               -it nekmo/telegram-upload:master
-               <command> <args>
+    $ docker run -v <files_dir>:/files/
+                 -v <config_dir>:/config
+                 -it nekmo/telegram-upload:master
+                 <command> <args>
 
 * ``<files_dir>``: upload or download directory.
 * ``<config_dir>``: Directory that will be created to store the telegram-upload configuration.
   It is created automatically.
 * ``<command>``: ``upload`` and ``download``.
 * ``<args>``: ``telegram-upload`` and ``telegram-download`` arguments.
 
 For example::
 
-    docker run -v /media/data/:/files/
-               -v $PWD/config:/config
-               -it nekmo/telegram-upload:master
-               upload file_to_upload.txt
-
+    $ docker run -v /media/data/:/files/
+                 -v $PWD/config:/config
+                 -it nekmo/telegram-upload:master
+                 upload file_to_upload.txt
+
+❤️ Thanks
+=========
+This project developed by `Nekmo <https://github.com/Nekmo>`_ & `collaborators <https://github.com/Nekmo/telegram-upload/graphs/contributors>`_ would not be possible without
+`Telethon <https://github.com/LonamiWebs/Telethon>`_, the library used as a Telegram client.
 
+Telegram-upload is licensed under the `MIT license <https://github.com/Nekmo/telegram-upload/blob/master/LICENSE>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `telegram-upload-0.6.1/telegram_upload.egg-info/SOURCES.txt` & `telegram-upload-0.7.0/telegram_upload.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,57 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
+docs/caption_format.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
 docs/troubleshooting.rst
 docs/usage.rst
 docs/_static/logo.png
 telegram_upload/__init__.py
 telegram_upload/_compat.py
+telegram_upload/caption_formatter.py
 telegram_upload/cli.py
-telegram_upload/client.py
 telegram_upload/config.py
 telegram_upload/download_files.py
 telegram_upload/exceptions.py
 telegram_upload/management.py
 telegram_upload/upload_files.py
 telegram_upload/utils.py
 telegram_upload/video.py
 telegram_upload.egg-info/PKG-INFO
 telegram_upload.egg-info/SOURCES.txt
 telegram_upload.egg-info/dependency_links.txt
 telegram_upload.egg-info/entry_points.txt
 telegram_upload.egg-info/not-zip-safe
 telegram_upload.egg-info/requires.txt
 telegram_upload.egg-info/top_level.txt
+telegram_upload/client/__init__.py
+telegram_upload/client/progress_bar.py
+telegram_upload/client/telegram_download_client.py
+telegram_upload/client/telegram_manager_client.py
+telegram_upload/client/telegram_upload_client.py
 tests/__init__.py
 tests/_compat.py
+tests/test_caption_formatter.py
 tests/test_cli.py
-tests/test_client.py
 tests/test_config.py
 tests/test_download_files.py
 tests/test_exceptions.py
 tests/test_files.py
 tests/test_management.py
+tests/test_upload_files.py
 tests/test_utils.py
-tests/test_video.py
+tests/test_video.py
+tests/test_client/__init__.py
+tests/test_client/test_progress_bar.py
+tests/test_client/test_telegram_download_client.py
+tests/test_client/test_telegram_manager_client.py
+tests/test_client/test_telegram_upload_client.py
```

### Comparing `telegram-upload-0.6.1/tests/test_cli.py` & `telegram-upload-0.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/tests/test_config.py` & `telegram-upload-0.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/tests/test_download_files.py` & `telegram-upload-0.7.0/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/tests/test_exceptions.py` & `telegram-upload-0.7.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/tests/test_files.py` & `telegram-upload-0.7.0/tests/test_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import unittest
-from unittest.mock import patch, Mock
+from unittest.mock import patch, Mock, MagicMock
 
+from telegram_upload.client.telegram_manager_client import USER_MAX_FILE_SIZE
 from telegram_upload.exceptions import TelegramInvalidFile
-from telegram_upload.upload_files import get_file_attributes, RecursiveFiles, NoDirectoriesFiles, MAX_FILE_SIZE, \
-    NoLargeFiles, SplitFiles, SplitFile
+from telegram_upload.upload_files import get_file_attributes, RecursiveFiles, NoDirectoriesFiles, NoLargeFiles, \
+    SplitFiles, SplitFile
 
 
 class TestGetFileAttributes(unittest.TestCase):
     def test_not_video(self):
         self.assertEqual(get_file_attributes('foo.png'), [])
 
     @patch('telegram_upload.upload_files.video_metadata')
@@ -25,75 +26,76 @@
         self.assertEqual(attrs[0].duration, 1000)
 
 
 class TestRecursiveFiles(unittest.TestCase):
     @patch('telegram_upload.upload_files.scantree', return_value=[])
     @patch('telegram_upload.upload_files.os.path.isdir', return_value=False)
     def test_one_file(self, m1, m2):
-        self.assertEqual(list(RecursiveFiles(['foo'])), ['foo'])
+        self.assertEqual(list(RecursiveFiles(MagicMock(), ['foo'])), ['foo'])
 
     @patch('telegram_upload.upload_files.scantree')
     @patch('telegram_upload.upload_files.os.path.isdir', return_value=True)
     def test_directory(self, m1, m2):
         directory = Mock()
         directory.is_dir.side_effect = [True, False]
         file = Mock()
         file.is_dir.return_value = False
         side_effect = [file] * 3
         m2.return_value = side_effect
-        self.assertEqual(list(RecursiveFiles(['foo'])), [x.path for x in side_effect])
+        self.assertEqual(list(RecursiveFiles(MagicMock(), ['foo'])), [x.path for x in side_effect])
 
 
 class TestNoDirectoriesFiles(unittest.TestCase):
     @patch('telegram_upload.upload_files.scantree', return_value=[])
     @patch('telegram_upload.upload_files.os.path.isdir', return_value=False)
     def test_one_file(self, m1, m2):
-        self.assertEqual(list(NoDirectoriesFiles(['foo'])), ['foo'])
+        self.assertEqual(list(NoDirectoriesFiles(MagicMock(), ['foo'])), ['foo'])
 
     @patch('telegram_upload.upload_files.os.path.isdir', return_value=True)
     def test_directory(self, m):
         with self.assertRaises(TelegramInvalidFile):
-            next(NoDirectoriesFiles(['foo']))
+            next(NoDirectoriesFiles(MagicMock(), ['foo']))
 
 
 class TestNoLargeFiles(unittest.TestCase):
-    @patch('telegram_upload.upload_files.os.path.getsize', return_value=MAX_FILE_SIZE - 1)
+    @patch('telegram_upload.upload_files.os.path.getsize', return_value=USER_MAX_FILE_SIZE - 1)
     @patch('telegram_upload.upload_files.File')
     def test_small_file(self, m1, m2):
-        self.assertEqual(len(list(NoLargeFiles(['foo']))), 1)
+        self.assertEqual(len(list(NoLargeFiles(MagicMock(max_file_size=USER_MAX_FILE_SIZE), ['foo']))), 1)
 
-    @patch('telegram_upload.upload_files.os.path.getsize', return_value=MAX_FILE_SIZE + 1)
+    @patch('telegram_upload.upload_files.os.path.getsize', return_value=USER_MAX_FILE_SIZE + 1)
     def test_big_file(self, m):
         with self.assertRaises(TelegramInvalidFile):
-            next(NoLargeFiles(['foo']))
+            next(NoLargeFiles(MagicMock(max_file_size=1024 ** 3), ['foo']))
 
 
 class TestSplitFile(unittest.TestCase):
     def test_file(self):
         this_file = os.path.abspath(__file__)
         size = os.path.getsize(this_file)
-        file0 = SplitFile(this_file, size - 100, 'test.py.00')
-        file1 = SplitFile(this_file, 100, 'test.py.01')
+        file0 = SplitFile(MagicMock(), this_file, size - 100, 'test.py.00')
+        file1 = SplitFile(MagicMock(), this_file, 100, 'test.py.01')
         file1.seek(size - 100, split_seek=True)
         with open(this_file, 'rb') as f:
             content = f.read()
         self.assertEqual(file0.readall() + file1.readall(), content)
         self.assertEqual(file0.file_name, 'test.py.00')
         self.assertEqual(file1.file_size, 100)
         file0.close()
         file1.close()
 
 
 class TestSplitFiles(unittest.TestCase):
-    @patch('telegram_upload.upload_files.os.path.getsize', return_value=MAX_FILE_SIZE - 1)
+    @patch('telegram_upload.upload_files.os.path.getsize', return_value=USER_MAX_FILE_SIZE - 1)
     @patch('telegram_upload.upload_files.File')
     def test_small_file(self, m1, m2):
-        self.assertEqual(len(list(SplitFiles(['foo']))), 1)
+        self.assertEqual(len(list(SplitFiles(MagicMock(max_file_size=USER_MAX_FILE_SIZE), ['foo']))), 1)
 
-    @patch('telegram_upload.upload_files.os.path.getsize', return_value=MAX_FILE_SIZE + 1000)
+    @patch('telegram_upload.upload_files.os.path.getsize', return_value=USER_MAX_FILE_SIZE + 1000)
     @patch('telegram_upload.upload_files.SplitFile.__init__', return_value=None)
     @patch('telegram_upload.upload_files.SplitFile.seek')
     def test_big_file(self, m_getsize, m_init, m_seek):
-        files = list(SplitFiles(['foo']))
+        mock_client = MagicMock(max_file_size=USER_MAX_FILE_SIZE)
+        files = list(SplitFiles(mock_client, ['foo']))
         self.assertEqual(len(files), 2)
-        self.assertEqual(m_init.call_args_list[0][0], ('foo', MAX_FILE_SIZE, 'foo.00'))
-        self.assertEqual(m_init.call_args_list[1][0], ('foo', 1000, 'foo.01'))
+        self.assertEqual(m_init.call_args_list[0][0], (mock_client, 'foo', USER_MAX_FILE_SIZE, 'foo.00'))
+        self.assertEqual(m_init.call_args_list[1][0], (mock_client, 'foo', 1000, 'foo.01'))
```

### Comparing `telegram-upload-0.6.1/tests/test_utils.py` & `telegram-upload-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.1/tests/test_video.py` & `telegram-upload-0.7.0/tests/test_video.py`

 * *Files identical despite different names*

