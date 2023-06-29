# Comparing `tmp/v3io-0.5.8.tar.gz` & `tmp/v3io-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/v3io-0.5.8.tar", last modified: Thu May 27 10:43:09 2021, max compression
+gzip compressed data, was "dist/v3io-0.5.9.tar", last modified: Thu Sep 23 12:08:15 2021, max compression
```

## Comparing `v3io-0.5.8.tar` & `v3io-0.5.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/
--rw-r--r--   0 root         (0) root         (0)       59 2021-05-27 10:42:07.000000 v3io-0.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14026 2021-05-27 10:43:09.000000 v3io-0.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      189 2021-05-27 10:42:07.000000 v3io-0.5.8/Pipfile
--rw-r--r--   0 root         (0) root         (0)    20706 2021-05-27 10:42:56.000000 v3io-0.5.8/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)    13032 2021-05-27 10:42:07.000000 v3io-0.5.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-27 10:43:09.000000 v3io-0.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2748 2021-05-27 10:42:07.000000 v3io-0.5.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/
--rw-r--r--   0 root         (0) root         (0)       22 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/aio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/aio/dataplane/
--rw-r--r--   0 root         (0) root         (0)       79 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3857 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/client.py
--rw-r--r--   0 root         (0) root         (0)     2383 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/container.py
--rw-r--r--   0 root         (0) root         (0)    16508 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/kv.py
--rw-r--r--   0 root         (0) root         (0)     3867 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/kv_cursor.py
--rw-r--r--   0 root         (0) root         (0)     3764 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/object.py
--rw-r--r--   0 root         (0) root         (0)    16106 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/aio/dataplane/transport/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/transport/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3449 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/aio/dataplane/transport/aiohttp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/common/
--rw-r--r--   0 root         (0) root         (0)        0 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      244 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/common/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/dataplane/
--rw-r--r--   0 root         (0) root         (0)       65 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4058 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/batch.py
--rw-r--r--   0 root         (0) root         (0)    45970 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/client.py
--rw-r--r--   0 root         (0) root         (0)     2388 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/container.py
--rw-r--r--   0 root         (0) root         (0)    16482 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/kv.py
--rw-r--r--   0 root         (0) root         (0)     1746 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/kv_array.py
--rw-r--r--   0 root         (0) root         (0)     4008 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/kv_cursor.py
--rw-r--r--   0 root         (0) root         (0)     1035 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/kv_timestamp.py
--rw-r--r--   0 root         (0) root         (0)      170 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/model.py
--rw-r--r--   0 root         (0) root         (0)     3854 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/object.py
--rw-r--r--   0 root         (0) root         (0)     7296 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/output.py
--rw-r--r--   0 root         (0) root         (0)    12180 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/request.py
--rw-r--r--   0 root         (0) root         (0)     1548 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/response.py
--rw-r--r--   0 root         (0) root         (0)    16207 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/dataplane/transport/
--rw-r--r--   0 root         (0) root         (0)      200 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/transport/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2555 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/transport/abstract.py
--rw-r--r--   0 root         (0) root         (0)     7585 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/transport/httpclient.py
--rw-r--r--   0 root         (0) root         (0)     2162 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/transport/requests.py
--rw-r--r--   0 root         (0) root         (0)      742 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/dataplane/transport/verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io/logger/
--rw-r--r--   0 root         (0) root         (0)       62 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2839 2021-05-27 10:42:07.000000 v3io-0.5.8/v3io/logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14026 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1138 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-05-27 10:43:09.000000 v3io-0.5.8/v3io.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/
+-rw-r--r--   0 root         (0) root         (0)       59 2021-09-23 12:07:18.000000 v3io-0.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14026 2021-09-23 12:08:15.000000 v3io-0.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      189 2021-09-23 12:07:18.000000 v3io-0.5.9/Pipfile
+-rw-r--r--   0 root         (0) root         (0)    22788 2021-09-23 12:08:01.000000 v3io-0.5.9/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)    13032 2021-09-23 12:07:18.000000 v3io-0.5.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-09-23 12:08:15.000000 v3io-0.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2748 2021-09-23 12:07:18.000000 v3io-0.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/
+-rw-r--r--   0 root         (0) root         (0)       22 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/aio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/aio/dataplane/
+-rw-r--r--   0 root         (0) root         (0)       79 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/client.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/container.py
+-rw-r--r--   0 root         (0) root         (0)    16508 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/kv.py
+-rw-r--r--   0 root         (0) root         (0)     3888 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/kv_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/object.py
+-rw-r--r--   0 root         (0) root         (0)    16106 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/aio/dataplane/transport/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/transport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/aio/dataplane/transport/aiohttp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      244 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/common/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/dataplane/
+-rw-r--r--   0 root         (0) root         (0)       65 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/batch.py
+-rw-r--r--   0 root         (0) root         (0)    45970 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/client.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/container.py
+-rw-r--r--   0 root         (0) root         (0)    16482 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/kv.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/kv_array.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/kv_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/kv_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)      170 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/model.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/object.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/output.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/request.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2021-09-23 12:07:18.000000 v3io-0.5.9/v3io/dataplane/response.py
+-rw-r--r--   0 root         (0) root         (0)    16207 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/dataplane/transport/
+-rw-r--r--   0 root         (0) root         (0)      200 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/transport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/transport/abstract.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/transport/httpclient.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/transport/requests.py
+-rw-r--r--   0 root         (0) root         (0)      742 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/dataplane/transport/verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io/logger/
+-rw-r--r--   0 root         (0) root         (0)       62 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2021-09-23 12:07:19.000000 v3io-0.5.9/v3io/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14026 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1138 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2021-09-23 12:08:15.000000 v3io-0.5.9/v3io.egg-info/top_level.txt
```

### Comparing `v3io-0.5.8/PKG-INFO` & `v3io-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io
-Version: 0.5.8
+Version: 0.5.9
 Summary: SDK for v3io
 Home-page: https://github.com/v3io/v3io-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `v3io-0.5.8/Pipfile.lock` & `v3io-0.5.9/Pipfile.lock`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9105639730639731%*

 * *Differences: {"'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:2bbf76fd432960138b3ef6dda3dde0544f27cbf8546c458e60baf371917ba9ee', "*

 * *              "'sha256:50b1e4f8446b06f41be7dd6338db18e0990601dce795c2b1686458aa7e8fa7d8'], "*

 * *              "'version': '==2021.5.30'}, 'idna': {'hashes': "*

 * *              "['sha256:14475042e284991034cb48e06f6851428fb14c4dc953acd9be9a5e95c7b6dd7a', "*

 * *              "'sha256:467fbad99067910785144ce333826c71fb0e63a425657295239737f7ecd125f3'], "*

 * *              '\'markers\': "python_v […]*

```diff
@@ -12,189 +12,215 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:1a4995114262bffbc2413b159f2a1a480c969de6e6eb13ee966d470af86af59c",
-                "sha256:719a74fb9e33b9bd44cc7f3a8d94bc35e4049deebe19ba7d8e108280cfd59830"
+                "sha256:2bbf76fd432960138b3ef6dda3dde0544f27cbf8546c458e60baf371917ba9ee",
+                "sha256:50b1e4f8446b06f41be7dd6338db18e0990601dce795c2b1686458aa7e8fa7d8"
             ],
-            "version": "==2020.12.5"
+            "version": "==2021.5.30"
         },
-        "chardet": {
+        "charset-normalizer": {
             "hashes": [
-                "sha256:0d6f53a15db4120f2b08c94f11e7d93d2c911ee118b6b30a04ec3ee8310179fa",
-                "sha256:f864054d66fd9118f2e67044ac8981a54775ec5b67aed0441892edb553d21da5"
+                "sha256:5d209c0a931f215cee683b6445e2d77677e7e75e159f78def0db09d68fafcaa6",
+                "sha256:5ec46d183433dcbd0ab716f2d7f29d8dee50505b3fdb40c6b985c7c4f5a3591f"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==4.0.0"
+            "markers": "python_version >= '3'",
+            "version": "==2.0.6"
         },
         "future": {
             "hashes": [
                 "sha256:b1bead90b70cf6ec3f0710ae53a525360fa360d306a86583adc6bf83a4db537d"
             ],
             "index": "pypi",
             "version": "==0.18.2"
         },
         "idna": {
             "hashes": [
-                "sha256:b307872f855b18632ce0c21c5e45be78c0ea7ae4c15c828c20788b26921eb3f6",
-                "sha256:b97d804b1e9b523befed77c48dacec60e6dcb0b5391d57af6a65a312a90648c0"
+                "sha256:14475042e284991034cb48e06f6851428fb14c4dc953acd9be9a5e95c7b6dd7a",
+                "sha256:467fbad99067910785144ce333826c71fb0e63a425657295239737f7ecd125f3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.10"
+            "markers": "python_version >= '3'",
+            "version": "==3.2"
         },
         "requests": {
             "hashes": [
-                "sha256:27973dd4a904a4f13b263a19c866c13b92a39ed1c964655f025f3f8d3d75b804",
-                "sha256:c210084e36a42ae6b9219e00e48287def368a26d03a048ddad7bfee44f75871e"
+                "sha256:6c1246513ecd5ecd4528a0906f910e8f0f9c6b8ec72030dc9fd154dc1a6efd24",
+                "sha256:b8aa58f8cf793ffd8782d3d8cb19e66ef36f7aba4353eec859e74678b01b07a7"
             ],
             "index": "pypi",
-            "version": "==2.25.1"
+            "version": "==2.26.0"
         },
         "ujson": {
             "hashes": [
-                "sha256:0190d26c0e990c17ad072ec8593647218fe1c675d11089cd3d1440175b568967",
-                "sha256:0ea07fe57f9157118ca689e7f6db72759395b99121c0ff038d2e38649c626fb1",
-                "sha256:30962467c36ff6de6161d784cd2a6aac1097f0128b522d6e9291678e34fb2b47",
-                "sha256:4d6d061563470cac889c0a9fd367013a5dbd8efc36ad01ab3e67a57e56cad720",
-                "sha256:5e1636b94c7f1f59a8ead4c8a7bab1b12cc52d4c21ababa295ffec56b445fd2a",
-                "sha256:7333e8bc45ea28c74ae26157eacaed5e5629dbada32e0103c23eb368f93af108",
-                "sha256:84b1dca0d53b0a8d58835f72ea2894e4d6cf7a5dd8f520ab4cbd698c81e49737",
-                "sha256:91396a585ba51f84dc71c8da60cdc86de6b60ba0272c389b6482020a1fac9394",
-                "sha256:a214ba5a21dad71a43c0f5aef917cd56a2d70bc974d845be211c66b6742a471c",
-                "sha256:aad6d92f4d71e37ea70e966500f1951ecd065edca3a70d3861b37b176dd6702c",
-                "sha256:b3a6dcc660220539aa718bcc9dbd6dedf2a01d19c875d1033f028f212e36d6bb",
-                "sha256:b5c70704962cf93ec6ea3271a47d952b75ae1980d6c56b8496cec2a722075939",
-                "sha256:c615a9e9e378a7383b756b7e7a73c38b22aeb8967a8bfbffd4741f7ffd043c4d",
-                "sha256:d3a87888c40b5bfcf69b4030427cd666893e826e82cc8608d1ba8b4b5e04ea99",
-                "sha256:e2cadeb0ddc98e3963bea266cc5b884e5d77d73adf807f0bda9eca64d1c509d5",
-                "sha256:e390df0dcc7897ffb98e17eae1f4c442c39c91814c298ad84d935a3c5c7a32fa",
-                "sha256:e6e90330670c78e727d6637bb5a215d3e093d8e3570d439fd4922942f88da361",
-                "sha256:eb6b25a7670c7537a5998e695fa62ff13c7f9c33faf82927adf4daa460d5f62e",
-                "sha256:f273a875c0b42c2a019c337631bc1907f6fdfbc84210cc0d1fff0e2019bbfaec",
-                "sha256:f8aded54c2bc554ce20b397f72101737dd61ee7b81c771684a7dd7805e6cca0c",
-                "sha256:fc51e545d65689c398161f07fd405104956ec27f22453de85898fa088b2cd4bb"
+                "sha256:0076de81aadc287f025525969bbc1272703be92933e988e5663a76ec5863628f",
+                "sha256:02f5a6acc5aa5b054c32bdccd17064c2cbd07c81b3a49449589a4552888f1961",
+                "sha256:0d61ae7a505105a16220a4282dbd552bef76968203e5e4f5edfdbb03d3159e3a",
+                "sha256:0db1acd8dbbf120095ce4ab118585219066ea2860332df2385a435c585036cae",
+                "sha256:0ebc82847938e417092fd463e593da39a280fd12585b998e435a2a45bb7a33f7",
+                "sha256:26e299caa9bfc2e532e16de38de2af48cde48258922cda5efc0dd447d42692fc",
+                "sha256:26ebe3ac1e0d18d58e11dbf7cdd0459adcefd5c025ede99be7fceae47bd1bfc6",
+                "sha256:32f4340c8d6a34e7fa1f9447919ebd4b6256afef0965868d51ea3cdf0694a8f7",
+                "sha256:3697cae44a92c2264cf307d4cdd9ea436faa75a009d35a4097362a6bbf221a1b",
+                "sha256:40235c3704ac7f29b24a7a785f856e1c45a567c8cd4b57a025f516733e358972",
+                "sha256:42f8def3e44d880774f644b53b4701a46889a9506e3fdc191c314c9e2e9b2a38",
+                "sha256:50ddff58727cc4f90ade4c818884c4f0fbeeb1f78f764ab2b2bc89cf1f4db126",
+                "sha256:50f413177206373b3568dff28c091b2d8c9145e5e54b0a524d3823293d7a29b8",
+                "sha256:535f1e5b336f7a0573da59bd9352e9cc6a93185bf4b1d96fb3379e07b4fc619a",
+                "sha256:5a885675252e041e19cb92ff76419251fdd1ab4c2ca9766cb3ecfa6ae07884d2",
+                "sha256:5f863b12d27867b733d380a9878fc8c3ad11d3aea8a3650c33e7a8c2a888e1eb",
+                "sha256:6182898d7031d083017f9be47c6d57f9c2155d9f4391b77ed6c020cab8e5a471",
+                "sha256:68088596e237dcda862c1760d1feb2236a8cc36804507a9fcfaa3ed21442ff64",
+                "sha256:6bccfff9910fbe3dae6a17ec080c48fca0bfe939b18e4b2622122109d4d2570d",
+                "sha256:6e8c30186eaa4f982b9b56cad30b173b71aac9d6a393d97cbcbc4ca805e87943",
+                "sha256:74961587e9c1682d3e04fe29e02b67ec9c88cb0c3406ad94cc617d04c6fa6db2",
+                "sha256:78f8da27231b20d589319f743bd65011862691c102922be85c9f27e40656a0f7",
+                "sha256:8ec19982b7a40fb526b8ffd6edfff2c5c10556a54416d554c4bc83b1e4140a4c",
+                "sha256:944dfdfae0cb4e4274a23e5070be913f7ff8f05666d8d143f2356cf873f9a77a",
+                "sha256:99322e08e53580867c9909637747343354b7028a8208dc5df3d09233c8f52c30",
+                "sha256:a6e27ff0f92c719de004b806d84f471fff0157679e57517092b8f89345eb3a79",
+                "sha256:ab70a29914fc202f7c8f6353bb0622b91f878e2892e57a4c7293b341d5a85133",
+                "sha256:adca402a97b8388c378d92c55b2bf4e8402baa5dfa059a85870a41e2f142a0d0",
+                "sha256:b55dde52028f3c426197b9a928618fbb2b548172eb45824ddb19cdcdf8e493f9",
+                "sha256:bac42d0131740b6f1d2b6a15f770c1fef0db97d05aba8564f3c75bb59a9c91c7",
+                "sha256:bc9e2e6933ecec17a7d351116f555caee84b798076a4c5276ab1e8654c83bd90",
+                "sha256:bff484c162bd77877bc9ae6333b0a684493037ce3c5d8b664e8339becf9ad139",
+                "sha256:c53653a12f6ce67b12e7806c190cce1db09c75de31212a5a9adbdbd7a2aba116",
+                "sha256:c7b2643b063f33e5e0d539cf2811793a7df9da525e63483f70c9262a343bd59d",
+                "sha256:c9723a5e2743ded9bc6106cb04f86244dd779ad847d8ac189cfe808ab16946c1",
+                "sha256:cf272e6302c62a42ed0125efcc1d891dd909bcfb3c6aa075d89de209b2b8e930",
+                "sha256:d0abc1526d32ebe2f2b6fefcf82b9ee8661da3f45ecac087beee6aeaa21b39ec",
+                "sha256:d9a0252da73d8b69de60811252cbfde215d76ee6eea935a519e223353352026c",
+                "sha256:dd98d659365fb9271d9f9ba21160670ddfecb93deaec8a5350519a0ab3604654",
+                "sha256:e7c8cffd9e45248569fa576d19b043951a3edc67cbee3dca2a6b77e6998cb1ec",
+                "sha256:fa68b25c987b73fb1c83ece34e52856c2c6da3031384f72638696c56fa8baca9",
+                "sha256:fae1e251d9f9362ebc4adbbb252d0f4a023f66f180390624826fcb1812b808e9",
+                "sha256:ff0ae4b1dc70c3362b04f4127e228b17e84946de611f85b32f565b990762deaf",
+                "sha256:fffe509f556861c7343c6cba57ed05fe7bcf4b48a934a5b946ccb45428cf8883"
             ],
             "index": "pypi",
-            "version": "==4.0.2"
+            "version": "==4.2.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:753a0374df26658f99d826cfe40394a686d05985786d946fbe4165b5148f5a7c",
-                "sha256:a7acd0977125325f516bda9735fa7142b909a8d01e8b2e4c8108d0984e6e0098"
+                "sha256:4987c65554f7a2dbf30c18fd48778ef124af6fab771a377103da0585e2336ece",
+                "sha256:c4fdf4019605b6e5423637e01bc9fe4daef873709a7973e195ceba0a62bbc844"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.5"
+            "version": "==1.26.7"
         }
     },
     "develop": {
         "bleach": {
             "hashes": [
-                "sha256:6123ddc1052673e52bab52cdc955bcb57a015264a1c57d37bea2f6b817af0125",
-                "sha256:98b3170739e5e83dd9dc19633f074727ad848cbedb6026708c8ac2d3b697a433"
+                "sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da",
+                "sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==3.3.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==4.1.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:1a4995114262bffbc2413b159f2a1a480c969de6e6eb13ee966d470af86af59c",
-                "sha256:719a74fb9e33b9bd44cc7f3a8d94bc35e4049deebe19ba7d8e108280cfd59830"
+                "sha256:2bbf76fd432960138b3ef6dda3dde0544f27cbf8546c458e60baf371917ba9ee",
+                "sha256:50b1e4f8446b06f41be7dd6338db18e0990601dce795c2b1686458aa7e8fa7d8"
             ],
-            "version": "==2020.12.5"
+            "version": "==2021.5.30"
         },
         "cffi": {
             "hashes": [
-                "sha256:005a36f41773e148deac64b08f233873a4d0c18b053d37da83f6af4d9087b813",
-                "sha256:04c468b622ed31d408fea2346bec5bbffba2cc44226302a0de1ade9f5ea3d373",
-                "sha256:06d7cd1abac2ffd92e65c0609661866709b4b2d82dd15f611e602b9b188b0b69",
-                "sha256:06db6321b7a68b2bd6df96d08a5adadc1fa0e8f419226e25b2a5fbf6ccc7350f",
-                "sha256:0857f0ae312d855239a55c81ef453ee8fd24136eaba8e87a2eceba644c0d4c06",
-                "sha256:0f861a89e0043afec2a51fd177a567005847973be86f709bbb044d7f42fc4e05",
-                "sha256:1071534bbbf8cbb31b498d5d9db0f274f2f7a865adca4ae429e147ba40f73dea",
-                "sha256:158d0d15119b4b7ff6b926536763dc0714313aa59e320ddf787502c70c4d4bee",
-                "sha256:1bf1ac1984eaa7675ca8d5745a8cb87ef7abecb5592178406e55858d411eadc0",
-                "sha256:1f436816fc868b098b0d63b8920de7d208c90a67212546d02f84fe78a9c26396",
-                "sha256:24a570cd11895b60829e941f2613a4f79df1a27344cbbb82164ef2e0116f09c7",
-                "sha256:24ec4ff2c5c0c8f9c6b87d5bb53555bf267e1e6f70e52e5a9740d32861d36b6f",
-                "sha256:2894f2df484ff56d717bead0a5c2abb6b9d2bf26d6960c4604d5c48bbc30ee73",
-                "sha256:29314480e958fd8aab22e4a58b355b629c59bf5f2ac2492b61e3dc06d8c7a315",
-                "sha256:293e7ea41280cb28c6fcaaa0b1aa1f533b8ce060b9e701d78511e1e6c4a1de76",
-                "sha256:34eff4b97f3d982fb93e2831e6750127d1355a923ebaeeb565407b3d2f8d41a1",
-                "sha256:35f27e6eb43380fa080dccf676dece30bef72e4a67617ffda586641cd4508d49",
-                "sha256:3c3f39fa737542161d8b0d680df2ec249334cd70a8f420f71c9304bd83c3cbed",
-                "sha256:3d3dd4c9e559eb172ecf00a2a7517e97d1e96de2a5e610bd9b68cea3925b4892",
-                "sha256:43e0b9d9e2c9e5d152946b9c5fe062c151614b262fda2e7b201204de0b99e482",
-                "sha256:48e1c69bbacfc3d932221851b39d49e81567a4d4aac3b21258d9c24578280058",
-                "sha256:51182f8927c5af975fece87b1b369f722c570fe169f9880764b1ee3bca8347b5",
-                "sha256:58e3f59d583d413809d60779492342801d6e82fefb89c86a38e040c16883be53",
-                "sha256:5de7970188bb46b7bf9858eb6890aad302577a5f6f75091fd7cdd3ef13ef3045",
-                "sha256:65fa59693c62cf06e45ddbb822165394a288edce9e276647f0046e1ec26920f3",
-                "sha256:681d07b0d1e3c462dd15585ef5e33cb021321588bebd910124ef4f4fb71aef55",
-                "sha256:69e395c24fc60aad6bb4fa7e583698ea6cc684648e1ffb7fe85e3c1ca131a7d5",
-                "sha256:6c97d7350133666fbb5cf4abdc1178c812cb205dc6f41d174a7b0f18fb93337e",
-                "sha256:6e4714cc64f474e4d6e37cfff31a814b509a35cb17de4fb1999907575684479c",
-                "sha256:72d8d3ef52c208ee1c7b2e341f7d71c6fd3157138abf1a95166e6165dd5d4369",
-                "sha256:8ae6299f6c68de06f136f1f9e69458eae58f1dacf10af5c17353eae03aa0d827",
-                "sha256:8b198cec6c72df5289c05b05b8b0969819783f9418e0409865dac47288d2a053",
-                "sha256:99cd03ae7988a93dd00bcd9d0b75e1f6c426063d6f03d2f90b89e29b25b82dfa",
-                "sha256:9cf8022fb8d07a97c178b02327b284521c7708d7c71a9c9c355c178ac4bbd3d4",
-                "sha256:9de2e279153a443c656f2defd67769e6d1e4163952b3c622dcea5b08a6405322",
-                "sha256:9e93e79c2551ff263400e1e4be085a1210e12073a31c2011dbbda14bda0c6132",
-                "sha256:9ff227395193126d82e60319a673a037d5de84633f11279e336f9c0f189ecc62",
-                "sha256:a465da611f6fa124963b91bf432d960a555563efe4ed1cc403ba5077b15370aa",
-                "sha256:ad17025d226ee5beec591b52800c11680fca3df50b8b29fe51d882576e039ee0",
-                "sha256:afb29c1ba2e5a3736f1c301d9d0abe3ec8b86957d04ddfa9d7a6a42b9367e396",
-                "sha256:b85eb46a81787c50650f2392b9b4ef23e1f126313b9e0e9013b35c15e4288e2e",
-                "sha256:bb89f306e5da99f4d922728ddcd6f7fcebb3241fc40edebcb7284d7514741991",
-                "sha256:cbde590d4faaa07c72bf979734738f328d239913ba3e043b1e98fe9a39f8b2b6",
-                "sha256:cc5a8e069b9ebfa22e26d0e6b97d6f9781302fe7f4f2b8776c3e1daea35f1adc",
-                "sha256:cd2868886d547469123fadc46eac7ea5253ea7fcb139f12e1dfc2bbd406427d1",
-                "sha256:d42b11d692e11b6634f7613ad8df5d6d5f8875f5d48939520d351007b3c13406",
-                "sha256:df5052c5d867c1ea0b311fb7c3cd28b19df469c056f7fdcfe88c7473aa63e333",
-                "sha256:f2d45f97ab6bb54753eab54fffe75aaf3de4ff2341c9daee1987ee1837636f1d",
-                "sha256:fd78e5fee591709f32ef6edb9a015b4aa1a5022598e36227500c8f4e02328d9c"
-            ],
-            "version": "==1.14.5"
+                "sha256:06c54a68935738d206570b20da5ef2b6b6d92b38ef3ec45c5422c0ebaf338d4d",
+                "sha256:0c0591bee64e438883b0c92a7bed78f6290d40bf02e54c5bf0978eaf36061771",
+                "sha256:19ca0dbdeda3b2615421d54bef8985f72af6e0c47082a8d26122adac81a95872",
+                "sha256:22b9c3c320171c108e903d61a3723b51e37aaa8c81255b5e7ce102775bd01e2c",
+                "sha256:26bb2549b72708c833f5abe62b756176022a7b9a7f689b571e74c8478ead51dc",
+                "sha256:33791e8a2dc2953f28b8d8d300dde42dd929ac28f974c4b4c6272cb2955cb762",
+                "sha256:3c8d896becff2fa653dc4438b54a5a25a971d1f4110b32bd3068db3722c80202",
+                "sha256:4373612d59c404baeb7cbd788a18b2b2a8331abcc84c3ba40051fcd18b17a4d5",
+                "sha256:487d63e1454627c8e47dd230025780e91869cfba4c753a74fda196a1f6ad6548",
+                "sha256:48916e459c54c4a70e52745639f1db524542140433599e13911b2f329834276a",
+                "sha256:4922cd707b25e623b902c86188aca466d3620892db76c0bdd7b99a3d5e61d35f",
+                "sha256:55af55e32ae468e9946f741a5d51f9896da6b9bf0bbdd326843fec05c730eb20",
+                "sha256:57e555a9feb4a8460415f1aac331a2dc833b1115284f7ded7278b54afc5bd218",
+                "sha256:5d4b68e216fc65e9fe4f524c177b54964af043dde734807586cf5435af84045c",
+                "sha256:64fda793737bc4037521d4899be780534b9aea552eb673b9833b01f945904c2e",
+                "sha256:6d6169cb3c6c2ad50db5b868db6491a790300ade1ed5d1da29289d73bbe40b56",
+                "sha256:7bcac9a2b4fdbed2c16fa5681356d7121ecabf041f18d97ed5b8e0dd38a80224",
+                "sha256:80b06212075346b5546b0417b9f2bf467fea3bfe7352f781ffc05a8ab24ba14a",
+                "sha256:818014c754cd3dba7229c0f5884396264d51ffb87ec86e927ef0be140bfdb0d2",
+                "sha256:8eb687582ed7cd8c4bdbff3df6c0da443eb89c3c72e6e5dcdd9c81729712791a",
+                "sha256:99f27fefe34c37ba9875f224a8f36e31d744d8083e00f520f133cab79ad5e819",
+                "sha256:9f3e33c28cd39d1b655ed1ba7247133b6f7fc16fa16887b120c0c670e35ce346",
+                "sha256:a8661b2ce9694ca01c529bfa204dbb144b275a31685a075ce123f12331be790b",
+                "sha256:a9da7010cec5a12193d1af9872a00888f396aba3dc79186604a09ea3ee7c029e",
+                "sha256:aedb15f0a5a5949ecb129a82b72b19df97bbbca024081ed2ef88bd5c0a610534",
+                "sha256:b315d709717a99f4b27b59b021e6207c64620790ca3e0bde636a6c7f14618abb",
+                "sha256:ba6f2b3f452e150945d58f4badd92310449876c4c954836cfb1803bdd7b422f0",
+                "sha256:c33d18eb6e6bc36f09d793c0dc58b0211fccc6ae5149b808da4a62660678b156",
+                "sha256:c9a875ce9d7fe32887784274dd533c57909b7b1dcadcc128a2ac21331a9765dd",
+                "sha256:c9e005e9bd57bc987764c32a1bee4364c44fdc11a3cc20a40b93b444984f2b87",
+                "sha256:d2ad4d668a5c0645d281dcd17aff2be3212bc109b33814bbb15c4939f44181cc",
+                "sha256:d950695ae4381ecd856bcaf2b1e866720e4ab9a1498cba61c602e56630ca7195",
+                "sha256:e22dcb48709fc51a7b58a927391b23ab37eb3737a98ac4338e2448bef8559b33",
+                "sha256:e8c6a99be100371dbb046880e7a282152aa5d6127ae01783e37662ef73850d8f",
+                "sha256:e9dc245e3ac69c92ee4c167fbdd7428ec1956d4e754223124991ef29eb57a09d",
+                "sha256:eb687a11f0a7a1839719edd80f41e459cc5366857ecbed383ff376c4e3cc6afd",
+                "sha256:eb9e2a346c5238a30a746893f23a9535e700f8192a68c07c0258e7ece6ff3728",
+                "sha256:ed38b924ce794e505647f7c331b22a693bee1538fdf46b0222c4717b42f744e7",
+                "sha256:f0010c6f9d1a4011e429109fda55a225921e3206e7f62a0c22a35344bfd13cca",
+                "sha256:f0c5d1acbfca6ebdd6b1e3eded8d261affb6ddcf2186205518f1428b8569bb99",
+                "sha256:f10afb1004f102c7868ebfe91c28f4a712227fe4cb24974350ace1f90e1febbf",
+                "sha256:f174135f5609428cc6e1b9090f9268f5c8935fddb1b25ccb8255a2d50de6789e",
+                "sha256:f3ebe6e73c319340830a9b2825d32eb6d8475c1dac020b4f0aa774ee3b898d1c",
+                "sha256:f627688813d0a4140153ff532537fbe4afea5a3dffce1f9deb7f91f848a832b5",
+                "sha256:fd4305f86f53dfd8cd3522269ed7fc34856a8ee3709a5e28b2836b2db9d4cd69"
+            ],
+            "version": "==1.14.6"
         },
-        "chardet": {
+        "charset-normalizer": {
             "hashes": [
-                "sha256:0d6f53a15db4120f2b08c94f11e7d93d2c911ee118b6b30a04ec3ee8310179fa",
-                "sha256:f864054d66fd9118f2e67044ac8981a54775ec5b67aed0441892edb553d21da5"
+                "sha256:5d209c0a931f215cee683b6445e2d77677e7e75e159f78def0db09d68fafcaa6",
+                "sha256:5ec46d183433dcbd0ab716f2d7f29d8dee50505b3fdb40c6b985c7c4f5a3591f"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==4.0.0"
+            "markers": "python_version >= '3'",
+            "version": "==2.0.6"
         },
         "colorama": {
             "hashes": [
                 "sha256:5941b2b48a20143d2267e95b1c2a7603ce057ee39fd88e7329b0c292aa16869b",
                 "sha256:9f47eda37229f68eee03b24b9748937c7dc3868f906e8ba69fbcbdd3bc5dc3e2"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.4.4"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0f1212a66329c80d68aeeb39b8a16d54ef57071bf22ff4e521657b27372e327d",
-                "sha256:1e056c28420c072c5e3cb36e2b23ee55e260cb04eee08f702e0edfec3fb51959",
-                "sha256:240f5c21aef0b73f40bb9f78d2caff73186700bf1bc6b94285699aff98cc16c6",
-                "sha256:26965837447f9c82f1855e0bc8bc4fb910240b6e0d16a664bb722df3b5b06873",
-                "sha256:37340614f8a5d2fb9aeea67fd159bfe4f5f4ed535b1090ce8ec428b2f15a11f2",
-                "sha256:3d10de8116d25649631977cb37da6cbdd2d6fa0e0281d014a5b7d337255ca713",
-                "sha256:3d8427734c781ea5f1b41d6589c293089704d4759e34597dce91014ac125aad1",
-                "sha256:7ec5d3b029f5fa2b179325908b9cd93db28ab7b85bb6c1db56b10e0b54235177",
-                "sha256:8e56e16617872b0957d1c9742a3f94b43533447fd78321514abbe7db216aa250",
-                "sha256:de4e5f7f68220d92b7637fc99847475b59154b7a1b3868fb7385337af54ac9ca",
-                "sha256:eb8cc2afe8b05acbd84a43905832ec78e7b3873fb124ca190f574dca7389a87d",
-                "sha256:ee77aa129f481be46f8d92a1a7db57269a2f23052d5f2433b4621bb457081cc9"
+                "sha256:0a7dcbcd3f1913f664aca35d47c1331fce738d44ec34b7be8b9d332151b0b01e",
+                "sha256:1eb7bb0df6f6f583dd8e054689def236255161ebbcf62b226454ab9ec663746b",
+                "sha256:21ca464b3a4b8d8e86ba0ee5045e103a1fcfac3b39319727bc0fc58c09c6aff7",
+                "sha256:34dae04a0dce5730d8eb7894eab617d8a70d0c97da76b905de9efb7128ad7085",
+                "sha256:3520667fda779eb788ea00080124875be18f2d8f0848ec00733c0ec3bb8219fc",
+                "sha256:3c4129fc3fdc0fa8e40861b5ac0c673315b3c902bbdc05fc176764815b43dd1d",
+                "sha256:3fa3a7ccf96e826affdf1a0a9432be74dc73423125c8f96a909e3835a5ef194a",
+                "sha256:5b0fbfae7ff7febdb74b574055c7466da334a5371f253732d7e2e7525d570498",
+                "sha256:695104a9223a7239d155d7627ad912953b540929ef97ae0c34c7b8bf30857e89",
+                "sha256:8695456444f277af73a4877db9fc979849cd3ee74c198d04fc0776ebc3db52b9",
+                "sha256:94cc5ed4ceaefcbe5bf38c8fba6a21fc1d365bb8fb826ea1688e3370b2e24a1c",
+                "sha256:94fff993ee9bc1b2440d3b7243d488c6a3d9724cc2b09cdb297f6a886d040ef7",
+                "sha256:9965c46c674ba8cc572bc09a03f4c649292ee73e1b683adb1ce81e82e9a6a0fb",
+                "sha256:a00cf305f07b26c351d8d4e1af84ad7501eca8a342dedf24a7acb0e7b7406e14",
+                "sha256:a305600e7a6b7b855cd798e00278161b681ad6e9b7eca94c721d5f588ab212af",
+                "sha256:cd65b60cfe004790c795cc35f272e41a3df4631e2fb6b35aa7ac6ef2859d554e",
+                "sha256:d2a6e5ef66503da51d2110edf6c403dc6b494cc0082f85db12f54e9c5d4c3ec5",
+                "sha256:d9ec0e67a14f9d1d48dd87a2531009a9b251c02ea42851c060b25c782516ff06",
+                "sha256:f44d141b8c4ea5eb4dbc9b3ad992d45580c1d22bf5e24363f2fbf50c2d7ae8a7"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.4.7"
+            "version": "==3.4.8"
         },
         "docutils": {
             "hashes": [
                 "sha256:686577d2e4c32380bb50cbb22f575ed742d58168cee37e99117a854bcd88f125",
                 "sha256:cf316c8370a737a022b72b56874f6602acf974a37a9fba42ec2876387549fc61"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -206,65 +232,65 @@
                 "sha256:bf8fd333346d844f616e8d47905ef3a3384edae6b4e9beb0c5101e25e3110907"
             ],
             "index": "pypi",
             "version": "==3.9.2"
         },
         "idna": {
             "hashes": [
-                "sha256:b307872f855b18632ce0c21c5e45be78c0ea7ae4c15c828c20788b26921eb3f6",
-                "sha256:b97d804b1e9b523befed77c48dacec60e6dcb0b5391d57af6a65a312a90648c0"
+                "sha256:14475042e284991034cb48e06f6851428fb14c4dc953acd9be9a5e95c7b6dd7a",
+                "sha256:467fbad99067910785144ce333826c71fb0e63a425657295239737f7ecd125f3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.10"
+            "markers": "python_version >= '3'",
+            "version": "==3.2"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:057e92c15bc8d9e8109738a48db0ccb31b4d9d5cfbee5a8670879a30be66304b",
-                "sha256:b7e52a1f8dec14a75ea73e0891f3060099ca1d8e6a462a4dff11c3e119ea1b31"
+                "sha256:b618b6d2d5ffa2f16add5697cf57a46c76a56229b0ed1c438322e4e95645bd15",
+                "sha256:f284b3e11256ad1e5d03ab86bb2ccd6f5339688ff17a4d797a0fe7df326f23b1"
             ],
             "markers": "python_version < '3.8'",
-            "version": "==4.2.0"
+            "version": "==4.8.1"
         },
         "jeepney": {
             "hashes": [
-                "sha256:7d59b6622675ca9e993a6bd38de845051d315f8b0c72cca3aef733a20b648657",
-                "sha256:aec56c0eb1691a841795111e184e13cad504f7703b9a64f63020816afa79a8ae"
+                "sha256:1b5a0ea5c0e7b166b2f5895b91a08c14de8915afda4407fb5022a195224958ac",
+                "sha256:fa9e232dfa0c498bd0b8a3a73b8d8a31978304dcef0515adc859d4e096f96f4f"
             ],
             "markers": "sys_platform == 'linux'",
-            "version": "==0.6.0"
+            "version": "==0.7.1"
         },
         "keyring": {
             "hashes": [
-                "sha256:045703609dd3fccfcdb27da201684278823b72af515aedec1a8515719a038cb8",
-                "sha256:8f607d7d1cc502c43a932a275a56fe47db50271904513a379d39df1af277ac48"
+                "sha256:6334aee6073db2fb1f30892697b1730105b5e9a77ce7e61fca6b435225493efe",
+                "sha256:bd2145a237ed70c8ce72978b497619ddfcae640b6dcf494402d5143e37755c6e"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==23.0.1"
+            "version": "==23.2.1"
         },
         "mccabe": {
             "hashes": [
                 "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
                 "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
             ],
             "version": "==0.6.1"
         },
         "packaging": {
             "hashes": [
-                "sha256:5b327ac1320dc863dca72f4514ecc086f31186744b84a230374cc1fd776feae5",
-                "sha256:67714da7f7bc052e064859c05c595155bd1ee9f69f76557e21f051443c20947a"
+                "sha256:7dc96269f53a4ccec5c0670940a4281106dd0bb343f47b7471f779df49c2fbe7",
+                "sha256:c86254f9220d55e31cc94d69bade760f0847da8000def4dfe1c6b872fd14ff14"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==20.9"
+            "markers": "python_version >= '3.6'",
+            "version": "==21.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:029a70cb45c6171c329dfc890cde0879f8c52d6f3922794796e06f577bb03db4",
-                "sha256:9fdbea6495622e022cc72c2e5e1b735218e4ffb2a2a69cde2694a6c1f16afb75"
+                "sha256:37ecd857b47e5f55949c41ed061eb51a0bee97a87c969219d144c0e023982779",
+                "sha256:e7432f81d08adec7297633191bbf0bd47faf13cd8724c3a13250e51d542635bd"
             ],
-            "version": "==1.7.0"
+            "version": "==1.7.1"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:514f76d918fcc0b55c6680472f0a37970994e07bbb80725808c17089be302068",
                 "sha256:c389c1d06bf7904078ca03399a4816f974a1d590090fecea0c63ec26ebaf1cef"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -284,19 +310,19 @@
                 "sha256:f5bc8ecabc05bb9d291eb5203d6810b49040f6ff446a756326104746cc00c1db"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.3.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:a18f47b506a429f6f4b9df81bb02beab9ca21d0a5fee38ed15aef65f0545519f",
-                "sha256:d66e804411278594d764fc69ec36ec13d9ae9147193a1740cd34d272ca383b8e"
+                "sha256:b8e67fe6af78f492b3c4b3e2970c0624cbf08beb1e493b2c99b9fa1b67a20380",
+                "sha256:f398865f7eb6874156579fdf36bc840a03cab64d1cde9e93d68f46a425ec52c6"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==2.9.0"
+            "version": "==2.10.0"
         },
         "pyparsing": {
             "hashes": [
                 "sha256:c203ec8783bf771a155b207279b9bccb8dea02d8f0c9e5f8ead507bc3246ecc1",
                 "sha256:ef9d7589ef3c200abe66653d3f1ab1033c3c419ae9b9bdb1240a85b024efc88b"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2'",
@@ -307,19 +333,19 @@
                 "sha256:63b4075c6698fcfa78e584930f07f39e05d46f3ec97f65006e430b595ca6348c",
                 "sha256:92fd5ac2bf8677f310f3303aa4bce5b9d5f9f2094ab98c29f13791d7b805a3db"
             ],
             "version": "==29.0"
         },
         "requests": {
             "hashes": [
-                "sha256:27973dd4a904a4f13b263a19c866c13b92a39ed1c964655f025f3f8d3d75b804",
-                "sha256:c210084e36a42ae6b9219e00e48287def368a26d03a048ddad7bfee44f75871e"
+                "sha256:6c1246513ecd5ecd4528a0906f910e8f0f9c6b8ec72030dc9fd154dc1a6efd24",
+                "sha256:b8aa58f8cf793ffd8782d3d8cb19e66ef36f7aba4353eec859e74678b01b07a7"
             ],
             "index": "pypi",
-            "version": "==2.25.1"
+            "version": "==2.26.0"
         },
         "requests-toolbelt": {
             "hashes": [
                 "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
                 "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
             ],
             "version": "==0.9.1"
@@ -345,55 +371,55 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'",
             "version": "==1.16.0"
         },
         "tqdm": {
             "hashes": [
-                "sha256:736524215c690621b06fc89d0310a49822d75e599fcd0feb7cc742b98d692493",
-                "sha256:cd5791b5d7c3f2f1819efc81d36eb719a38e0906a7380365c556779f585ea042"
+                "sha256:8dd278a422499cd6b727e6ae4061c40b48fce8b76d1ccbf5d34fca9b7f925b0c",
+                "sha256:d359de7217506c9851b7869f3708d8ee53ed70a1b8edbba4dbcb47442592920d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.61.0"
+            "version": "==4.62.3"
         },
         "twine": {
             "hashes": [
-                "sha256:16f706f2f1687d7ce30e7effceee40ed0a09b7c33b9abb5ef6434e5551565d83",
-                "sha256:a56c985264b991dc8a8f4234eb80c5af87fa8080d0c224ad8f2cd05a2c22e83b"
+                "sha256:087328e9bb405e7ce18527a2dca4042a84c7918658f951110b38bc135acab218",
+                "sha256:4caec0f1ed78dc4c9b83ad537e453d03ce485725f2aea57f1bb3fdde78dae936"
             ],
             "index": "pypi",
-            "version": "==3.4.1"
+            "version": "==3.4.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:0ac0f89795dd19de6b97debb0c6af1c70987fd80a2d62d1958f7e56fcc31b497",
-                "sha256:50b6f157849174217d0656f99dc82fe932884fb250826c18350e159ec6cdf342",
-                "sha256:779383f6086d90c99ae41cf0ff39aac8a7937a9283ce0a414e5dd782f4c94a84"
+                "sha256:49f75d16ff11f1cd258e1b988ccff82a3ca5570217d7ad8c5f48205dd99a677e",
+                "sha256:d8226d10bc02a29bcc81df19a26e56a9647f8b0a6d4a83924139f4a8b01f17b7",
+                "sha256:f1d25edafde516b146ecd0613dabcc61409817af4766fbbcfb8d1ad4ec441a34"
             ],
             "markers": "python_version < '3.8'",
-            "version": "==3.10.0.0"
+            "version": "==3.10.0.2"
         },
         "urllib3": {
             "hashes": [
-                "sha256:753a0374df26658f99d826cfe40394a686d05985786d946fbe4165b5148f5a7c",
-                "sha256:a7acd0977125325f516bda9735fa7142b909a8d01e8b2e4c8108d0984e6e0098"
+                "sha256:4987c65554f7a2dbf30c18fd48778ef124af6fab771a377103da0585e2336ece",
+                "sha256:c4fdf4019605b6e5423637e01bc9fe4daef873709a7973e195ceba0a62bbc844"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.5"
+            "version": "==1.26.7"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:3607921face881ba3e026887d8150cca609d517579abe052ac81fc5aeffdbd76",
-                "sha256:51cb66cc54621609dd593d1787f286ee42a5c0adbb4b29abea5a63edc3e03098"
+                "sha256:957cfda87797e389580cb8b9e3870841ca991e2125350677b2ca83a0e99390a3",
+                "sha256:f5812b1e007e48cff63449a5e9f4e7ebea716b4111f9c4f9a645f91d579bf0c4"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.4.1"
+            "version": "==3.5.0"
         }
     }
 }
```

### Comparing `v3io-0.5.8/README.md` & `v3io-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/setup.py` & `v3io-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/client.py` & `v3io-0.5.9/v3io/aio/dataplane/client.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/container.py` & `v3io-0.5.9/v3io/aio/dataplane/container.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/kv.py` & `v3io-0.5.9/v3io/aio/dataplane/kv.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/kv_cursor.py` & `v3io-0.5.9/v3io/aio/dataplane/kv_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                                                              calculated_limit,
                                                              self.segment,
                                                              self.total_segments,
                                                              self.sort_key_range_start,
                                                              self.sort_key_range_end)
 
         # raise if there was an issue
-        self._current_response.raise_for_status()
+        self._current_response.raise_for_status(self.raise_for_status)
 
         # set items
         self._current_items = self._current_response.output.items
         self._current_item_index = 0
 
         # and recurse into next now that we repopulated response
         return await self.next_item()
```

### Comparing `v3io-0.5.8/v3io/aio/dataplane/object.py` & `v3io-0.5.9/v3io/aio/dataplane/object.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/stream.py` & `v3io-0.5.9/v3io/aio/dataplane/stream.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/aio/dataplane/transport/aiohttp.py` & `v3io-0.5.9/v3io/aio/dataplane/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/batch.py` & `v3io-0.5.9/v3io/dataplane/batch.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/client.py` & `v3io-0.5.9/v3io/dataplane/client.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/container.py` & `v3io-0.5.9/v3io/dataplane/container.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/kv.py` & `v3io-0.5.9/v3io/dataplane/kv.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/kv_array.py` & `v3io-0.5.9/v3io/dataplane/kv_array.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/kv_cursor.py` & `v3io-0.5.9/v3io/dataplane/kv_cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                                                        calculated_limit,
                                                        self.segment,
                                                        self.total_segments,
                                                        self.sort_key_range_start,
                                                        self.sort_key_range_end)
 
         # raise if there was an issue
-        self._current_response.raise_for_status()
+        self._current_response.raise_for_status(self.raise_for_status)
 
         # set items
         self._current_items = self._current_response.output.items
         self._current_item_index = 0
 
         # and recurse into next now that we repopulated response
         return self.next_item()
```

### Comparing `v3io-0.5.8/v3io/dataplane/kv_timestamp.py` & `v3io-0.5.9/v3io/dataplane/kv_timestamp.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/object.py` & `v3io-0.5.9/v3io/dataplane/object.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/output.py` & `v3io-0.5.9/v3io/dataplane/output.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/request.py` & `v3io-0.5.9/v3io/dataplane/request.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/response.py` & `v3io-0.5.9/v3io/dataplane/response.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/stream.py` & `v3io-0.5.9/v3io/dataplane/stream.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/transport/abstract.py` & `v3io-0.5.9/v3io/dataplane/transport/abstract.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/transport/httpclient.py` & `v3io-0.5.9/v3io/dataplane/transport/httpclient.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/transport/requests.py` & `v3io-0.5.9/v3io/dataplane/transport/requests.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/dataplane/transport/verifier.py` & `v3io-0.5.9/v3io/dataplane/transport/verifier.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io/logger/logger.py` & `v3io-0.5.9/v3io/logger/logger.py`

 * *Files identical despite different names*

### Comparing `v3io-0.5.8/v3io.egg-info/PKG-INFO` & `v3io-0.5.9/v3io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io
-Version: 0.5.8
+Version: 0.5.9
 Summary: SDK for v3io
 Home-page: https://github.com/v3io/v3io-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `v3io-0.5.8/v3io.egg-info/SOURCES.txt` & `v3io-0.5.9/v3io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

