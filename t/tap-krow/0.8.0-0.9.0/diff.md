# Comparing `tmp/tap_krow-0.8.0.tar.gz` & `tmp/tap_krow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_krow-0.8.0.tar", max compression
+gzip compressed data, was "tap_krow-0.9.0.tar", max compression
```

## Comparing `tap_krow-0.8.0.tar` & `tap_krow-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1045 2023-04-27 00:02:26.710002 tap_krow-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/__init__.py
--rw-r--r--   0        0        0      399 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/auth.py
--rw-r--r--   0        0        0     9385 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/client.py
--rw-r--r--   0        0        0     2719 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/normalize.py
--rw-r--r--   0        0        0    12491 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/streams.py
--rw-r--r--   0        0        0     1257 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tap.py
--rw-r--r--   0        0        0       31 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/__init__.py
--rw-r--r--   0        0        0    24080 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/applicants/applicants_default.json
--rw-r--r--   0        0        0     1509 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_no_relationships_property.json
--rw-r--r--   0        0        0      549 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json
--rw-r--r--   0        0        0     4922 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/locations/locations_default.json
--rw-r--r--   0        0        0    60100 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_default.json
--rw-r--r--   0        0        0      575 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json
--rw-r--r--   0        0        0     7860 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json
--rw-r--r--   0        0        0     4411 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/positions/positions_default.json
--rw-r--r--   0        0        0     4311 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/api_responses/regions/regions_default.json
--rw-r--r--   0        0        0      959 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_applicants_stream.py
--rw-r--r--   0        0        0     3186 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_client.py
--rw-r--r--   0        0        0      681 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_core.py
--rw-r--r--   0        0        0     1375 2023-04-27 00:02:25.805999 tap_krow-0.8.0/tap_krow/tests/test_locations_stream.py
--rw-r--r--   0        0        0     1723 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_normalize.py
--rw-r--r--   0        0        0     1523 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_organizations_stream.py
--rw-r--r--   0        0        0     1678 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_paginator.py
--rw-r--r--   0        0        0     1261 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_positions_stream.py
--rw-r--r--   0        0        0     1360 2023-04-27 00:02:25.809999 tap_krow-0.8.0/tap_krow/tests/test_regions_stream.py
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 tap_krow-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1045 2023-06-29 15:54:36.704169 tap_krow-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/__init__.py
+-rw-r--r--   0        0        0      399 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/auth.py
+-rw-r--r--   0        0        0     9385 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/client.py
+-rw-r--r--   0        0        0     2719 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/normalize.py
+-rw-r--r--   0        0        0    12634 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/streams.py
+-rw-r--r--   0        0        0     1257 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tap.py
+-rw-r--r--   0        0        0       31 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/__init__.py
+-rw-r--r--   0        0        0    38646 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/applicants/applicants_default.json
+-rw-r--r--   0        0        0     1509 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/campaigns/campaigns_no_relationships_property.json
+-rw-r--r--   0        0        0      549 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json
+-rw-r--r--   0        0        0     4922 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/locations/locations_default.json
+-rw-r--r--   0        0        0    60100 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_default.json
+-rw-r--r--   0        0        0      575 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json
+-rw-r--r--   0        0        0     7860 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json
+-rw-r--r--   0        0        0     4411 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/positions/positions_default.json
+-rw-r--r--   0        0        0     4311 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/api_responses/regions/regions_default.json
+-rw-r--r--   0        0        0      996 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/test_applicants_stream.py
+-rw-r--r--   0        0        0     3186 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/test_client.py
+-rw-r--r--   0        0        0      681 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/test_core.py
+-rw-r--r--   0        0        0     1375 2023-06-29 15:54:35.948159 tap_krow-0.9.0/tap_krow/tests/test_locations_stream.py
+-rw-r--r--   0        0        0     1723 2023-06-29 15:54:35.952159 tap_krow-0.9.0/tap_krow/tests/test_normalize.py
+-rw-r--r--   0        0        0     1523 2023-06-29 15:54:35.952159 tap_krow-0.9.0/tap_krow/tests/test_organizations_stream.py
+-rw-r--r--   0        0        0     1678 2023-06-29 15:54:35.952159 tap_krow-0.9.0/tap_krow/tests/test_paginator.py
+-rw-r--r--   0        0        0     1261 2023-06-29 15:54:35.952159 tap_krow-0.9.0/tap_krow/tests/test_positions_stream.py
+-rw-r--r--   0        0        0     1360 2023-06-29 15:54:35.952159 tap_krow-0.9.0/tap_krow/tests/test_regions_stream.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 tap_krow-0.9.0/PKG-INFO
```

### Comparing `tap_krow-0.8.0/pyproject.toml` & `tap_krow-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-krow"
-version = "0.8.0"
+version = "0.9.0"
 description = "`tap-krow` is a Singer tap for the KROW API, built with the Meltano SDK for Singer Taps."
 authors = ["Datateer"]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.12"
 requests = "^2.25.1"
```

### Comparing `tap_krow-0.8.0/tap_krow/client.py` & `tap_krow-0.9.0/tap_krow/client.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/normalize.py` & `tap_krow-0.9.0/tap_krow/normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             # is effectively removed from the resulting dict
         else:
             if isinstance(d[key], dict):
                 # recurse through the children
                 res[key] = remove_unnecessary_keys(value, keys_to_remove, path)
             else:
                 res[key] = value
-    # run the same function for each child dict, using the output as the new value
+    # Run the same function for each child dict, using the output as the new value
     return res
 
 
 def flatten_dict(d, parent_key: str = "", delimiter: str = "_"):
     return dict(_flatten_dict_gen(d, parent_key, delimiter))
```

### Comparing `tap_krow-0.8.0/tap_krow/streams.py` & `tap_krow-0.9.0/tap_krow/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
         Property("created_at", DateTimeType),
         Property("first_name", StringType),
         Property("full_name", StringType),
         Property("last_name", StringType),
         Property("interview_id", StringType),
         Property("locality_id", StringType),
         Property("locality_type", StringType),
+        Property("retainment_id", StringType),
         Property("status", StringType),
         Property("opening_position_id", StringType),
         Property("organization_id", StringType),
         Property("state_action", StringType),
         Property("state_changed_at", DateTimeType),
         Property("state_name", StringType),
         Property("updated_at", DateTimeType, required=True),
@@ -209,18 +210,24 @@
         """Return a context dictionary for the child streams.
         Refer to https://sdk.meltano.com/en/latest/parent_streams.html"""
         return {"calendar_id": record["id"]}
 
     def validate_response(self, response):
         # Still catch error status codes
         if response.status_code == 404:
-            msg = f"{response.status_code} Customer without Calendar in this Region: " f"{response.reason} for url: {response.url}"
+            msg = (
+                f"{response.status_code} Customer without Calendar in this Region: "
+                f"{response.reason} for url: {response.url}"
+            )
             raise CustomerNotEnabledError(msg)
         if response.status_code == 409:
-            msg = f"{response.status_code} Conflict Error: " f"{response.reason} for url: {response.url}"
+            msg = (
+                f"{response.status_code} Conflict Error: "
+                f"{response.reason} for url: {response.url}"
+            )
             raise CustomerNotEnabledError(msg)
 
 
 class LocationCalendarStream(KrowStream):
     name = "location_calendars"
     path = "/locations/{location_id}/calendar"
     schema = PropertiesList(
```

### Comparing `tap_krow-0.8.0/tap_krow/tap.py` & `tap_krow-0.9.0/tap_krow/tap.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_no_relationships_property.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/campaigns/campaigns_no_relationships_property.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/campaigns/campaigns_zero_records.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/locations/locations_default.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/locations/locations_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_default.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_last_page.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/organizations/orgs_records_before_and_after_2020-01-01.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/positions/positions_default.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/positions/positions_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/api_responses/regions/regions_default.json` & `tap_krow-0.9.0/tap_krow/tests/api_responses/regions/regions_default.json`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_applicants_stream.py` & `tap_krow-0.9.0/tap_krow/tests/test_applicants_stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,12 +23,13 @@
     assert "created_at" in res[0]
     assert "first_name" in res[0]
     assert "last_name" in res[0]
     assert "full_name" in res[0]
     assert "locality_id" in res[0]
     assert "locality_type" in res[0]
     assert "opening_position_id" in res[0]
+    assert "retainment_id" in res[0]
     assert "state_changed_at" in res[0]
     assert "state_action" in res[0]
     assert "state_name" in res[0]
     assert "status" in res[0]
     assert "transitioning" not in res[0]
```

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_client.py` & `tap_krow-0.9.0/tap_krow/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_core.py` & `tap_krow-0.9.0/tap_krow/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_locations_stream.py` & `tap_krow-0.9.0/tap_krow/tests/test_locations_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_normalize.py` & `tap_krow-0.9.0/tap_krow/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_organizations_stream.py` & `tap_krow-0.9.0/tap_krow/tests/test_organizations_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_paginator.py` & `tap_krow-0.9.0/tap_krow/tests/test_paginator.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_positions_stream.py` & `tap_krow-0.9.0/tap_krow/tests/test_positions_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/tap_krow/tests/test_regions_stream.py` & `tap_krow-0.9.0/tap_krow/tests/test_regions_stream.py`

 * *Files identical despite different names*

### Comparing `tap_krow-0.8.0/PKG-INFO` & `tap_krow-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-krow
-Version: 0.8.0
+Version: 0.9.0
 Summary: `tap-krow` is a Singer tap for the KROW API, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Author: Datateer
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

