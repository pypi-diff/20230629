# Comparing `tmp/rosetta-ce-1.3.0.tar.gz` & `tmp/rosetta-ce-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.0.tar", last modified: Thu Jun 29 15:07:02 2023, max compression
+gzip compressed data, was "rosetta-ce-1.3.1.tar", last modified: Thu Jun 29 15:23:42 2023, max compression
```

## Comparing `rosetta-ce-1.3.0.tar` & `rosetta-ce-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.666349 rosetta-ce-1.3.0/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.0/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:07:02.666054 rosetta-ce-1.3.0/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.0/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.660006 rosetta-ce-1.3.0/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.0/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.662026 rosetta-ce-1.3.0/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.0/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.0/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.0/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    33530 2023-06-29 15:05:33.000000 rosetta-ce-1.3.0/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     7785 2023-06-29 06:42:23.000000 rosetta-ce-1.3.0/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.664106 rosetta-ce-1.3.0/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 15:07:02.000000 rosetta-ce-1.3.0/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 15:07:02.666393 rosetta-ce-1.3.0/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 15:05:54.000000 rosetta-ce-1.3.0/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:07:02.665521 rosetta-ce-1.3.0/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.0/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.0/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.0/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.410446 rosetta-ce-1.3.1/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.1/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:23:42.410121 rosetta-ce-1.3.1/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.1/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.404608 rosetta-ce-1.3.1/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.1/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.406458 rosetta-ce-1.3.1/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.1/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.1/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.1/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    33530 2023-06-29 15:05:33.000000 rosetta-ce-1.3.1/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8454 2023-06-29 15:22:28.000000 rosetta-ce-1.3.1/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.408362 rosetta-ce-1.3.1/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-29 15:23:42.000000 rosetta-ce-1.3.1/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-29 15:23:42.410504 rosetta-ce-1.3.1/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-29 15:22:47.000000 rosetta-ce-1.3.1/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-29 15:23:42.409611 rosetta-ce-1.3.1/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.1/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.1/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.1/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.0/LICENSE` & `rosetta-ce-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/PKG-INFO` & `rosetta-ce-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.0
+Version: 1.3.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.0/README.md` & `rosetta-ce-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/constants/sensors.py` & `rosetta-ce-1.3.1/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/constants/sources.py` & `rosetta-ce-1.3.1/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/constants/systems.py` & `rosetta-ce-1.3.1/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/rconverter.py` & `rosetta-ce-1.3.1/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/rfaker.py` & `rosetta-ce-1.3.1/rosetta/rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/rosetta/rsender.py` & `rosetta-ce-1.3.1/rosetta/rsender.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
             Returns:
                 None.
     """
 
     def __init__(self, data_type: str, destination: str,
                  worker_name: Optional[str] = 'worker_'+str(datetime.now()), count: Optional[int] = 1,
-                 interval: Optional[int] = 1, observables: Optional[Observables] = None, fields: Optional[str] = None,
+                 interval: Optional[int] = 1, vendor: Optional[str] = None, product: Optional[str] = None,
+                 version: Optional[str] = None, observables: Optional[Observables] = None, fields: Optional[str] = None,
                  verify_ssl: Optional[bool] = None, datetime_obj: Optional[datetime] = None):
         """
         Constructor for DataSenderWorker class.
 
         :param data_type: A value from the WorkerTypeEnum indicating the type of data to send. Options include:
             - SYSLOG
             - CEF
@@ -69,25 +70,31 @@
             - WINEVENT
             - JSON
             - INCIDENT
         :param destination: str, destination address and port in the format <scheme>://<address>:<port>.
         :param worker_name: str, name of the worker.
         :param count: int, number of times to send the data.
         :param interval: int, time interval between two consecutive data sends.
+        :param vendor: Optional. The vendor.
+        :param product: Optional. The product.
+        :param version: Optional. The version.
         :param observables: Observables, list of observables.
         :param fields: str, comma-separated list of fields to include in incident data.
         :param verify_ssl: bool, handling ssl verification errors.
 
         :return: None
         """
         self.thread = None
         self.worker_name = worker_name
         self.data_type = data_type
         self.count = count
         self.interval = interval
+        self.vendor = vendor
+        self.product = product
+        self.version = version
         self.destination = destination
         self.created_at = datetime.now()
         self.status = "Stopped"
         self.observables = observables
         self.fields = fields
         self.verify_ssl = verify_ssl
         self.datetime_obj = datetime_obj
@@ -129,17 +136,21 @@
         while self.status == "Running" and self.count > 0:
             try:
                 self.count -= 1
                 if self.data_type in ["SYSLOG", "CEF", "LEEF"]:
                     if self.data_type == "SYSLOG":
                         fake_message = Events.syslog(count=1, timestamp=self.datetime_obj, observables=self.observables)
                     if self.data_type == "CEF":
-                        fake_message = Events.cef(count=1, timestamp=self.datetime_obj, observables=self.observables)
+                        fake_message = Events.cef(count=1, timestamp=self.datetime_obj, vendor=self.vendor,
+                                                  product=self.product, version=self.version,
+                                                  observables=self.observables)
                     if self.data_type == "LEEF":
-                        fake_message = Events.leef(count=1, timestamp=self.datetime_obj, observables=self.observables)
+                        fake_message = Events.leef(count=1, timestamp=self.datetime_obj, vendor=self.vendor,
+                                                   product=self.product, version=self.version,
+                                                   observables=self.observables)
                     ip_address = self.destination.split(':')[1]
                     port = self.destination.split(':')[2]
                     if 'tcp' in self.destination:
                         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                         sock.settimeout(5)
                         sock.connect((ip_address, int(port)))
                         print(f"Worker: {self.worker_name} sending log message to {ip_address} ")
```

### Comparing `rosetta-ce-1.3.0/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.3.1/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.0
+Version: 1.3.1
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.0/setup.py` & `rosetta-ce-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.0",
+    version="1.3.1",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.0/tests/test_rconverter.py` & `rosetta-ce-1.3.1/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/tests/test_rfaker.py` & `rosetta-ce-1.3.1/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.0/tests/test_rsender.py` & `rosetta-ce-1.3.1/tests/test_rsender.py`

 * *Files identical despite different names*

