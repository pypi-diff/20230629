# Comparing `tmp/idun_mock-0.1.2.tar.gz` & `tmp/idun_mock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_mock-0.1.2.tar", max compression
+gzip compressed data, was "idun_mock-0.1.3.tar", max compression
```

## Comparing `idun_mock-0.1.2.tar` & `idun_mock-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1310 2023-06-27 21:12:32.598105 idun_mock-0.1.2/README.md
--rw-r--r--   0        0        0      148 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/__init__.py
--rw-r--r--   0        0        0     7617 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/client/__init__.py
--rw-r--r--   0        0        0     5631 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/client/__main__.py
--rw-r--r--   0        0        0      167 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/__init__.py
--rw-r--r--   0        0        0     8398 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/connection_pool.py
--rw-r--r--   0        0        0     4930 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/generator.py
--rw-r--r--   0        0        0     3081 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets-0.txt
--rw-r--r--   0        0        0    17548 2023-06-27 21:12:32.598105 idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets.txt
--rw-r--r--   0        0        0      731 2023-06-27 21:12:32.598105 idun_mock-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 idun_mock-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1310 2023-06-29 14:02:32.150903 idun_mock-0.1.3/README.md
+-rw-r--r--   0        0        0      148 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/__init__.py
+-rw-r--r--   0        0        0     8504 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/client/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/client/__main__.py
+-rw-r--r--   0        0        0      167 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/data_generator/__init__.py
+-rw-r--r--   0        0        0     8398 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/data_generator/connection_pool.py
+-rw-r--r--   0        0        0     4930 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/data_generator/generator.py
+-rw-r--r--   0        0        0     3081 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/data_generator/igeb_test_packets-0.txt
+-rw-r--r--   0        0        0    17548 2023-06-29 14:02:32.150903 idun_mock-0.1.3/idun_mock/data_generator/igeb_test_packets.txt
+-rw-r--r--   0        0        0      809 2023-06-29 14:02:32.150903 idun_mock-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 idun_mock-0.1.3/PKG-INFO
```

### Comparing `idun_mock-0.1.2/README.md` & `idun_mock-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/idun_mock/client/__init__.py` & `idun_mock-0.1.3/idun_mock/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio, json, csv, httpx
 import websockets.exceptions
 from datetime import datetime
-from idun_data_models import RecordingIn, RecordingConfig, DataStreams
+from idun_data_models import RecordingIn, RecordingStatusIn, RecordingConfig, DataStreams
 from idun_tools import logger
 from ..data_generator import generate_queue, GeneratorTime
 
 
 class MockGuardianDataGenerator:
     def __init__(self):
         self.message_queue = asyncio.Queue(maxsize=int(1e7))
@@ -53,40 +53,37 @@
 
     async def register_recordings(self, rest_api_url: str) -> None:
         async def register_recording(client, deviceID, recordingID):
             payload = RecordingIn(
                 recordingID=recordingID,
                 deviceID=deviceID,
                 displayName="mock data generator",
-                config=RecordingConfig(
-                    data_stream_subscription=DataStreams(bandpass_eeg=True)
-                ),
+                config=RecordingConfig(data_stream_subscription=DataStreams(bandpass_eeg=True)),
             )
             logger.bind(payload=payload).info("Registering recording")
             await http_post(
                 client,
-                f"{rest_api_url}/api/recording/{deviceID}/recordings",
+                f"{rest_api_url}/devices/{deviceID}/recordings",
                 auth=(deviceID, ""),
                 content=payload.json(),
             )
 
         recordingIDs = await self.gather_recordingIDs()
         async with httpx.AsyncClient() as client, asyncio.TaskGroup() as tg:
             for i in recordingIDs:
-                tg.create_task(
-                    register_recording(client, i["deviceID"], i["recordingID"])
-                )
+                tg.create_task(register_recording(client, i["deviceID"], i["recordingID"]))
         logger.info("Recordings registered")
 
     async def stop_recordings(self, rest_api_url: str) -> None:
         async def stop_recording(client, deviceID, recordingID):
-            await http_post(
+            await http_put(
                 client,
-                f"{rest_api_url}/api/recording/{deviceID}/{recordingID}/stop",
+                f"{rest_api_url}/devices/{deviceID}/recordings/{recordingID}/status",
                 auth=(deviceID, ""),
+                content=RecordingStatusIn(stopped=True).json(),
             )
 
         recordingIDs = await self.gather_recordingIDs()
         async with httpx.AsyncClient() as client, asyncio.TaskGroup() as tg:
             for i in recordingIDs:
                 tg.create_task(stop_recording(client, i["deviceID"], i["recordingID"]))
         logger.info("Recordings stopped")
@@ -126,17 +123,15 @@
 
         async def may_block(latency_f):
             message = json.loads(await websocket.recv())
             if "bp_filter_eeg" in message:
                 ts = message["bp_filter_eeg"]["timestamp"][0]
                 latency = datetime.now().timestamp() - ts
                 samples_in_message = len(message["bp_filter_eeg"]["timestamp"])
-                logger.info(
-                    f"Latency: {latency} ({samples_in_message} samples in message)"
-                )
+                logger.info(f"Latency: {latency} ({samples_in_message} samples in message)")
                 latency_f.writerow(
                     {
                         "timestamp": ts,
                         "deviceID": message["deviceID"],
                         "latency": latency,
                     }
                 )
@@ -151,17 +146,15 @@
                 if latency_f.tell() == 0:
                     latency_csv.writeheader()
                 while not stop.is_set():
                     await asyncio.wait_for(may_block(latency_csv), timeout=6.0)
         except asyncio.TimeoutError:
             logger.info("Receiving timed out")
 
-    async def send_kinesis(
-        self, kinesis_client, stream_name, stop: asyncio.Event = None
-    ):
+    async def send_kinesis(self, kinesis_client, stream_name, stop: asyncio.Event = None):
         "Put data to Kinesis from the queue"
 
         if stop is None:
             stop = self.stop
 
         async def may_block():
             message = await self.message_queue.get()
@@ -200,11 +193,36 @@
             http_headers=err.response.headers,
             elapsed_sec=err.response.elapsed.total_seconds(),
         ).warning(f"Received error code from POST {url}")
     except httpx.RequestError as err:
         logger.bind(error=err).error("HTTP request error")
 
 
+async def http_put(client: httpx.AsyncClient, url: str, auth, content=None):
+    try:
+        response = await client.put(
+            url,
+            content=content,
+            auth=auth,
+            headers=httpx.Headers({"Content-Type": "application/json"}),
+        )
+        response.raise_for_status()
+    except httpx.HTTPStatusError as err:
+        status_code = err.response.status_code
+        logger.bind(
+            request=err.request,
+            response=err.response,
+            reason=err.response.reason_phrase,
+            reason_text=err.response.text,
+            status_code=status_code,
+            http_version=err.response.http_version,
+            http_headers=err.response.headers,
+            elapsed_sec=err.response.elapsed.total_seconds(),
+        ).warning(f"Received error code from PUT {url}")
+    except httpx.RequestError as err:
+        logger.bind(error=err).error("HTTP request error")
+
+
 def apiGatewayTransform(message: dict):
     "Wrap message with the API gateway's template transform"
     message["connectionID"] = "a"
     return message
```

### Comparing `idun_mock-0.1.2/idun_mock/client/__main__.py` & `idun_mock-0.1.3/idun_mock/client/__main__.py`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/idun_mock/data_generator/connection_pool.py` & `idun_mock-0.1.3/idun_mock/data_generator/connection_pool.py`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/idun_mock/data_generator/generator.py` & `idun_mock-0.1.3/idun_mock/data_generator/generator.py`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets-0.txt` & `idun_mock-0.1.3/idun_mock/data_generator/igeb_test_packets-0.txt`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/idun_mock/data_generator/igeb_test_packets.txt` & `idun_mock-0.1.3/idun_mock/data_generator/igeb_test_packets.txt`

 * *Files identical despite different names*

### Comparing `idun_mock-0.1.2/PKG-INFO` & `idun_mock-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-mock
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mock a real IDUN Guardian device for testing purposes
 Author: Konstantinos Samaras-Tsakiris
 Author-email: konstantinos@iduntechnologies.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

