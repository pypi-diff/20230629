# Comparing `tmp/beewi_smartclim_ble-0.2.0.tar.gz` & `tmp/beewi_smartclim_ble-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beewi_smartclim_ble-0.2.0.tar", max compression
+gzip compressed data, was "beewi_smartclim_ble-0.3.0.tar", max compression
```

## Comparing `beewi_smartclim_ble-0.2.0.tar` & `beewi_smartclim_ble-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/LICENSE
--rw-r--r--   0        0        0     2477 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/README.md
--rw-r--r--   0        0        0     2257 2023-05-20 15:16:56.276544 beewi_smartclim_ble-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-20 15:16:56.220544 beewi_smartclim_ble-0.2.0/src/smartclim_ble/__init__.py
--rw-r--r--   0        0        0     6707 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/src/smartclim_ble/parser.py
--rw-r--r--   0        0        0        0 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/src/smartclim_ble/py.typed
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2477 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/README.md
+-rw-r--r--   0        0        0     2257 2023-06-29 21:07:44.120238 beewi_smartclim_ble-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-29 21:07:44.088237 beewi_smartclim_ble-0.3.0/src/smartclim_ble/__init__.py
+-rw-r--r--   0        0        0     7106 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/src/smartclim_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:07:43.152213 beewi_smartclim_ble-0.3.0/src/smartclim_ble/py.typed
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.3.0/PKG-INFO
```

### Comparing `beewi_smartclim_ble-0.2.0/LICENSE` & `beewi_smartclim_ble-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.2.0/README.md` & `beewi_smartclim_ble-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.2.0/pyproject.toml` & `beewi_smartclim_ble-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beewi-smartclim-ble"
-version = "0.2.0"
+version = "0.3.0"
 description = "Parser for the BeeWi SmartClim device"
 authors = ["f-davin <none@none.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/f-davin/hassis_beewi_smartclim.git"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `beewi_smartclim_ble-0.2.0/src/smartclim_ble/parser.py` & `beewi_smartclim_ble-0.3.0/src/smartclim_ble/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,26 @@
     manufacturer: str = ""
     model: str = ""
     serial: str = ""
     fw_revision: str = ""
     hw_revision: str = ""
     soft_revision: str = ""
 
+    def __hash__(self) -> int:
+        return hash(
+            (
+                self.manufacturer,
+                self.model,
+                self.serial,
+                self.fw_revision,
+                self.hw_revision,
+                self.soft_revision,
+            )
+        )
+
 
 @dataclass
 class SmartClimSensorData:
     """Data to store the information about the sensor."""
 
     # Constants
     __CONNECTED_DATA_SIZE = 10
@@ -108,14 +120,17 @@
         data = adv_data.manufacturer_data
         if self.__ADVERTISING_MANUFACTURING_DATA_KEY in data.keys():
             ret = bytearray(data[self.__ADVERTISING_MANUFACTURING_DATA_KEY])
         else:
             raise Exception("Invalid data for this sensor.")
         return ret
 
+    def __hash__(self) -> int:
+        return hash((self.name, self.temperature, self.humidity, self.battery))
+
 
 @dataclass
 class BeeWiSmartClimAdvertisement:
     """Class to realize the treatment of an advertising frame."""
 
     device: BLEDevice = None
     readings: SmartClimSensorData = SmartClimSensorData()
```

### Comparing `beewi_smartclim_ble-0.2.0/PKG-INFO` & `beewi_smartclim_ble-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beewi-smartclim-ble
-Version: 0.2.0
+Version: 0.3.0
 Summary: Parser for the BeeWi SmartClim device
 Home-page: https://github.com/f-davin/hassis_beewi_smartclim.git
 License: MIT
 Author: f-davin
 Author-email: none@none.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

