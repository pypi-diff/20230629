# Comparing `tmp/shortloop_python-0.1.6.tar.gz` & `tmp/shortloop_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortloop_python-0.1.6.tar", max compression
+gzip compressed data, was "shortloop_python-0.1.7.tar", max compression
```

## Comparing `shortloop_python-0.1.6.tar` & `shortloop_python-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      439 2023-06-12 11:23:58.944592 shortloop_python-0.1.6/README.md
--rw-r--r--   0        0        0     1220 2023-06-28 09:19:15.673750 shortloop_python-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       57 2023-06-12 11:23:58.945584 shortloop_python-0.1.6/shortloop_python/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.945789 shortloop_python-0.1.6/shortloop_python/core/__init__.py
--rw-r--r--   0        0        0     1617 2023-06-12 11:23:58.946003 shortloop_python-0.1.6/shortloop_python/core/always_capture_sync.py
--rw-r--r--   0        0        0     6347 2023-06-12 11:23:58.946179 shortloop_python-0.1.6/shortloop_python/core/api_processor.py
--rw-r--r--   0        0        0     3363 2023-06-28 09:18:26.909745 shortloop_python-0.1.6/shortloop_python/core/auto_configuration.py
--rw-r--r--   0        0        0     1765 2023-06-12 11:23:58.946538 shortloop_python-0.1.6/shortloop_python/core/buffer/abstract_buffer_manager.py
--rw-r--r--   0        0        0      842 2023-06-12 11:23:58.946678 shortloop_python-0.1.6/shortloop_python/core/buffer/api_buffer_key.py
--rw-r--r--   0        0        0      404 2023-06-12 11:23:58.946866 shortloop_python-0.1.6/shortloop_python/core/buffer/buffer.py
--rw-r--r--   0        0        0     1846 2023-06-28 09:18:26.910162 shortloop_python-0.1.6/shortloop_python/core/buffer/buffer_manager_worker.py
--rw-r--r--   0        0        0     3111 2023-06-12 11:23:58.947157 shortloop_python-0.1.6/shortloop_python/core/buffer/discovered_buffer_manager.py
--rw-r--r--   0        0        0      503 2023-06-28 09:18:26.910528 shortloop_python-0.1.6/shortloop_python/core/buffer/no_op_buffer_manager.py
--rw-r--r--   0        0        0     4027 2023-06-12 11:23:58.947419 shortloop_python-0.1.6/shortloop_python/core/buffer/registered_buffer_manager.py
--rw-r--r--   0        0        0      832 2023-06-12 11:23:58.947572 shortloop_python-0.1.6/shortloop_python/core/buffer/simple_buffer.py
--rw-r--r--   0        0        0      373 2023-06-12 11:23:58.947779 shortloop_python-0.1.6/shortloop_python/core/config/config_manager.py
--rw-r--r--   0        0        0      316 2023-06-12 11:23:58.947921 shortloop_python-0.1.6/shortloop_python/core/config/config_update_listener.py
--rw-r--r--   0        0        0     1921 2023-06-12 11:23:58.948077 shortloop_python-0.1.6/shortloop_python/core/config/config_validators.py
--rw-r--r--   0        0        0     4175 2023-06-28 09:18:26.911124 shortloop_python-0.1.6/shortloop_python/core/config/simple_config_manager.py
--rw-r--r--   0        0        0      140 2023-06-12 11:23:58.948592 shortloop_python-0.1.6/shortloop_python/core/constant/__init__.py
--rw-r--r--   0        0        0      207 2023-06-12 11:23:58.948773 shortloop_python-0.1.6/shortloop_python/core/constant/http_method.py
--rw-r--r--   0        0        0      156 2023-06-12 11:23:58.949037 shortloop_python-0.1.6/shortloop_python/core/constant/segment_template_type.py
--rw-r--r--   0        0        0      163 2023-06-12 11:23:58.949294 shortloop_python-0.1.6/shortloop_python/core/filter/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-12 11:23:58.949442 shortloop_python-0.1.6/shortloop_python/core/filter/always_capture_filter.py
--rw-r--r--   0        0        0     3041 2023-06-12 11:23:58.949593 shortloop_python-0.1.6/shortloop_python/core/filter/filter.py
--rw-r--r--   0        0        0      271 2023-06-12 11:23:58.949807 shortloop_python-0.1.6/shortloop_python/core/http/__init__.py
--rw-r--r--   0        0        0     2845 2023-06-12 11:23:58.949952 shortloop_python-0.1.6/shortloop_python/core/http/context.py
--rw-r--r--   0        0        0     5232 2023-06-12 11:23:58.950111 shortloop_python-0.1.6/shortloop_python/core/http/http_connection.py
--rw-r--r--   0        0        0     1260 2023-06-12 11:23:58.950257 shortloop_python-0.1.6/shortloop_python/core/http/http_request.py
--rw-r--r--   0        0        0      267 2023-06-12 11:23:58.950434 shortloop_python-0.1.6/shortloop_python/core/http/http_response.py
--rw-r--r--   0        0        0      350 2023-06-12 11:23:58.950634 shortloop_python-0.1.6/shortloop_python/core/model/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-12 11:23:58.950778 shortloop_python-0.1.6/shortloop_python/core/model/agent_config.py
--rw-r--r--   0        0        0      692 2023-06-12 11:23:58.950913 shortloop_python-0.1.6/shortloop_python/core/model/api_config.py
--rw-r--r--   0        0        0     3277 2023-06-12 11:23:58.951048 shortloop_python-0.1.6/shortloop_python/core/model/api_sample.py
--rw-r--r--   0        0        0     1122 2023-06-12 11:23:58.951183 shortloop_python-0.1.6/shortloop_python/core/model/black_list_rule.py
--rw-r--r--   0        0        0      536 2023-06-12 11:23:58.951348 shortloop_python-0.1.6/shortloop_python/core/model/observed_api.py
--rw-r--r--   0        0        0     2068 2023-06-12 11:23:58.951520 shortloop_python-0.1.6/shortloop_python/core/model/sdk_options.py
--rw-r--r--   0        0        0     1955 2023-06-12 11:23:58.951686 shortloop_python-0.1.6/shortloop_python/core/model/uri.py
--rw-r--r--   0        0        0      199 2023-06-12 11:23:58.951820 shortloop_python-0.1.6/shortloop_python/core/scheduled_timer.py
--rw-r--r--   0        0        0     2290 2023-06-20 08:53:46.661321 shortloop_python-0.1.6/shortloop_python/core/shortlook_sdk.py
--rw-r--r--   0        0        0     1184 2023-06-12 11:23:58.952193 shortloop_python-0.1.6/shortloop_python/core/util/filter_utils.py
--rw-r--r--   0        0        0      420 2023-06-12 11:23:58.952340 shortloop_python-0.1.6/shortloop_python/core/util/masking_utils.py
--rw-r--r--   0        0        0      929 2023-06-12 11:23:58.952476 shortloop_python-0.1.6/shortloop_python/core/util/uri_utils.py
--rw-r--r--   0        0        0       87 2023-06-12 11:23:58.952669 shortloop_python-0.1.6/shortloop_python/integrations/__init__.py
--rw-r--r--   0        0        0     3230 2023-06-22 10:17:36.031400 shortloop_python-0.1.6/shortloop_python/integrations/django.py
--rw-r--r--   0        0        0      558 2023-06-12 11:23:58.953206 shortloop_python-0.1.6/shortloop_python/sdk_logger.py
--rw-r--r--   0        0        0      152 2023-06-12 11:23:58.953369 shortloop_python-0.1.6/shortloop_python/sdk_version.py
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      439 2023-06-12 11:23:58.944592 shortloop_python-0.1.7/README.md
+-rw-r--r--   0        0        0     1220 2023-06-29 09:23:32.847449 shortloop_python-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-06-12 11:23:58.945584 shortloop_python-0.1.7/shortloop_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.945789 shortloop_python-0.1.7/shortloop_python/core/__init__.py
+-rw-r--r--   0        0        0     1617 2023-06-12 11:23:58.946003 shortloop_python-0.1.7/shortloop_python/core/always_capture_sync.py
+-rw-r--r--   0        0        0     6347 2023-06-12 11:23:58.946179 shortloop_python-0.1.7/shortloop_python/core/api_processor.py
+-rw-r--r--   0        0        0     3118 2023-06-29 09:23:02.138750 shortloop_python-0.1.7/shortloop_python/core/auto_configuration.py
+-rw-r--r--   0        0        0     1765 2023-06-12 11:23:58.946538 shortloop_python-0.1.7/shortloop_python/core/buffer/abstract_buffer_manager.py
+-rw-r--r--   0        0        0      842 2023-06-12 11:23:58.946678 shortloop_python-0.1.7/shortloop_python/core/buffer/api_buffer_key.py
+-rw-r--r--   0        0        0      404 2023-06-12 11:23:58.946866 shortloop_python-0.1.7/shortloop_python/core/buffer/buffer.py
+-rw-r--r--   0        0        0     1893 2023-06-29 09:23:02.139277 shortloop_python-0.1.7/shortloop_python/core/buffer/buffer_manager_worker.py
+-rw-r--r--   0        0        0     3111 2023-06-12 11:23:58.947157 shortloop_python-0.1.7/shortloop_python/core/buffer/discovered_buffer_manager.py
+-rw-r--r--   0        0        0      503 2023-06-28 09:18:26.910528 shortloop_python-0.1.7/shortloop_python/core/buffer/no_op_buffer_manager.py
+-rw-r--r--   0        0        0     4027 2023-06-12 11:23:58.947419 shortloop_python-0.1.7/shortloop_python/core/buffer/registered_buffer_manager.py
+-rw-r--r--   0        0        0      832 2023-06-12 11:23:58.947572 shortloop_python-0.1.7/shortloop_python/core/buffer/simple_buffer.py
+-rw-r--r--   0        0        0      373 2023-06-12 11:23:58.947779 shortloop_python-0.1.7/shortloop_python/core/config/config_manager.py
+-rw-r--r--   0        0        0      316 2023-06-12 11:23:58.947921 shortloop_python-0.1.7/shortloop_python/core/config/config_update_listener.py
+-rw-r--r--   0        0        0     1921 2023-06-12 11:23:58.948077 shortloop_python-0.1.7/shortloop_python/core/config/config_validators.py
+-rw-r--r--   0        0        0     4222 2023-06-29 09:23:02.139696 shortloop_python-0.1.7/shortloop_python/core/config/simple_config_manager.py
+-rw-r--r--   0        0        0      140 2023-06-12 11:23:58.948592 shortloop_python-0.1.7/shortloop_python/core/constant/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-12 11:23:58.948773 shortloop_python-0.1.7/shortloop_python/core/constant/http_method.py
+-rw-r--r--   0        0        0      156 2023-06-12 11:23:58.949037 shortloop_python-0.1.7/shortloop_python/core/constant/segment_template_type.py
+-rw-r--r--   0        0        0      163 2023-06-12 11:23:58.949294 shortloop_python-0.1.7/shortloop_python/core/filter/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-12 11:23:58.949442 shortloop_python-0.1.7/shortloop_python/core/filter/always_capture_filter.py
+-rw-r--r--   0        0        0     3041 2023-06-12 11:23:58.949593 shortloop_python-0.1.7/shortloop_python/core/filter/filter.py
+-rw-r--r--   0        0        0      271 2023-06-12 11:23:58.949807 shortloop_python-0.1.7/shortloop_python/core/http/__init__.py
+-rw-r--r--   0        0        0     2845 2023-06-12 11:23:58.949952 shortloop_python-0.1.7/shortloop_python/core/http/context.py
+-rw-r--r--   0        0        0     5232 2023-06-12 11:23:58.950111 shortloop_python-0.1.7/shortloop_python/core/http/http_connection.py
+-rw-r--r--   0        0        0     1260 2023-06-12 11:23:58.950257 shortloop_python-0.1.7/shortloop_python/core/http/http_request.py
+-rw-r--r--   0        0        0      267 2023-06-12 11:23:58.950434 shortloop_python-0.1.7/shortloop_python/core/http/http_response.py
+-rw-r--r--   0        0        0      350 2023-06-12 11:23:58.950634 shortloop_python-0.1.7/shortloop_python/core/model/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-12 11:23:58.950778 shortloop_python-0.1.7/shortloop_python/core/model/agent_config.py
+-rw-r--r--   0        0        0      692 2023-06-12 11:23:58.950913 shortloop_python-0.1.7/shortloop_python/core/model/api_config.py
+-rw-r--r--   0        0        0     3277 2023-06-12 11:23:58.951048 shortloop_python-0.1.7/shortloop_python/core/model/api_sample.py
+-rw-r--r--   0        0        0     1122 2023-06-12 11:23:58.951183 shortloop_python-0.1.7/shortloop_python/core/model/black_list_rule.py
+-rw-r--r--   0        0        0      536 2023-06-12 11:23:58.951348 shortloop_python-0.1.7/shortloop_python/core/model/observed_api.py
+-rw-r--r--   0        0        0     2068 2023-06-12 11:23:58.951520 shortloop_python-0.1.7/shortloop_python/core/model/sdk_options.py
+-rw-r--r--   0        0        0     1955 2023-06-12 11:23:58.951686 shortloop_python-0.1.7/shortloop_python/core/model/uri.py
+-rw-r--r--   0        0        0      199 2023-06-12 11:23:58.951820 shortloop_python-0.1.7/shortloop_python/core/scheduled_timer.py
+-rw-r--r--   0        0        0     2290 2023-06-20 08:53:46.661321 shortloop_python-0.1.7/shortloop_python/core/shortlook_sdk.py
+-rw-r--r--   0        0        0     1184 2023-06-12 11:23:58.952193 shortloop_python-0.1.7/shortloop_python/core/util/filter_utils.py
+-rw-r--r--   0        0        0      420 2023-06-12 11:23:58.952340 shortloop_python-0.1.7/shortloop_python/core/util/masking_utils.py
+-rw-r--r--   0        0        0      929 2023-06-12 11:23:58.952476 shortloop_python-0.1.7/shortloop_python/core/util/uri_utils.py
+-rw-r--r--   0        0        0       87 2023-06-12 11:23:58.952669 shortloop_python-0.1.7/shortloop_python/integrations/__init__.py
+-rw-r--r--   0        0        0     3230 2023-06-22 10:17:36.031400 shortloop_python-0.1.7/shortloop_python/integrations/django.py
+-rw-r--r--   0        0        0      558 2023-06-12 11:23:58.953206 shortloop_python-0.1.7/shortloop_python/sdk_logger.py
+-rw-r--r--   0        0        0      152 2023-06-12 11:23:58.953369 shortloop_python-0.1.7/shortloop_python/sdk_version.py
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.7/PKG-INFO
```

### Comparing `shortloop_python-0.1.6/pyproject.toml` & `shortloop_python-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shortloop-python"
-version = "0.1.6"
+version = "0.1.7"
 description = "Official Shortloop SDK for Python"
 authors = ["ShortLoop <hello@shortloop.dev>"]
 maintainers = ["ShortLoop <hello@shortloop.dev>"]
 homepage = "https://shortloop.dev"
 documentation = "https://docs.shortloop.dev"
 readme = "README.md"
 packages = [{include = "shortloop_python"}]
```

### Comparing `shortloop_python-0.1.6/shortloop_python/core/always_capture_sync.py` & `shortloop_python-0.1.7/shortloop_python/core/always_capture_sync.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/api_processor.py` & `shortloop_python-0.1.7/shortloop_python/core/api_processor.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/auto_configuration.py` & `shortloop_python-0.1.7/shortloop_python/core/auto_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .always_capture_sync import ShortloopDataSyncService
 from .api_processor import ApiProcessor
 from .buffer.discovered_buffer_manager import DiscoveredApiBufferManager
 from .buffer.registered_buffer_manager import RegisteredApiBufferManager
 from .config.simple_config_manager import SimpleConfigManager
 from .http.http_connection import ShortLoopHttpConnection
 from .model.sdk_options import SdkOptions
-import signal
 
 class ShortLoopAutoConfiguration:
     def __init__(self, opts):
         self.__opts: SdkOptions = opts
         self.__filter: Optional[ShortLoopFilter] = None
 
     def init(self):
@@ -69,19 +68,13 @@
             registered_api_buffer_manager=registered_buffer_manager,
         )
 
         self.__filter = ShortLoopFilter(
             config_manager=config_manager, api_processor=api_processor, application_name=self.__opts.application_name
         )
 
-        def handle_signal(signum, frame):
-            config_manager.shutdown()
-            discovered_buffer_manager.shutdown()
-            registered_buffer_manager.shutdown()
-
-        signal.signal(signal.SIGINT, handle_signal)
         logger.debug("ShortLoopAutoConfiguration.__filter.init")
         self.__filter.init()
 
     @property
     def filter(self) -> Optional[ShortLoopFilter]:
         return self.__filter
```

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/abstract_buffer_manager.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/abstract_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/api_buffer_key.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/api_buffer_key.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/buffer_manager_worker.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/buffer_manager_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def __init__(self, agent_config):
         self._buffer_map: Dict[ApiBufferKey, Buffer] = {}
         self.__agent_config: AgentConfig = agent_config
         self.__buffer_sync_timer: Optional[ScheduledTimer] = ScheduledTimer(
             self.__agent_config.buffer_sync_freq_in_sec, self.sync_for_keys
         )
         self.__buffer_sync_timer.setName("sl-buffer-" + str(random.randrange(0, 1000)))
+        self.__buffer_sync_timer.daemon = True
         self.__buffer_sync_timer.start()
 
     @abstractmethod
     def init(self) -> bool:
         pass
 
     @abstractmethod
```

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/discovered_buffer_manager.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/discovered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/registered_buffer_manager.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/registered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/buffer/simple_buffer.py` & `shortloop_python-0.1.7/shortloop_python/core/buffer/simple_buffer.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/config/config_validators.py` & `shortloop_python-0.1.7/shortloop_python/core/config/config_validators.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/config/simple_config_manager.py` & `shortloop_python-0.1.7/shortloop_python/core/config/simple_config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             logger.error("Error while shutting down SimpleConfigManager.__execution_service", exc_info=e)
             return False
 
     def schedule_config_refresh(self, time_sec: int):
         if self.__execution_service and self.__execution_service.is_alive():
             self.__execution_service.cancel()
         self.__execution_service = Timer(time_sec, self.fetch_config_notify)
+        self.__execution_service.daemon = True
         self.__execution_service.start()
 
 
     def fetch_config_notify(self) -> None:
         config_or_error: SimpleConfigManager.ConfigOrError = self.fetch_config()
         if config_or_error.error_code:
             self.schedule_config_refresh(60)
```

### Comparing `shortloop_python-0.1.6/shortloop_python/core/filter/always_capture_filter.py` & `shortloop_python-0.1.7/shortloop_python/core/filter/always_capture_filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/filter/filter.py` & `shortloop_python-0.1.7/shortloop_python/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/http/context.py` & `shortloop_python-0.1.7/shortloop_python/core/http/context.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/http/http_connection.py` & `shortloop_python-0.1.7/shortloop_python/core/http/http_connection.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/http/http_request.py` & `shortloop_python-0.1.7/shortloop_python/core/http/http_request.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/agent_config.py` & `shortloop_python-0.1.7/shortloop_python/core/model/agent_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/api_config.py` & `shortloop_python-0.1.7/shortloop_python/core/model/api_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/api_sample.py` & `shortloop_python-0.1.7/shortloop_python/core/model/api_sample.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/black_list_rule.py` & `shortloop_python-0.1.7/shortloop_python/core/model/black_list_rule.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/observed_api.py` & `shortloop_python-0.1.7/shortloop_python/core/model/observed_api.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/sdk_options.py` & `shortloop_python-0.1.7/shortloop_python/core/model/sdk_options.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/model/uri.py` & `shortloop_python-0.1.7/shortloop_python/core/model/uri.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/shortlook_sdk.py` & `shortloop_python-0.1.7/shortloop_python/core/shortlook_sdk.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/util/filter_utils.py` & `shortloop_python-0.1.7/shortloop_python/core/util/filter_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/core/util/uri_utils.py` & `shortloop_python-0.1.7/shortloop_python/core/util/uri_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/integrations/django.py` & `shortloop_python-0.1.7/shortloop_python/integrations/django.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/shortloop_python/sdk_logger.py` & `shortloop_python-0.1.7/shortloop_python/sdk_logger.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.6/PKG-INFO` & `shortloop_python-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortloop-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: Official Shortloop SDK for Python
 Home-page: https://shortloop.dev
 Keywords: shortloop,middleware
 Author: ShortLoop
 Author-email: hello@shortloop.dev
 Maintainer: ShortLoop
 Maintainer-email: hello@shortloop.dev
```

