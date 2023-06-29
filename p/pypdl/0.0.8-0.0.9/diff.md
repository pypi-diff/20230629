# Comparing `tmp/pypdl-0.0.8.tar.gz` & `tmp/pypdl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdl-0.0.8.tar", last modified: Thu Jun 29 04:40:22 2023, max compression
+gzip compressed data, was "pypdl-0.0.9.tar", last modified: Thu Jun 29 07:51:16 2023, max compression
```

## Comparing `pypdl-0.0.8.tar` & `pypdl-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 04:40:22.993306 pypdl-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     9384 2023-06-29 04:40:22.991938 pypdl-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8795 2023-06-29 04:38:39.000000 pypdl-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 04:40:22.961466 pypdl-0.0.8/pypdl/
--rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-0.0.8/pypdl/__init__.py
--rw-rw-rw-   0        0        0    13865 2023-06-29 04:38:02.000000 pypdl-0.0.8/pypdl/main.py
--rw-rw-rw-   0        0        0     1227 2023-06-29 04:35:30.000000 pypdl-0.0.8/pypdl/test.py
--rw-rw-rw-   0        0        0    12153 2023-06-28 14:37:57.000000 pypdl-0.0.8/pypdl/test1.py
--rw-rw-rw-   0        0        0     6110 2023-06-28 17:27:57.000000 pypdl-0.0.8/pypdl/utls.py
-drwxrwxrwx   0        0        0        0 2023-06-29 04:40:22.990936 pypdl-0.0.8/pypdl.egg-info/
--rw-rw-rw-   0        0        0     9384 2023-06-29 04:40:22.000000 pypdl-0.0.8/pypdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-29 04:40:22.000000 pypdl-0.0.8/pypdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 04:40:22.000000 pypdl-0.0.8/pypdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 04:40:22.000000 pypdl-0.0.8/pypdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-29 04:40:22.000000 pypdl-0.0.8/pypdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 04:40:22.993306 pypdl-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-06-29 04:39:28.000000 pypdl-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.225355 pypdl-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-03-20 10:21:57.000000 pypdl-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9384 2023-06-29 07:51:16.224249 pypdl-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8795 2023-06-29 04:38:39.000000 pypdl-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.205378 pypdl-0.0.9/pypdl/
+-rw-rw-rw-   0        0        0       30 2023-03-21 10:24:52.000000 pypdl-0.0.9/pypdl/__init__.py
+-rw-rw-rw-   0        0        0    13931 2023-06-29 07:40:46.000000 pypdl-0.0.9/pypdl/main.py
+-rw-rw-rw-   0        0        0     1226 2023-06-29 07:39:20.000000 pypdl-0.0.9/pypdl/test.py
+-rw-rw-rw-   0        0        0    12153 2023-06-28 14:37:57.000000 pypdl-0.0.9/pypdl/test1.py
+-rw-rw-rw-   0        0        0     6110 2023-06-29 07:32:49.000000 pypdl-0.0.9/pypdl/utls.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:51:16.223236 pypdl-0.0.9/pypdl.egg-info/
+-rw-rw-rw-   0        0        0     9384 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 07:51:16.000000 pypdl-0.0.9/pypdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:51:16.225355 pypdl-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-06-29 07:51:06.000000 pypdl-0.0.9/setup.py
```

### Comparing `pypdl-0.0.8/LICENSE` & `pypdl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.8/PKG-INFO` & `pypdl-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
+Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.8/README.md` & `pypdl-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.8/pypdl/main.py` & `pypdl-0.0.9/pypdl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 from reprint import output
 from .utls import Multidown, Singledown, timestring
 
 
 class Downloader:
-    def __init__(self, StopEvent=threading.Event(), headers={}):
+    def __init__(self, StopEvent=None, headers=None):
         """
         Initializes the Downloader object.
 
         Parameters:
             StopEvent (threading.Event): Event to stop the download.
             headers (dict): User headers to be used in the download request.
         """
@@ -32,16 +32,16 @@
         self.progress = 0  # download progress percentage
         self.speed = 0  # download speed in MB/s
         self.download_mode = ""  # download mode: single-threaded or multi-threaded
         self.time_spent = None  # time spent downloading
         self.doneMB = 0  # amount of data downloaded in MB
         self.eta = "99:59:59"  # estimated time remaining for download completion
         self.remaining = 0  # amount of data remaining to be downloaded
-        self.Stop = StopEvent  # event to signal download stop
-        self.headers = headers  # user-defined headers
+        self.Stop = StopEvent if StopEvent else threading.Event() # event to signal download stop
+        self.headers = headers if headers else {} # user-defined headers
         self.Failed = False  # flag to indicate if download failure
 
     def download(self, url, filepath, num_connections, display, multithread):
         """
         Download a file from the given URL.
 
         Parameters:
@@ -138,32 +138,32 @@
         # use reprint library to print dynamic progress output
         with output(initial_len=5, interval=0) as dynamic_print:
             while True:
                 if not singlethread:
                     # save progress to progress file
                     json_file.write_text(json.dumps(self._dic, indent=4))
                 # check if all workers have completed
-                status = sum([i.completed for i in self._workers])
+                status = sum(i.completed for i in self._workers)
                 # get the total amount of data downloaded
                 downloaded = sum(i.curr for i in self._workers)
                 self.doneMB = downloaded / 1048576
                 # keep track of recent download speeds
                 self._recent.append(downloaded)
                 try:
                     # calculate download progress percentage
                     self.progress = int(100 * downloaded / total)
                 except ZeroDivisionError:
                     self.progress = 0
 
                 # calculate download speed
-                gt0 = len([i for i in self._recent if i])
-                if not gt0:
+                recent_speed = len([i for i in self._recent if i])
+                if not recent_speed:
                     self.speed = 0
                 else:
-                    recent = list(self._recent)[12 - gt0:]
+                    recent = list(self._recent)[12 - recent_speed:]
                     if len(recent) == 1:
                         self.speed = recent[0] / 1048576 / interval
                     else:
                         diff = [b - a for a, b in zip(recent, recent[1:])]
                         self.speed = sum(diff) / len(diff) / 1048576 / interval
 
                 # calculate estimated time remaining for download completion
@@ -222,15 +222,15 @@
 
         ended = datetime.now()
         self.time_spent = (ended - started).total_seconds()
 
         # print download result
         if display:
             if self.Stop.is_set():
-                print(f"Task interrupted!")
+                print("Task interrupted!")
             print(f"Time elapsed: {timestring(self.time_spent)}")
 
     def stop(self):
         """
         Stop the download process.
         """
         self.Stop.set()
```

### Comparing `pypdl-0.0.8/pypdl/test.py` & `pypdl-0.0.9/pypdl/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pypdl import Downloader
+from main import Downloader
 import time
 
 if __name__ == "__main__":
     d = Downloader()
     # url = "https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe"
     url = r"https://upcdn.io/kW15bUL/raw/y2mate.com%20-%20How%20to%20make%20dlls%20for%20m%20centers%20Minecraft%20bedrock_1080p.mp4"
     d.headers = {"Authorization": "Bearer public_kW15bUL8oWrFf4ZvEEcU5cGfpMp3"}
```

### Comparing `pypdl-0.0.8/pypdl/test1.py` & `pypdl-0.0.9/pypdl/test1.py`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.8/pypdl/utls.py` & `pypdl-0.0.9/pypdl/utls.py`

 * *Files identical despite different names*

### Comparing `pypdl-0.0.8/pypdl.egg-info/PKG-INFO` & `pypdl-0.0.9/pypdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pypdl
-Version: 0.0.8
+Version: 0.0.9
 Summary: A concurrent python download manager
 Home-page: https://github.com/m-jishnu/pypdl
 Author: m-jishnu
 Author-email: <jishnum499@gmail.com>
 License: MIT
 Keywords: python,downloader,concurrent-downloader,parrel-downloader,download manager,fast-downloader
+Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pypdl
 
 pypdl is a Python library for downloading files from the internet. It provides features such as multi-threaded downloads, retry download incase of failure and option to continue downloading using a different url if necessary, progress tracking, pause/resume functionality and many more.
```

### Comparing `pypdl-0.0.8/setup.py` & `pypdl-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A concurrent python download manager'
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="pypdl",
     version=VERSION,
```

