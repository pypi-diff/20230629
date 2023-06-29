# Comparing `tmp/ably-2.0.0b5.tar.gz` & `tmp/ably-2.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ably-2.0.0b5.tar", max compression
+gzip compressed data, was "ably-2.0.0b6.tar", max compression
```

## Comparing `ably-2.0.0b5.tar` & `ably-2.0.0b6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    10173 2022-10-12 21:24:17.455790 ably-2.0.0b5/LICENSE
--rw-r--r--   0        0        0      458 2022-10-12 21:24:17.455984 ably-2.0.0b5/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0      627 2023-03-27 17:12:46.756407 ably-2.0.0b5/ably/__init__.py
--rw-r--r--   0        0        0        0 2022-10-12 21:24:17.456796 ably-2.0.0b5/ably/http/__init__.py
--rw-r--r--   0        0        0     9687 2023-03-27 17:12:44.506385 ably-2.0.0b5/ably/http/http.py
--rw-r--r--   0        0        0     1058 2023-03-27 17:12:44.506703 ably-2.0.0b5/ably/http/httputils.py
--rw-r--r--   0        0        0     4204 2022-10-12 21:24:17.457251 ably-2.0.0b5/ably/http/paginatedresult.py
--rw-r--r--   0        0        0        0 2023-03-27 17:12:44.506796 ably-2.0.0b5/ably/realtime/__init__.py
--rw-r--r--   0        0        0     4157 2023-03-27 17:12:44.507350 ably-2.0.0b5/ably/realtime/connection.py
--rw-r--r--   0        0        0    22131 2023-03-27 17:12:44.508032 ably-2.0.0b5/ably/realtime/connectionmanager.py
--rw-r--r--   0        0        0     5677 2023-03-27 17:12:44.508548 ably-2.0.0b5/ably/realtime/realtime.py
--rw-r--r--   0        0        0    19058 2023-03-27 17:12:44.509189 ably-2.0.0b5/ably/realtime/realtime_channel.py
--rw-r--r--   0        0        0        0 2022-10-12 21:24:17.457418 ably-2.0.0b5/ably/rest/__init__.py
--rw-r--r--   0        0        0    17119 2023-03-27 17:12:44.509935 ably-2.0.0b5/ably/rest/auth.py
--rw-r--r--   0        0        0     7577 2023-03-27 17:12:44.510581 ably-2.0.0b5/ably/rest/channel.py
--rw-r--r--   0        0        0     6529 2023-03-27 17:12:44.511029 ably-2.0.0b5/ably/rest/push.py
--rw-r--r--   0        0        0     5210 2023-03-27 17:12:44.511458 ably-2.0.0b5/ably/rest/rest.py
--rw-r--r--   0        0        0        0 2022-10-12 21:24:17.458240 ably-2.0.0b5/ably/transport/__init__.py
--rw-r--r--   0        0        0     1787 2023-03-27 17:12:44.512076 ably-2.0.0b5/ably/transport/defaults.py
--rw-r--r--   0        0        0     8683 2023-03-27 17:12:44.512640 ably-2.0.0b5/ably/transport/websockettransport.py
--rw-r--r--   0        0        0        0 2022-10-12 21:24:17.458588 ably-2.0.0b5/ably/types/__init__.py
--rw-r--r--   0        0        0     4601 2022-10-12 21:24:17.458807 ably-2.0.0b5/ably/types/authoptions.py
--rw-r--r--   0        0        0     2238 2022-10-12 21:24:17.459010 ably-2.0.0b5/ably/types/capability.py
--rw-r--r--   0        0        0     2931 2022-10-12 21:24:17.459161 ably-2.0.0b5/ably/types/channeldetails.py
--rw-r--r--   0        0        0      507 2023-03-27 17:12:44.513192 ably-2.0.0b5/ably/types/channelstate.py
--rw-r--r--   0        0        0     1757 2022-10-12 21:24:17.459355 ably-2.0.0b5/ably/types/channelsubscription.py
--rw-r--r--   0        0        0      724 2023-03-27 17:12:44.513693 ably-2.0.0b5/ably/types/connectiondetails.py
--rw-r--r--   0        0        0      740 2023-03-27 17:12:44.514248 ably-2.0.0b5/ably/types/connectionerrors.py
--rw-r--r--   0        0        0      846 2023-03-27 17:12:44.514764 ably-2.0.0b5/ably/types/connectionstate.py
--rw-r--r--   0        0        0     3115 2022-10-12 21:24:17.459514 ably-2.0.0b5/ably/types/device.py
--rw-r--r--   0        0        0      413 2023-03-27 17:12:44.515316 ably-2.0.0b5/ably/types/flags.py
--rw-r--r--   0        0        0     6254 2023-02-20 15:06:15.951208 ably-2.0.0b5/ably/types/message.py
--rw-r--r--   0        0        0     2725 2023-02-20 15:06:15.951688 ably-2.0.0b5/ably/types/mixins.py
--rw-r--r--   0        0        0     9714 2023-03-27 17:12:44.516124 ably-2.0.0b5/ably/types/options.py
--rw-r--r--   0        0        0     5082 2023-02-20 15:06:15.952022 ably-2.0.0b5/ably/types/presence.py
--rw-r--r--   0        0        0     5944 2022-10-12 21:24:17.460814 ably-2.0.0b5/ably/types/stats.py
--rw-r--r--   0        0        0     2852 2023-03-27 17:12:44.516858 ably-2.0.0b5/ably/types/tokendetails.py
--rw-r--r--   0        0        0     2833 2022-10-12 21:24:17.461181 ably-2.0.0b5/ably/types/tokenrequest.py
--rw-r--r--   0        0        0     3272 2022-10-12 21:24:17.461399 ably-2.0.0b5/ably/types/typedbuffer.py
--rw-r--r--   0        0        0        0 2022-10-12 21:24:17.461575 ably-2.0.0b5/ably/util/__init__.py
--rw-r--r--   0        0        0      370 2022-10-12 21:24:17.461894 ably-2.0.0b5/ably/util/case.py
--rw-r--r--   0        0        0     5433 2023-03-27 17:12:44.517607 ably-2.0.0b5/ably/util/crypto.py
--rw-r--r--   0        0        0     6731 2023-03-27 17:12:44.518266 ably-2.0.0b5/ably/util/eventemitter.py
--rw-r--r--   0        0        0     2740 2023-03-27 17:12:44.518903 ably-2.0.0b5/ably/util/exceptions.py
--rw-r--r--   0        0        0     1046 2023-03-27 17:12:44.519432 ably-2.0.0b5/ably/util/helper.py
--rw-r--r--   0        0        0      221 2022-10-12 21:24:17.462632 ably-2.0.0b5/ably/util/nocrypto.py
--rw-r--r--   0        0        0     1623 2023-03-27 17:12:46.757184 ably-2.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 ably-2.0.0b5/setup.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 ably-2.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0    10173 2022-10-12 21:24:17.455790 ably-2.0.0b6/LICENSE
+-rw-r--r--   0        0        0      458 2022-10-12 21:24:17.455984 ably-2.0.0b6/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0      627 2023-05-05 16:43:53.632072 ably-2.0.0b6/ably/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-12 21:24:17.456796 ably-2.0.0b6/ably/http/__init__.py
+-rw-r--r--   0        0        0     9687 2023-05-05 16:43:51.749157 ably-2.0.0b6/ably/http/http.py
+-rw-r--r--   0        0        0     1058 2023-05-05 16:43:51.749407 ably-2.0.0b6/ably/http/httputils.py
+-rw-r--r--   0        0        0     4204 2022-10-12 21:24:17.457251 ably-2.0.0b6/ably/http/paginatedresult.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:43:51.749482 ably-2.0.0b6/ably/realtime/__init__.py
+-rw-r--r--   0        0        0     4157 2023-05-05 16:43:51.749738 ably-2.0.0b6/ably/realtime/connection.py
+-rw-r--r--   0        0        0    22144 2023-05-05 16:43:51.750072 ably-2.0.0b6/ably/realtime/connectionmanager.py
+-rw-r--r--   0        0        0     5677 2023-05-05 16:43:51.750347 ably-2.0.0b6/ably/realtime/realtime.py
+-rw-r--r--   0        0        0    19058 2023-05-05 16:43:51.750648 ably-2.0.0b6/ably/realtime/realtime_channel.py
+-rw-r--r--   0        0        0        0 2022-10-12 21:24:17.457418 ably-2.0.0b6/ably/rest/__init__.py
+-rw-r--r--   0        0        0    17119 2023-05-05 16:43:51.751090 ably-2.0.0b6/ably/rest/auth.py
+-rw-r--r--   0        0        0     7577 2023-05-05 16:43:51.751458 ably-2.0.0b6/ably/rest/channel.py
+-rw-r--r--   0        0        0     6529 2023-05-05 16:43:51.751781 ably-2.0.0b6/ably/rest/push.py
+-rw-r--r--   0        0        0     5210 2023-05-05 16:43:51.752092 ably-2.0.0b6/ably/rest/rest.py
+-rw-r--r--   0        0        0        0 2022-10-12 21:24:17.458240 ably-2.0.0b6/ably/transport/__init__.py
+-rw-r--r--   0        0        0     1787 2023-05-05 16:43:51.752413 ably-2.0.0b6/ably/transport/defaults.py
+-rw-r--r--   0        0        0     8683 2023-05-05 16:43:51.752677 ably-2.0.0b6/ably/transport/websockettransport.py
+-rw-r--r--   0        0        0        0 2022-10-12 21:24:17.458588 ably-2.0.0b6/ably/types/__init__.py
+-rw-r--r--   0        0        0     4601 2022-10-12 21:24:17.458807 ably-2.0.0b6/ably/types/authoptions.py
+-rw-r--r--   0        0        0     2238 2022-10-12 21:24:17.459010 ably-2.0.0b6/ably/types/capability.py
+-rw-r--r--   0        0        0     2931 2022-10-12 21:24:17.459161 ably-2.0.0b6/ably/types/channeldetails.py
+-rw-r--r--   0        0        0      507 2023-05-05 16:43:51.752927 ably-2.0.0b6/ably/types/channelstate.py
+-rw-r--r--   0        0        0     1757 2022-10-12 21:24:17.459355 ably-2.0.0b6/ably/types/channelsubscription.py
+-rw-r--r--   0        0        0      724 2023-05-05 16:43:51.753147 ably-2.0.0b6/ably/types/connectiondetails.py
+-rw-r--r--   0        0        0      740 2023-05-05 16:43:51.753361 ably-2.0.0b6/ably/types/connectionerrors.py
+-rw-r--r--   0        0        0      846 2023-05-05 16:43:51.753578 ably-2.0.0b6/ably/types/connectionstate.py
+-rw-r--r--   0        0        0     3115 2022-10-12 21:24:17.459514 ably-2.0.0b6/ably/types/device.py
+-rw-r--r--   0        0        0      413 2023-05-05 16:43:51.753787 ably-2.0.0b6/ably/types/flags.py
+-rw-r--r--   0        0        0     6254 2023-02-20 15:06:15.951208 ably-2.0.0b6/ably/types/message.py
+-rw-r--r--   0        0        0     2725 2023-02-20 15:06:15.951688 ably-2.0.0b6/ably/types/mixins.py
+-rw-r--r--   0        0        0     9714 2023-05-05 16:43:51.754127 ably-2.0.0b6/ably/types/options.py
+-rw-r--r--   0        0        0     5082 2023-02-20 15:06:15.952022 ably-2.0.0b6/ably/types/presence.py
+-rw-r--r--   0        0        0     5944 2022-10-12 21:24:17.460814 ably-2.0.0b6/ably/types/stats.py
+-rw-r--r--   0        0        0     2852 2023-05-05 16:43:51.754447 ably-2.0.0b6/ably/types/tokendetails.py
+-rw-r--r--   0        0        0     2833 2022-10-12 21:24:17.461181 ably-2.0.0b6/ably/types/tokenrequest.py
+-rw-r--r--   0        0        0     3272 2022-10-12 21:24:17.461399 ably-2.0.0b6/ably/types/typedbuffer.py
+-rw-r--r--   0        0        0        0 2022-10-12 21:24:17.461575 ably-2.0.0b6/ably/util/__init__.py
+-rw-r--r--   0        0        0      370 2022-10-12 21:24:17.461894 ably-2.0.0b6/ably/util/case.py
+-rw-r--r--   0        0        0     5433 2023-05-05 16:43:51.754788 ably-2.0.0b6/ably/util/crypto.py
+-rw-r--r--   0        0        0     6731 2023-05-05 16:43:51.755026 ably-2.0.0b6/ably/util/eventemitter.py
+-rw-r--r--   0        0        0     2740 2023-05-05 16:43:51.755354 ably-2.0.0b6/ably/util/exceptions.py
+-rw-r--r--   0        0        0     1046 2023-05-05 16:43:51.755566 ably-2.0.0b6/ably/util/helper.py
+-rw-r--r--   0        0        0      221 2022-10-12 21:24:17.462632 ably-2.0.0b6/ably/util/nocrypto.py
+-rw-r--r--   0        0        0     1623 2023-05-05 16:43:53.632386 ably-2.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 ably-2.0.0b6/setup.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 ably-2.0.0b6/PKG-INFO
```

### Comparing `ably-2.0.0b5/LICENSE` & `ably-2.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/__init__.py` & `ably-2.0.0b6/ably/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 import logging
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 api_version = '1.2'
-lib_version = '2.0.0-beta.5'
+lib_version = '2.0.0-beta.6'
```

### Comparing `ably-2.0.0b5/ably/http/http.py` & `ably-2.0.0b6/ably/http/http.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/http/httputils.py` & `ably-2.0.0b6/ably/http/httputils.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/http/paginatedresult.py` & `ably-2.0.0b6/ably/http/paginatedresult.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/realtime/connection.py` & `ably-2.0.0b6/ably/realtime/connection.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/realtime/connectionmanager.py` & `ably-2.0.0b6/ably/realtime/connectionmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.__fallback_hosts: list[str] = self.options.get_fallback_realtime_hosts()
         self.queued_messages: Queue = Queue()
         self.__error_reason: Optional[AblyException] = None
         super().__init__()
 
     def enact_state_change(self, state: ConnectionState, reason: Optional[AblyException] = None) -> None:
         current_state = self.__state
-        log.info(f'ConnectionManager.enact_state_change(): {current_state} -> {state}')
+        log.info(f'ConnectionManager.enact_state_change(): {current_state} -> {state}; reason = {reason}')
         self.__state = state
         if reason:
             self.__error_reason = reason
         self._emit('connectionstate', ConnectionStateChange(current_state, state, state, reason))
 
     def check_connection(self) -> bool:
         try:
@@ -239,15 +239,15 @@
             if self.__ping_id == id:
                 if not self.__ping_future.cancelled():
                     self.__ping_future.set_result(None)
                 self.__ping_future = None
 
     def deactivate_transport(self, reason: Optional[AblyException] = None):
         self.transport = None
-        self.enact_state_change(ConnectionState.DISCONNECTED, reason)
+        self.notify_state(ConnectionState.DISCONNECTED, reason)
 
     def request_state(self, state: ConnectionState, force=False) -> None:
         log.info(f'ConnectionManager.request_state(): state = {state}')
 
         if not force and state == self.state:
             return
```

### Comparing `ably-2.0.0b5/ably/realtime/realtime.py` & `ably-2.0.0b6/ably/realtime/realtime.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/realtime/realtime_channel.py` & `ably-2.0.0b6/ably/realtime/realtime_channel.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/rest/auth.py` & `ably-2.0.0b6/ably/rest/auth.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/rest/channel.py` & `ably-2.0.0b6/ably/rest/channel.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/rest/push.py` & `ably-2.0.0b6/ably/rest/push.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/rest/rest.py` & `ably-2.0.0b6/ably/rest/rest.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/transport/defaults.py` & `ably-2.0.0b6/ably/transport/defaults.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/transport/websockettransport.py` & `ably-2.0.0b6/ably/transport/websockettransport.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/authoptions.py` & `ably-2.0.0b6/ably/types/authoptions.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/capability.py` & `ably-2.0.0b6/ably/types/capability.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/channeldetails.py` & `ably-2.0.0b6/ably/types/channeldetails.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/channelsubscription.py` & `ably-2.0.0b6/ably/types/channelsubscription.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/connectiondetails.py` & `ably-2.0.0b6/ably/types/connectiondetails.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/connectionerrors.py` & `ably-2.0.0b6/ably/types/connectionerrors.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/connectionstate.py` & `ably-2.0.0b6/ably/types/connectionstate.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/device.py` & `ably-2.0.0b6/ably/types/device.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/message.py` & `ably-2.0.0b6/ably/types/message.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/mixins.py` & `ably-2.0.0b6/ably/types/mixins.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/options.py` & `ably-2.0.0b6/ably/types/options.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/presence.py` & `ably-2.0.0b6/ably/types/presence.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/stats.py` & `ably-2.0.0b6/ably/types/stats.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/tokendetails.py` & `ably-2.0.0b6/ably/types/tokendetails.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/tokenrequest.py` & `ably-2.0.0b6/ably/types/tokenrequest.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/types/typedbuffer.py` & `ably-2.0.0b6/ably/types/typedbuffer.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/util/crypto.py` & `ably-2.0.0b6/ably/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/util/eventemitter.py` & `ably-2.0.0b6/ably/util/eventemitter.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/util/exceptions.py` & `ably-2.0.0b6/ably/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/ably/util/helper.py` & `ably-2.0.0b6/ably/util/helper.py`

 * *Files identical despite different names*

### Comparing `ably-2.0.0b5/pyproject.toml` & `ably-2.0.0b6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ably"
-version = "2.0.0-beta.5"
+version = "2.0.0-beta.6"
 description = "Python REST and Realtime client library SDK for Ably realtime messaging service"
 license = "Apache-2.0"
 authors = ["Ably <support@ably.com>"]
 readme = "LONG_DESCRIPTION.rst"
 homepage = "https://ably.com"
 repository = "https://github.com/ably/ably-python"
 classifiers = [
```

### Comparing `ably-2.0.0b5/setup.py` & `ably-2.0.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'websockets>=10.3,<11.0']
 
 extras_require = \
 {'crypto': ['pycryptodome'], 'oldcrypto': ['pycrypto>=2.6.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'ably',
-    'version': '2.0.0b5',
+    'version': '2.0.0b6',
     'description': 'Python REST and Realtime client library SDK for Ably realtime messaging service',
     'long_description': 'Official Ably Bindings for Python\n==================================\n\nA Python client library for Ably Realtime messaging.\n\n\nSetup\n-----\n\nYou can install this package by using the pip tool and installing:\n\n    pip install ably\n\n\nUsing Ably for Python\n---------------------\n\n- Sign up for Ably at https://ably.com/sign-up\n- Get usage examples at https://github.com/ably/ably-python\n- Visit https://ably.com/docs for a complete API reference and more examples\n',
     'author': 'Ably',
     'author_email': 'support@ably.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ably.com',
```

### Comparing `ably-2.0.0b5/PKG-INFO` & `ably-2.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ably
-Version: 2.0.0b5
+Version: 2.0.0b6
 Summary: Python REST and Realtime client library SDK for Ably realtime messaging service
 Home-page: https://ably.com
 License: Apache-2.0
 Author: Ably
 Author-email: support@ably.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 6 - Mature
```

