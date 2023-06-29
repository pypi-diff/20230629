# Comparing `tmp/shioaji_realtime_kbars-1.0.1.tar.gz` & `tmp/shioaji_realtime_kbars-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shioaji_realtime_kbars-1.0.1.tar", last modified: Sat Jun 17 13:43:44 2023, max compression
+gzip compressed data, was "shioaji_realtime_kbars-1.0.3.tar", last modified: Thu Jun 29 16:01:52 2023, max compression
```

## Comparing `shioaji_realtime_kbars-1.0.1.tar` & `shioaji_realtime_kbars-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.1/LICENSE
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4056 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3462 2023-06-17 12:40:44.000000 shioaji_realtime_kbars-1.0.1/README.md
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.1/pyproject.toml
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      757 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/setup.cfg
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/src/
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars/__init__.py
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5170 2023-06-17 13:38:48.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
-drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 13:43:44.215323 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4056 2023-06-17 13:43:44.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/PKG-INFO
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-06-17 13:43:44.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-06-17 13:43:44.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-06-17 13:43:44.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/requires.txt
--rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-06-17 13:43:44.000000 shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/top_level.txt
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-17 08:10:47.000000 shioaji_realtime_kbars-1.0.3/LICENSE
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4244 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     3650 2023-06-29 16:01:34.000000 shioaji_realtime_kbars-1.0.3/README.md
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      103 2023-06-17 08:14:47.000000 shioaji_realtime_kbars-1.0.3/pyproject.toml
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      757 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/setup.cfg
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.015000 shioaji_realtime_kbars-1.0.3/src/
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       78 2023-06-17 13:37:43.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/__init__.py
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     5152 2023-06-29 15:59:45.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py
+drwxrwxr-x   0 dearestbee  (1000) dearestbee  (1000)        0 2023-06-29 16:01:52.019000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)     4244 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/PKG-INFO
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)      383 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/SOURCES.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)        1 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/dependency_links.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       15 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/requires.txt
+-rw-rw-r--   0 dearestbee  (1000) dearestbee  (1000)       23 2023-06-29 16:01:52.000000 shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/top_level.txt
```

### Comparing `shioaji_realtime_kbars-1.0.1/PKG-INFO` & `shioaji_realtime_kbars-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji_realtime_kbars
-Version: 1.0.1
+Version: 1.0.3
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -44,15 +44,15 @@
 When you use Shioaji Python API for technical analysis, you may need real-time data, and in different time dimensions, this package can help you subscribe to tick data and convert it into Kbars type (exactly the same as Shioaji Kbars ), to assist you in converting from Kbars to use more immediate data.
 
 ## Description
 
 1. To use the extension just initialize the object
 ```
 import shioaji_realtime_kbars
-Contracts = shioaji_realtime_kbars.shioaji_realtime_kbars(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 ```
 2. Get the real-time Kbars data with function
 ```
 shioaji_realtime_kbars.Kbars(
     contract: shioaji.contracts.BaseContract,
     period: str = '5min'
 ) -> shioaji.data.Kbars
@@ -91,38 +91,41 @@
 df = pd.DataFrame({**kbars})
 df.ts = pd.to_datetime(df.ts)
 df.tail(5)
 ```
 Change to
 
 ```
-Contracts = Realtime_Contracts(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1)
 Contracts.subscribe(api.Contracts.Futures.TXF.TXFR1)
 
 @api.on_tick_stk_v1()
 def callback(exchange: Exchange, tick : TickSTKv1):
     Contracts.update(tick, "stk")
 
 @api.on_tick_fop_v1()
 def callback(exchange : Exchange, tick : TickFOPv1):
     Contracts.update(tick, "fop")
-
+        
 while True:
-        MXFR1_1K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
-        df = pd.DataFrame({**MXFR1_1K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
-        MXFR1_5K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
-        df = pd.DataFrame({**MXFR1_5K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
+    MXFR1_1K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
+    df = pd.DataFrame({**MXFR1_1K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
+    MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
+    df = pd.DataFrame({**MXFR1_5K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.3 (2023/6/30)
+### v1.0.2 (2023/6/30)
+#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
```

### Comparing `shioaji_realtime_kbars-1.0.1/README.md` & `shioaji_realtime_kbars-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 When you use Shioaji Python API for technical analysis, you may need real-time data, and in different time dimensions, this package can help you subscribe to tick data and convert it into Kbars type (exactly the same as Shioaji Kbars ), to assist you in converting from Kbars to use more immediate data.
 
 ## Description
 
 1. To use the extension just initialize the object
 ```
 import shioaji_realtime_kbars
-Contracts = shioaji_realtime_kbars.shioaji_realtime_kbars(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 ```
 2. Get the real-time Kbars data with function
 ```
 shioaji_realtime_kbars.Kbars(
     contract: shioaji.contracts.BaseContract,
     period: str = '5min'
 ) -> shioaji.data.Kbars
@@ -75,38 +75,41 @@
 df = pd.DataFrame({**kbars})
 df.ts = pd.to_datetime(df.ts)
 df.tail(5)
 ```
 Change to
 
 ```
-Contracts = Realtime_Contracts(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1)
 Contracts.subscribe(api.Contracts.Futures.TXF.TXFR1)
 
 @api.on_tick_stk_v1()
 def callback(exchange: Exchange, tick : TickSTKv1):
     Contracts.update(tick, "stk")
 
 @api.on_tick_fop_v1()
 def callback(exchange : Exchange, tick : TickFOPv1):
     Contracts.update(tick, "fop")
-
+        
 while True:
-        MXFR1_1K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
-        df = pd.DataFrame({**MXFR1_1K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
-        MXFR1_5K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
-        df = pd.DataFrame({**MXFR1_5K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
+    MXFR1_1K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
+    df = pd.DataFrame({**MXFR1_1K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
+    MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
+    df = pd.DataFrame({**MXFR1_5K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.3 (2023/6/30)
+### v1.0.2 (2023/6/30)
+#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
```

### Comparing `shioaji_realtime_kbars-1.0.1/setup.cfg` & `shioaji_realtime_kbars-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shioaji_realtime_kbars
-version = 1.0.1
+version = 1.0.3
 author = NickLin910221
 author_email = nicklin910221@gmail.com
 description = An Extensions help you streaming with real-time data
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = shioaji
 url = https://github.com/NickLin910221/Shioaji_Realtime_Kline
```

### Comparing `shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py` & `shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars/shioaji_realtime_kbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     def __init__(self, api):
         self.api = api
         self.stk_Contracts, self.fop_Contracts = [], []
 
     def subscribe(self, contract, last_days = 0):
         if contract.__class__ is sj.contracts.Stock:
             for _contract_ in self.stk_Contracts:
-                if contract.contract.code == _contract_.contract.code: return
+                if contract.code == _contract_.contract.code: return
             self.stk_Contracts.append(Contracts(self.api, contract, last_days = last_days))    
         elif contract.__class__ is sj.contracts.Future or contract.__class__ is sj.contracts.Option:
             for _contract_ in self.fop_Contracts:
                 if contract.target_code == _contract_.contract.target_code or contract.code == _contract_.contract.code: return
             self.fop_Contracts.append(Contracts(self.api, contract, last_days = last_days))
             
     def update(self, tick, type):
@@ -96,13 +96,13 @@
         elif type == "fop":
             for _contract_ in self.fop_Contracts:
                 if tick.code == _contract_.contract.target_code or tick.code == _contract_.contract.code: _contract_.update(tick)
     
     def kbars(self, contract, period):
         if contract.__class__ is sj.contracts.Stock:
             for _contract_ in self.stk_Contracts:
-                if contract.contract.code == _contract_.contract.code: return _contract_.getklines(period)
+                if contract.code == _contract_.contract.code: return _contract_.getklines(period)
             return Kbars(ts = [], Open = [], High = [], Low = [], Close = [], Volume = [], Amount = []) 
         elif contract.__class__ is sj.contracts.Future or contract.__class__ is sj.contracts.Option:
             for _contract_ in self.fop_Contracts:
                 if contract.code == _contract_.contract.code: return _contract_.getklines(period)
             return Kbars(ts = [], Open = [], High = [], Low = [], Close = [], Volume = [], Amount = [])
```

### Comparing `shioaji_realtime_kbars-1.0.1/src/shioaji_realtime_kbars.egg-info/PKG-INFO` & `shioaji_realtime_kbars-1.0.3/src/shioaji_realtime_kbars.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shioaji-realtime-kbars
-Version: 1.0.1
+Version: 1.0.3
 Summary: An Extensions help you streaming with real-time data
 Home-page: https://github.com/NickLin910221/Shioaji_Realtime_Kline
 Author: NickLin910221
 Author-email: nicklin910221@gmail.com
 Project-URL: Bug Tracker, https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues
 Keywords: shioaji
 Classifier: Programming Language :: Python :: 3
@@ -44,15 +44,15 @@
 When you use Shioaji Python API for technical analysis, you may need real-time data, and in different time dimensions, this package can help you subscribe to tick data and convert it into Kbars type (exactly the same as Shioaji Kbars ), to assist you in converting from Kbars to use more immediate data.
 
 ## Description
 
 1. To use the extension just initialize the object
 ```
 import shioaji_realtime_kbars
-Contracts = shioaji_realtime_kbars.shioaji_realtime_kbars(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 ```
 2. Get the real-time Kbars data with function
 ```
 shioaji_realtime_kbars.Kbars(
     contract: shioaji.contracts.BaseContract,
     period: str = '5min'
 ) -> shioaji.data.Kbars
@@ -91,38 +91,41 @@
 df = pd.DataFrame({**kbars})
 df.ts = pd.to_datetime(df.ts)
 df.tail(5)
 ```
 Change to
 
 ```
-Contracts = Realtime_Contracts(api)
+Contracts = shioaji_realtime_kbars.ShioajiRealtimeKbars(api)
 Contracts.subscribe(api.Contracts.Futures.MXF.MXFR1)
 Contracts.subscribe(api.Contracts.Futures.TXF.TXFR1)
 
 @api.on_tick_stk_v1()
 def callback(exchange: Exchange, tick : TickSTKv1):
     Contracts.update(tick, "stk")
 
 @api.on_tick_fop_v1()
 def callback(exchange : Exchange, tick : TickFOPv1):
     Contracts.update(tick, "fop")
-
+        
 while True:
-        MXFR1_1K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
-        df = pd.DataFrame({**MXFR1_1K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
-        MXFR1_5K = Contracts.Kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
-        df = pd.DataFrame({**MXFR1_5K })
-        df.ts = pd.to_datetime(df.ts)
-        df.tail(5)
+    MXFR1_1K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "1min")
+    df = pd.DataFrame({**MXFR1_1K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
+    MXFR1_5K = Contracts.kbars(api.Contracts.Futures.MXF.MXFR1, "5min")
+    df = pd.DataFrame({**MXFR1_5K })
+    df.ts = pd.to_datetime(df.ts)
+    print(df.tail(2), end = "\n")
 ```
 
 ## Version
+### v1.0.3 (2023/6/30)
+### v1.0.2 (2023/6/30)
+#### * Fix Stock kbars problem [issue](https://github.com/NickLin910221/shioaji_realtime_kbars/issues/1)
 ### v1.0.1 
 #### * Fix Naming Problem
 ### v1.0.0
 
 ## Roadmap
 
 See the [open issues](https://github.com/NickLin910221/Shioaji_Realtime_Kline/issues) for a list of proposed features (and known issues).
```

