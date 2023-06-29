# Comparing `tmp/warpzone_sdk-7.0.1.tar.gz` & `tmp/warpzone_sdk-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-7.0.1.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.0.0.tar", max compression
```

## Comparing `warpzone_sdk-7.0.1.tar` & `warpzone_sdk-8.0.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0     1121 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/pyproject.toml
--rw-r--r--   0        0        0     1182 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3035 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/monitor.py
--rw-r--r--   0        0        0     1486 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/process.py
--rw-r--r--   0        0        0       32 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0     1910 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/signature.py
--rw-r--r--   0        0        0       80 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-06-21 06:33:58.999712 warpzone_sdk-7.0.1/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2470 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0      219 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     2939 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/data.py
--rw-r--r--   0        0        0     1833 2023-06-21 06:33:59.003712 warpzone_sdk-7.0.1/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-7.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1279 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3419 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1486 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0     1910 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1604 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1330 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       47 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      521 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2470 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      219 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2939 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1833 2023-06-29 10:52:05.278320 warpzone_sdk-8.0.0/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.0.0/PKG-INFO
```

### Comparing `warpzone_sdk-7.0.1/pyproject.toml` & `warpzone_sdk-8.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "7.0.1"
+version = "8.0.0"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
-authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
+authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.4.3"
```

### Comparing `warpzone_sdk-7.0.1/warpzone/blobstorage/client.py` & `warpzone_sdk-8.0.0/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/functionize.py` & `warpzone_sdk-8.0.0/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/integrations.py` & `warpzone_sdk-8.0.0/warpzone/function/integrations.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import azure.functions as func
 import pandas as pd
 
 from warpzone.blobstorage.client import BlobData, WarpzoneBlobClient
 from warpzone.enums.topicenum import Topic
 from warpzone.servicebus.data.client import DataMessage, WarpzoneDataClient
 from warpzone.servicebus.events.client import EventMessage, WarpzoneEventClient
-from warpzone.tablestorage.client import WarpzoneTableClient
-from warpzone.tablestorage.client_async import WarpzoneTableClientAsync
+from warpzone.tablestorage.db.client import WarpzoneDatabaseClient
+from warpzone.tablestorage.db.client_async import WarpzoneDatabaseClientAsync
+from warpzone.tablestorage.tables.client import WarpzoneTableClient
+from warpzone.tablestorage.tables.client_async import WarpzoneTableClientAsync
 
 
 def get_data_client() -> WarpzoneDataClient:
     return WarpzoneDataClient.from_connection_strings(
         service_bus_conn_str=os.environ["SERVICE_BUS_CONNECTION_STRING"],
         storage_account_conn_str=os.environ["DATA_STORAGE_ACCOUNT_CONNECTION_STRING"],
     )
@@ -32,14 +34,26 @@
 
 def get_table_client_async() -> WarpzoneTableClientAsync:
     return WarpzoneTableClientAsync.from_connection_string(
         conn_str=os.environ["DATA_STORAGE_ACCOUNT_CONNECTION_STRING"],
     )
 
 
+def get_db_client() -> WarpzoneDatabaseClient:
+    return WarpzoneDatabaseClient.from_connection_string(
+        conn_str=os.environ["DATA_STORAGE_ACCOUNT_CONNECTION_STRING"],
+    )
+
+
+def get_db_client_async() -> WarpzoneDatabaseClientAsync:
+    return WarpzoneDatabaseClientAsync.from_connection_string(
+        conn_str=os.environ["DATA_STORAGE_ACCOUNT_CONNECTION_STRING"],
+    )
+
+
 def get_blob_client() -> WarpzoneBlobClient:
     return WarpzoneBlobClient.from_connection_string(
         conn_str=os.environ["ARCHIVE_STORAGE_ACCOUNT_CONNECTION_STRING"]
     )
 
 
 def func_msg_to_event(msg: func.ServiceBusMessage) -> EventMessage:
@@ -78,23 +92,19 @@
 def send_pandas(
     df: pd.DataFrame, topic: Topic, subject: str, schema: dict = None
 ) -> None:
     data_msg = DataMessage.from_pandas(df, subject, schema=schema)
     send_data(data_msg, topic)
 
 
-async def read_pandas(
+def read_pandas(
     table_name: str,
-    query: str,
+    time_interval: pd.Interval = None,
 ) -> pd.DataFrame:
-    table_client = get_table_client_async()
-    records = await table_client.query(table_name, query)
-    if not records:
-        return pd.DataFrame()
-    df = pd.DataFrame.from_records(records)
-    df = df.drop(columns=["PartitionKey", "RowKey"])
-    return df
+    db_client = get_db_client()
+
+    return db_client.query(table_name, time_interval)
 
 
 def upload_blob(blob_data: BlobData, container_name: str) -> None:
     blob_client = get_blob_client()
     blob_client.upload(container_name=container_name, blob_data=blob_data)
```

### Comparing `warpzone_sdk-7.0.1/warpzone/function/monitor.py` & `warpzone_sdk-8.0.0/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/process.py` & `warpzone_sdk-8.0.0/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.0.0/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.0.0/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/function/signature.py` & `warpzone_sdk-8.0.0/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.0.0/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/healthchecks/model.py` & `warpzone_sdk-8.0.0/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/monitor/logs.py` & `warpzone_sdk-8.0.0/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/monitor/traces.py` & `warpzone_sdk-8.0.0/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.0.0/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.0.0/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/tablestorage/client.py` & `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
     HttpResponseError,
     ServiceResponseError,
     ServiceResponseTimeoutError,
 )
 from azure.data.tables import TableServiceClient
 
 from warpzone.healthchecks import HealthCheckResult, HealthStatus
-from warpzone.tablestorage.operations import TableOperations
+from warpzone.tablestorage.tables.operations import TableOperations
 
 
 class WarpzoneTableClient:
-    """Class to interact with Azure Table"""
+    """Class to interact with Azure Table Storage for record lookups"""
 
     def __init__(self, table_service_client: TableServiceClient):
         self._table_service_client = table_service_client
 
     @classmethod
     def from_connection_string(cls, conn_str: str):
         """Get table client from connection string
```

### Comparing `warpzone_sdk-7.0.1/warpzone/tablestorage/client_async.py` & `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Module w.r.t. Azure table storage logic."""
 
 import asyncio
 
 from azure.data.tables.aio import TableServiceClient
 
-from warpzone.tablestorage.operations import TableOperations
+from warpzone.tablestorage.tables.operations import TableOperations
 
 
 class WarpzoneTableClientAsync:
     """Class to interact with Azure Table asyncronously."""
 
     def __init__(self, table_service_client: TableServiceClient):
         self._table_service_client = table_service_client
```

### Comparing `warpzone_sdk-7.0.1/warpzone/tablestorage/helpers.py` & `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/tablestorage/operations.py` & `warpzone_sdk-8.0.0/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/testing/assertions.py` & `warpzone_sdk-8.0.0/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/testing/data.py` & `warpzone_sdk-8.0.0/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/transform/data.py` & `warpzone_sdk-8.0.0/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/warpzone/transform/schema.py` & `warpzone_sdk-8.0.0/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-7.0.1/PKG-INFO` & `warpzone_sdk-8.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 7.0.1
+Version: 8.0.0
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
-Author: Anders Launer Baek-Petersen
-Author-email: alp@energinet.dk
+Author: Mikkel Ladekarl Folmersen Nygaard
+Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: azure-core-tracing-opentelemetry (>=1.0.0b9,<2.0.0)
```

