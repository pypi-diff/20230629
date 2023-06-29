# Comparing `tmp/rpi_reactive_gpio-0.1.4.tar.gz` & `tmp/rpi_reactive_gpio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.4.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.5.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.4.tar` & `rpi_reactive_gpio-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/LICENSE
--rw-r--r--   0        0        0       80 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/README.md
--rw-r--r--   0        0        0      766 2023-05-30 13:33:45.678206 rpi_reactive_gpio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      207 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3504 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      478 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      850 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1102 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-29 15:42:19.679609 rpi_reactive_gpio-0.1.5/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-29 15:42:19.679609 rpi_reactive_gpio-0.1.5/README.md
+-rw-r--r--   0        0        0      766 2023-06-29 15:42:38.531732 rpi_reactive_gpio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1603 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3504 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      478 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1263 2023-06-29 15:42:19.683609 rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.5/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.4/LICENSE` & `rpi_reactive_gpio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.4/pyproject.toml` & `rpi_reactive_gpio-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.4"
+version = "0.1.5"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/buttons.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/leds.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.5/rpi_reactive_gpio/scene.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import time
 from abc import ABC
 from .pin_manager import PinManagerProtocol, Tickable
 from .buttons import ButtonClick
 
 
 class Scene(ABC):
+    
+    _is_running = False
+    
     def main_loop(self, update_interval: float = 1.0, ticks_count: int = 100):
+        self._is_running = True
+        
         attributes = [getattr(self, a) for a in dir(self)]
         self.managers = filter(lambda a: isinstance(a, PinManagerProtocol), attributes)
         self.tickables = filter(lambda a: isinstance(a, Tickable), attributes)
         self.events = filter(lambda a: isinstance(a, ButtonClick), attributes)
         
         for event in self.events:
             event.pass_args = [self]
         
-        while True:
-            self.update_all()
+        while self._is_running:
+            self._update_all()
             for i in range(ticks_count):
-                self.tick_all(i / ticks_count)
+                self._tick_all(i / ticks_count)
                 time.sleep(update_interval / ticks_count)
                 
-    def update_all(self):
+    def stop(self):
+        self._is_running = False
+                
+    def _update_all(self):
         for manager in self.managers:
             manager.update(self)
             
-    def tick_all(self, period: float = 1.0):
+    def _tick_all(self, period: float = 1.0):
         '''period must be in range 0.0...1.0'''
         for tickable in self.tickables:
             tickable.tick(period)
```

### Comparing `rpi_reactive_gpio-0.1.4/PKG-INFO` & `rpi_reactive_gpio-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.4
+Version: 0.1.5
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

