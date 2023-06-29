# Comparing `tmp/python-matter-server-3.6.2.tar.gz` & `tmp/python-matter-server-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.6.2.tar", last modified: Wed Jun 28 15:04:06 2023, max compression
+gzip compressed data, was "python-matter-server-3.6.3.tar", last modified: Thu Jun 29 08:56:13 2023, max compression
```

## Comparing `python-matter-server-3.6.2.tar` & `python-matter-server-3.6.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.976177 python-matter-server-3.6.2/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    35120 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-28 15:03:52.000000 python-matter-server-3.6.2/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-28 15:03:55.000000 python-matter-server-3.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:04:04.000000 python-matter-server-3.6.2/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 15:04:06.000000 python-matter-server-3.6.2/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-28 15:04:06.980177 python-matter-server-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36859 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-29 08:56:00.000000 python-matter-server-3.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-29 08:56:12.000000 python-matter-server-3.6.3/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:12.000000 python-matter-server-3.6.3/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:11.000000 python-matter-server-3.6.3/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/setup.cfg
```

### Comparing `python-matter-server-3.6.2/LICENSE` & `python-matter-server-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/PKG-INFO` & `python-matter-server-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.2
+Version: 3.6.3
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.2/README.md` & `python-matter-server-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/client/client.py` & `python-matter-server-3.6.3/matter_server/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 from .models.node import MatterFabricData, MatterNode
 
 if TYPE_CHECKING:
     from chip.clusters.Objects import ClusterCommand
 
 SUB_WILDCARD: Final = "*"
 
+# pylint: disable=too-many-public-methods
+
 
 class MatterClient:
     """Manage a Matter server over WebSockets."""
 
     def __init__(self, ws_server_url: str, aiohttp_session: ClientSession):
         """Initialize the Client class."""
         self.connection = MatterClientConnection(ws_server_url, aiohttp_session)
@@ -227,14 +229,42 @@
             command_name=command_name,
             payload=dataclass_to_dict(command),
             response_type=response_type,
             timed_request_timeout_ms=timed_request_timeout_ms,
             interaction_timeout_ms=interaction_timeout_ms,
         )
 
+    async def read_attribute(
+        self,
+        node_id: int,
+        attribute_path: str,
+    ) -> Any:
+        """Read a single attribute on a node."""
+        return await self.send_command(
+            APICommand.READ_ATTRIBUTE,
+            require_schema=4,
+            node_id=node_id,
+            attribute_path=attribute_path,
+        )
+
+    async def write_attribute(
+        self,
+        node_id: int,
+        attribute_path: str,
+        value: Any,
+    ) -> Any:
+        """Write an attribute(value) on a target node."""
+        return await self.send_command(
+            APICommand.WRITE_ATTRIBUTE,
+            require_schema=4,
+            node_id=node_id,
+            attribute_path=attribute_path,
+            value=value,
+        )
+
     async def remove_node(self, node_id: int) -> None:
         """Remove a Matter node/device from the fabric."""
         await self.send_command(APICommand.REMOVE_NODE, node_id=node_id)
 
     async def subscribe_attribute(
         self, node_id: int, attribute_path: str | list[str]
     ) -> None:
```

### Comparing `python-matter-server-3.6.2/matter_server/client/connection.py` & `python-matter-server-3.6.3/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/client/exceptions.py` & `python-matter-server-3.6.3/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/client/models/device_types.py` & `python-matter-server-3.6.3/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/client/models/node.py` & `python-matter-server-3.6.3/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/common/errors.py` & `python-matter-server-3.6.3/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/common/helpers/api.py` & `python-matter-server-3.6.3/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/common/helpers/json.py` & `python-matter-server-3.6.3/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/common/helpers/util.py` & `python-matter-server-3.6.3/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/common/models.py` & `python-matter-server-3.6.3/matter_server/common/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     OPEN_COMMISSIONING_WINDOW = "open_commissioning_window"
     DISCOVER = "discover"
     INTERVIEW_NODE = "interview_node"
     DEVICE_COMMAND = "device_command"
     REMOVE_NODE = "remove_node"
     GET_VENDOR_NAMES = "get_vendor_names"
     SUBSCRIBE_ATTRIBUTE = "subscribe_attribute"
+    READ_ATTRIBUTE = "read_attribute"
+    WRITE_ATTRIBUTE = "write_attribute"
 
 
 EventCallBackType = Callable[[EventType, Any], None]
 
 # Generic model(s)
```

### Comparing `python-matter-server-3.6.2/matter_server/server/__main__.py` & `python-matter-server-3.6.3/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/client_handler.py` & `python-matter-server-3.6.3/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/const.py` & `python-matter-server-3.6.3/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/device_controller.py` & `python-matter-server-3.6.3/matter_server/server/device_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,14 +379,58 @@
                 endpoint=endpoint_id,
                 payload=command,
                 responseType=response_type,
                 timedRequestTimeoutMs=timed_request_timeout_ms,
                 interactionTimeoutMs=interaction_timeout_ms,
             )
 
+    @api_command(APICommand.READ_ATTRIBUTE)
+    async def read_attribute(
+        self,
+        node_id: int,
+        attribute_path: str,
+    ) -> Any:
+        """Read a single attribute on a node."""
+        if self.chip_controller is None:
+            raise RuntimeError("Device Controller not initialized.")
+        node_lock = self._get_node_lock(node_id)
+        await self._resolve_node(node_id=node_id)
+        endpoint_id, cluster_id, attribute_id = parse_attribute_path(attribute_path)
+        attribute: Type[ClusterAttributeDescriptor] = ALL_ATTRIBUTES[cluster_id][
+            attribute_id
+        ]
+        async with node_lock:
+            result: Attribute.AsyncReadTransaction.ReadResponse = (
+                await self.chip_controller.Read(
+                    nodeid=node_id,
+                    attributes=[(endpoint_id, attribute)],
+                    fabricFiltered=False,
+                )
+            )
+            read_atributes = self._parse_attributes_from_read_result(result.attributes)
+            return read_atributes[attribute_path]
+
+    @api_command(APICommand.WRITE_ATTRIBUTE)
+    async def write_attribute(
+        self,
+        node_id: int,
+        attribute_path: str,
+        value: Any,
+    ) -> Any:
+        """Write an attribute(value) on a target node."""
+        if self.chip_controller is None:
+            raise RuntimeError("Device Controller not initialized.")
+        endpoint_id, cluster_id, attribute_id = parse_attribute_path(attribute_path)
+        attribute = ALL_ATTRIBUTES[cluster_id][attribute_id]()
+        attribute.value = value
+        return await self.chip_controller.WriteAttribute(
+            nodeid=node_id,
+            attributes=[(endpoint_id, attribute)],
+        )
+
     @api_command(APICommand.REMOVE_NODE)
     async def remove_node(self, node_id: int) -> None:
         """Remove a Matter node/device from the fabric."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         if node_id not in self._nodes:
```

### Comparing `python-matter-server-3.6.2/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.6.3/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/server.py` & `python-matter-server-3.6.3/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/stack.py` & `python-matter-server-3.6.3/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/storage.py` & `python-matter-server-3.6.3/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/matter_server/server/vendor_info.py` & `python-matter-server-3.6.3/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.2/pyproject.toml` & `python-matter-server-3.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.6.2"
+version = "3.6.3"
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "The Home Assistant Authors", email = "hello@home-assistant.io" },
 ]
 classifiers = [
```

### Comparing `python-matter-server-3.6.2/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.6.3/python_matter_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.2
+Version: 3.6.3
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.2/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.6.3/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

