# Comparing `tmp/video_process-0.2.0.tar.gz` & `tmp/video_process-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_process-0.2.0.tar", max compression
+gzip compressed data, was "video_process-0.2.1.tar", max compression
```

## Comparing `video_process-0.2.0.tar` & `video_process-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      453 2023-06-29 04:39:16.921432 video_process-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      125 2023-06-28 09:02:50.789446 video_process-0.2.0/video_process/__init__.py
--rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.0/video_process/graph_builder.py
--rwxr-xr-x   0        0        0     1474 2023-06-29 04:38:45.241540 video_process-0.2.0/video_process/index.py
--rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.2.0/video_process/lib.py
--rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.0/video_process/subtitle.py
--rw-r--r--   0        0        0     3384 2023-06-26 06:38:17.094573 video_process-0.2.0/video_process/utils.py
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      453 2023-06-29 06:26:11.309204 video_process-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-06-28 09:02:50.789446 video_process-0.2.1/video_process/__init__.py
+-rw-r--r--   0        0        0     5517 2023-06-29 03:51:51.970247 video_process-0.2.1/video_process/graph_builder.py
+-rwxr-xr-x   0        0        0     1464 2023-06-29 06:24:47.835149 video_process-0.2.1/video_process/index.py
+-rw-r--r--   0        0        0     1685 2023-06-21 08:58:19.044108 video_process-0.2.1/video_process/lib.py
+-rw-r--r--   0        0        0     1134 2023-06-28 08:59:43.686218 video_process-0.2.1/video_process/subtitle.py
+-rw-r--r--   0        0        0     3384 2023-06-26 06:38:17.094573 video_process-0.2.1/video_process/utils.py
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 video_process-0.2.1/PKG-INFO
```

### Comparing `video_process-0.2.0/video_process/graph_builder.py` & `video_process-0.2.1/video_process/graph_builder.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.0/video_process/index.py` & `video_process-0.2.1/video_process/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         gb.add_bg(body["bg"], x, y)
 
     if body.get("enable_layers"):
         layers = body["layers"]
         for layer in layers:
             gb.add_overlay(layer)
 
-    if body.get("enable_bg_music"):
-        gb.add_bg_music(body["bg_music"])
+    if body.get("enable_bgm"):
+        gb.add_bg_music(body["bgm"])
 
     if body.get("enable_subtitle"):
         print("enable_subtitle")
         set_script_info(body["subtitle"]["subtitle_path"], gb.width, gb.height)
         gb.add_subtitle(body["subtitle"]["subtitle_path"])
     output_path = os.path.join(base_dir, "output.mp4")
     gb.drop_first_frame()
```

### Comparing `video_process-0.2.0/video_process/lib.py` & `video_process-0.2.1/video_process/lib.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.0/video_process/subtitle.py` & `video_process-0.2.1/video_process/subtitle.py`

 * *Files identical despite different names*

### Comparing `video_process-0.2.0/video_process/utils.py` & `video_process-0.2.1/video_process/utils.py`

 * *Files identical despite different names*

