# Comparing `tmp/reolink_aio-0.7.1.tar.gz` & `tmp/reolink_aio-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.1.tar", last modified: Sun Jun 18 09:46:36 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.2.tar", last modified: Thu Jun 29 08:55:01 2023, max compression
```

## Comparing `reolink_aio-0.7.1.tar` & `reolink_aio-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   192151 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15190 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-18 09:46:36.000000 reolink_aio-0.7.1/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-18 09:46:36.853476 reolink_aio-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-18 09:46:24.000000 reolink_aio-0.7.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192290 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-29 08:55:01.000000 reolink_aio-0.7.2/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:01.227276 reolink_aio-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-06-29 08:54:42.000000 reolink_aio-0.7.2/tests/test.py
```

### Comparing `reolink_aio-0.7.1/LICENSE` & `reolink_aio-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/PKG-INFO` & `reolink_aio-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -127,7 +127,16 @@
     asyncio.run(print_mac_address())
 ````
 
 ### Acknowledgment
 This library is based on the work of:
 - fwestenberg: https://github.com/fwestenberg/reolink_dev
 - JimStar: https://github.com/JimStar/reolink_ip
+
+**Author**
+
+@starkillerOG: https://github.com/starkillerOG
+
+**Contributors**
+
+- @xannor: https://github.com/xannor
+- @mnpg: https://github.com/mnpg
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.1 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.2 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -47,8 +47,10 @@
 Host('192.168.1.109','admin', 'admin1234', port=80) # connect and obtain/cache
 device settings and capabilities await host.get_host_data() # check if it is a
 camera or an NVR print("It is an NVR: %s, number of channels: %s", host.is_nvr,
 host.num_channels) # print mac address print(host.mac_address) # close the
 device connection await host.logout() if __name__ == "__main__": asyncio.run
 (print_mac_address()) ```` ### Acknowledgment This library is based on the work
 of: - fwestenberg: https://github.com/fwestenberg/reolink_dev - JimStar: https:
-//github.com/JimStar/reolink_ip
+//github.com/JimStar/reolink_ip **Author** @starkillerOG: https://github.com/
+starkillerOG **Contributors** - @xannor: https://github.com/xannor - @mnpg:
+https://github.com/mnpg
```

### Comparing `reolink_aio-0.7.1/README.md` & `reolink_aio-0.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -104,7 +104,16 @@
     asyncio.run(print_mac_address())
 ````
 
 ### Acknowledgment
 This library is based on the work of:
 - fwestenberg: https://github.com/fwestenberg/reolink_dev
 - JimStar: https://github.com/JimStar/reolink_ip
+
+**Author**
+
+@starkillerOG: https://github.com/starkillerOG
+
+**Contributors**
+
+- @xannor: https://github.com/xannor
+- @mnpg: https://github.com/mnpg
```

### Comparing `reolink_aio-0.7.1/reolink_aio/api.py` & `reolink_aio-0.7.2/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1936,15 +1936,15 @@
         if response.content_length is None:
             response.release()
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_length' in the response")
         if response.content_disposition is None or response.content_disposition.filename is None:
             response.release()
             raise UnexpectedDataError(f"Host {self._host}:{self._port}: Download VOD: no 'content_disposition.filename' in the response")
 
-        return typings.VOD_download(response.content_length, response.content_disposition.filename, response.content, response.headers.get("ETag"))
+        return typings.VOD_download(response.content_length, response.content_disposition.filename, response.content, response.release, response.headers.get("ETag"))
 
     def map_host_json_response(self, json_data: typings.reolink_json):
         """Map the JSON objects to internal cache-objects."""
         for data in json_data:
             try:
                 if data["code"] == 1:  # Error, like "ability error"
                     continue
@@ -3610,15 +3610,16 @@
             if expected_response_type == "image/jpeg":
                 async with self._send_mutex:
                     response = await self._aiohttp_session.get(url=self._url, params=param, allow_redirects=False)
 
                 data = await response.read()  # returns bytes
             elif expected_response_type == "application/octet-stream":
                 async with self._send_mutex:
-                    response = await self._aiohttp_session.get(url=self._url, params=param, allow_redirects=False)
+                    dl_timeout = aiohttp.ClientTimeout(connect=self.timeout, sock_read=self.timeout)
+                    response = await self._aiohttp_session.get(url=self._url, params=param, allow_redirects=False, timeout=dl_timeout)
 
                 data = ""  # Response will be a file and be large, pass the response instead of reading it here.
             else:
                 _LOGGER.debug("%s/%s:%s::send() HTTP Request body =\n%s\n", self.nvr_name, self._host, self._port, str(body).replace(self._password, "<password>"))
 
                 async with self._send_mutex:
                     response = await self._aiohttp_session.post(url=self._url, json=body, params=param, allow_redirects=False)
```

### Comparing `reolink_aio-0.7.1/reolink_aio/enums.py` & `reolink_aio-0.7.2/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/reolink_aio/exceptions.py` & `reolink_aio-0.7.2/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/reolink_aio/software_version.py` & `reolink_aio-0.7.2/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/reolink_aio/templates.py` & `reolink_aio-0.7.2/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/reolink_aio/typings.py` & `reolink_aio-0.7.2/reolink_aio/typings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 """ Typings for type validation and documentation """
 from __future__ import annotations
 
 import logging
 from enum import IntFlag, auto
-from typing import Any, ClassVar, Collection, Iterator, Mapping, NamedTuple, Optional, TypedDict
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Collection,
+    Iterator,
+    Mapping,
+    NamedTuple,
+    Optional,
+    TypedDict,
+)
 import datetime as dtc
 from typing_extensions import SupportsIndex
 
 from aiohttp import StreamReader
 from .utils import reolink_time_to_datetime
 
 _LOGGER = logging.getLogger(__name__)
@@ -296,15 +306,24 @@
         ("date", dtc.date),
         ("start", dtc.time),
         ("end", dtc.time),
         ("triggers", VOD_trigger),
     ],
 )
 
-VOD_download = NamedTuple("VOD_download", [("length", int), ("filename", str), ("stream", StreamReader), ("etag", Optional[str])])
+VOD_download = NamedTuple(
+    "VOD_download",
+    [
+        ("length", int),
+        ("filename", str),
+        ("stream", StreamReader),
+        ("close", Callable[[], None]),
+        ("etag", Optional[str]),
+    ],
+)
 
 
 class VOD_file:
     """Contains information about the VOD file."""
 
     def __init__(self, data: dict[str, Any], tzinfo: Optional[dtc.tzinfo] = None) -> None:
         # {'EndTime': {'day': 17, 'hour': 2, 'min': 43, 'mon': 4, 'sec': 50, 'year': 2023},
```

### Comparing `reolink_aio-0.7.1/reolink_aio/utils.py` & `reolink_aio-0.7.2/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.1/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.2/reolink_aio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.7.1
+Version: 0.7.2
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -127,7 +127,16 @@
     asyncio.run(print_mac_address())
 ````
 
 ### Acknowledgment
 This library is based on the work of:
 - fwestenberg: https://github.com/fwestenberg/reolink_dev
 - JimStar: https://github.com/JimStar/reolink_ip
+
+**Author**
+
+@starkillerOG: https://github.com/starkillerOG
+
+**Contributors**
+
+- @xannor: https://github.com/xannor
+- @mnpg: https://github.com/mnpg
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.1 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.2 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -47,8 +47,10 @@
 Host('192.168.1.109','admin', 'admin1234', port=80) # connect and obtain/cache
 device settings and capabilities await host.get_host_data() # check if it is a
 camera or an NVR print("It is an NVR: %s, number of channels: %s", host.is_nvr,
 host.num_channels) # print mac address print(host.mac_address) # close the
 device connection await host.logout() if __name__ == "__main__": asyncio.run
 (print_mac_address()) ```` ### Acknowledgment This library is based on the work
 of: - fwestenberg: https://github.com/fwestenberg/reolink_dev - JimStar: https:
-//github.com/JimStar/reolink_ip
+//github.com/JimStar/reolink_ip **Author** @starkillerOG: https://github.com/
+starkillerOG **Contributors** - @xannor: https://github.com/xannor - @mnpg:
+https://github.com/mnpg
```

### Comparing `reolink_aio-0.7.1/setup.py` & `reolink_aio-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.1',
+      version='0.7.2',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
@@ -36,8 +36,8 @@
           "Operating System :: OS Independent",
           "Topic :: Software Development :: Libraries",
           "Topic :: Home Automation",
           "Programming Language :: Python",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
-          ])
+          ])
```

### Comparing `reolink_aio-0.7.1/tests/test.py` & `reolink_aio-0.7.2/tests/test.py`

 * *Files identical despite different names*

