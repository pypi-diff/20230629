# Comparing `tmp/wf_video_io-3.3.5.tar.gz` & `tmp/wf_video_io-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.3.5.tar", max compression
+gzip compressed data, was "wf_video_io-3.4.0.tar", max compression
```

## Comparing `wf_video_io-3.3.5.tar` & `wf_video_io-3.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.5/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.5/README.md
--rw-r--r--   0        0        0     1162 2023-05-29 18:34:29.454143 wf_video_io-3.3.5/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.5/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.5/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    17319 2023-05-29 18:34:10.695630 wf_video_io-3.3.5/video_io/client/core.py
--rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.5/video_io/client/errors.py
--rw-r--r--   0        0        0     3385 2023-05-25 18:28:00.924148 wf_video_io-3.3.5/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.5/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.5/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.5/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.5/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.5/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.5/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.4.0/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.4.0/README.md
+-rw-r--r--   0        0        0     1181 2023-06-29 21:08:51.791466 wf_video_io-3.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.4.0/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.4.0/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    18738 2023-06-29 21:12:27.242562 wf_video_io-3.4.0/video_io/client/core.py
+-rw-r--r--   0        0        0      265 2023-06-29 21:08:51.793888 wf_video_io-3.4.0/video_io/client/errors.py
+-rw-r--r--   0        0        0     3412 2023-06-29 21:08:51.794977 wf_video_io-3.4.0/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.4.0/video_io/config.py
+-rwxr-xr-x   0        0        0    49247 2023-06-29 21:14:15.999435 wf_video_io-3.4.0/video_io/core.py
+-rw-r--r--   0        0        0       41 2023-06-29 21:08:51.797796 wf_video_io-3.4.0/video_io/errors.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.4.0/video_io/log_retry.py
+-rw-r--r--   0        0        0    11076 2023-06-29 21:14:05.674928 wf_video_io-3.4.0/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.4.0/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.4.0/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.4.0/PKG-INFO
```

### Comparing `wf_video_io-3.3.5/LICENSE` & `wf_video_io-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.5/pyproject.toml` & `wf_video_io-3.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "wf-video-io"
-dynamic = ["version"]
+#dynamic = ["version"]
+version = "3.4.0"
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.3.5"
+version = "3.4.0"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.3.5/video_io/client/core.py` & `wf_video_io-3.4.0/video_io/client/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import asyncio
 import concurrent.futures
+from datetime import datetime
 from io import BytesIO
 import json
 from json.decoder import JSONDecodeError
 import logging
 import os
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Union, Optional
 
 from cachetools import TTLCache
 import requests
 from requests.adapters import HTTPAdapter
-from typing import Optional
+import tenacity
 import yaml
 
 import video_io.config
 from video_io.log_retry import LogRetry
-from video_io.client.errors import SyncError, BadVideoError
+from video_io.client.errors import SyncError
+from video_io.errors import BadVideoError
 from video_io.client.utils import (
     client_token,
     parse_path,
     get_video_file_details,
     chunks,
     FPS_PATH,
 )
@@ -28,27 +30,28 @@
 
 logger = logging.getLogger(__name__)
 
 
 UPLOAD_FAILED_REASON_BAD_VIDEO = "BAD_VIDEO"
 UPLOAD_FAILED_REASON_BAD_PATH_TO_VIDEO = "BAD_PATH_TO_VIDEO"
 
+
 class VideoStorageClient:
     DEFAULT_CONNECTION_POOL_SIZE = 10
 
     def __init__(
         self,
         token=None,
         cache_directory=video_io.config.VIDEO_STORAGE_LOCAL_CACHE_DIRECTORY,
         url=video_io.config.VIDEO_STORAGE_URL,
         auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
         audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
         client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
         client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
-        connection_pool_size: Optional[int] = None
+        connection_pool_size: Optional[int] = None,
     ):
         self.CACHE_DIRECTORY = cache_directory
         self.URL = url
 
         self.auth_domain = auth_domain
         self.audience = audience
         self.client_id = client_id
@@ -56,31 +59,35 @@
 
         self.headers = {}  # {"Content-Type": "application/json"}
 
         self.tokens = {}
         if token is not None:
             self.tokens["access_token"] = token
 
-        self.request_session = self.init_request_session(connection_pool_size=connection_pool_size)
+        self.request_session = self.init_request_session(
+            connection_pool_size=connection_pool_size
+        )
 
     @staticmethod
     def init_request_session(connection_pool_size=None):
         retry_strategy = LogRetry(
             total=6,
             status_forcelist=[429, 500, 502, 503, 504],
             method_whitelist=["HEAD", "GET", "OPTIONS", "POST"],
             backoff_factor=0.5,
         )
         _connection_pool_size = connection_pool_size
         if _connection_pool_size is None:
             _connection_pool_size = VideoStorageClient.DEFAULT_CONNECTION_POOL_SIZE
 
-        adapter = HTTPAdapter(max_retries=retry_strategy,
-                              pool_connections=_connection_pool_size,
-                              pool_maxsize=_connection_pool_size)
+        adapter = HTTPAdapter(
+            max_retries=retry_strategy,
+            pool_connections=_connection_pool_size,
+            pool_maxsize=_connection_pool_size,
+        )
         request_session = requests.Session()
         request_session.mount("https://", adapter)
         request_session.mount("http://", adapter)
         return request_session
 
     def refresh_token(self):
         try:
@@ -114,45 +121,68 @@
         }
 
     @headers.setter
     def headers(self, header_dict: dict):
         self._headers = header_dict
 
     async def get_videos(
-        self, environment_id, start_date, end_date, camera_id=None, destination=None
+        self,
+        environment_id: str,
+        start_date: datetime,
+        end_date: datetime,
+        camera_id: str = None,
+        destination: Union[Path, str] = None,
     ):
         if destination is None:
             destination = self.CACHE_DIRECTORY
         if not hasattr(destination, "mkdir"):
             destination = Path(destination)
         destination.mkdir(parents=True, exist_ok=True)
         meta = self.get_videos_metadata_paginated(
-            environment_id, start_date, end_date, camera_id
+            environment_id=environment_id,
+            start_date=start_date,
+            end_date=end_date,
+            camera_id=camera_id,
         )
         futures = []
         with concurrent.futures.ThreadPoolExecutor(max_workers=4) as e:
             async for vid_meta in meta:
                 f = e.submit(
                     asyncio.run,
                     self.get_video(
                         path=vid_meta["meta"]["path"], destination=destination
                     ),
                 )
                 futures.append(f)
         list(concurrent.futures.as_completed(futures))
 
+    @tenacity.retry(
+        wait=tenacity.wait_incrementing(start=5, increment=1),
+        stop=tenacity.stop_after_attempt(3),
+        retry=tenacity.retry_if_exception_type(requests.exceptions.RequestException),
+    )
     async def get_video(self, path: str, destination: str, overwrite: bool = False):
         p = Path(destination) / path
+
+        if p.is_file():
+            try:
+                get_video_file_details(p.absolute())
+            except Exception as e:
+                logger.error(
+                    f"Could not ffprobe video file {p.absolute()} - {e}. Removing file and attempting to re-download"
+                )
+                os.remove(p.absolute())
+
         if not p.is_file() or overwrite:
             logger.info("Downloading video file %s", path)
             request = {
                 "method": "GET",
                 "url": f"{self.URL}/video/{path}/data",
                 "headers": self.headers,
-                "timeout": 45
+                "timeout": 45,
             }
             try:
                 response = self.request_session.request(**request)
                 response.raise_for_status()
 
                 pp = p.parent
                 if not pp.exists():
@@ -171,15 +201,21 @@
                     "Failing fetching video file %s with exception %s", path, e
                 )
                 raise e
         else:
             logger.info("Video file %s already exists", path)
 
     async def get_videos_metadata_paginated(
-        self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100
+        self,
+        environment_id: str,
+        start_date: datetime,
+        end_date: datetime,
+        camera_id: str = None,
+        skip: int = 0,
+        limit: int = 1000,
     ):
         current_skip = skip
         while True:
             page = await self.get_videos_metadata(
                 environment_id,
                 start_date,
                 end_date,
@@ -189,16 +225,21 @@
             )
             for item in page:
                 yield item
             current_skip += limit
             if len(page) == 0:
                 break
 
+    @tenacity.retry(
+        wait=tenacity.wait_incrementing(start=5, increment=1),
+        stop=tenacity.stop_after_attempt(3),
+        retry=tenacity.retry_if_exception_type(requests.exceptions.RequestException),
+    )
     async def get_videos_metadata(
-        self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=100
+        self, environment_id, start_date, end_date, camera_id=None, skip=0, limit=1000
     ):
         request = {
             "method": "GET",
             "url": f"{self.URL}/videos/{environment_id}/device/{camera_id}"
             if camera_id is not None
             else f"{self.URL}/videos/{environment_id}",
             "headers": self.headers,
@@ -232,53 +273,59 @@
                 start_date,
                 end_date,
                 e,
             )
             raise e
 
     async def upload_video(self, path: str, local_cache_directory: str = None):
-        response = await self.upload_videos(paths=[path], local_cache_directory=local_cache_directory)
+        response = await self.upload_videos(
+            paths=[path], local_cache_directory=local_cache_directory
+        )
         return response[0]
 
     async def upload_videos(self, paths: List[str], local_cache_directory: str = None):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
 
         bad_file_results: List[dict] = []
         all_file_details: List[dict] = []
-        for ii, path in enumerate(paths):
+        for path in paths:
             full_path = local_cache_directory / path
             ptype, file_details = parse_path(path)
             if ptype == "file":
                 file_details["ptype"] = ptype
                 file_details["path"] = full_path
                 file_details["filepath"] = path
                 all_file_details.append(file_details)
             else:
-                bad_file_results.append({
-                    "id": None,
-                    "path": path,
-                    "uploaded": False,
-                    "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_PATH_TO_VIDEO,
-                    "upload_failed_error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4",
-                    "disposition": None
-                })
+                bad_file_results.append(
+                    {
+                        "id": None,
+                        "path": path,
+                        "uploaded": False,
+                        "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_PATH_TO_VIDEO,
+                        "upload_failed_error": f"Invalid path. '{path}' doesn't match pattern [environment_id]/[camera_id]/[year]/[month]/[day]/[hour]/[min]-[second].mp4",
+                        "disposition": None,
+                    }
+                )
 
         upload_results = []
         if len(all_file_details) > 0:
             upload_results = await self._upload_videos(all_file_details)
         return [*upload_results, *bad_file_results]
 
     def prepare_video(self, file_details: Dict) -> (Dict, BytesIO):
         path = file_details["path"]
 
         try:
             video_properties = get_video_file_details(path)
         except Exception as e:
-            raise BadVideoError(f"Could not ffprobe video file {file_details['path']} - {e}")
+            raise BadVideoError(
+                f"Could not ffprobe video file {file_details['path']} - {e}"
+            ) from e
 
         if file_details["ptype"] == "file":
             ts = f"{file_details['year']}-{file_details['month']}-{file_details['day']}T{file_details['hour']}:{file_details['file'][0:2]}:{file_details['file'][3:5]}.0000"
             meta = {
                 "timestamp": ts,
                 "meta": {
                     "environment_id": file_details["environment_id"],
@@ -298,14 +345,19 @@
             with p.open("r", encoding="utf8") as fp:
                 meta = yaml.safe_load(fp.read())
         return (
             meta,
             open(path, "rb"),  # pylint: disable=R1732
         )
 
+    @tenacity.retry(
+        wait=tenacity.wait_incrementing(start=5, increment=1),
+        stop=tenacity.stop_after_attempt(3),
+        retry=tenacity.retry_if_exception_type(requests.exceptions.RequestException),
+    )
     async def _upload_videos(self, file_details: List[Dict]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos",
             "headers": self.headers,
         }
 
@@ -315,19 +367,19 @@
         for details in file_details:
             try:
                 meta, fileio = self.prepare_video(details)
             except BadVideoError as e:
                 results.append(
                     {
                         "id": None,
-                        "path": details['filepath'],
+                        "path": details["filepath"],
                         "uploaded": False,
                         "upload_failed_reason": UPLOAD_FAILED_REASON_BAD_VIDEO,
                         "upload_failed_error": str(e),
-                        "disposition": None
+                        "disposition": None,
                     }
                 )
                 continue
 
             files.append(
                 (
                     "files",
@@ -379,15 +431,15 @@
             raise e
 
     async def video_existence_check(self, paths: List[str]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos/check",
             "headers": self.headers,
-            "json": paths
+            "json": paths,
         }
         try:
             r = requests.Request(**request).prepare()
             response = self.request_session.send(r, timeout=45)
             try:
                 return response.json()
             except Exception:
@@ -414,15 +466,14 @@
         max_workers=video_io.config.MAX_SYNC_WORKERS,
     ):
         if local_cache_directory is None:
             local_cache_directory = self.CACHE_DIRECTORY
         local_cache_directory = Path(local_cache_directory)
         strpath = str(path)
         t, details = parse_path(strpath[:-1] if strpath[-1] == "/" else strpath)
-        logging.info("ptype is %s", t)
         if details:
             if t in ("file", "fileV2"):
                 raise SyncError(
                     "didn't expect file, expected directory, try `upload_video`"
                 )
             if t == "year":
                 raise SyncError("cannot sync a year of videos, try limiting to a day")
@@ -446,15 +497,15 @@
                         file_details["ptype"] = ptype
                         file_details["path"] = full_path
                         file_details["filepath"] = path
                         files_found.append(file_details)
             details["files_found"] = len(files_found)
             details["files_uploaded"] = 0
             details["details"] = []
-            logger.debug("found %s files to be uploaded", len(files_found))
+            logger.debug(f"found {len(files_found)} files to be uploaded")
             with concurrent.futures.ThreadPoolExecutor(
                 max_workers=max_workers
             ) as executor:
                 results = executor.map(
                     self._upload_videos, chunks(files_found, batch_size)
                 )
                 logger.debug(results)
```

### Comparing `wf_video_io-3.3.5/video_io/client/utils.py` & `wf_video_io-3.4.0/video_io/client/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 
-import ffmpeg
 from tenacity import retry, wait_random, stop_after_attempt
 from auth0.v3.authentication import GetToken
 from cachetools.func import ttl_cache
 import jmespath
 
+import video_io.utils
+
 
 @ttl_cache(ttl=60 * 60 * 4)
 def is_v2_directory(path):
     index_file = path / "wf-video-index.yml"
     return index_file.exists()
 
 
@@ -25,15 +26,15 @@
     return api_token, expires_in
 
 
 @ttl_cache(ttl=60 * 60 * 4)
 def get_video_file_details(path):
     # check for video file if it exists load that and return its contents.
     # if not then run ffprobe and return a new meta document
-    return ffmpeg.probe(path)
+    video_io.utils.get_video_file_details(path)
 
 
 CACHE_PATH_FILE = re.compile(
     "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})/(?P<file>.*)$"
 )
 CACHE_PATH_HOUR = re.compile(
     "^(?P<environment_id>[a-fA-F0-9-]*)/(?P<camera_id>[a-fA-F0-9-]*)/(?P<year>[0-9]{4})/(?P<month>[0-9]{2})/(?P<day>[0-9]{2})/(?P<hour>[0-9]{2})$"
```

### Comparing `wf_video_io-3.3.5/video_io/config.py` & `wf_video_io-3.4.0/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.5/video_io/core.py` & `wf_video_io-3.4.0/video_io/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Downloads videos that match search parameters and returns their metadata.
 
     This function simply combines the operations of fetch_video_metadata() and
     download_video_files(). See documentation of those functions for details.
 
@@ -75,14 +76,15 @@
         client_id (str): Auth0 client ID for Honeycomb (default is value of HONEYCOMB_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         client_secret (str): Auth0 client secret for Honeycomb (default is value of HONEYCOMB_CLIENT_SECRET AUTH0_CLIENT_SECRET environment variable)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for videos with local path information appended
     """
     logger.info("Fetching metadata for videos that match specified parameters")
     video_metadata = fetch_video_metadata(
         start=start,
@@ -103,26 +105,28 @@
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     logger.info("Downloading video files")
     video_metadata_with_local_paths = download_video_files(
         video_metadata=video_metadata,
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     return video_metadata_with_local_paths
 
 
 def fetch_images(
     image_timestamps,
     camera_assignment_ids=None,
@@ -145,14 +149,15 @@
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Downloads images that match search parameters and returns their metadata.
 
     This function simply combines the operations of fetch_image_metadata() and
     download_image_files(). See documentation of those functions for details.
 
@@ -178,14 +183,15 @@
         client_id (str): Auth0 client ID for Honeycomb (default is value of HONEYCOMB_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         client_secret (str): Auth0 client secret for Honeycomb (default is value of HONEYCOMB_CLIENT_SECRET AUTH0_CLIENT_SECRET environment variable)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for images with local path information appended
     """
     logger.info("Fetching metadata for images that match specified parameters")
     image_metadata = fetch_image_metadata(
         image_timestamps=image_timestamps,
@@ -204,28 +210,30 @@
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     logger.info("Downloading image files")
     image_metadata_with_local_paths = download_image_files(
         image_metadata=image_metadata,
         local_image_directory=local_image_directory,
         image_filename_extension=image_filename_extension,
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     return image_metadata_with_local_paths
 
 
 def fetch_video_metadata(
     start=None,
     end=None,
@@ -245,14 +253,15 @@
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Searches Honeycomb for videos that match specified search parameters and
     returns their metadata.
 
     If start and end are specified, returns all videos that overlap with
     specified start and end (e.g., if start is 10:32:56 and end is 10:33:20,
@@ -287,14 +296,15 @@
         client_id (str): Auth0 client ID for Honeycomb (default is value of HONEYCOMB_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         client_secret (str): Auth0 client secret for Honeycomb (default is value of HONEYCOMB_CLIENT_SECRET AUTH0_CLIENT_SECRET environment variable)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for videos that match search parameters
     """
     video_metadata_raw = fetch_video_metadata_raw(
         start=start,
         end=end,
@@ -314,31 +324,32 @@
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     logger.info("Parsing %s returned video metadata", len(video_metadata_raw))
-    video_metadata = list()
+    video_metadata = []
     for datum in video_metadata_raw:
         meta = datum.get("meta", {})
         video_metadata.append(
             {
                 "data_id": datum.get("id"),
                 "video_timestamp": datetime.datetime.fromisoformat(
                     datum.get("timestamp")
                 ),
                 "environment_id": meta.get("environment_id"),
                 "assignment_id": meta.get("assignment_id"),
                 "device_id": meta.get("camera_id"),
                 "path": meta.get("path"),
                 "duration_seconds": meta.get("duration_seconds"),
-                "fps": meta.get("fps"),
+                "fps": 10,  # meta.get("fps"),
                 "frame_offsets": meta.get("frame_offsets"),
             }
         )
     return video_metadata
 
 
 def fetch_video_metadata_raw(
@@ -360,14 +371,15 @@
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     if (start is not None or end is not None) and video_timestamps is not None:
         raise ValueError("Cannot specify start/end and list of video timestamps")
     if video_timestamps is None and (start is None or end is None):
         raise ValueError(
             "If not specifying specific timestamps, must specify both start and end times"
         )
@@ -458,14 +470,15 @@
             environment_id=environment_id,
             camera_device_ids=camera_device_ids,
             video_storage_url=video_storage_url,
             video_storage_auth_domain=video_storage_auth_domain,
             video_storage_audience=video_storage_audience,
             video_storage_client_id=video_storage_client_id,
             video_storage_client_secret=video_storage_client_secret,
+            video_client=video_client,
         )
     )
     return video_metadata_raw
 
 
 async def _fetch_video_metadata(
     video_timestamp_min_utc,
@@ -474,23 +487,26 @@
     environment_id,
     camera_device_ids,
     video_storage_url,
     video_storage_auth_domain,
     video_storage_audience,
     video_storage_client_id,
     video_storage_client_secret,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
-    video_client = video_io.client.VideoStorageClient(
-        token=None,
-        url=video_storage_url,
-        auth_domain=video_storage_auth_domain,
-        audience=video_storage_audience,
-        client_id=video_storage_client_id,
-        client_secret=video_storage_client_secret,
-    )
+    if video_client is None:
+        video_client = video_io.client.VideoStorageClient(
+            token=None,
+            url=video_storage_url,
+            auth_domain=video_storage_auth_domain,
+            audience=video_storage_audience,
+            client_id=video_storage_client_id,
+            client_secret=video_storage_client_secret,
+        )
+
     result = []
     if video_timestamps_utc is None:
         if camera_device_ids is None:
             logger.info(
                 "Fetching video metadata for all cameras in specified environment"
             )
             video_metadata_pages = video_client.get_videos_metadata_paginated(
@@ -555,14 +571,15 @@
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
     overwrite: bool = False,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Downloads videos from video service to local directory tree and returns metadata with
     local path information added.
 
     Videos are specified as a list of dictionaries, as returned by the function
     fetch_video_metadata(). Each dictionary is assumed to have the following
@@ -583,14 +600,15 @@
         max_workers (int): Maximum number of processes to launch when downloading video (default is number of CPUs - 1)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
         overwrite (bool): If set to true, any cached video snippets will be overwritten
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for videos with local path information appended
     """
     if video_filename_extension is not None:
         raise NotImplementedError(
             "Specifying video filename extension is no longer supported"
@@ -602,38 +620,41 @@
             max_workers=max_workers,
             video_storage_url=video_storage_url,
             video_storage_auth_domain=video_storage_auth_domain,
             video_storage_audience=video_storage_audience,
             video_storage_client_id=video_storage_client_id,
             video_storage_client_secret=video_storage_client_secret,
             overwrite=overwrite,
+            video_client=video_client,
         )
     )
     return video_metadata
 
 
 async def _download_video_files(
     video_metadata,
     local_video_directory,
     max_workers,
     video_storage_url,
     video_storage_auth_domain,
     video_storage_audience,
     video_storage_client_id,
     video_storage_client_secret,
+    video_client: video_io.client.VideoStorageClient = None,
     overwrite: bool = False,
 ):
-    video_client = video_io.client.VideoStorageClient(
-        token=None,
-        url=video_storage_url,
-        auth_domain=video_storage_auth_domain,
-        audience=video_storage_audience,
-        client_id=video_storage_client_id,
-        client_secret=video_storage_client_secret,
-    )
+    if video_client is None:
+        video_client = video_io.client.VideoStorageClient(
+            token=None,
+            url=video_storage_url,
+            auth_domain=video_storage_auth_domain,
+            audience=video_storage_audience,
+            client_id=video_storage_client_id,
+            client_secret=video_storage_client_secret,
+        )
     futures = []
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as e:
         for video_metadatum in video_metadata:
             f = e.submit(
                 asyncio.run,
                 video_client.get_video(
                     path=video_metadatum["path"],
@@ -666,14 +687,15 @@
     client_id=video_io.config.HONEYCOMB_CLIENT_ID,
     client_secret=video_io.config.HONEYCOMB_CLIENT_SECRET,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Searches Honeycomb for videos containing images that match specified search
     parameters and returns video/image metadata.
 
     Image timestamps are rounded to the nearest tenth of a second to synchronize
     with video frames. Videos containing these images must match all specified
@@ -704,14 +726,15 @@
         client_id (str): Auth0 client ID for Honeycomb (default is value of HONEYCOMB_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         client_secret (str): Auth0 client secret for Honeycomb (default is value of HONEYCOMB_CLIENT_SECRET AUTH0_CLIENT_SECRET environment variable)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for images that match search parameters
     """
     image_metadata_by_video_timestamp = {}
     for image_timestamp in image_timestamps:
         image_timestamp = image_timestamp.astimezone(datetime.timezone.utc)
@@ -745,14 +768,15 @@
         client_id=client_id,
         client_secret=client_secret,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     image_metadata = []
     for video in video_metadata:
         for image in image_metadata_by_video_timestamp[video["video_timestamp"]]:
             image_metadata.append({**video, **image})
     return image_metadata
 
@@ -765,14 +789,15 @@
     video_filename_extension=None,
     max_workers=video_io.config.MAX_DOWNLOAD_WORKERS,
     video_storage_url=video_io.config.VIDEO_STORAGE_URL,
     video_storage_auth_domain=video_io.config.VIDEO_STORAGE_AUTH_DOMAIN,
     video_storage_audience=video_io.config.VIDEO_STORAGE_AUDIENCE,
     video_storage_client_id=video_io.config.VIDEO_STORAGE_CLIENT_ID,
     video_storage_client_secret=video_io.config.VIDEO_STORAGE_CLIENT_SECRET,
+    video_client: video_io.client.VideoStorageClient = None,
 ):
     """
     Downloads videos from video service to local directory tree, extract images,
     saves images to local directory tree, and returns metadata with local path
     information added.
 
     Images are specified as a list of dictionaries, as returned by the function
@@ -796,28 +821,30 @@
         video_filename_extension (str): Filename extension for video files [NO LONGER SUPPORTED]
         max_workers (int): Maximum number of processes to launch when downloading video (default is number of CPUs - 1)
         video_storage_url (str): Server URL for video service (default is value of VIDEO_STORAGE_URL environment variable)
         video_storage_auth_domain (str): Auth0 domain for video service (default is value of VIDEO_STORAGE_AUTH_DOMAIN or AUTH0_DOMAIN environment variable)
         video_storage_audience (str): Auth0 audience for video service (default is value of VIDEO_STORAGE_AUDIENCE or API_AUDIENCE environment variable)
         video_storage_client_id (str): Auth0 client ID for video service (default is value of VIDEO_STORAGE_CLIENT_ID or AUTH0_CLIENT_ID environment variable)
         video_storage_client_secret (str): Auth0 client secret for video service (default is value of VIDEO_STORAGE_CLIENT_SECRET or AUTH0_CLIENT_SECRET environment variable)
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (list of dict): Metadata for images with local path information appended
     """
     image_metadata_with_local_video_paths = download_video_files(
         video_metadata=image_metadata,
         local_video_directory=local_video_directory,
         video_filename_extension=video_filename_extension,
         max_workers=max_workers,
         video_storage_url=video_storage_url,
         video_storage_auth_domain=video_storage_auth_domain,
         video_storage_audience=video_storage_audience,
         video_storage_client_id=video_storage_client_id,
         video_storage_client_secret=video_storage_client_secret,
+        video_client=video_client,
     )
     image_metadata_with_local_paths = []
     for image in image_metadata_with_local_video_paths:
         download_path = image_local_path(
             local_image_directory=local_image_directory,
             environment_id=image.get("environment_id"),
             device_id=image.get("device_id"),
@@ -905,14 +932,15 @@
     end: datetime,
     output_directory: str,
     camera_names: Optional[List[str]] = None,
     workers: int = cpu_count() - 1,
     video_snippet_directory: str = None,
     overwrite_video_snippets: bool = False,
     overwrite_concatenated_video: bool = False,
+    video_client: video_io.client.VideoStorageClient = None,
 ) -> Optional[pd.DataFrame]:
     """
     Create concatenated video files for each camera in a particular environment given a provided start and end time.
 
     Function will download individual video snippets across each camera, concatenate those snippets, and trim the videos
     to exactly match the provided start and end time.
 
@@ -922,26 +950,28 @@
         end (datetime): End of time period
         output_directory (str): Directory to write concatenated video files to. Video file names are written as "{environment_id}_{camera_device_id}_{start.strftime('%m%d%YT%H%M%S%f%z')}_{end.strftime('%m%d%YT%H%M%S%f%z')}.mp4"
         camera_names (List[str]): Filter cameras to a specific subset (default value is None which means to filter and concatenated video will be generated for all cameras)
         workers (int): Number of processes to be used to download video files
         video_snippet_directory (str): Directory to store video snippets. If no directory is provided, videos will be downloaded to the operating systems temp directory and destroyed once the function finishes
         overwrite_video_snippets (bool): If set, any cached video snippets will be overwritten
         overwrite_concatenated_video (bool): If set, any previously generated concatenated video will be overwritten
+        video_client (VideoStorageClient): Reusable video client
 
     Returns:
         (dataframe): Dataframe object include "environment_id", "camera_assignment_id", "camera_device_id", and the concatenated video files' "file_path"
 
     """
     os.makedirs(output_directory, exist_ok=True)
 
     video_metadata = fetch_video_metadata(
         start=start,
         end=end,
         environment_name=environment_name,
         camera_names=camera_names,
+        video_client=video_client,
     )
     if video_metadata is None or len(video_metadata) == 0:
         logger.warning(
             f"Found 0 videos for {environment_name} between {start} and {end}"
         )
         return None
 
@@ -953,14 +983,15 @@
             os.makedirs(video_snippet_storage_dir, exist_ok=True)
 
         video_metadata_with_file_paths = download_video_files(
             video_metadata=video_metadata,
             local_video_directory=video_snippet_storage_dir,
             max_workers=workers,
             overwrite=overwrite_video_snippets,
+            video_client=video_client,
         )
 
         concatenated_video_output = concat_videos(
             video_metadata=video_metadata_with_file_paths,
             start=start,
             end=end,
             output_directory=output_directory,
```

### Comparing `wf_video_io-3.3.5/video_io/utils.py` & `wf_video_io-3.4.0/video_io/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,23 @@
         ), df_video_files_by_device in (
             pd.DataFrame(video_metadata)
             .sort_values(by=["device_id", "video_timestamp"])
             .groupby(["environment_id", "assignment_id", "device_id"], dropna=False)
         ):
             video_output_path = f"{output_directory}/{environment_id}_{camera_device_id}_{start.strftime('%m%d%YT%H%M%S%f%z')}_{end.strftime('%m%d%YT%H%M%S%f%z')}.mp4"
 
+            if os.path.exists(video_output_path):
+                try:
+                    get_video_file_details(video_output_path)
+                except Exception as e:
+                    logger.error(
+                        f"Could not ffprobe video file {video_output_path} - {e}. Removing file and attempting to rebuild."
+                    )
+                    os.remove(video_output_path)
+
             if not os.path.exists(video_output_path) or overwrite:
                 # tmp_concat_demuxer_file is a temp file containing a list of video files to concatenate. This file
                 # gets input into ffmpeg.
                 with tempfile.NamedTemporaryFile() as tmp_concat_demuxer_file:
                     for idx, video_file_row in df_video_files_by_device.iterrows():
                         video_path = video_file_row["video_local_path"]
                         final_video_snippet_path = video_path
@@ -95,25 +104,31 @@
                             )
 
                         tmp_concat_demuxer_file.write(
                             str.encode(f"file 'file:{final_video_snippet_path}'\n")
                         )
                         tmp_concat_demuxer_file.flush()
 
-                    ffmpeg.input(
-                        f"file:{tmp_concat_demuxer_file.name}",
-                        format="concat",
-                        safe=0,
-                        r=video_snippet_fps,
-                    ).output(
-                        f"file:{video_output_path}",
-                        c="copy",
-                        r=video_snippet_fps,
-                        vsync=0,
-                    ).overwrite_output().run()
+                    try:
+                        ffmpeg.input(
+                            f"file:{tmp_concat_demuxer_file.name}",
+                            format="concat",
+                            safe=0,
+                            r=video_snippet_fps,
+                        ).output(
+                            f"file:{video_output_path}",
+                            c="copy",
+                            r=video_snippet_fps,
+                            vsync=0,
+                        ).overwrite_output().global_args(
+                            "-hide_banner", "-loglevel", "warning"
+                        ).run()
+                    except Exception as e:
+                        logger.error(e)
+                        raise e
 
             concatenated_video_output.append(
                 {
                     "environment_id": environment_id,
                     "camera_assignment_id": camera_assignment_id,
                     "camera_device_id": camera_device_id,
                     "file_path": video_output_path,
@@ -147,45 +162,44 @@
         end_trim (float): Trim to a given time, in seconds. This is NOT duration. (default is video's length in seconds)
         fps (int): Desired frames per second of output file (default is 10)
 
     Returns:
         (boolean): True if video could be trimmed and output to the given output_path
     """
     logging.info(
-        "Trimming video '{}' from {} seconds to {} seconds".format(
-            input_path, start_trim, end_trim
-        )
+        f"Trimming video '{input_path}' to a slice that starts at the {start_trim} second mark to the {end_trim} second mark"
     )
 
     if not os.path.exists(input_path):
         err = f"'{input_path}' does not exist, unable to trim video. Raising FileNotFoundError exception."
         logger.error(err)
         raise (FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), err))
 
+    video_reader = VideoReader(input_path)
     if end_trim is None:
-        video_reader = VideoReader(input_path)
         end_trim = video_reader.duration()
 
     tmp_file = None
     should_overwrite_input = input_path == output_path
     ffmpeg_output_path = output_path
     try:
         if should_overwrite_input:
             tmp_file = tempfile.NamedTemporaryFile(suffix=".mp4")
             ffmpeg_output_path = tmp_file.name
 
-        duration_seconds = end_trim - start_trim
-        ffmpeg.input(input_path, ss=start_trim, to=end_trim).output(
-            ffmpeg_output_path, r=fps, vframes=int(duration_seconds * fps)
-        ).overwrite_output().run()
+        ffmpeg.input(input_path).output(
+            ffmpeg_output_path,
+            r=fps,
+            vf=f"trim=start_frame={int(start_trim * video_reader.fps())}:end_frame={int(end_trim * video_reader.fps())}",
+        ).overwrite_output().global_args("-hide_banner", "-loglevel", "warning").run()
 
         if should_overwrite_input:
             shutil.copy(ffmpeg_output_path, input_path)
     except ffmpeg._run.Error as e:
-        logging.error("Failed trimming video {}".format(input_path))
+        logging.error(f"Failed trimming video {input_path}")
         logging.error(e)
 
         # Cleanup
         if tmp_file is None and os.path.exists(ffmpeg_output_path):
             try:
                 os.remove(ffmpeg_output_path)
             except:
@@ -235,15 +249,15 @@
 
     def get_grid(n):
         if n <= 0:
             return []
 
         row_width = math.ceil(math.sqrt(n))
         shape = []
-        for ii in range(row_width, n + 1, row_width):
+        for _ in range(row_width, n + 1, row_width):
             shape.append(row_width)
 
         if n > sum(shape):
             shape.append(n - sum(shape))
 
         return shape
 
@@ -262,10 +276,16 @@
         inputs=len(ffmpeg_inputs),
         layout="|".join(layout),
         # fill="black[out]"
     )
 
     ffmpeg.output(
         vout, _output_path, pix_fmt="yuv420p", vcodec="libx264"
-    ).overwrite_output().run()
+    ).overwrite_output().global_args("-hide_banner", "-loglevel", "warning").run()
 
     return _output_path
+
+
+def get_video_file_details(path):
+    # check for video file if it exists load that and return its contents.
+    # if not then run ffprobe and return a new meta document
+    return ffmpeg.probe(path)
```

### Comparing `wf_video_io-3.3.5/video_io/video_reader.py` & `wf_video_io-3.4.0/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.5/setup.py` & `wf_video_io-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.3.5',
+    'version': '3.4.0',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.3.5/PKG-INFO` & `wf_video_io-3.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.3.5
+Version: 3.4.0
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```

