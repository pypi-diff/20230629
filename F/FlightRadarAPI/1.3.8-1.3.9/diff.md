# Comparing `tmp/flightradarapi-1.3.8.tar.gz` & `tmp/flightradarapi-1.3.9.tar.gz`

## Comparing `flightradarapi-1.3.8.tar` & `flightradarapi-1.3.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/requirements.txt
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/__init__.py
--rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/api.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/core.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/errors.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/request.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/__init__.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/airport.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/entity.py
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/FlightRadar24/entities/flight.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/tests/package.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/tests/test_api.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/LICENSE
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/README.md
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 flightradarapi-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/requirements.txt
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/__init__.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/api.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/core.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/errors.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/request.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/entities/__init__.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/entities/airport.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/entities/entity.py
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/FlightRadar24/entities/flight.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/tests/package.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/tests/test_api.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/tests/util.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/LICENSE
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/README.md
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 flightradarapi-1.3.9/PKG-INFO
```

### Comparing `flightradarapi-1.3.8/.github/workflows/python-package.yml` & `flightradarapi-1.3.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/__init__.py` & `flightradarapi-1.3.9/FlightRadar24/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 See more information at:
 https://www.flightradar24.com/premium/
 https://www.flightradar24.com/terms-and-conditions
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 from .api import FlightRadar24API, FlightTrackerConfig
 from .entities import Airport, Flight
```

### Comparing `flightradarapi-1.3.8/FlightRadar24/api.py` & `flightradarapi-1.3.9/FlightRadar24/api.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/core.py` & `flightradarapi-1.3.9/FlightRadar24/core.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/request.py` & `flightradarapi-1.3.9/FlightRadar24/request.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/entities/airport.py` & `flightradarapi-1.3.9/FlightRadar24/entities/airport.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/entities/entity.py` & `flightradarapi-1.3.9/FlightRadar24/entities/entity.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/FlightRadar24/entities/flight.py` & `flightradarapi-1.3.9/FlightRadar24/entities/flight.py`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/LICENSE` & `flightradarapi-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flightradarapi-1.3.8/pyproject.toml` & `flightradarapi-1.3.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 exclude = ["tests"]
 requires-python = ">=3.7"
 dependencies = [
   "Brotli",
-  "Deprecated",
   "requests",
 ]
 
 [project.optional-dependencies]
 tests = [
   "pytest",
 ]
```

### Comparing `flightradarapi-1.3.8/PKG-INFO` & `flightradarapi-1.3.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlightRadarAPI
-Version: 1.3.8
+Version: 1.3.9
 Summary: API for FlightRadar24
 Project-URL: Homepage, https://github.com/JeanExtreme002/FlightRadarAPI
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,flightradar24
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: brotli
-Requires-Dist: deprecated
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # FlightRadarAPI
 Unofficial API for [FlightRadar24](https://www.flightradar24.com/) written in Python 3.
@@ -30,74 +29,101 @@
 
 [![Python Package](https://github.com/JeanExtreme002/FlightRadarAPI/workflows/Python%20Package/badge.svg)](https://github.com/JeanExtreme002/FlightRadarAPI/actions)
 [![Pypi](https://img.shields.io/pypi/v/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
 [![License](https://img.shields.io/pypi/l/FlightRadarAPI)](https://pypi.org/project/FlightRadarAPI/)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/FlightRadarAPI/)
 [![Downloads](https://static.pepy.tech/personalized-badge/flightradarapi?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/FlightRadarAPI/)
 
-# Installing FlightRadarAPI:
+## Installing FlightRadarAPI:
 ```
 pip3 install FlightRadarAPI
 ```
 
-# Basic Usage:
-Just create a `FlightRadar24API` object after importing it.
-
+## Basic Usage:
+Import the class `FlightRadar24API` and create an instance of it.
 ```
 from FlightRadar24 import FlightRadar24API
-fr_api = FlightRadar24API()
+fr_api = FlightRadar24API(...)
 ```
 
-**Getting airports list:**
+**Getting flights list:**
 ```
-airports = fr_api.get_airports()
+flights = fr_api.get_flights(...)  # Returns a list of Flight objects
 ```
 
-**Getting airlines list:**
+**Getting airports list:**
 ```
-airlines = fr_api.get_airlines()
+airports = fr_api.get_airports(...)  # Returns a list of Airport objects
 ```
 
-**Getting flights list:**
+**Getting airlines list:**
 ```
-flights = fr_api.get_flights(...)
+airlines = fr_api.get_airlines()
 ```
 
 **Getting zones list:**
 ```
 zones = fr_api.get_zones()
 ```
 
-You can also get more information about a specific flight such as: aircraft images, estimated time, trail, etc.
+You can also get more information about a specific flight such as: estimated time, trail, aircraft details, etc.
 ```
-details = fr_api.get_flight_details(flight.id)
-flight.set_flight_details(details)
+flight_details = fr_api.get_flight_details(flight.id)
+flight.set_flight_details(flight_details)
 
 print("Flying to", flight.destination_airport_name)
 ```
 
-# Filtering flights and airports:
-**Getting flights by airline:**
+Or get more information about a specific airport such as: runways, temperature, arrived flights, etc.
 ```
-airline_icao = "AZU"
-thy_flights = fr_api.get_flights(airline = airline_icao)
+airport_details = fr_api.get_airport_details(airport.icao)
 ```
 
-**Getting flights by bounds:**
+## Filtering flights and airports:
+The `get_flights(...)` method has some parameters to search for flights by: area line, bounds (customized coordinates 
+or obtained by the `get_zones()` method), aircraft registration or aircraft type. See the example below:
 ```
+airline_icao = "UAE"
+aircraft_type = "B77W"
+
+# You may also set a custom region, such as: bounds = "73,-12,-156,38"
+zone = fr_api.get_zones()["northamerica"]
 bounds = fr_api.get_bounds(zone)
-flights = fr_api.get_flights(bounds = bounds)
+
+emirates_flights = fr_api.get_flights(
+    aircraft_type = aircraft_type
+    airline = airline_icao,
+    bounds = bounds
+)
 ```
+There are more configurations that you may set by using the `set_flight_tracker_config(...)` method. See the method documentation
+for more information.
 
 **Getting airport by ICAO or IATA:**
 ```
-airport_icao = "VNLK"
-lukla_airport = fr_api.get_airport(airport_icao)
+lukla_airport = fr_api.get_airport(code = "VNLK")
+```
+
+## Getting the distance between flights and airports:
+The `Flight` and `Airport` classes inherit from `Entity`, which contains the `get_distance_from(...)` method. That method
+returns the distance between the self instance and another entity in kilometers. Example:
+```
+airport = fr_api.get_airport("KJFK")
+distance = flight.get_distance_from(airport)
+
+print(f"The flight is {distance} km away from the airport.")
 ```
 
-**Getting and configuring Real-time Flight Tracker parameters:**
+## Setting and getting Real-time Flight Tracker parameters:
+Set it by using the `set_flight_tracker_config(...)` method. It receives a `FlightTrackerConfig` dataclass instance, but
+you can also use keyword arguments directly to the method.
+
+Get the current configuration with the `get_flight_tracker_config()` method, that returns a `FlightTrackerConfig` 
+instance. Note: creating a new `FlightTrackerConfig` instance means resetting all parameters to default.
 ```
-config = fr_api.get_flight_tracker_config()
+flight_tracker = fr_api.get_flight_tracker_config()
+flight_tracker.limit = 10
+
+fr_api.set_flight_tracker_config(flight_tracker, ...)
 
-new_config = FlightTrackerConfig(...)
-fr_api.set_flight_tracker_config(new_config, limit = 500, ...)
+flights = fr_api.get_flights(...)  # Returns only 10 flights
 ```
```

