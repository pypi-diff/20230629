# Comparing `tmp/zkaccess_c3-0.0.6.tar.gz` & `tmp/zkaccess_c3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkaccess_c3-0.0.6.tar", last modified: Sun Jun 25 20:55:47 2023, max compression
+gzip compressed data, was "zkaccess_c3-0.0.7.tar", last modified: Thu Jun 29 19:35:45 2023, max compression
```

## Comparing `zkaccess_c3-0.0.6.tar` & `zkaccess_c3-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.579343 zkaccess_c3-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/c3/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_CancelAlarms.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_Discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_GetDeviceParam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_GetRTLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_OutputOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 20:55:47.579343 zkaccess_c3-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_crc16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:45.168112 zkaccess_c3-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-29 19:35:45.164112 zkaccess_c3-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:45.164112 zkaccess_c3-0.0.7/c3/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19483 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/c3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:45.164112 zkaccess_c3-0.0.7/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/cli/C3_CancelAlarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/cli/C3_Discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/cli/C3_GetDeviceParam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/cli/C3_GetRTLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/cli/C3_OutputOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:35:45.168112 zkaccess_c3-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:45.164112 zkaccess_c3-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_crc16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 19:35:31.000000 zkaccess_c3-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:35:45.164112 zkaccess_c3-0.0.7/zkaccess_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-29 19:35:45.000000 zkaccess_c3-0.0.7/zkaccess_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-29 19:35:45.000000 zkaccess_c3-0.0.7/zkaccess_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:35:45.000000 zkaccess_c3-0.0.7/zkaccess_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-29 19:35:45.000000 zkaccess_c3-0.0.7/zkaccess_c3.egg-info/top_level.txt
```

### Comparing `zkaccess_c3-0.0.6/LICENSE` & `zkaccess_c3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/PKG-INFO` & `zkaccess_c3-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess_c3
-Version: 0.0.6
+Version: 0.0.7
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `zkaccess_c3-0.0.6/c3/consts.py` & `zkaccess_c3-0.0.7/c3/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,20 +134,22 @@
     NORMAL_OPEN_TZ_OVER = 204, "Normal Open Time Zone Over"
     REMOTE_NORMAL_OPEN = 205, "Remote Normal Opening"
     DEVICE_START = 206, "Device Start"
     DOOR_OPEN_BY_SUPERUSER = 208, "Door Opened by Superuser"
     AUX_INPUT_DISCONNECT = 220, "Auxiliary Input Disconnected"
     AUX_INPUT_SHORT = 221, "Auxiliary Input Shorted"
     DOOR_ALARM_STATUS = 255, "Current door and alarm status"
+    UNKNOWN_UNSUPPORTED = 999, "Unknown"
 
 
 class InOutDirection(_IntEnumWithDescription):
     ENTRY = 0, "Entry"
     EXIT = 3,  "Exit"
     NONE = 2,  "None"
+    UNKNOWN_UNSUPPORTED = 15, "Unknown"
 
 
 class AlarmStatus(_IntEnumWithDescription):
     NONE = 0,              "None"
     ALARM = 1,             "Alarm"
     DOOR_OPEN_TIMEOUT = 2, "Door opening timeout"
```

### Comparing `zkaccess_c3-0.0.6/c3/controldevice.py` & `zkaccess_c3-0.0.7/c3/controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/c3/core.py` & `zkaccess_c3-0.0.7/c3/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,19 +120,22 @@
         return bytes_written
 
     def _receive(self) -> tuple[bytearray, int]:
         # Get the first 5 bytes
         header = self._sock.recv(5)
         self.log.debug("Receiving header: %s", header.hex())
 
+        message = bytearray()
         received_command, data_size = self._get_message_header(header)
-        # Get the message data and signature
+        # Get the optional message data, checksum and end marker
         payload = self._sock.recv(data_size + 3)
-        self.log.debug("Receiving payload: %s", payload.hex())
-        message = self._get_message(header + payload)
+        if data_size > 0:
+            # Process message in case data available
+            self.log.debug("Receiving payload: %s", payload.hex())
+            message = self._get_message(header + payload)
 
         if len(message) != data_size:
             raise ValueError(f"Length of received message ({len(message)}) does not match specified size ({data_size})")
 
         if received_command == consts.C3_REPLY_OK:
             pass
         elif received_command == consts.C3_REPLY_ERROR:
@@ -145,23 +148,27 @@
         return message, data_size
 
     def _send_receive(self, command: consts.Command, data=None) -> tuple[bytearray, int]:
         bytes_received = 0
         receive_data = bytearray()
         session_offset = 0
 
-        bytes_written = self._send(command, data)
-        if bytes_written > 0:
-            receive_data, bytes_received = self._receive()
-            if not self._session_less and bytes_received > 2:
-                session_offset = 4
-                session_id = (receive_data[1] << 8) + receive_data[0]
-                # msg_seq = (receive_data[3] << 8) + receive_data[2]
-                if self._session_id != session_id:
-                    raise ValueError("Data received with invalid session ID")
+        try:
+            bytes_written = self._send(command, data)
+            if bytes_written > 0:
+                receive_data, bytes_received = self._receive()
+                if not self._session_less and bytes_received > 2:
+                    session_offset = 4
+                    session_id = (receive_data[1] << 8) + receive_data[0]
+                    # msg_seq = (receive_data[3] << 8) + receive_data[2]
+                    if self._session_id != session_id:
+                        raise ValueError("Data received with invalid session ID")
+        except BrokenPipeError as ex:
+            self._connected = False
+            raise ConnectionError(f"Unexpected connection end: {ex}") from ex
 
         return receive_data[session_offset:], bytes_received-session_offset
 
     def is_connected(self) -> bool:
         # try:
         #    # this will try to read bytes without blocking and also without removing them from buffer (peek only)
         #    data = self._sock.recv(1, socket.MSG_DONTWAIT | socket.MSG_PEEK)
```

### Comparing `zkaccess_c3-0.0.6/c3/crc.py` & `zkaccess_c3-0.0.7/c3/crc.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/c3/rtlog.py` & `zkaccess_c3-0.0.7/c3/rtlog.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,22 @@
         self.time_second = 0
 
     @classmethod
     def from_bytes(cls, data: bytes):
         record = DoorAlarmStatusRecord()
         record.alarm_status = bytes(data[0:4])
         record.dss_status = bytes(data[4:8])
-        record.verified = consts.VerificationMode(data[9])
-        record.event_type = consts.EventType(data[10])
+        try:
+            record.verified = consts.VerificationMode(data[9])
+        except ValueError:
+            record.verified = consts.VerificationMode.OTHER
+        try:
+            record.event_type = consts.EventType(data[10])
+        except ValueError:
+            record.event_type = consts.EventType.UNKNOWN_UNSUPPORTED
         record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
         return record
 
     def is_door_alarm(self) -> bool:
         return True
 
     def is_event(self) -> bool:
@@ -149,18 +155,27 @@
         self.time_second = 0
 
     @classmethod
     def from_bytes(cls, data: bytes):
         record = EventRecord()
         record.card_no = int.from_bytes(data[0:4], byteorder="little")
         record.pin = int.from_bytes(data[4:8], byteorder="little")
-        record.verified = consts.VerificationMode(data[8])
+        try:
+            record.verified = consts.VerificationMode(data[8])
+        except ValueError:
+            record.verified = consts.VerificationMode.OTHER
         record.door_id = data[9]
-        record.event_type = consts.EventType(data[10])
-        record.in_out_state = consts.InOutDirection(data[11])
+        try:
+            record.event_type = consts.EventType(data[10])
+        except ValueError:
+            record.event_type = consts.EventType.UNKNOWN_UNSUPPORTED
+        try:
+            record.in_out_state = consts.InOutDirection(data[11])
+        except ValueError:
+            record.in_out_state = consts.InOutDirection.UNKNOWN_UNSUPPORTED
         record.time_second = C3DateTime.from_value(int.from_bytes(data[12:16], byteorder="little"))
         return record
 
     def is_door_alarm(self) -> bool:
         return False
 
     def is_event(self) -> bool:
```

### Comparing `zkaccess_c3-0.0.6/c3/utils.py` & `zkaccess_c3-0.0.7/c3/utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/cli/C3_CancelAlarms.py` & `zkaccess_c3-0.0.7/cli/C3_CancelAlarms.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/cli/C3_Discover.py` & `zkaccess_c3-0.0.7/cli/C3_Discover.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/cli/C3_GetDeviceParam.py` & `zkaccess_c3-0.0.7/cli/C3_GetDeviceParam.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/cli/C3_GetRTLog.py` & `zkaccess_c3-0.0.7/cli/C3_GetRTLog.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/cli/C3_OutputOperation.py` & `zkaccess_c3-0.0.7/cli/C3_OutputOperation.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/pyproject.toml` & `zkaccess_c3-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zkaccess_c3"
-version = "0.0.6"
+version = "0.0.7"
 description = "A native Python library for communicating with the ZKAccess C3 Access Control Panels."
 authors = [
     {name = "Vwout", email="vwout@users.noreply.github.com"},
 ]
 #license = "GPL-3.0-or-later"
 readme = "readme.md"
 requires-python = ">=3.7"
```

### Comparing `zkaccess_c3-0.0.6/readme.md` & `zkaccess_c3-0.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/tests/test_consts.py` & `zkaccess_c3-0.0.7/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/tests/test_controldevice.py` & `zkaccess_c3-0.0.7/tests/test_controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/tests/test_core.py` & `zkaccess_c3-0.0.7/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from unittest import mock
 import time
+import pytest
 
 from c3 import rtlog
 from c3.core import C3
 from c3 import consts
 from c3 import controldevice
 
 
@@ -17,18 +18,18 @@
     assert panel.aux_out_status(2) == consts.InOutStatus.UNKNOWN
 
 
 def test_core_get_device_param():
     with mock.patch('socket.socket') as mock_socket:
         panel = C3('localhost')
         mock_socket.return_value.send.return_value = 8
-        mock_socket.return_value.recv.side_effect = [bytes.fromhex("aa01c80400"),
-                                                     bytes.fromhex("d18a0000915255"),
-                                                     bytes.fromhex("aa01c80400"),
-                                                     bytes.fromhex("d18a0000")]
+        mock_socket.return_value.recv.side_effect = [
+            bytes.fromhex("aa01c80400"), bytes.fromhex("d18a0000915255"),
+            bytes.fromhex("aa01c80400"), bytes.fromhex("d18a000055")
+        ]
 
         assert panel.connect() is True
 
         mock_socket.return_value.recv.side_effect = [bytes.fromhex("aa01c84800"),
                                                      bytes.fromhex(
             "d18a02007e5a4b465056657273696f6e3d31302c4c6f636b436f756e743d322c5265616465"
             "72436f756e743d342c417578496e436f756e743d322c4175784f7574436f756e743d32783f55")]
@@ -36,15 +37,47 @@
         assert params["~ZKFPVersion"] == "10"
         assert params["LockCount"] == "2"
         assert params["ReaderCount"] == "4"
         assert params["AuxInCount"] == "2"
         assert params["AuxOutCount"] == "2"
 
 
-def test_core_get_device_param_session_less():
+def test_core_connect_response_incomplete():
+    with mock.patch('socket.socket') as mock_socket:
+        panel = C3('localhost')
+        mock_socket.return_value.send.return_value = 8
+        mock_socket.return_value.recv.side_effect = [
+            bytes.fromhex("aa01c80400"), bytes.fromhex("d18a0000915255"),
+            bytes.fromhex("aa01c80400"), bytes.fromhex("d18a000055")
+        ]
+
+        assert panel.connect() is True
+
+        mock_socket.return_value.recv.side_effect = [bytes.fromhex("aa01c80800"), bytes.fromhex("d18a020012345678")]
+        with pytest.raises(ValueError):
+            panel.get_device_param([])
+
+
+def test_core_connect_response_no_data():
+    with mock.patch('socket.socket') as mock_socket:
+        panel = C3('localhost')
+        mock_socket.return_value.send.return_value = 8
+        mock_socket.return_value.recv.side_effect = [
+            bytes.fromhex("aa01c80400"), bytes.fromhex("d18a0000915255"),
+            bytes(), bytes()
+        ]
+
+        assert panel.connect() is True
+
+        mock_socket.return_value.recv.side_effect = [bytes.fromhex("aa01c80800"), bytes()]
+        with pytest.raises(ValueError):
+            panel.get_device_param([])
+
+
+def test_core_connect_session_less():
     with mock.patch('socket.socket') as mock_socket:
         panel = C3('localhost')
         mock_socket.return_value.send.return_value = 8
         mock_socket.return_value.recv.side_effect = [
             # Reject response to session connect attempt
             bytes.fromhex("aa01c90100"), bytes.fromhex("f313d955"),
             # Confirm session-less connection attempt
```

### Comparing `zkaccess_c3-0.0.6/tests/test_crc16.py` & `zkaccess_c3-0.0.7/tests/test_crc16.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/tests/test_utils.py` & `zkaccess_c3-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.6/zkaccess_c3.egg-info/PKG-INFO` & `zkaccess_c3-0.0.7/zkaccess_c3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess-c3
-Version: 0.0.6
+Version: 0.0.7
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `zkaccess_c3-0.0.6/zkaccess_c3.egg-info/SOURCES.txt` & `zkaccess_c3-0.0.7/zkaccess_c3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

