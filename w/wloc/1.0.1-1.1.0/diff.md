# Comparing `tmp/wloc-1.0.1.tar.gz` & `tmp/wloc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wloc-1.0.1.tar", last modified: Thu Dec 15 15:48:02 2022, max compression
+gzip compressed data, was "wloc-1.1.0.tar", last modified: Thu Jun 29 12:59:23 2023, max compression
```

## Comparing `wloc-1.0.1.tar` & `wloc-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.466793 wloc-1.0.1/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      127 2022-08-04 07:50:03.000000 wloc-1.0.1/.bandit.yml
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)    35821 2022-12-11 16:00:06.000000 wloc-1.0.1/LICENSE
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      207 2022-12-15 15:10:15.000000 wloc-1.0.1/MANIFEST.in
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2893 2022-12-15 15:48:02.465793 wloc-1.0.1/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2081 2022-12-15 15:47:52.000000 wloc-1.0.1/README.md
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.462793 wloc-1.0.1/licenses/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2021-05-30 09:37:40.000000 wloc-1.0.1/licenses/noto-emoji.LICENSE.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1083 2021-05-17 16:58:29.000000 wloc-1.0.1/licenses/pywifi.LICENSE.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1409 2022-12-15 15:47:52.000000 wloc-1.0.1/pyproject.toml
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2022-12-15 15:48:02.466793 wloc-1.0.1/setup.cfg
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.460793 wloc-1.0.1/src/
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.462793 wloc-1.0.1/src/wloc/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3708 2022-12-11 16:37:03.000000 wloc-1.0.1/src/wloc/__init__.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.463793 wloc-1.0.1/src/wloc/app/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     4311 2022-12-11 16:37:03.000000 wloc-1.0.1/src/wloc/app/__init__.py
--rwxr-xr-x   0 vitaly    (1000) vitaly    (1000)      758 2022-12-11 16:37:03.000000 wloc-1.0.1/src/wloc/app/run.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.464793 wloc-1.0.1/src/wloc/backends/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2142 2022-12-11 16:37:03.000000 wloc-1.0.1/src/wloc/backends/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1724 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/backends/google.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      551 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/backends/mozilla.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1724 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/backends/yandex.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1007 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/exceptions.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.464793 wloc-1.0.1/src/wloc/fetchers/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1192 2022-12-11 16:37:03.000000 wloc-1.0.1/src/wloc/fetchers/__init__.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.464793 wloc-1.0.1/src/wloc/fetchers/android/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      582 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/android/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1443 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/android/termux.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      989 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/factory.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.465793 wloc-1.0.1/src/wloc/fetchers/linux/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      604 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/linux/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1178 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/linux/netman.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      987 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/native.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.465793 wloc-1.0.1/src/wloc/fetchers/windows/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      590 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/windows/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     4978 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/windows/structures.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     8735 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/fetchers/windows/wlan.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      844 2022-12-12 13:56:33.000000 wloc-1.0.1/src/wloc/helpers.py
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.463793 wloc-1.0.1/src/wloc.egg-info/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2893 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/PKG-INFO
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      925 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/SOURCES.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/dependency_links.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)       43 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/entry_points.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      185 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/requires.txt
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)        5 2022-12-15 15:48:02.000000 wloc-1.0.1/src/wloc.egg-info/top_level.txt
-drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2022-12-15 15:48:02.465793 wloc-1.0.1/tests/
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2022-12-11 15:36:48.000000 wloc-1.0.1/tests/__init__.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3543 2022-08-04 07:50:03.000000 wloc-1.0.1/tests/test_library.py
--rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1625 2022-12-12 08:34:01.000000 wloc-1.0.1/tox.ini
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.465221 wloc-1.1.0/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      127 2023-06-27 12:13:48.000000 wloc-1.1.0/.bandit.yml
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)    35821 2022-12-11 16:00:06.000000 wloc-1.1.0/LICENSE
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      207 2023-06-27 12:13:48.000000 wloc-1.1.0/MANIFEST.in
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2893 2023-06-29 12:59:23.465221 wloc-1.1.0/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2081 2022-12-15 15:47:52.000000 wloc-1.1.0/README.md
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.461221 wloc-1.1.0/licenses/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    11357 2021-05-30 09:37:40.000000 wloc-1.1.0/licenses/noto-emoji.LICENSE.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1083 2021-05-17 16:58:29.000000 wloc-1.1.0/licenses/pywifi.LICENSE.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1348 2023-06-29 12:58:35.000000 wloc-1.1.0/pyproject.toml
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       38 2023-06-29 12:59:23.465221 wloc-1.1.0/setup.cfg
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.459221 wloc-1.1.0/src/
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.462221 wloc-1.1.0/src/wloc/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3708 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/__init__.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.463221 wloc-1.1.0/src/wloc/app/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     4311 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/app/__init__.py
+-rwxr-xr-x   0 vitaly    (1000) vitaly    (1000)      758 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/app/run.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.463221 wloc-1.1.0/src/wloc/backends/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2174 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/backends/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1773 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/backends/google.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      551 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/backends/mozilla.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1773 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/backends/yandex.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1007 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/exceptions.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.464221 wloc-1.1.0/src/wloc/fetchers/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1192 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/__init__.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.464221 wloc-1.1.0/src/wloc/fetchers/android/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      582 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/android/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1451 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/android/termux.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      989 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/factory.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.464221 wloc-1.1.0/src/wloc/fetchers/linux/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      604 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/linux/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1617 2023-06-29 12:58:35.000000 wloc-1.1.0/src/wloc/fetchers/linux/netman.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      987 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/native.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.465221 wloc-1.1.0/src/wloc/fetchers/windows/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      590 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/windows/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     4978 2022-12-12 13:56:33.000000 wloc-1.1.0/src/wloc/fetchers/windows/structures.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     8743 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/fetchers/windows/wlan.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      844 2023-06-27 12:13:48.000000 wloc-1.1.0/src/wloc/helpers.py
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.463221 wloc-1.1.0/src/wloc.egg-info/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     2893 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/PKG-INFO
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      925 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/SOURCES.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        1 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/dependency_links.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)       43 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/entry_points.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      156 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/requires.txt
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)        5 2023-06-29 12:59:23.000000 wloc-1.1.0/src/wloc.egg-info/top_level.txt
+drwxr-xr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-06-29 12:59:23.465221 wloc-1.1.0/tests/
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)      114 2023-06-27 12:13:48.000000 wloc-1.1.0/tests/__init__.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     3543 2023-06-27 12:13:48.000000 wloc-1.1.0/tests/test_library.py
+-rw-r--r--   0 vitaly    (1000) vitaly    (1000)     1625 2023-06-27 12:13:48.000000 wloc-1.1.0/tox.ini
```

### Comparing `wloc-1.0.1/LICENSE` & `wloc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/PKG-INFO` & `wloc-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wloc
-Version: 1.0.1
+Version: 1.1.0
 Summary: Simple Wi-Fi geolocation library and tool
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/wloc
 Project-URL: documentation, https://github.com/xvitaly/wloc/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/wloc
 Keywords: api,application,geolocation,google-geolocation,library,mozilla-geolocation,tool,wi-fi,wi-fi-geolocation,yandex-geolocation
```

### Comparing `wloc-1.0.1/README.md` & `wloc-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/licenses/noto-emoji.LICENSE.txt` & `wloc-1.1.0/licenses/noto-emoji.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/licenses/pywifi.LICENSE.txt` & `wloc-1.1.0/licenses/pywifi.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/pyproject.toml` & `wloc-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [project]
 name = "wloc"
-version = "1.0.1"
+version = "1.1.0"
 license = { text = "GPL-3.0-or-later" }
 readme = "README.md"
 dependencies = [
-    "comtypes>=1.1.8; sys_platform == 'win32'",
-    "dbus-python>=1.2.16; sys_platform == 'linux'",
-    "python-networkmanager>=2.2; sys_platform == 'linux'",
-    "requests>=2.22.0"
+    "comtypes>=1.2.0; sys_platform == 'win32'",
+    "pygobject>=3.42.0; sys_platform == 'linux'",
+    "requests>=2.28.0"
 ]
 authors = [
     { name = "Vitaly Zaitsev", email="vitaly@easycoding.org" }
 ]
 description = "Simple Wi-Fi geolocation library and tool"
 keywords = [
     "api",
```

### Comparing `wloc-1.0.1/src/wloc/__init__.py` & `wloc-1.1.0/src/wloc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 
 from .backends.google import BackendGoogle
 from .backends.mozilla import BackendMozilla
```

### Comparing `wloc-1.0.1/src/wloc/app/__init__.py` & `wloc-1.1.0/src/wloc/app/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import argparse
 import logging
 import os
```

### Comparing `wloc-1.0.1/src/wloc/app/run.py` & `wloc-1.1.0/src/wloc/app/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import logging
 import sys
 
 from wloc.app import App
```

### Comparing `wloc-1.0.1/src/wloc/backends/__init__.py` & `wloc-1.1.0/src/wloc/backends/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import abc
 import json
 
 from ..exceptions import BackendError, MissingTokenError, NetworksNotFoundError
@@ -62,7 +62,8 @@
 
     def __init__(self, apikey: str):
         """
         Main constructor of the BackendCommon class.
         :param apikey: String with the API token (key).
         """
         self._apikey: str = apikey
+        self._timeout: int = 30
```

### Comparing `wloc-1.0.1/src/wloc/backends/google.py` & `wloc-1.1.0/src/wloc/backends/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import requests
 
 from ..backends import BackendCommon
@@ -25,15 +25,16 @@
         jdata = {'considerIp': 'false', 'wifiAccessPoints': []}
 
         # Retrieving available networks...
         for arr in netlist:
             jdata['wifiAccessPoints'].append({'macAddress': arr[0], 'signalStrength': arr[1], 'age': 0})
 
         # Sending our JSON to API...
-        r = requests.post(self._uri, data=json.dumps(jdata), headers={'content-type': 'application/json'})
+        r = requests.post(self._uri, data=json.dumps(jdata), headers={'content-type': 'application/json'},
+                          timeout=self._timeout)
 
         # Checking return code...
         self._check_response(r)
 
         # Parsing JSON response...
         result = json.loads(r.content)
```

### Comparing `wloc-1.0.1/src/wloc/backends/mozilla.py` & `wloc-1.1.0/src/wloc/backends/mozilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from .google import BackendGoogle
 
 
 class BackendMozilla(BackendGoogle):
```

### Comparing `wloc-1.0.1/src/wloc/backends/yandex.py` & `wloc-1.1.0/src/wloc/backends/yandex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import requests
 
 from ..backends import BackendCommon
@@ -25,15 +25,16 @@
         jdata = {'common': {'version': '1.0', 'api_key': self._apikey}, 'wifi_networks': []}
 
         # Retrieving available networks...
         for arr in netlist:
             jdata['wifi_networks'].append({'mac': arr[0], 'signal_strength': arr[1], 'age': 0})
 
         # Sending our JSON to API...
-        r = requests.post(self._uri, data={'json': json.dumps(jdata)}, headers={'content-type': 'application/json'})
+        r = requests.post(self._uri, data={'json': json.dumps(jdata)}, headers={'content-type': 'application/json'},
+                          timeout=self._timeout)
 
         # Checking return code...
         self._check_response(r)
 
         # Parsing JSON response...
         result = json.loads(r.content)
```

### Comparing `wloc-1.0.1/src/wloc/exceptions.py` & `wloc-1.1.0/src/wloc/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 __all__ = ['BackendError', 'FetcherError', 'MissingTokenError', 'MissingArgumentError', 'NetworksNotFoundError',
            'PlatformError', 'PlatformNotSupported']
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/__init__.py` & `wloc-1.1.0/src/wloc/fetchers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import abc
 
 
 class FetcherCommon(metaclass=abc.ABCMeta):
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/android/__init__.py` & `wloc-1.1.0/src/wloc/fetchers/android/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from .termux import TermuxNativeAPI
 from ...fetchers import FetcherCommon
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/android/termux.py` & `wloc-1.1.0/src/wloc/fetchers/android/termux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import subprocess
 
 from ..native import NativeBackendCommon
@@ -31,15 +31,15 @@
         """
         networks = json.loads(self._json)
         if not isinstance(networks, list):
             raise FetcherError(next(iter(networks.values())))
         for network in networks:
             self._network_list.append([network['bssid'], network['rssi']])
 
-    def _fetch_list(self):
+    def _fetch_list(self) -> None:
         """
         Fetches the list of available Wi-Fi networks using public
         D-Bus methods.
         """
         self._fetch_json()
         self._parse_json()
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/factory.py` & `wloc-1.1.0/src/wloc/fetchers/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 
 from ..exceptions import PlatformNotSupported
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/linux/__init__.py` & `wloc-1.1.0/src/wloc/fetchers/linux/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from .netman import NetworkManagerNativeAPI
 from ...fetchers import FetcherCommon
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/native.py` & `wloc-1.1.0/src/wloc/fetchers/native.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import abc
 
 
 class NativeBackendCommon(metaclass=abc.ABCMeta):
@@ -32,8 +32,8 @@
         return self._network_list
 
     def __init__(self) -> None:
         """
         Main constructor of the FetcherBackendCommon class.
         """
         self._network_list: list = []
-        self._sleep_seconds: int = 3
+        self._sleep_seconds: int = 5
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/windows/__init__.py` & `wloc-1.1.0/src/wloc/fetchers/windows/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from .wlan import WlanNativeAPI
 from ...fetchers import FetcherCommon
```

### Comparing `wloc-1.0.1/src/wloc/fetchers/windows/structures.py` & `wloc-1.1.0/src/wloc/fetchers/windows/structures.py`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/src/wloc/fetchers/windows/wlan.py` & `wloc-1.1.0/src/wloc/fetchers/windows/wlan.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                                                 networks[i].dot11Ssid, networks[i].bSecurityEnabled)
                 bsses = ctypes.cast(bss_list.contents.wlanBssEntries, ctypes.POINTER(structures.WLAN_BSS_ENTRY))
                 for j in range(bss_list.contents.dwNumberOfItems):
                     network_list.append(
                         [':'.join([f'{bssid:02x}' for bssid in bsses[j].dot11Bssid[0:6]]), bsses[j].lRssi])
         return network_list
 
-    def _fetch_list(self):
+    def _fetch_list(self) -> None:
         """
         Gets available network interfaces and fetches available wireless
         networks into a special private field.
         """
         for interface in self._get_interfaces():
             networks = self._get_networks(interface)
             if len(networks) < 2:
```

### Comparing `wloc-1.0.1/src/wloc/helpers.py` & `wloc-1.1.0/src/wloc/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 
 class Helpers:
     """
     Static class with helper methods.
```

### Comparing `wloc-1.0.1/src/wloc.egg-info/PKG-INFO` & `wloc-1.1.0/src/wloc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wloc
-Version: 1.0.1
+Version: 1.1.0
 Summary: Simple Wi-Fi geolocation library and tool
 Author-email: Vitaly Zaitsev <vitaly@easycoding.org>
 License: GPL-3.0-or-later
 Project-URL: homepage, https://github.com/xvitaly/wloc
 Project-URL: documentation, https://github.com/xvitaly/wloc/blob/master/docs/README.md
 Project-URL: repository, https://github.com/xvitaly/wloc
 Keywords: api,application,geolocation,google-geolocation,library,mozilla-geolocation,tool,wi-fi,wi-fi-geolocation,yandex-geolocation
```

### Comparing `wloc-1.0.1/src/wloc.egg-info/SOURCES.txt` & `wloc-1.1.0/src/wloc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wloc-1.0.1/tests/test_library.py` & `wloc-1.1.0/tests/test_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import os
 import unittest
 import wloc
```

### Comparing `wloc-1.0.1/tox.ini` & `wloc-1.1.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2015-2022 EasyCoding Team
+# SPDX-FileCopyrightText: 2015-2023 EasyCoding Team
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 # =====================================
 # ===== General Tox configuration =====
 # =====================================
```

