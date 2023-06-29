# Comparing `tmp/specklia-1.1.4.tar.gz` & `tmp/specklia-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.4.tar", last modified: Thu Jun 29 10:17:31 2023, max compression
+gzip compressed data, was "specklia-1.1.5.tar", last modified: Thu Jun 29 13:34:09 2023, max compression
```

## Comparing `specklia-1.1.4.tar` & `specklia-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 09:58:06.000000 specklia-1.1.4/LICENCE
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 10:17:31.108687 specklia-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 09:58:06.000000 specklia-1.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 10:17:31.108687 specklia-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-29 09:58:06.000000 specklia-1.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 09:58:06.000000 specklia-1.1.4/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24283 2023-06-29 10:17:28.000000 specklia-1.1.4/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 09:58:06.000000 specklia-1.1.4/specklia/websocket_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)    10065 2023-06-29 10:17:28.000000 specklia-1.1.4/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 09:58:06.000000 specklia-1.1.4/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:34:09.509611 specklia-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 13:33:59.000000 specklia-1.1.5/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 13:34:09.509611 specklia-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 13:33:59.000000 specklia-1.1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 13:34:09.509611 specklia-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-29 13:33:59.000000 specklia-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:34:09.505611 specklia-1.1.5/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 13:33:59.000000 specklia-1.1.5/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24421 2023-06-29 13:33:59.000000 specklia-1.1.5/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 13:33:59.000000 specklia-1.1.5/specklia/websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:34:09.509611 specklia-1.1.5/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 13:34:09.000000 specklia-1.1.5/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 13:34:09.000000 specklia-1.1.5/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 13:34:09.000000 specklia-1.1.5/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 13:34:09.000000 specklia-1.1.5/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 13:34:09.000000 specklia-1.1.5/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:34:09.509611 specklia-1.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)    10182 2023-06-29 13:33:59.000000 specklia-1.1.5/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 13:33:59.000000 specklia-1.1.5/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.4/LICENCE` & `specklia-1.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.4/PKG-INFO` & `specklia-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.4/README.md` & `specklia-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.4/setup.py` & `specklia-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.4/specklia/client.py` & `specklia-1.1.5/specklia/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,18 @@
             self.server_url + "/users",
             headers={"Authorization": "Bearer " + self.auth_token},
             params={'group_id': group_id})
         _check_response_ok(response)
         _log.info('listed users within group_id %s.', group_id)
         return pd.DataFrame(response.json()).convert_dtypes()
 
-    def query(self: Specklia, dataset_id: str, epsg4326_polygon: Polygon,  # noqa: CFQ002
-              min_datetime: datetime, max_datetime: datetime,
-              columns_to_return: List[str],
-              additional_filters: List[Dict[str, Union[float, str]]]) -> Tuple[gpd.GeoDataFrame, Dict]:
+    def query_dataset(self: Specklia, dataset_id: str, epsg4326_polygon: Polygon,  # noqa: CFQ002
+                      min_datetime: datetime, max_datetime: datetime,
+                      columns_to_return: List[str],
+                      additional_filters: List[Dict[str, Union[float, str]]]) -> Tuple[gpd.GeoDataFrame, Dict]:
         """
         Query data within a dataset.
 
         You must be part of the group that owns the dataset in order to do this.
 
         All provided conditions are applied to the dataset via logical AND
         (i.e. only points that meet all of the conditions will be returned).
@@ -154,15 +154,16 @@
         if response['status'] == HTTPStatus.OK:
             _log.info('queried dataset with ID %s.', dataset_id)
             return response['gdf'], response['sources']
         else:
             _log.error('Failed to interact with Specklia server, error was %s', str(response))
             raise RuntimeError(str(response))
 
-    def update(self: Specklia, _dataset_id: str, _new_points: pd.DataFrame, _source_description: Dict) -> None:
+    def update_points_in_dataset(
+            self: Specklia, _dataset_id: str, _new_points: pd.DataFrame, _source_description: Dict) -> None:
         """
         Update previously existing data within a dataset.
 
         You must have READ_WRITE or ADMIN permissions within the group that owns the dataset in order to do this.
         Should be called once for each separate source of data.
 
         Parameters
@@ -181,15 +182,16 @@
         ------
         NotImplementedError
             This route is not yet implemented.
         """
         _log.error('this method is not yet implemented.')
         raise NotImplementedError()
 
-    def ingest(self: Specklia, dataset_id: str, new_points: gpd.GeoDataFrame, source_description: Dict) -> None:
+    def add_points_to_dataset(
+            self: Specklia, dataset_id: str, new_points: gpd.GeoDataFrame, source_description: Dict) -> None:
         """
         Add new data to a dataset.
 
         You must have READ_WRITE or ADMIN permissions within the group that owns the dataset in order to do this.
 
         Note that Ingests are temporarily restricted to those that have READ_WRITE permissions
         within the all_users group (i.e. Specklia is read-only to the general public).
@@ -224,15 +226,15 @@
         response = websocket_helpers.receive_object_from_websocket(ws, self._data_streaming_timeout_s)
         if response['status'] == HTTPStatus.OK:
             _log.info('Added new data to specklia dataset ID %s.', dataset_id)
         else:
             _log.error('Failed to interact with Specklia server, error was %s', str(response))
             raise RuntimeError(str(response))
 
-    def delete_data(self: Specklia, _dataset_id: str, _row_ids_to_delete: List[str]) -> None:
+    def delete_points_in_dataset(self: Specklia, _dataset_id: str, _row_ids_to_delete: List[str]) -> None:
         """
         Delete data from a dataset.
 
         You must have READ_WRITE or ADMIN permissions within the group that owns the dataset in order to do this.
         Note that this does not delete the dataset itself. Instead, this method is for deleting specific rows within
         the dataset.
 
@@ -288,17 +290,17 @@
         """
         response = requests.post(self.server_url + "/groups", json={'group_name': group_name},
                                  headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('created new group with name %s.', group_name)
         return response.text.strip('\n"')
 
-    def change_group_name(self: Specklia, group_id: str, new_group_name: str) -> str:
+    def update_group_name(self: Specklia, group_id: str, new_group_name: str) -> str:
         """
-        Change the name of a group.
+        Update the name of a group.
 
         You must have ADMIN permissions within the group in order to do this.
 
         Parameters
         ----------
         group_id : str
             UUID of group
@@ -311,15 +313,15 @@
             Response from server
         """
         response = requests.put(
             self.server_url + "/groups",
             json={'group_id': group_id, 'new_group_name': new_group_name},
             headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
-        _log.info('changed name of group ID %s to %s.', group_id, new_group_name)
+        _log.info('updated name of group ID %s to %s.', group_id, new_group_name)
         return response.text.strip('\n"')
 
     def delete_group(self: Specklia, group_id: str) -> str:
         """
         Delete an existing group.
 
         You must have ADMIN permissions within the group in order to do this.
@@ -358,15 +360,15 @@
 
     def add_user_to_group(self: Specklia, group_id: str, user_to_add_id: str) -> str:
         """
         Add a user to an existing group.
 
         You must have ADMIN permissions within the group in order to do this.
         The user will initially be granted READ_ONLY permissions within the group.
-        Use Specklia.set_user_privileges() to change this after you have moved them into the group.
+        Use Specklia.update_user_privileges() to change this after you have moved them into the group.
 
         Parameters
         ----------
         group_id: str
             The group's UUID
 
         user_to_add_id : str
@@ -380,17 +382,17 @@
         response = requests.post(self.server_url + "/groupmembership",
                                  json={'group_id': group_id, "user_to_add_id": user_to_add_id},
                                  headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
         _log.info('added user ID %s to group ID %s', user_to_add_id, group_id)
         return response.text.strip('\n"')
 
-    def set_user_privileges(self: Specklia, group_id: str, user_to_update_id: str, new_privileges: str) -> str:
+    def update_user_privileges(self: Specklia, group_id: str, user_to_update_id: str, new_privileges: str) -> str:
         """
-        Set a user's privileges within a particular group.
+        Update a user's privileges within a particular group.
 
         You must have ADMIN permissions within the group in order to do this.
 
         These privileges determine what a user can do with the datasets and users in the group:
         - READ_ONLY means that the user can read the datasets, but cannot write to them,
           or change properties of the group.
         - READ_WRITE means that the user can write to existing datasets as well as read from them,
@@ -400,15 +402,15 @@
           and can add and remove datasets from the group.
 
         Parameters
         ----------
         group_id : str
             The group's UUID
         user_to_update_id : str
-            UUID of user to set privileges for
+            UUID of user to update privileges for
         new_privileges : str
             New privileges of the users. Must be 'READ_ONLY', 'READ_WRITE' or 'ADMIN'.
 
         Returns
         -------
         str
             Response from server
@@ -416,15 +418,16 @@
         response = requests.put(
             self.server_url + "/groupmembership",
             json={'group_id': group_id,
                   "user_to_update_id": user_to_update_id,
                   'new_privileges': new_privileges},
             headers={"Authorization": "Bearer " + self.auth_token})
         _check_response_ok(response)
-        _log.info('Set user ID %s privileges to %s within group ID %s.', user_to_update_id, new_privileges, group_id)
+        _log.info('Updated user ID %s privileges to %s within group ID %s.',
+                  user_to_update_id, new_privileges, group_id)
         return response.text.strip('\n"')
 
     def delete_user_from_group(self: Specklia, group_id: str, user_to_delete_id: str,) -> str:
         """
         Remove a user from an existing group.
 
         You must have ADMIN permissions within the group in order to do this.
```

### Comparing `specklia-1.1.4/specklia/websocket_helpers.py` & `specklia-1.1.5/specklia/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.4/specklia.egg-info/PKG-INFO` & `specklia-1.1.5/specklia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.4/tests/test_client.py` & `specklia-1.1.5/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Unit tests for the Specklia Client."""
 from datetime import datetime
 from http import HTTPStatus
 from typing import Dict
-from unittest.mock import call, MagicMock, patch
+from unittest.mock import call
+from unittest.mock import MagicMock
+from unittest.mock import patch
 
 import geopandas as gpd
 import pytest
-from shapely import Point, Polygon
+from shapely import Point
+from shapely import Polygon
 
 from specklia import Specklia
 
 
 @pytest.fixture()
 def example_geodataframe() -> gpd.GeoDataFrame:
     return gpd.GeoDataFrame({
@@ -40,36 +43,36 @@
     patched_requests_with_response['response'].json.return_value = [{'name': 'fred', 'email': 'fred@fred.fred'}]
     test_client.list_users(group_id='hazbin')
     patched_requests_with_response['requests'].get.assert_has_calls([
         call('https://localhost/users', headers={'Authorization': 'Bearer fake_token'},
              params={"group_id": "hazbin"})])
 
 
-def test_ingest_data(test_client: Specklia, example_geodataframe: gpd.GeoDataFrame):
+def test_add_points_to_dataset(test_client: Specklia, example_geodataframe: gpd.GeoDataFrame):
     with (patch('specklia.client.simple_websocket') as mock_simple_websocket,
             patch('specklia.client.websocket_helpers') as mock_websocket_helpers):
         mock_client = MagicMock(name="mock_client")
         mock_simple_websocket.Client.return_value = mock_client
         mock_websocket_helpers.receive_object_from_websocket.return_value = {'status': HTTPStatus.OK}
-        test_client.ingest(
+        test_client.add_points_to_dataset(
             dataset_id='dummy_dataset', new_points=example_geodataframe, source_description={'reference': 'cheese'})
 
         mock_websocket_helpers.send_object_to_websocket.assert_called_with(
             mock_client, {
                 'dataset_id': 'dummy_dataset', 'gdf': example_geodataframe, 'source': {'reference': 'cheese'}})
 
 
-def test_query_data(test_client: Specklia):
+def test_query_dataset(test_client: Specklia):
     with (patch('specklia.client.simple_websocket') as mock_simple_websocket,
             patch('specklia.client.websocket_helpers') as mock_websocket_helpers):
         mock_client = MagicMock(name="mock_client")
         mock_simple_websocket.Client.return_value = mock_client
         mock_websocket_helpers.receive_object_from_websocket.return_value = {
             'status': HTTPStatus.OK, 'gdf': 'dummy', 'sources': {}}
-        test_client.query(
+        test_client.query_dataset(
             dataset_id='dummy_dataset',
             epsg4326_polygon=Polygon(((0, 0), (0, 1), (1, 1), (0, 0))),
             min_datetime=datetime(2020, 5, 6),
             max_datetime=datetime(2020, 5, 10),
             columns_to_return=['lat', 'lon'],
             additional_filters=[
                 {'column': 'cheese', 'operator': '<', 'threshold': 6.57},
@@ -97,16 +100,16 @@
     Specklia(url='https://localhost', auth_token='fake_token').create_group("ducks")
     patched_requests_with_response['requests'].post.assert_has_calls([
         call('https://localhost/groups',
              json={"group_name": "ducks"},
              headers={'Authorization': 'Bearer fake_token'})])
 
 
-def test_change_group_name(patched_requests_with_response: Dict[str, MagicMock]):
-    Specklia(url='https://localhost', auth_token='fake_token').change_group_name(
+def test_update_group_name(patched_requests_with_response: Dict[str, MagicMock]):
+    Specklia(url='https://localhost', auth_token='fake_token').update_group_name(
         group_id="ducks",
         new_group_name="pigeons")
     patched_requests_with_response['requests'].put.assert_has_calls([
         call('https://localhost/groups',
              json={"group_id": "ducks", "new_group_name": "pigeons"},
              headers={'Authorization': 'Bearer fake_token'})])
 
@@ -130,18 +133,18 @@
                                                                                  user_to_add_id='donald')
     patched_requests_with_response['requests'].post.assert_has_calls([
         call('https://localhost/groupmembership',
              json={"group_id": "ducks", "user_to_add_id": "donald"},
              headers={'Authorization': 'Bearer fake_token'})])
 
 
-def test_set_user_privileges(patched_requests_with_response: Dict[str, MagicMock]):
-    Specklia(url='https://localhost', auth_token='fake_token').set_user_privileges(group_id="ducks",
-                                                                                   user_to_update_id="donald",
-                                                                                   new_privileges="ADMIN")
+def test_update_user_privileges(patched_requests_with_response: Dict[str, MagicMock]):
+    Specklia(url='https://localhost', auth_token='fake_token').update_user_privileges(group_id="ducks",
+                                                                                      user_to_update_id="donald",
+                                                                                      new_privileges="ADMIN")
     patched_requests_with_response['requests'].put.assert_has_calls([
         call('https://localhost/groupmembership',
              json={"group_id": "ducks", "user_to_update_id": "donald", "new_privileges": "ADMIN"},
              headers={'Authorization': 'Bearer fake_token'})])
 
 
 def test_delete_user_from_group(patched_requests_with_response: Dict[str, MagicMock]):
```

### Comparing `specklia-1.1.4/tests/test_websocket_helpers.py` & `specklia-1.1.5/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

