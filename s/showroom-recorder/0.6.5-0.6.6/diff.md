# Comparing `tmp/showroom-recorder-0.6.5.tar.gz` & `tmp/showroom-recorder-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.6.5.tar", last modified: Tue Jun 27 16:06:00 2023, max compression
+gzip compressed data, was "showroom-recorder-0.6.6.tar", last modified: Thu Jun 29 16:46:44 2023, max compression
```

## Comparing `showroom-recorder-0.6.5.tar` & `showroom-recorder-0.6.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      562 2023-06-27 12:42:56.000000 showroom-recorder-0.6.5/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.293148 showroom-recorder-0.6.5/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-27 14:29:02.000000 showroom-recorder-0.6.5/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3497 2023-06-27 14:25:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     2970 2023-06-27 16:03:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/uploader.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     9597 2023-06-27 13:26:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     5519 2023-06-27 12:53:30.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-25 15:22:32.000000 showroom-recorder-0.6.5/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-27 16:05:21.000000 showroom-recorder-0.6.5/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      835 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       66 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-27 16:06:00.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-26 11:29:31.000000 showroom-recorder-0.6.5/src/showroom_recorder.egg-info/zip-safe
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-27 16:06:00.297148 showroom-recorder-0.6.5/test/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      424 2023-06-27 14:26:00.000000 showroom-recorder-0.6.5/test/test_config.py
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    35149 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/LICENSE
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       53 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1307 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/PKG-INFO
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1394 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/README.md
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      964 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/description.md
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       38 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/setup.cfg
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1175 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/setup.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      562 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       48 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      185 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     3497 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        0 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    31904 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     2973 2023-06-29 16:38:34.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/uploader.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     9677 2023-06-29 16:35:11.000000 showroom-recorder-0.6.6/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        0 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     5538 2023-06-29 16:35:28.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)    16581 2023-06-26 14:07:51.000000 showroom-recorder-0.6.6/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       46 2023-06-29 16:40:29.000000 showroom-recorder-0.6.6/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.512138 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)     1307 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      835 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        1 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       71 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       66 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)       18 2023-06-29 16:46:44.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)        1 2023-06-26 14:12:42.000000 showroom-recorder-0.6.6/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1002) vacabun   (1002)        0 2023-06-29 16:46:44.516138 showroom-recorder-0.6.6/test/
+-rw-rw-r--   0 vacabun   (1002) vacabun   (1002)      424 2023-06-27 14:38:51.000000 showroom-recorder-0.6.6/test/test_config.py
```

### Comparing `showroom-recorder-0.6.5/LICENSE` & `showroom-recorder-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/PKG-INFO` & `showroom-recorder-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.5
+Version: 0.6.6
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.5/README.md` & `showroom-recorder-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/description.md` & `showroom-recorder-0.6.6/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/setup.py` & `showroom-recorder-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/showroom-recorder.json` & `showroom-recorder-0.6.6/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/common.py` & `showroom-recorder-0.6.6/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.6.6/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/processor/uploader.py` & `showroom-recorder-0.6.6/src/showroom_recorder/processor/uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 import time
 import os
 from webdav4.client import Client
 from biliup.plugins.bili_webup import BiliBili, Data
 
 
 class UploaderBili:
-    def __init__(self, file_path, room_url_key, room_name, time_str, login_cookie):
+    def __init__(self, file_path, room_url_key, room_name, time_str, login_cookie, lines='AUTO'):
         self.file_path = file_path
         self.room_url_key = room_url_key
         self.room_name = room_name
         self.time_str = time_str
         self.login_cookie = login_cookie
+        self.lines = lines
 
     def upload(self):
         logging.info('upload by biliup.')
         video = Data()
         video.title = self.room_name + ' showroom ' + self.time_str
-        video.desc = self.room_name + ' showroom ' + self.time_str
+        video.desc = ''
         video.source = 'https://www.showroom-live.com/' + self.room_url_key
         video.tid = 137
         video.set_tag(['showroom'])
         video.copyright = 2
-        lines = 'AUTO'
-        tasks = 3
+        lines = self.lines
+        tasks = 32
         dtime = 0
         file_list = [self.file_path]
         try:
             with BiliBili(video) as bili:
                 bili.login("bili.cookie", self.login_cookie)
                 # bili.login_by_password("username", "password")
                 for file in file_list:
```

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.6.6/src/showroom_recorder/processor/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,16 @@
                 room_url_key=self.room_url_key, output=self.output))
 
             if self.upload_to_bilibili:
                 uploader_bili = UploaderBili(file_path=self.output,
                                              room_url_key=self.room_url_key,
                                              room_name=self.room_name,
                                              time_str=self.time_str,
-                                             login_cookie=get_bili_cookie('bili_cookie.json'))
+                                             login_cookie=get_bili_cookie('bili_cookie.json'),
+                                             lines=self.config['biliup_lines'])
                 self.uploader_queue.put(uploader_bili)
 
             if self.config['upload_webdav']:
                 uploader_webdav = UploaderWebDav(self.output,
                                                  self.output,
                                                  self.config['webdav_url'],
                                                  self.config['webdav_username'],
```

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.6.6/src/showroom_recorder/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 [video_settings]
 interval = 10
 upload_webdav = 0
 webdav_delete_source_file = 0
 webdav_url = http://webdav_url
 webdav_username = username
 webdav_password = password
-
+biliup_lines = AUTO
 """
     # create file if not present
     path = os.getcwd()
     filenamepath = os.path.join(path, filename)
     if not os.path.isfile(filenamepath):
         with open(filenamepath, 'w', encoding='utf8') as fp:
             fp.write(settingsTxt)
```

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.6.6/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.6.6/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.6.5
+Version: 0.6.6
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.6.5/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.6.6/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

