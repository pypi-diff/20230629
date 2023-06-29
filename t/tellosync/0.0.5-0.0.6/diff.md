# Comparing `tmp/tellosync-0.0.5.tar.gz` & `tmp/tellosync-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellosync-0.0.5.tar", last modified: Thu Jun 29 01:41:31 2023, max compression
+gzip compressed data, was "tellosync-0.0.6.tar", last modified: Thu Jun 29 02:55:52 2023, max compression
```

## Comparing `tellosync-0.0.5.tar` & `tellosync-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 01:41:31.323372 tellosync-0.0.5/
--rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2132 2023-06-29 01:41:31.322369 tellosync-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2023-06-22 13:01:38.000000 tellosync-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 01:41:31.324367 tellosync-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-06-29 01:41:15.000000 tellosync-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:41:31.293365 tellosync-0.0.5/tellosync/
--rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.5/tellosync/__init__.py
--rw-rw-rw-   0        0        0     2227 2023-06-27 11:55:49.000000 tellosync-0.0.5/tellosync/stats.py
--rw-rw-rw-   0        0        0     1047 2023-06-29 01:40:51.000000 tellosync-0.0.5/tellosync/synchro.py
--rw-rw-rw-   0        0        0     8799 2023-06-29 01:29:11.000000 tellosync-0.0.5/tellosync/tello.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:41:31.320367 tellosync-0.0.5/tellosync.egg-info/
--rw-rw-rw-   0        0        0     2132 2023-06-29 01:41:31.000000 tellosync-0.0.5/tellosync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-29 01:41:31.000000 tellosync-0.0.5/tellosync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 01:41:31.000000 tellosync-0.0.5/tellosync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-29 01:41:31.000000 tellosync-0.0.5/tellosync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-29 01:41:31.000000 tellosync-0.0.5/tellosync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 02:55:52.316222 tellosync-0.0.6/
+-rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2619 2023-06-29 02:55:52.316222 tellosync-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2041 2023-06-29 02:55:12.000000 tellosync-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 02:55:52.316222 tellosync-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-29 02:41:11.000000 tellosync-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 02:55:52.290756 tellosync-0.0.6/tellosync/
+-rw-rw-rw-   0        0        0      223 2023-06-22 13:01:38.000000 tellosync-0.0.6/tellosync/__init__.py
+-rw-rw-rw-   0        0        0     2227 2023-06-27 11:55:49.000000 tellosync-0.0.6/tellosync/stats.py
+-rw-rw-rw-   0        0        0     1072 2023-06-29 02:03:12.000000 tellosync-0.0.6/tellosync/synchro.py
+-rw-rw-rw-   0        0        0     8801 2023-06-29 02:40:47.000000 tellosync-0.0.6/tellosync/tello.py
+drwxrwxrwx   0        0        0        0 2023-06-29 02:55:52.315330 tellosync-0.0.6/tellosync.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-06-29 02:55:52.000000 tellosync-0.0.6/tellosync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-29 02:55:52.000000 tellosync-0.0.6/tellosync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 02:55:52.000000 tellosync-0.0.6/tellosync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-29 02:55:52.000000 tellosync-0.0.6/tellosync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-29 02:55:52.000000 tellosync-0.0.6/tellosync.egg-info/top_level.txt
```

### Comparing `tellosync-0.0.5/LICENSE` & `tellosync-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.5/PKG-INFO` & `tellosync-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# easyTello
-[![version info](https://img.shields.io/pypi/pyversions/easytello.svg)](https://pypi.org/project/easytello/)
-[![liscence](https://img.shields.io/pypi/l/easytello.svg)](https://pypi.org/project/easytello/)
-[![PyPI](https://img.shields.io/pypi/v/easytello.svg)](https://pypi.org/project/easytello/)
+# tellosync 
+[![version info](https://img.shields.io/pypi/pyversions/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![liscence](https://img.shields.io/pypi/l/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![PyPI](https://img.shields.io/pypi/v/tellosync.svg)](https://pypi.org/project/tellosync/)
 
-**Note: Not under active development**
-
-**easyTello** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+**tellosync** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+This library is based off of easyTello. tellosync is meant to add the ability to sync multiple computers using Arduinos. Each computer that is communicating with a drone is connected to an Arduino which then syncs with the Arduinos of other drones. This is a work in  progress as of 6/28/2023 and is mostly for the sake of learning. 
 
 ## Installation
 To install the library, simply run:
 ```
-pip install easytello
+pip install tellosync 
 ```
 or to install from cloned source:
 ```
-$ git clone https://github.com/Virodroid/easyTello.git
+$ git clone https://github.com/vwu1888/easyTello
 $ cd easyTello
 $ python setup.py install
 ```
-**Note:** easyTello requires OpenCV-Python. If you don't have it installed, simply run:
+**Note:** tellosync requires OpenCV-Python and pySerial. These should automatically install with tellosync, however, you can manually install it by running:
 ```
 pip install opencv-python
+
+pip install pyserial
 ```
 For more information on OpenCV-Python click [here](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html).
 
+For more information on pySerial click [here](https://pyserial.readthedocs.io/en/latest/index.html#).
+
 ## Examples
 Creating a drone object in Python:
 ```python
 from easytello import tello
 
 my_drone = tello.Tello()
 ```
```

### Comparing `tellosync-0.0.5/README.md` & `tellosync-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-# easyTello
-[![version info](https://img.shields.io/pypi/pyversions/easytello.svg)](https://pypi.org/project/easytello/)
-[![liscence](https://img.shields.io/pypi/l/easytello.svg)](https://pypi.org/project/easytello/)
-[![PyPI](https://img.shields.io/pypi/v/easytello.svg)](https://pypi.org/project/easytello/)
+# tellosync 
+[![version info](https://img.shields.io/pypi/pyversions/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![liscence](https://img.shields.io/pypi/l/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![PyPI](https://img.shields.io/pypi/v/tellosync.svg)](https://pypi.org/project/tellosync/)
 
-**Note: Not under active development**
-
-**easyTello** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+**tellosync** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+This library is based off of easyTello. tellosync is meant to add the ability to sync multiple computers using Arduinos. Each computer that is communicating with a drone is connected to an Arduino which then syncs with the Arduinos of other drones. This is a work in  progress as of 6/28/2023 and is mostly for the sake of learning. 
 
 ## Installation
 To install the library, simply run:
 ```
-pip install easytello
+pip install tellosync 
 ```
 or to install from cloned source:
 ```
-$ git clone https://github.com/Virodroid/easyTello.git
+$ git clone https://github.com/vwu1888/easyTello
 $ cd easyTello
 $ python setup.py install
 ```
-**Note:** easyTello requires OpenCV-Python. If you don't have it installed, simply run:
+**Note:** tellosync requires OpenCV-Python and pySerial. These should automatically install with tellosync, however, you can manually install it by running:
 ```
 pip install opencv-python
+
+pip install pyserial
 ```
 For more information on OpenCV-Python click [here](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html).
 
+For more information on pySerial click [here](https://pyserial.readthedocs.io/en/latest/index.html#).
+
 ## Examples
 Creating a drone object in Python:
 ```python
 from easytello import tello
 
 my_drone = tello.Tello()
 ```
```

### Comparing `tellosync-0.0.5/setup.py` & `tellosync-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tellosync',
-    version='0.0.5',
+    version='0.0.6',
     author='Ezra Fielding, Vincent Wu',
     author_email='ezra.fielding@gmail.com, vwu1888@gmail.com',
     description='An easy framework to support DJI Tello scripting in Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vwu1888/easyTello',
     packages=setuptools.find_packages(),
```

### Comparing `tellosync-0.0.5/tellosync/stats.py` & `tellosync-0.0.6/tellosync/stats.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.5/tellosync/synchro.py` & `tellosync-0.0.6/tellosync/synchro.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,12 @@
         self.ser.write(b"RESYNC")
     
     def start(self) -> None:
         self.ser.reset_input_buffer()
         self.ser.reset_output_buffer()
 
         self.ser.write(b"START")
+
+        time.sleep(1.0)
     
     def finished(self) -> None:
         self.ser.write(b"FINISH")
```

### Comparing `tellosync-0.0.5/tellosync/tello.py` & `tellosync-0.0.6/tellosync/tello.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             self.wait(abs(delay))
 
         self.wait_for_sync()
 
     def _keep_alive(self):
         # Sending command to Tello
         print("Keeping connection alive")
-        self.socket.sendto("stop".encode('utf-8'), self.tello_address)
+        self.socket.sendto("speed?".encode('utf-8'), self.tello_address)
 
     def _receive_thread(self):
         while True:
             # Checking for Tello response, throws socket error
             try:
                 self.response, ip = self.socket.recvfrom(1024)
                 self.log[-1].add_response(self.response.decode('utf-8'))
```

### Comparing `tellosync-0.0.5/tellosync.egg-info/PKG-INFO` & `tellosync-0.0.6/tellosync.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.5
+Version: 0.0.6
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# easyTello
-[![version info](https://img.shields.io/pypi/pyversions/easytello.svg)](https://pypi.org/project/easytello/)
-[![liscence](https://img.shields.io/pypi/l/easytello.svg)](https://pypi.org/project/easytello/)
-[![PyPI](https://img.shields.io/pypi/v/easytello.svg)](https://pypi.org/project/easytello/)
+# tellosync 
+[![version info](https://img.shields.io/pypi/pyversions/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![liscence](https://img.shields.io/pypi/l/tellosync.svg)](https://pypi.org/project/tellosync/)
+[![PyPI](https://img.shields.io/pypi/v/tellosync.svg)](https://pypi.org/project/tellosync/)
 
-**Note: Not under active development**
-
-**easyTello** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+**tellosync** is a Python library created to provide users with a simple way to interface and send commands to the DJI Tello drone, as well as to simply and easily teach students how to control the drone using Python 3. All the commands outlined in the DJI Tello SDK 1.3.0.0 are present in this library.
+This library is based off of easyTello. tellosync is meant to add the ability to sync multiple computers using Arduinos. Each computer that is communicating with a drone is connected to an Arduino which then syncs with the Arduinos of other drones. This is a work in  progress as of 6/28/2023 and is mostly for the sake of learning. 
 
 ## Installation
 To install the library, simply run:
 ```
-pip install easytello
+pip install tellosync 
 ```
 or to install from cloned source:
 ```
-$ git clone https://github.com/Virodroid/easyTello.git
+$ git clone https://github.com/vwu1888/easyTello
 $ cd easyTello
 $ python setup.py install
 ```
-**Note:** easyTello requires OpenCV-Python. If you don't have it installed, simply run:
+**Note:** tellosync requires OpenCV-Python and pySerial. These should automatically install with tellosync, however, you can manually install it by running:
 ```
 pip install opencv-python
+
+pip install pyserial
 ```
 For more information on OpenCV-Python click [here](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html).
 
+For more information on pySerial click [here](https://pyserial.readthedocs.io/en/latest/index.html#).
+
 ## Examples
 Creating a drone object in Python:
 ```python
 from easytello import tello
 
 my_drone = tello.Tello()
 ```
```

