# Comparing `tmp/maxsmart-0.1.6.tar.gz` & `tmp/maxsmart-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxsmart-0.1.6.tar", last modified: Thu Jun 22 19:35:41 2023, max compression
+gzip compressed data, was "maxsmart-0.1.7.tar", last modified: Thu Jun 29 09:47:07 2023, max compression
```

## Comparing `maxsmart-0.1.6.tar` & `maxsmart-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-22 19:35:41.581021 maxsmart-0.1.6/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.6/LICENSE
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-22 19:35:41.581021 maxsmart-0.1.6/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     6862 2023-06-19 08:19:13.000000 maxsmart-0.1.6/README.md
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-22 19:35:41.581021 maxsmart-0.1.6/maxsmart/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.6/maxsmart/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5532 2023-06-22 19:30:58.000000 maxsmart-0.1.6/maxsmart/maxsmart.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-22 19:35:41.581021 maxsmart-0.1.6/maxsmart.egg-info/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-22 19:35:41.000000 maxsmart-0.1.6/maxsmart.egg-info/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-06-22 19:35:41.000000 maxsmart-0.1.6/maxsmart.egg-info/SOURCES.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-06-22 19:35:41.000000 maxsmart-0.1.6/maxsmart.egg-info/dependency_links.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-06-22 19:35:41.000000 maxsmart-0.1.6/maxsmart.egg-info/requires.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-06-22 19:35:41.000000 maxsmart-0.1.6/maxsmart.egg-info/top_level.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-06-22 19:35:41.581021 maxsmart-0.1.6/setup.cfg
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-06-22 19:31:51.000000 maxsmart-0.1.6/setup.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-22 19:35:41.581021 maxsmart-0.1.6/tests/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.6/tests/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.6/tests/test_maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.7/LICENSE
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-29 09:47:07.468305 maxsmart-0.1.7/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     7581 2023-06-22 20:20:51.000000 maxsmart-0.1.7/README.md
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.464972 maxsmart-0.1.7/maxsmart/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.7/maxsmart/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5149 2023-06-29 09:36:05.000000 maxsmart-0.1.7/maxsmart/maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/maxsmart.egg-info/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/SOURCES.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/dependency_links.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/requires.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/top_level.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-06-29 09:47:07.468305 maxsmart-0.1.7/setup.cfg
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-06-29 09:21:45.000000 maxsmart-0.1.7/setup.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/tests/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.7/tests/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.7/tests/test_maxsmart.py
```

### Comparing `maxsmart-0.1.6/LICENSE` & `maxsmart-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.6/PKG-INFO` & `maxsmart-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.6/README.md` & `maxsmart-0.1.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -47,95 +47,106 @@
 - The `maxsmart` Python module installed. You can install it by following the instructions in the [Installation](#installation) section.
 
 ### Running the Test Script
 
 To run the test script, execute the following command in your terminal:
 
 ```bash
-python test_script.py
+python test_scripts/test_script.py
 ```
 
-The script will attempt to discover MaxSmart devices on the network
-
-. If no devices are found, it will display an error message. If devices are found, you will be presented with a menu to select a device for testing.
+The script will attempt to discover MaxSmart devices on the network. If no devices are found, it will display an error message. If devices are found, you will be presented with a menu to select a device for testing.
 
 Follow the on-screen instructions and warnings to proceed with the test.
 
-### Output and Example
-
-The test script provides detailed output during the test execution. It displays the status of each action, countdown during the waiting periods, and the retrieved consumption data in tabular format.
+## Installation
 
-Here is an example command to run the test script:
+To install the `maxsmart` module, you can use `pip`, the Python package installer. Open your terminal or command prompt and run the following command:
 
+```bash
+pip install maxsmart
 ```
-python test_script.py
-```
+This will install the `maxsmart` module and its dependencies.
 
-This command will run the test script and attempt to discover MaxSmart devices on the network. If devices are found, you will be presented with a menu to select a device for testing. Follow the on-screen instructions and warnings to proceed with the test.
+## Usage
 
-## Getting started
+### Discovery 
 
-### Prerequisites
+Discovery will help you find your MaxSmart device details on the local network. You can use the `MaxSmartDiscovery` class. There are two ways of using this class: 
 
-- Python 3.x installed on your system.
-- The `maxsmart` Python module installed. You can install it by following the instructions in the [Installation](#installation) section.
+Without argument, MaxSmartDiscovery will send a broadcast to the local network and expect all available devices to send data in return.
 
-### Installation
+```python
+from maxsmart import MaxSmartDiscovery
+devices = MaxSmartDiscovery.discover_maxsmart()
+```
 
-To install the `maxsmart` module, you can use `pip`, the Python package installer. Open your terminal or command prompt and run the following command:
+**Note:** If broadcast is blocked on your network, you will not get any result.
 
-```bash
-pip install maxsmart
+With an ip address as argument, MaxSmartDiscovery will send a unicast message to the specified IP address. In that case, only that specific device, if present, will return data. You'll have therefore to run discovery for each specific MaxSmart device.
+
+```python
+from maxsmart import MaxSmartDiscovery
+devices = MaxSmartDiscovery.discover_maxsmart(192.168.0.25)
 ```
-This will install the `maxsmart` module and its dependencies.
 
-### Usage
+The `discover_maxsmart` method returns a list of dictionaries, each representing a discovered MaxSmart device on the network. Each dictionary contains information such as the device's IP address (ip), serial number (sn), name, port name dictonary (pname), firmware version (ver).
+
+### Device Operations
 
-To use the `maxsmart` module, follow these steps:
+When you have the ip addresses of your devices, you can operate using the MaxSmartDevice method:
 
-1. Import the module: `from maxsmart import MaxSmart`
-2. Create an instance of the `MaxSmart` class, providing the IP address and serial number of your PowerStrip:
+The MaxSmart Power strip as 6 ports, and the Smart plug has 1 port. Operations are made against port numbers.
+
+1. Import the module and create an instance of the `MaxSmartDevice` class, providing the IP address of the device. For example:
 
    ```python
-   maxsmart = MaxSmart('192.168.1.1', 'test_sn')
+   from maxsmart import MaxSmartDevice
+
+   device = MaxSmartDevice(192.168.0.25)
    ```
 
-3. Use the available methods to control the PowerStrip:
+2. Use the available methods to control the device. Note that port 0 is a master port affecting all ports on the device simultaneously:
 
    - Turn on a specific port/socket:
      ```python
-     maxsmart.turn_on(1)  # Turns on port 1
+     device.turn_on(1)  # Turns on port 1
+     ```
+
+   - Turn on all ports/sockets:
+     ```python
+     device.turn_on(0)  # Turns on all ports
      ```
 
    - Turn off a specific port/socket:
      ```python
-     maxsmart.turn_off(2)  # Turns off port 2
+     device.turn_off(2)  # Turns off port 2
      ```
 
    - Check the state of all ports/sockets:
      ```python
-     state = maxsmart.check_state()  # Returns a list with the state of each port
+     state = device.check_state()  # Returns a list with the state of each port
      ```
 
    - Check the state of a specific port/socket:
      ```python
-     port_state = maxsmart.check_port_state(3)  # Returns the state of port 3
+     port_state = device.check_port_state(3)  # Returns the state of port 3
+     ```
+
+   - Retrieve real-time power consumption data for a specific port/socket (watts):
+     ```python
+     power_data = device.get_power_data(3)   # Get the power data for the specified port
+     ```
+
+   - Retrieve 24-hour points of consumption data for a specific port/socket (kWh):
+     ```python
+     hourly_data = device.get_hourly_data(3)  # Get the last 24 points of hourly consumption data for the specified port
      ```
 
-    - Retrieve real time power consumption data for a specific port/socket (amps and watts):
-      ```python
-      power_data = maxsmart.get_power_data(3)   # Get the power data for the specified port
-      ```
-
-    - Retrieve 24 hours points of consumption data for a specific port/socket:
-      ```python
-      hourly_data = maxsmart.get_hourly_data(3)  # Get the last 24 points of hourly consumption data for specified port
-      ```
-     
-**Important:** Please note that the `maxsmart` module is specifically designed for Revogi-based Max Hauri MaxSmart PowerStrips running on v1.x firmware. Compatibility with other devices or firmware versions is not guaranteed.
+**DISCLAIMER:** Please note that the `MaxSmartDevice` class is specifically designed for Revogi-based Max Hauri MaxSmart PowerStrips running on v1.30 firmware. Compatibility with other devices or firmware versions is not guaranteed.
 
 ## Credits
 
 The `maxsmart` module has been made possible by the reverse engineering and documentation work done by GitHub user `@altery`. They have provided valuable insights into the communication protocol of MaxSmart PowerStrips. You can find their documentation here: [GitHub - mh-maxsmart-powerstation](https://github.com/altery/mh-maxsmart-powerstation)
 
 ## License
```

### Comparing `maxsmart-0.1.6/maxsmart/maxsmart.py` & `maxsmart-0.1.7/maxsmart/maxsmart.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,15 @@
             sock.settimeout(5)
 
             while True:
                 try:
                     data, addr = sock.recvfrom(1024)
                     raw_result = data.decode()
 
-                    preprocessed_result = MaxSmartDiscovery._preprocess_json_string(raw_result)
-                    json_data = json.loads(preprocessed_result)
+                    json_data = json.loads(raw_result)
                     ip_address = addr[0]
                     device_data = json_data.get("data")
 
                     if device_data:
                         sn = device_data.get("sn")
                         name = device_data.get("name")
                         pname = device_data.get("pname")
@@ -51,22 +50,14 @@
                     break
 
         MaxSmartDiscovery._validate_firmware_versions(maxsmart_devices)
 
         return maxsmart_devices
 
     @staticmethod
-    def _preprocess_json_string(json_str):
-        json_str = json_str.strip()
-        json_str = json_str.replace("'", '"')
-        json_str = json_str.replace("False", '"False"')
-        json_str = json_str.replace("True", '"True"')
-        return json_str
-
-    @staticmethod
     def _validate_firmware_versions(devices):
         for device in devices:
             firmware_version = device.get('ver')
             if firmware_version != '1.30':
                 raise IncompatibleFirmwareError(f"Device with IP {device['ip']} has firmware version {firmware_version}. This module has been tested with MaxSmart devices with firmware version 1.30.")
 
 class MaxSmartDevice:
```

### Comparing `maxsmart-0.1.6/maxsmart.egg-info/PKG-INFO` & `maxsmart-0.1.7/maxsmart.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.6/setup.py` & `maxsmart-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='maxsmart',
-    version='0.1.6',
+    version='0.1.7',
     author='Akim Sissaoui',
     author_email='superkikim@sissaoui.com',
     description='A Python module for operating network connected power strips',
     long_description='''A Python module for operating network connected power strips.
                         It provides functionality to turn on/off sockets, check their state, and retrieve power consumption data.''',
     url='https://github.com/superkikim/maxsmart',
     packages=find_packages(),
```

### Comparing `maxsmart-0.1.6/tests/test_maxsmart.py` & `maxsmart-0.1.7/tests/test_maxsmart.py`

 * *Files identical despite different names*

