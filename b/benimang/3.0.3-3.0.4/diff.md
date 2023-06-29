# Comparing `tmp/benimang-3.0.3.tar.gz` & `tmp/benimang-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-3.0.3.tar", last modified: Thu Jun 29 02:23:59 2023, max compression
+gzip compressed data, was "benimang-3.0.4.tar", last modified: Thu Jun 29 07:13:21 2023, max compression
```

## Comparing `benimang-3.0.3.tar` & `benimang-3.0.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 02:23:59.223030 benimang-3.0.3/
--rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-3.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-06-29 02:23:59.222030 benimang-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-3.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 02:23:59.215029 benimang-3.0.3/beni/
--rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-3.0.3/beni/__init__.py
--rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-3.0.3/beni/bbyte.py
--rw-rw-rw-   0        0        0     5745 2023-06-29 02:16:56.000000 benimang-3.0.3/beni/bcache.py
--rw-rw-rw-   0        0        0    11460 2023-06-29 01:45:35.000000 benimang-3.0.3/beni/bcmd.py
--rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-3.0.3/beni/bcolor.py
--rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-3.0.3/beni/bexecute.py
--rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-3.0.3/beni/bfile.py
--rw-rw-rw-   0        0        0     4482 2023-06-29 02:19:04.000000 benimang-3.0.3/beni/bfunc.py
--rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-3.0.3/beni/bhash.py
--rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-3.0.3/beni/bhttp.py
--rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-3.0.3/beni/binput.py
--rw-rw-rw-   0        0        0     5695 2023-06-26 06:18:37.000000 benimang-3.0.3/beni/block.py
--rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-3.0.3/beni/blog.py
--rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-3.0.3/beni/bpath.py
--rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-3.0.3/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-3.0.3/beni/bprogress.py
--rw-rw-rw-   0        0        0     3373 2023-06-29 01:32:58.000000 benimang-3.0.3/beni/bqiniu.py
--rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-3.0.3/beni/bsqlite.py
--rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-3.0.3/beni/bstorage.py
--rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-3.0.3/beni/btable.py
--rw-rw-rw-   0        0        0     4987 2023-06-29 01:28:43.000000 benimang-3.0.3/beni/btask.py
--rw-rw-rw-   0        0        0     1420 2023-06-27 03:36:08.000000 benimang-3.0.3/beni/btime.py
--rw-rw-rw-   0        0        0      295 2023-06-29 01:20:30.000000 benimang-3.0.3/beni/btype.py
--rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-3.0.3/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-06-29 02:23:59.220029 benimang-3.0.3/benimang.egg-info/
--rw-rw-rw-   0        0        0      258 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-29 02:23:59.000000 benimang-3.0.3/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-06-29 02:23:27.000000 benimang-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 02:23:59.223030 benimang-3.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 02:23:59.221028 benimang-3.0.3/test/
--rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-3.0.3/test/test_sample.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:13:21.528899 benimang-3.0.4/
+-rw-rw-rw-   0        0        0       29 2023-05-30 09:18:28.000000 benimang-3.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      258 2023-06-29 07:13:21.528899 benimang-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:13:21.520898 benimang-3.0.4/beni/
+-rw-rw-rw-   0        0        0        0 2023-05-30 09:18:28.000000 benimang-3.0.4/beni/__init__.py
+-rw-rw-rw-   0        0        0     6350 2023-06-29 02:15:26.000000 benimang-3.0.4/beni/bbyte.py
+-rw-rw-rw-   0        0        0     5783 2023-06-29 07:11:14.000000 benimang-3.0.4/beni/bcache.py
+-rw-rw-rw-   0        0        0    11460 2023-06-29 07:06:28.000000 benimang-3.0.4/beni/bcmd.py
+-rw-rw-rw-   0        0        0     1941 2023-06-09 08:30:18.000000 benimang-3.0.4/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-06-29 07:09:07.000000 benimang-3.0.4/beni/bdefine.py
+-rw-rw-rw-   0        0        0     2423 2023-06-26 06:18:37.000000 benimang-3.0.4/beni/bexecute.py
+-rw-rw-rw-   0        0        0     1908 2023-06-29 01:45:33.000000 benimang-3.0.4/beni/bfile.py
+-rw-rw-rw-   0        0        0     4482 2023-06-29 02:19:04.000000 benimang-3.0.4/beni/bfunc.py
+-rw-rw-rw-   0        0        0     1029 2023-06-28 03:38:59.000000 benimang-3.0.4/beni/bhash.py
+-rw-rw-rw-   0        0        0     5745 2023-06-26 09:08:25.000000 benimang-3.0.4/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2583 2023-06-13 01:57:12.000000 benimang-3.0.4/beni/binput.py
+-rw-rw-rw-   0        0        0     5695 2023-06-26 06:18:37.000000 benimang-3.0.4/beni/block.py
+-rw-rw-rw-   0        0        0     3989 2023-06-29 01:25:39.000000 benimang-3.0.4/beni/blog.py
+-rw-rw-rw-   0        0        0     5790 2023-06-29 01:32:58.000000 benimang-3.0.4/beni/bpath.py
+-rw-rw-rw-   0        0        0     2450 2023-06-29 01:26:10.000000 benimang-3.0.4/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1058 2023-06-27 03:17:47.000000 benimang-3.0.4/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3373 2023-06-29 01:32:58.000000 benimang-3.0.4/beni/bqiniu.py
+-rw-rw-rw-   0        0        0     9866 2023-06-29 01:31:14.000000 benimang-3.0.4/beni/bsqlite.py
+-rw-rw-rw-   0        0        0      759 2023-06-29 01:45:35.000000 benimang-3.0.4/beni/bstorage.py
+-rw-rw-rw-   0        0        0     1981 2023-06-26 02:57:46.000000 benimang-3.0.4/beni/btable.py
+-rw-rw-rw-   0        0        0     4987 2023-06-29 01:28:43.000000 benimang-3.0.4/beni/btask.py
+-rw-rw-rw-   0        0        0     1378 2023-06-29 07:10:32.000000 benimang-3.0.4/beni/btime.py
+-rw-rw-rw-   0        0        0      295 2023-06-29 01:20:30.000000 benimang-3.0.4/beni/btype.py
+-rw-rw-rw-   0        0        0     2392 2023-06-29 02:21:02.000000 benimang-3.0.4/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:13:21.526898 benimang-3.0.4/benimang.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-29 07:13:21.000000 benimang-3.0.4/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-06-29 07:12:28.000000 benimang-3.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:13:21.529899 benimang-3.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 07:13:21.527898 benimang-3.0.4/test/
+-rw-rw-rw-   0        0        0      638 2023-05-30 09:18:28.000000 benimang-3.0.4/test/test_sample.py
```

### Comparing `benimang-3.0.3/beni/bbyte.py` & `benimang-3.0.4/beni/bbyte.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bcache.py` & `benimang-3.0.4/beni/bcache.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pickle
 from datetime import datetime, timedelta
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, Coroutine, cast
 
 from beni import bfile, bfunc, bhash, bpath, btime
+from beni.bdefine import END_DATETIME
 
 
 class Store:
 
     def __init__(self, cache_dir: Path) -> None:
         self._CACHE_DIR = cache_dir
         self._DEADLINE = _StoreDeadline(cache_dir)
@@ -24,15 +25,15 @@
                 file,
                 pickle.dumps(data),
             )
             if not deadline:
                 if duration:
                     deadline = btime.datetime() + duration
                 else:
-                    deadline = btime.FOREVER
+                    deadline = END_DATETIME
             self._DEADLINE.update(key, deadline)
             return True
         except:
             await bpath.remove(file)
             self._DEADLINE.clear(key)
             return False
```

### Comparing `benimang-3.0.3/beni/bcmd.py` & `benimang-3.0.4/beni/bcmd.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bcolor.py` & `benimang-3.0.4/beni/bcolor.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bexecute.py` & `benimang-3.0.4/beni/bexecute.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bfile.py` & `benimang-3.0.4/beni/bfile.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bfunc.py` & `benimang-3.0.4/beni/bfunc.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bhash.py` & `benimang-3.0.4/beni/bhash.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bhttp.py` & `benimang-3.0.4/beni/bhttp.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/binput.py` & `benimang-3.0.4/beni/binput.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/block.py` & `benimang-3.0.4/beni/block.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/blog.py` & `benimang-3.0.4/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bpath.py` & `benimang-3.0.4/beni/bpath.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bplaywright.py` & `benimang-3.0.4/beni/bplaywright.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bprogress.py` & `benimang-3.0.4/beni/bprogress.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bqiniu.py` & `benimang-3.0.4/beni/bqiniu.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bsqlite.py` & `benimang-3.0.4/beni/bsqlite.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/bstorage.py` & `benimang-3.0.4/beni/bstorage.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/btable.py` & `benimang-3.0.4/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/btask.py` & `benimang-3.0.4/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/beni/btime.py` & `benimang-3.0.4/beni/btime.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import datetime as xdatetime
 import time as xtime
 
 from beni import bhttp
 
-FOREVER = xdatetime.datetime(9999, 9, 9)
-
 _server_time: float = xtime.time()
 _init_time: float = xtime.monotonic()
 
 
 async def network():
     _, response = await bhttp.get('https://www.baidu.com')
     date_str = response.headers['Date']
```

### Comparing `benimang-3.0.3/beni/bzip.py` & `benimang-3.0.4/beni/bzip.py`

 * *Files identical despite different names*

### Comparing `benimang-3.0.3/benimang.egg-info/SOURCES.txt` & `benimang-3.0.4/benimang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 beni/__init__.py
 beni/bbyte.py
 beni/bcache.py
 beni/bcmd.py
 beni/bcolor.py
+beni/bdefine.py
 beni/bexecute.py
 beni/bfile.py
 beni/bfunc.py
 beni/bhash.py
 beni/bhttp.py
 beni/binput.py
 beni/block.py
```

### Comparing `benimang-3.0.3/pyproject.toml` & `benimang-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://peps.python.org/pep-0621/#example
 
 [project]
 name = "benimang"
-version = "3.0.3"
+version = "3.0.4"
 description = "utils library for Beni"
 requires-python = ">=3.10"
 keywords = ["benimang", "beni"]
 authors = [
   {email = "benimang@126.com"},
   {name = "Beni Mang"}
 ]
```

### Comparing `benimang-3.0.3/test/test_sample.py` & `benimang-3.0.4/test/test_sample.py`

 * *Files identical despite different names*

