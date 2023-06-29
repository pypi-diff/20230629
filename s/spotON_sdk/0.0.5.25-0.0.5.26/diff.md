# Comparing `tmp/spotON_sdk-0.0.5.25.tar.gz` & `tmp/spotON_sdk-0.0.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.25.tar", last modified: Tue Jun  6 23:18:32 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.26.tar", last modified: Thu Jun 29 09:36:23 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.25.tar` & `spotON_sdk-0.0.5.26.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.25/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.25/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.25/LICENSE
--rw-r--r--   0        0        0      380 2023-06-06 23:00:41.979147 spotON_sdk-0.0.5.25/pyproject.toml
--rw-r--r--   0        0        0     1225 2023-06-02 16:15:25.317306 spotON_sdk-0.0.5.25/spotON_sdk/API/API_Call.py
--rw-r--r--   0        0        0     1433 2023-06-05 11:04:54.850603 spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/auth.py
--rw-r--r--   0        0        0      789 2023-06-06 23:13:35.152489 spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/hub.py
--rw-r--r--   0        0        0     1166 2023-06-06 23:13:32.739879 spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/light.py
--rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.25/spotON_sdk/API/__init__.py
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     3012 2023-06-01 08:37:08.552222 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.25/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      478 2023-06-06 23:18:29.070945 spotON_sdk-0.0.5.25/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      163 2023-06-06 23:18:18.249108 spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     1853 2023-06-06 23:14:11.446293 spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/time_helper.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.25/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.25/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.26/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.26/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.26/LICENSE
+-rw-r--r--   0        0        0      380 2023-06-06 23:00:41.979147 spotON_sdk-0.0.5.26/pyproject.toml
+-rw-r--r--   0        0        0     1225 2023-06-02 16:15:25.317306 spotON_sdk-0.0.5.26/spotON_sdk/API/API_Call.py
+-rw-r--r--   0        0        0     1433 2023-06-11 16:51:01.099711 spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/auth.py
+-rw-r--r--   0        0        0      789 2023-06-11 16:51:02.270454 spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/hub.py
+-rw-r--r--   0        0        0     1166 2023-06-11 16:51:08.318240 spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/light.py
+-rw-r--r--   0        0        0      101 2023-06-01 17:06:55.423781 spotON_sdk-0.0.5.26/spotON_sdk/API/__init__.py
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-29 09:35:25.034081 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      239 2023-06-01 17:02:39.339895 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     3012 2023-06-01 08:37:08.552222 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-06-01 17:04:16.714855 spotON_sdk-0.0.5.26/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      478 2023-06-29 09:35:52.371582 spotON_sdk-0.0.5.26/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      163 2023-06-06 23:18:18.249108 spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     1853 2023-06-06 23:14:11.446293 spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/time_helper.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.26/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      266 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.26/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.25/.gitignore` & `spotON_sdk-0.0.5.26/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/LICENSE` & `spotON_sdk-0.0.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/API/API_Call.py` & `spotON_sdk-0.0.5.26/spotON_sdk/API/API_Call.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/auth.py` & `spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/auth.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/hub.py` & `spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/hub.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/API/HASS/light.py` & `spotON_sdk-0.0.5.26/spotON_sdk/API/HASS/light.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-from math import e
-from mimetypes import init
-from os import name
 from typing import List, Union
 from pydantic import  Field, validator, root_validator
+import json
+
 from .timeframes import Timeframes,Timeframe
 from .markets import Market, Markets
 from .customBaseModel import CustomBaseModel
 
-import json
-
 class Interrupted_On_Time(CustomBaseModel):
     name: str = Field(default="Interrupted_On_Time",init = False)
+    minimum_hours_on: int = Field(default=1,init = False)
     pass
 
-
 class Continuous_On_Time(CustomBaseModel):
     name: str = Field(default="Continuous_On_Time",init = False)
     week: int = Field(default=None)
     best_hour: int = Field(default=None)
 
 class Price_Logic(CustomBaseModel):
     nr_of_hours_on: int
```

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.26/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.25/spotON_sdk/data_helpers/time_helper.py` & `spotON_sdk-0.0.5.26/spotON_sdk/data_helpers/time_helper.py`

 * *Files identical despite different names*

