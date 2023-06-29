# Comparing `tmp/neon-phal-plugin-linear_led-0.2.2a1.tar.gz` & `tmp/neon-phal-plugin-linear_led-0.2.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-linear_led-0.2.2a1.tar", last modified: Fri Jun 23 18:31:32 2023, max compression
+gzip compressed data, was "neon-phal-plugin-linear_led-0.2.2a2.tar", last modified: Tue Jun 27 17:08:28 2023, max compression
```

## Comparing `neon-phal-plugin-linear_led-0.2.2a1.tar` & `neon-phal-plugin-linear_led-0.2.2a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:31:32.985941 neon-phal-plugin-linear_led-0.2.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-23 18:31:32.985941 neon-phal-plugin-linear_led-0.2.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:31:32.985941 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/neopixel_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/smbus_led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:31:32.985941 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 18:31:32.000000 neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:31:32.985941 neon-phal-plugin-linear_led-0.2.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-23 18:31:29.000000 neon-phal-plugin-linear_led-0.2.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.325366 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/
+-rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/neopixel_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/smbus_led.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:08:28.000000 neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:08:28.329366 neon-phal-plugin-linear_led-0.2.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-27 17:08:22.000000 neon-phal-plugin-linear_led-0.2.2a2/setup.py
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/LICENSE.md` & `neon-phal-plugin-linear_led-0.2.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/PKG-INFO` & `neon-phal-plugin-linear_led-0.2.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear_led
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/README.md` & `neon-phal-plugin-linear_led-0.2.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/__init__.py` & `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             LOG.debug("Offline mode, never report disconnected")
             return False
         message = Message("ovos.PHAL.internet_check")
         resp = self.bus.wait_for_response(message)
         if not resp:
             LOG.warning("No network status responses, use last known value")
             return self._internet_disconnected
-        internet = message.data.get('internet_connected')
+        internet = resp.data.get('internet_connected')
         if internet is None:
             LOG.error(f"Invalid internet status response. data={resp.data}")
             return self._internet_disconnected
         if internet:
             # TODO: Better method to check when to stop animation
             self._disconnected_animation.stop()
         self._internet_disconnected = not internet
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/neopixel_led.py` & `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/neopixel_led.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led/smbus_led.py` & `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led/smbus_led.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/neon_phal_plugin_linear_led.egg-info/PKG-INFO` & `neon-phal-plugin-linear_led-0.2.2a2/neon_phal_plugin_linear_led.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear-led
-Version: 0.2.2a1
+Version: 0.2.2a2
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-linear_led-0.2.2a1/setup.py` & `neon-phal-plugin-linear_led-0.2.2a2/setup.py`

 * *Files identical despite different names*

