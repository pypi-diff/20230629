# Comparing `tmp/wf_process_cuwb_data-1.8.0.tar.gz` & `tmp/wf_process_cuwb_data-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_process_cuwb_data-1.8.0.tar", max compression
+gzip compressed data, was "wf_process_cuwb_data-1.9.0.tar", max compression
```

## Comparing `wf_process_cuwb_data-1.8.0.tar` & `wf_process_cuwb_data-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1088 2021-11-26 03:56:53.131426 wf_process_cuwb_data-1.8.0/LICENSE
--rw-r--r--   0        0        0     6733 2023-01-27 22:57:57.201897 wf_process_cuwb_data-1.8.0/README.md
--rw-r--r--   0        0        0      147 2023-01-31 16:50:05.088330 wf_process_cuwb_data-1.8.0/process_cuwb_data/__init__.py
--rw-r--r--   0        0        0      215 2021-11-26 03:56:53.131988 wf_process_cuwb_data-1.8.0/process_cuwb_data/__main__.py
--rw-r--r--   0        0        0     3244 2023-01-31 17:20:07.893012 wf_process_cuwb_data-1.8.0/process_cuwb_data/camera_helper.py
--rw-r--r--   0        0        0     7502 2023-01-31 17:25:23.814777 wf_process_cuwb_data-1.8.0/process_cuwb_data/camera_uwb_line_of_sight.py
--rw-r--r--   0        0        0    29636 2023-02-22 21:26:12.312916 wf_process_cuwb_data-1.8.0/process_cuwb_data/cli.py
--rw-r--r--   0        0        0    24963 2023-02-22 21:26:12.313142 wf_process_cuwb_data-1.8.0/process_cuwb_data/core.py
--rw-r--r--   0        0        0       98 2021-11-26 03:56:53.132545 wf_process_cuwb_data-1.8.0/process_cuwb_data/filters/__init__.py
--rw-r--r--   0        0        0      246 2021-11-26 03:56:53.132630 wf_process_cuwb_data-1.8.0/process_cuwb_data/filters/butter.py
--rw-r--r--   0        0        0      279 2021-11-26 03:56:53.132713 wf_process_cuwb_data-1.8.0/process_cuwb_data/filters/filt_filt.py
--rw-r--r--   0        0        0      387 2021-11-26 03:56:53.132799 wf_process_cuwb_data-1.8.0/process_cuwb_data/filters/savgol.py
--rw-r--r--   0        0        0      401 2023-01-27 18:17:19.452432 wf_process_cuwb_data-1.8.0/process_cuwb_data/filters/sos_filt_filt.py
--rw-r--r--   0        0        0     8667 2023-02-03 18:58:25.834083 wf_process_cuwb_data-1.8.0/process_cuwb_data/geom_render.py
--rw-r--r--   0        0        0     1487 2023-01-31 16:55:15.939791 wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_imu_data.py
--rw-r--r--   0        0        0     3071 2023-01-31 17:09:50.206521 wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_pose_data.py
--rw-r--r--   0        0        0       22 2023-01-27 18:17:19.453424 wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_service/__init__.py
--rw-r--r--   0        0        0     3408 2023-02-22 21:26:12.313317 wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_service/client.py
--rw-r--r--   0        0        0    30921 2023-02-22 21:26:12.313531 wf_process_cuwb_data-1.8.0/process_cuwb_data/parse_events.py
--rw-r--r--   0        0        0        0 2021-11-26 03:56:53.133594 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/__init__.py
--rw-r--r--   0        0        0     1413 2023-01-27 18:17:19.454645 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/case_insensitive_enum.py
--rw-r--r--   0        0        0       60 2023-02-22 21:26:12.313653 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/const.py
--rw-r--r--   0        0        0     5087 2023-02-22 21:26:12.313799 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/io.py
--rw-r--r--   0        0        0     1451 2023-01-31 16:49:48.811312 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/log.py
--rw-r--r--   0        0        0     1209 2023-01-31 16:59:03.644325 wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/util.py
--rw-r--r--   0        0        0     2568 2023-01-31 17:19:59.116920 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_extract_data.py
--rw-r--r--   0        0        0     8092 2023-01-31 17:33:14.865301 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_human_activity.py
--rw-r--r--   0        0        0     6796 2023-01-31 17:33:14.737881 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_random_forest.py
--rw-r--r--   0        0        0     8458 2023-01-31 17:33:14.899433 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_tray_carry.py
--rw-r--r--   0        0        0      184 2023-01-27 18:17:19.462717 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_enum_carry_categories.py
--rw-r--r--   0        0        0      196 2023-01-27 18:17:19.462954 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_enum_groundtruth_data_source.py
--rw-r--r--   0        0        0      428 2023-01-27 18:17:19.463173 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_enum_human_activities.py
--rw-r--r--   0        0        0      422 2023-01-27 18:17:19.463393 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_enum_interaction_types.py
--rw-r--r--   0        0        0     4546 2023-01-31 17:24:47.486123 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_events.py
--rw-r--r--   0        0        0    36381 2023-02-22 21:26:12.314025 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_features.py
--rw-r--r--   0        0        0     7977 2023-01-27 18:17:19.464876 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_filters.py
--rw-r--r--   0        0        0     4067 2023-01-31 16:55:15.988058 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_ground_truth.py
--rw-r--r--   0        0        0    44313 2023-02-22 21:26:12.314300 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_tray_interactions.py
--rw-r--r--   0        0        0    10361 2023-01-31 16:55:16.026611 wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_predict_tray_centroids.py
--rw-r--r--   0        0        0    31640 2023-01-31 17:42:22.470104 wf_process_cuwb_data-1.8.0/process_cuwb_data/visualize.py
--rw-r--r--   0        0        0     1471 2023-02-22 21:26:19.522976 wf_process_cuwb_data-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     8378 1970-01-01 00:00:00.000000 wf_process_cuwb_data-1.8.0/setup.py
--rw-r--r--   0        0        0     8367 1970-01-01 00:00:00.000000 wf_process_cuwb_data-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2021-11-26 03:56:53.131426 wf_process_cuwb_data-1.9.0/LICENSE
+-rw-r--r--   0        0        0     6733 2023-01-27 22:57:57.201897 wf_process_cuwb_data-1.9.0/README.md
+-rw-r--r--   0        0        0      147 2023-01-31 16:50:05.088330 wf_process_cuwb_data-1.9.0/process_cuwb_data/__init__.py
+-rw-r--r--   0        0        0      215 2021-11-26 03:56:53.131988 wf_process_cuwb_data-1.9.0/process_cuwb_data/__main__.py
+-rw-r--r--   0        0        0     3244 2023-01-31 17:20:07.893012 wf_process_cuwb_data-1.9.0/process_cuwb_data/camera_helper.py
+-rw-r--r--   0        0        0     7898 2023-06-29 21:55:32.898889 wf_process_cuwb_data-1.9.0/process_cuwb_data/camera_uwb_line_of_sight.py
+-rw-r--r--   0        0        0    29636 2023-02-22 21:26:12.312916 wf_process_cuwb_data-1.9.0/process_cuwb_data/cli.py
+-rw-r--r--   0        0        0    24963 2023-02-22 21:26:12.313142 wf_process_cuwb_data-1.9.0/process_cuwb_data/core.py
+-rw-r--r--   0        0        0       98 2021-11-26 03:56:53.132545 wf_process_cuwb_data-1.9.0/process_cuwb_data/filters/__init__.py
+-rw-r--r--   0        0        0      246 2021-11-26 03:56:53.132630 wf_process_cuwb_data-1.9.0/process_cuwb_data/filters/butter.py
+-rw-r--r--   0        0        0      279 2021-11-26 03:56:53.132713 wf_process_cuwb_data-1.9.0/process_cuwb_data/filters/filt_filt.py
+-rw-r--r--   0        0        0      387 2021-11-26 03:56:53.132799 wf_process_cuwb_data-1.9.0/process_cuwb_data/filters/savgol.py
+-rw-r--r--   0        0        0      401 2023-01-27 18:17:19.452432 wf_process_cuwb_data-1.9.0/process_cuwb_data/filters/sos_filt_filt.py
+-rw-r--r--   0        0        0     1777 2023-06-29 21:55:32.899035 wf_process_cuwb_data-1.9.0/process_cuwb_data/find_active_tags.py
+-rw-r--r--   0        0        0     8937 2023-06-29 21:55:32.899233 wf_process_cuwb_data-1.9.0/process_cuwb_data/geom_render.py
+-rw-r--r--   0        0        0     1510 2023-06-29 21:55:32.899406 wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_imu_data.py
+-rw-r--r--   0        0        0     3071 2023-01-31 17:09:50.206521 wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_pose_data.py
+-rw-r--r--   0        0        0       22 2023-01-27 18:17:19.453424 wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_service/__init__.py
+-rw-r--r--   0        0        0     3408 2023-02-22 21:26:12.313317 wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_service/client.py
+-rw-r--r--   0        0        0    30921 2023-02-22 21:26:12.313531 wf_process_cuwb_data-1.9.0/process_cuwb_data/parse_events.py
+-rw-r--r--   0        0        0        0 2021-11-26 03:56:53.133594 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/__init__.py
+-rw-r--r--   0        0        0     1413 2023-01-27 18:17:19.454645 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/case_insensitive_enum.py
+-rw-r--r--   0        0        0       60 2023-02-22 21:26:12.313653 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/const.py
+-rw-r--r--   0        0        0     5087 2023-02-22 21:26:12.313799 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/io.py
+-rw-r--r--   0        0        0     1894 2023-06-29 21:55:32.899576 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/log.py
+-rw-r--r--   0        0        0     1209 2023-01-31 16:59:03.644325 wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/util.py
+-rw-r--r--   0        0        0     2568 2023-01-31 17:19:59.116920 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_extract_data.py
+-rw-r--r--   0        0        0     8092 2023-01-31 17:33:14.865301 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_human_activity.py
+-rw-r--r--   0        0        0     6796 2023-01-31 17:33:14.737881 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_random_forest.py
+-rw-r--r--   0        0        0     8458 2023-01-31 17:33:14.899433 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_tray_carry.py
+-rw-r--r--   0        0        0      184 2023-01-27 18:17:19.462717 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_enum_carry_categories.py
+-rw-r--r--   0        0        0      196 2023-01-27 18:17:19.462954 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_enum_groundtruth_data_source.py
+-rw-r--r--   0        0        0      428 2023-01-27 18:17:19.463173 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_enum_human_activities.py
+-rw-r--r--   0        0        0      422 2023-01-27 18:17:19.463393 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_enum_interaction_types.py
+-rw-r--r--   0        0        0     4546 2023-01-31 17:24:47.486123 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_events.py
+-rw-r--r--   0        0        0    36381 2023-02-22 21:26:12.314025 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_features.py
+-rw-r--r--   0        0        0     7977 2023-01-27 18:17:19.464876 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_filters.py
+-rw-r--r--   0        0        0     4067 2023-01-31 16:55:15.988058 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_ground_truth.py
+-rw-r--r--   0        0        0    44453 2023-06-29 21:55:32.899865 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_tray_interactions.py
+-rw-r--r--   0        0        0    10361 2023-01-31 16:55:16.026611 wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_predict_tray_centroids.py
+-rw-r--r--   0        0        0    31640 2023-01-31 17:42:22.470104 wf_process_cuwb_data-1.9.0/process_cuwb_data/visualize.py
+-rw-r--r--   0        0        0     1518 2023-06-29 21:55:46.422124 wf_process_cuwb_data-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8447 1970-01-01 00:00:00.000000 wf_process_cuwb_data-1.9.0/PKG-INFO
```

### Comparing `wf_process_cuwb_data-1.8.0/LICENSE` & `wf_process_cuwb_data-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/README.md` & `wf_process_cuwb_data-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/camera_helper.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/camera_helper.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/camera_uwb_line_of_sight.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/camera_uwb_line_of_sight.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         default_camera_device_id,
         environment_id=None,
         environment_name=None,
         camera_device_ids=None,
         camera_calibrations=None,
         position_window_seconds=4,
         imputed_z_position=1.0,
+        df_cuwb_position_data=None,
         chunk_size=100,
         client=None,
         uri=None,
         token_uri=None,
         audience=None,
         client_id=None,
         client_secret=None,
@@ -54,29 +55,35 @@
         if camera_device_ids is None:
             camera_info = honeycomb_caching_client.fetch_camera_devices(
                 environment_id=environment_id, environment_name=environment_name, start=timestamp, end=timestamp
             )
             camera_device_ids = camera_info.index.unique().tolist()
         if camera_calibrations is None:
             camera_calibrations = honeycomb_caching_client.fetch_camera_calibrations(
-                camera_ids=camera_device_ids, start=timestamp, end=timestamp
+                camera_ids=tuple(camera_device_ids), start=timestamp, end=timestamp
             )
         position_window_start = timestamp - datetime.timedelta(seconds=position_window_seconds / 2)
         position_window_end = timestamp + datetime.timedelta(seconds=position_window_seconds / 2)
-        position_data = honeycomb_io.fetch_cuwb_position_data(
-            start=position_window_start,
-            end=position_window_end,
-            device_ids=[tag_device_id],
-            environment_id=None,
-            environment_name=None,
-            device_types=["UWBTAG"],
-            output_format="dataframe",
-            sort_arguments=None,
-            **client_params,
-        )
+        if df_cuwb_position_data is not None:
+            position_data = df_cuwb_position_data.loc[
+                (df_cuwb_position_data.index >= position_window_start)
+                & (df_cuwb_position_data.index <= position_window_end)
+            ]
+        else:
+            position_data = honeycomb_io.fetch_cuwb_position_data(
+                start=position_window_start,
+                end=position_window_end,
+                device_ids=[tag_device_id],
+                environment_id=None,
+                environment_name=None,
+                device_types=["UWBTAG"],
+                output_format="dataframe",
+                sort_arguments=None,
+                **client_params,
+            )
         if len(position_data) == 0:
             err = f"Unable to find position data between {position_window_start} and {position_window_end}, cannot determine best camera views"
             logger.warning(err)
             raise ValueError(err)
 
         position = np.nanmedian(position_data.loc[:, ["x", "y", "z"]].values, axis=0)
         if imputed_z_position is not None:
@@ -106,18 +113,18 @@
                 in_frame = True
                 distance_from_image_center = np.linalg.norm(
                     np.subtract(
                         image_position, [camera_calibration["image_width"] / 2, camera_calibration["image_height"] / 2]
                     )
                 )
                 in_middle = (
-                    image_position[0] > camera_calibration["image_width"] * (1.0 / 10.0)
-                    and image_position[0] < camera_calibration["image_width"] * (9.0 / 10.0)
-                    and image_position[1] > camera_calibration["image_height"] * (1.0 / 10.0)
-                    and image_position[1] < camera_calibration["image_height"] * (9.0 / 10.0)
+                    image_position[0] > camera_calibration["image_width"] * (3.5 / 10.0)
+                    and image_position[0] < camera_calibration["image_width"] * (6.5 / 10.0)
+                    and image_position[1] > camera_calibration["image_height"] * (2.0 / 10.0)
+                    and image_position[1] < camera_calibration["image_height"] * (8.0 / 10.0)
                 )
             else:
                 in_frame = False
                 distance_from_image_center = None
                 in_middle = False
             view_data_list.append(
                 {
@@ -127,15 +134,15 @@
                     "image_position": image_position,
                     "distance_from_image_center": distance_from_image_center,
                     "in_frame": in_frame,
                     "in_middle": in_middle,
                 }
             )
         df_view_data = pd.DataFrame(view_data_list).set_index("camera_device_id")
-        df_view_data = df_view_data.sort_values("distance_from_camera")
+        df_view_data = df_view_data.sort_values("distance_from_image_center")
         self.df_view_data = df_view_data
 
     def all_camera_views(self):
         return self.df_view_data
 
     def in_frame_camera_views(self):
         return self.df_view_data.loc[self.df_view_data["in_frame"]].sort_values("distance_from_camera")
@@ -148,31 +155,34 @@
         return self.df_view_data.loc[self.df_view_data["in_middle"]].sort_values("distance_from_camera")
 
     def all_in_middle_camera_views_device_ids(self):
         df_in_middle_views = self.in_middle_camera_views()
         return df_in_middle_views.index.to_list()
 
     def best_camera_view(self):
-        if not self.df_view_data["in_frame"].any():
+        if self.df_view_data["in_middle"].any():
+            best_camera_view = self.df_view_data.loc[self.df_view_data["in_middle"]]
+        elif self.df_view_data["in_frame"].any():
+            best_camera_view = self.df_view_data.loc[self.df_view_data["in_frame"]]
+        else:
             best_camera_view = pd.DataFrame(
                 [
                     {
                         "camera_device_id": self.default_camera_device_id,
                         "position": None,
                         "distance_from_camera": None,
                         "image_position": None,
                         "distance_from_image_center": None,
                         "in_frame": None,
                         "in_middle": None,
                     }
                 ]
             ).set_index(["camera_device_id"])
-        elif not self.df_view_data["in_middle"].any():
-            best_camera_view = self.df_view_data.sort_values("distance_from_image_center")
-        else:
-            best_camera_view = self.df_view_data.loc[self.df_view_data["in_middle"]]
 
-        return best_camera_view.sort_values("distance_from_camera").iloc[:1]
+        return best_camera_view.sort_values("distance_from_image_center").iloc[:1]
+
+    def test(self):
+        return True
 
     def best_camera_view_device_id(self):
         df_best_camera_view = self.best_camera_view()
         return df_best_camera_view.index[0]
```

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/cli.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/cli.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/core.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/core.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/geom_render.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/geom_render.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,31 @@
 from process_cuwb_data.uwb_motion_filters import TrayMotionButterFiltFiltFilter
 
 
 def fetch_geoms_2d(
     environment_name,
     start_time,
     end_time,
+    df_cuwb_position_data=None,
     z_axis_override=0.5,
     device_ids=None,
     smooth=False,
     frames_per_second=10.0,
     progress_bar=False,
     notebook=False,
 ):
     # Fetch CUWB position data
-    df_position = fetch_imu_data(imu_type="position", environment_name=environment_name, start=start_time, end=end_time)
-    if z_axis_override:
-        df_position["z"] = z_axis_override
+    if df_cuwb_position_data is not None:
+        df_position = df_cuwb_position_data.loc[
+            (df_cuwb_position_data.index >= start_time) & (df_cuwb_position_data.index <= end_time)
+        ]
+    else:
+        df_position = fetch_imu_data(
+            imu_type="position", environment_name=environment_name, start=start_time, end=end_time
+        )
 
     df_position = df_position[
         [
             "x",
             "y",
             "z",
             "assignment_id",
@@ -44,14 +50,17 @@
             "person_anonymized_short_name",
             "material_id",
             "material_assignment_id",
             "material_name",
         ]
     ]
 
+    if z_axis_override:
+        df_position["z"] = z_axis_override
+
     if device_ids:
         df_position = df_position[df_position["device_id"].isin(device_ids)]
 
     if smooth:
         position_filter = TrayMotionButterFiltFiltFilter(useSosFiltFilt=True)
         df_position_smoothed = pd.DataFrame(data=None, columns=df_position.columns)
         for device_id in df_position["device_id"].unique().tolist():
```

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_imu_data.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_imu_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     add_device_entity_assignment_info,
     add_tray_material_assignment_info,
 )
 
 from .utils.util import filter_entity_type
 
 
-def fetch_imu_data(imu_type, environment_name, start, end, entity_type="all"):
+def fetch_imu_data(imu_type, environment_name, start, end, device_ids=None, entity_type="all"):
     if imu_type == "position":
         fetch = fetch_cuwb_position_data
     elif imu_type == "accelerometer":
         fetch = fetch_cuwb_accelerometer_data
     elif imu_type == "gyroscope":
         fetch = fetch_cuwb_gyroscope_data
     elif imu_type == "magnetometer":
         fetch = fetch_cuwb_magnetometer_data
     else:
         raise ValueError(f"Unexpected IMU type: {imu_type}")
 
     df = fetch(
         start=start,
         end=end,
-        device_ids=None,
+        device_ids=device_ids,
         environment_id=None,
         environment_name=environment_name,
         device_types=["UWBTAG"],
         output_format="dataframe",
         sort_arguments={"field": "timestamp"},
         chunk_size=20000,
     )
```

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_pose_data.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_pose_data.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/honeycomb_service/client.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/honeycomb_service/client.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/parse_events.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/parse_events.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/case_insensitive_enum.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/case_insensitive_enum.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/io.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/io.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/log.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import logging
+import os
 import sys
 
 import pandas as pd
 
 
 class Logger:
     def __init__(self):
         self.set_pandas_output()
 
         formatter = logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
         stdout_handler = logging.StreamHandler(sys.stdout)
         stdout_handler.setLevel(logging.DEBUG)
         stdout_handler.setFormatter(formatter)
 
-        minimal_honeycomb = logging.getLogger("minimal_honeycomb")
-        minimal_honeycomb.setLevel(logging.DEBUG)
-        minimal_honeycomb.addHandler(stdout_handler)
-
-        minimal_honeycomb = logging.getLogger("honeycomb_io")
-        minimal_honeycomb.setLevel(logging.DEBUG)
-        minimal_honeycomb.addHandler(stdout_handler)
-
-        gqlpycgen = logging.getLogger("gqlpycgen")  # .client
-        gqlpycgen.setLevel(logging.DEBUG)
-        gqlpycgen.addHandler(stdout_handler)
-
-        g_logger = logging.getLogger("groundtruth_default_log")
-        g_logger.setLevel(logging.DEBUG)
-        g_logger.addHandler(stdout_handler)
+        if os.getenv("ENABLE_HONEYCOMB_LOGS", "false").lower() in ["true", "t"]:
+            honeycomb_logger = logging.getLogger("minimal_honeycomb")
+            honeycomb_logger.setLevel(logging.DEBUG)
+            honeycomb_logger.addHandler(stdout_handler)
+
+            honeycomb_logger = logging.getLogger("honeycomb_io")
+            honeycomb_logger.setLevel(logging.DEBUG)
+            honeycomb_logger.addHandler(stdout_handler)
+
+            gqlpycgen_logger = logging.getLogger("gqlpycgen")  # .client
+            gqlpycgen_logger.setLevel(logging.DEBUG)
+            gqlpycgen_logger.addHandler(stdout_handler)
+
+        if os.getenv("ENABLE_GEOM_RENDER_LOGS", "false").lower() in ["true", "t"]:
+            geom_render_core_logger = logging.getLogger("geom_render.core")
+            geom_render_core_logger.setLevel(logging.DEBUG)
+            geom_render_core_logger.addHandler(stdout_handler)
+
+        default_logger = logging.getLogger("process_cuwb_data")
+        default_logger.setLevel(logging.DEBUG)
+        default_logger.addHandler(stdout_handler)
 
-        self._logger = g_logger
+        self._logger = default_logger
 
     def set_pandas_output(self, max_rows=100, max_columns=None, width=None, max_colwidth=None):
         pd.set_option("display.max_rows", max_rows)
         pd.set_option("display.max_columns", max_columns)
         pd.set_option("display.width", width)
         pd.set_option("display.max_colwidth", max_colwidth)
```

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/utils/util.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/utils/util.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_extract_data.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_extract_data.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_human_activity.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_human_activity.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_random_forest.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_random_forest.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_classifier_tray_carry.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_classifier_tray_carry.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_events.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_events.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_features.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_features.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_filters.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_filters.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_ground_truth.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_ground_truth.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_motion_tray_interactions.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_motion_tray_interactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from functools import partial
 import multiprocessing
 import sys
 import time
 
 import numpy as np
 import pandas as pd
-from scipy.spatial.distance import cdist
+from torch import cdist
+
+# from scipy.spatial.distance import cdist
 
 from process_cuwb_data.utils.log import logger
 from process_cuwb_data.utils.util import dataframe_tuple_columns_to_underscores
 from process_cuwb_data.uwb_motion_enum_interaction_types import InteractionType
 
 
 # TODO: Ignoring z-axis when computing distance for now, reconsider after further testing CUWB anchors
@@ -213,32 +215,34 @@
             )
             sys.stdout.flush()
             v_start.value = time.time()
 
         v_count.value += 1
 
     if idx not in _df_people.index:
-        logger.warning(
-            f"No people tags at {idx}, cannot/will not try to compute distance coefficients between people and trays for this time instance"
-        )
+        # logger.debug(
+        #     f"No people tags at {idx}, cannot/will not try to compute distance coefficients between people and trays for this time instance"
+        # )
         return None
     df_people_by_idx = _df_people.loc[[idx]]
 
     if idx not in _df_trays.index:
-        logger.warning(
-            f"No tray tags at {idx}, cannot/will not try to compute distance coefficients between people and trays for this time instance"
-        )
+        # logger.debug(
+        #     f"No tray tags at {idx}, cannot/will not try to compute distance coefficients between people and trays for this time instance"
+        # )
         return None
     df_trays_by_idx = _df_trays.loc[[idx]]
 
     position_cols = map_column_name_to_dimension_space("position", DIMENSIONS_WHEN_COMPUTING_CHILD_TRAY_DISTANCE)
 
     df_people_and_trays = df_people_by_idx.join(df_trays_by_idx, how="inner", lsuffix="_person", rsuffix="_tray")
     distances = cdist(
-        df_people_by_idx[position_cols].to_numpy(), df_trays_by_idx[position_cols].to_numpy(), metric="euclidean"
+        # df_people_by_idx[position_cols].to_numpy(), df_trays_by_idx[position_cols].to_numpy(), metric="euclidean"
+        df_people_by_idx[position_cols].to_numpy(),
+        df_trays_by_idx[position_cols].to_numpy(),
     )
 
     return df_people_and_trays.assign(person_tray_distance=distances.flatten())
 
 
 def generate_person_tray_distances(df_people_features, df_tray_features):
     """
```

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/uwb_predict_tray_centroids.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/uwb_predict_tray_centroids.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/process_cuwb_data/visualize.py` & `wf_process_cuwb_data-1.9.0/process_cuwb_data/visualize.py`

 * *Files identical despite different names*

### Comparing `wf_process_cuwb_data-1.8.0/pyproject.toml` & `wf_process_cuwb_data-1.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
-name = "PROJECT_NAME"
+name = "wf-process-cuwb-data"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-process-cuwb-data"
-version = "1.8.0"
+version = "1.9.0"
 description = "Tools for reading, processing, and writing CUWB data"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/WildflowerSchools/wf-process-cuwb-data"
 license = "MIT"
 classifiers = [
     'Intended Audience :: Developers',
@@ -20,30 +20,32 @@
     { include = "process_cuwb_data" }
 ]
 
 [tool.poetry.dependencies]
 boto3 = "^1.17"
 click = "^8.0.0"
 click-log = "^0.4.0"
+deprecated = "^1.2.13"
 matplotlib = "^3.4.1"
-nocasedict = "^1.0.2"
+nocasedict = "^2.0.0"
 numpy = "^1.20.2"
 pandas = "^1.2.4"
+platformdirs = "^3.0.0"
 python = ">=3.8,<3.12"
-python-dotenv = "^0.21.0"
+python-dotenv = "^1.0.0"
 python-slugify = "^8.0.0"
+pyyaml = "^6.0"
+scikit-learn = "^1.2.2"
 scipy = "^1.6.3"
-scikit-learn = "^1.1.2"
 toml = "^0.10.2"
+torch = "^2.0.1"
 wf-honeycomb-io = "^2.0.0"
 wf-process-pose-data = "^6.2.0"
-pyyaml = "^6.0"
-wf-geom-render = "^0.4.0"
-platformdirs = "^3.0.0"
-deprecated = "^1.2.13"
+wf-geom-render = "^0.5.0"
+wf-video-io = "^3.4.0"
 
 [tool.poetry.scripts]
 process_cuwb_data = "process_cuwb_data.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 pylint = "^2.15.0"
```

### Comparing `wf_process_cuwb_data-1.8.0/PKG-INFO` & `wf_process_cuwb_data-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-process-cuwb-data
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tools for reading, processing, and writing CUWB data
 Home-page: https://github.com/WildflowerSchools/wf-process-cuwb-data
 License: MIT
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
@@ -17,27 +17,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.17,<2.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
-Requires-Dist: nocasedict (>=1.0.2,<2.0.0)
+Requires-Dist: nocasedict (>=2.0.0,<3.0.0)
 Requires-Dist: numpy (>=1.20.2,<2.0.0)
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
 Requires-Dist: platformdirs (>=3.0.0,<4.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.0,<9.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.6.3,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: wf-geom-render (>=0.4.0,<0.5.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: wf-geom-render (>=0.5.0,<0.6.0)
 Requires-Dist: wf-honeycomb-io (>=2.0.0,<3.0.0)
 Requires-Dist: wf-process-pose-data (>=6.2.0,<7.0.0)
+Requires-Dist: wf-video-io (>=3.4.0,<4.0.0)
 Project-URL: Repository, https://github.com/WildflowerSchools/wf-process-cuwb-data
 Description-Content-Type: text/markdown
 
 # process_cuwb_data
 
 Tools for reading, processing, and writing CUWB data
```

