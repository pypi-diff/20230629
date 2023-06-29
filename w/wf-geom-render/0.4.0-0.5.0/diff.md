# Comparing `tmp/wf_geom_render-0.4.0.tar.gz` & `tmp/wf_geom_render-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_geom_render-0.4.0.tar", max compression
+gzip compressed data, was "wf_geom_render-0.5.0.tar", max compression
```

## Comparing `wf_geom_render-0.4.0.tar` & `wf_geom_render-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2022-12-08 20:29:18.948326 wf_geom_render-0.4.0/LICENSE
--rw-r--r--   0        0        0       64 2022-12-08 20:29:18.948326 wf_geom_render-0.4.0/README.md
--rw-r--r--   0        0        0       31 2022-12-08 20:29:18.948326 wf_geom_render-0.4.0/geom_render/__init__.py
--rw-r--r--   0        0        0    38499 2023-02-03 19:52:42.045670 wf_geom_render-0.4.0/geom_render/core.py
--rw-r--r--   0        0        0      903 2023-02-03 19:52:42.045670 wf_geom_render-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 wf_geom_render-0.4.0/setup.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 wf_geom_render-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-11-16 17:49:10.220553 wf_geom_render-0.5.0/LICENSE
+-rw-r--r--   0        0        0       64 2022-11-16 17:49:10.220703 wf_geom_render-0.5.0/README.md
+-rw-r--r--   0        0        0       31 2022-11-16 17:49:10.220929 wf_geom_render-0.5.0/geom_render/__init__.py
+-rw-r--r--   0        0        0    39560 2023-06-29 21:41:40.701203 wf_geom_render-0.5.0/geom_render/core.py
+-rw-r--r--   0        0        0      918 2023-06-29 21:40:08.843075 wf_geom_render-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 wf_geom_render-0.5.0/setup.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 wf_geom_render-0.5.0/PKG-INFO
```

### Comparing `wf_geom_render-0.4.0/LICENSE` & `wf_geom_render-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_geom_render-0.4.0/geom_render/core.py` & `wf_geom_render-0.5.0/geom_render/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,20 +56,15 @@
                 coordinates = np.array(coordinates)
             except:
                 raise ValueError("Coordinates for geom must be array-like")
             if coordinates.ndim > 3:
                 raise ValueError("Coordinates for geom must be of dimension 3 or less")
             while coordinates.ndim < 3:
                 coordinates = np.expand_dims(coordinates, axis=0)
-        if (
-            time_index is not None
-            and start_time is None
-            and frames_per_second is None
-            and num_frames is None
-        ):
+        if time_index is not None:
             # Ragged time index
             try:
                 time_index = np.array(time_index)
             except:
                 raise ValueError("Time index must be array-like")
             if time_index.ndim != 1:
                 raise ValueError("Time index must be one-dimensional")
@@ -138,43 +133,29 @@
                 num_points,
                 process_time_elapsed,
                 10**6 * process_time_elapsed / num_points,
             )
         )
         return json_output
 
-    def get_time_slice(self, index):
-        new_geom = copy.deepcopy(self)
-        new_geom.coordinates = np.expand_dims(self.coordinates[index], axis=0)
-        new_geom.time_index = None
-        new_geom.start_time = None
-        new_geom.frames_per_second = None
-        new_geom.num_frames = None
-        return new_geom
-
     def resample(
         self,
         new_time_index=None,
         new_start_time=None,
         new_frames_per_second=None,
         new_num_frames=None,
         method="interpolate",
         progress_bar=False,
         notebook=False,
     ):
         if method not in ["interpolate", "fill"]:
             raise ValueError(
                 "Available resampling methods are 'interpolate' and 'fill'"
             )
-        if (
-            new_time_index is not None
-            and new_start_time is None
-            and new_frames_per_second is None
-            and new_num_frames is None
-        ):
+        if new_time_index is not None:
             # New ragged time index
             try:
                 new_time_index = np.array(new_time_index)
             except:
                 raise ValueError("New time index must be array-like")
             if new_time_index.ndim != 1:
                 raise ValueError("New time index must be one-dimensional")
@@ -227,20 +208,15 @@
             old_time_between_frames = datetime.timedelta(
                 microseconds=int(round(10**6 / self.frames_per_second))
             )
             old_time_index = [
                 self.start_time + i * old_time_between_frames
                 for i in range(self.num_frames)
             ]
-        elif (
-            self.time_index is not None
-            and self.start_time is None
-            and self.frames_per_second is None
-            and self.num_frames is None
-        ):
+        elif self.time_index is not None:
             old_time_index = self.time_index
         else:
             raise ValueError(
                 "Current time index is malformed. Must include time index or all of start time/fps/number of frames or neither."
             )
         coordinates_time_slice_shape = self.coordinates.shape[1:]
         new_coordinates_shape = (
@@ -305,47 +281,44 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if self.coordinates is not None and self.coordinates.shape[-1] != 2:
             raise ValueError("For 2D geoms, size of last dimension must be 2")
 
     def plot_matplotlib(
         self,
+        frame_index,
         image_size=None,
         background_image=None,
         background_alpha=None,
         show_axes=True,
         show=True,
     ):
         if image_size is None and background_image is not None:
             image_size = np.array(
                 [background_image.shape[1], background_image.shape[0]]
             )
         fig, axes = plt.subplots()
-        self.draw_matplotlib(axes)
+        self.draw_matplotlib(axes, frame_index)
         cv_utils.format_2d_image_plot(image_size, show_axes)
         if background_image is not None:
             cv_utils.draw_background_image(background_image, background_alpha)
         if show:
             plt.show()
 
     def overlay_video(
         self,
         input_path,
         output_path,
         start_time=None,
+        include_timestamp=False,
         progress_bar=False,
         notebook=False,
     ):
         video_input = cv_utils.VideoInput(input_path=input_path, start_time=start_time)
-        if (
-            self.time_index is not None
-            or self.start_time is not None
-            or self.frames_per_second is not None
-            or self.num_frames is not None
-        ):
+        if self.time_index is not None:
             video_start_time = video_input.video_parameters.start_time
             video_fps = video_input.video_parameters.fps
             video_frame_count = video_input.video_parameters.frame_count
             if (
                 video_start_time is None
                 or video_fps is None
                 or video_frame_count is None
@@ -367,16 +340,21 @@
                 if frame is None:
                     raise ValueError(
                         "Input video ended unexpectedly at frame number {}".format(
                             frame_index
                         )
                     )
                 if frame_index < self.time_index.shape[0]:
-                    overlay_geom = self.get_time_slice(frame_index)
-                    frame = overlay_geom.draw_opencv(frame)
+                    frame = self.draw_opencv(image=frame, frame_index=frame_index)
+                    if include_timestamp:
+                        frame = cv_utils.draw_timestamp(
+                            original_image=frame,
+                            timestamp=self.time_index[frame_index],
+                            box_alpha=0.6,
+                        )
                 video_output.write_frame(frame)
                 if progress_bar:
                     t.update()
         else:
             video_output = cv_utils.VideoOutput(
                 output_path, video_parameters=video_input.video_parameters
             )
@@ -388,15 +366,15 @@
                 else:
                     t = tqdm.tqdm(total=video_input.video_parameters.frame_count)
             frame_count_stream = 0
             while video_input.is_opened():
                 frame = video_input.get_frame()
                 if frame is not None:
                     frame_count_stream += 1
-                    frame = self.draw_opencv(frame)
+                    frame = self.draw_opencv(frame, frame_index=frame_count_stream)
                     video_output.write_frame(frame)
                     if progress_bar:
                         t.update()
                 else:
                     break
             if video_input.video_parameters.frame_count is not None and int(
                 frame_count_stream
@@ -437,14 +415,21 @@
             )
         )
         process_start_time = time.time()
         image_corners = None
         if frame_width is not None and frame_height is not None:
             image_corners = [[0, 0], [frame_width, frame_height]]
 
+        logger.info(f"Coord: {self.coordinates.reshape((-1, 3))}")
+        logger.info(f"RV: {rotation_vector}")
+        logger.info(f"TV: {translation_vector}")
+        logger.info(f"CM: {camera_matrix}")
+        logger.info(f"DC: {distortion_coefficients}")
+        logger.info(f"IC: {image_corners}")
+
         new_coordinates_flattened = cv_utils.project_points(
             self.coordinates.reshape((-1, 3)),
             rotation_vector,
             translation_vector,
             camera_matrix,
             distortion_coefficients,
             remove_behind_camera=True,
@@ -508,20 +493,15 @@
                 raise ValueError(
                     "All geoms in list must have the same frame width (if specified)"
                 )
             if geom.frame_height is not None and geom.frame_height != frame_height:
                 raise ValueError(
                     "All geoms in list must have the same frame height (if specified)"
                 )
-            if (
-                geom.time_index is not None
-                and geom.start_time is None
-                and geom.frames_per_second is None
-                and geom.num_frames is None
-            ):
+            if geom.time_index is not None:
                 this_geom_timestamp_set = geom.time_index
                 new_timestamp_set = new_timestamp_set.union(this_geom_timestamp_set)
             elif (
                 geom.time_index is None
                 and geom.start_time is not None
                 and geom.frames_per_second is not None
                 and geom.num_frames is not None
@@ -547,94 +527,100 @@
                     "One of the geoms in the list has a malformed time index. Must include time index or all of start time/fps/number of frames or neither"
                 )
 
             new_num_points += geom.coordinates.shape[1]
             new_time_indexes.append(this_geom_timestamp_set)
 
         new_calculated_num_frames = len(rounded_time_index)
-        new_time_index = None
-
-        new_start_time = None
-        new_frames_per_second = None
-        new_num_frames = None
         new_coordinates = np.full(
             (new_calculated_num_frames, new_num_points, num_spatial_dimensions), np.nan
         )
         new_geom_list = list()
         new_coordinates_point_index = 0
         if progress_bar:
             if notebook:
                 geom_list = tqdm.tqdm_notebook(geom_list)
             else:
                 geom_list = tqdm.tqdm(geom_list)
         for idx, geom in enumerate(geom_list):
             all_timestamps_list = list(
                 set(rounded_time_index).union(new_time_indexes[idx])
             )
-            all_timestamps_series = pd.Series(
-                all_timestamps_list, index=all_timestamps_list, name="coordinates"
-            )
-
-            def map_timestamp_to_coordinates(timestamp):
-                coordinates = geom.coordinates[np.where(geom.time_index == timestamp)]
-                if len(coordinates) > 0:
-                    return coordinates[0].reshape((3,))
-                else:
-                    return np.full((3,), np.nan)
 
-            timestamps_mapped_to_coordinates = all_timestamps_series.map(
-                map_timestamp_to_coordinates
-            ).sort_index(ascending=True)
+            all_timestamps_mapped_to_nan = pd.Series(
+                np.full(
+                    (
+                        len(all_timestamps_list),
+                        3,
+                    ),
+                    np.nan,
+                ).tolist(),
+                index=all_timestamps_list,
+            )
+            geom_timestamps_mapped_to_coordinates = pd.Series(
+                geom.coordinates.reshape(
+                    (
+                        len(geom.time_index),
+                        3,
+                    )
+                ).tolist(),
+                index=geom.time_index,
+            )
+            all_timestamps_mapped_to_coordinates = (
+                geom_timestamps_mapped_to_coordinates.combine_first(
+                    all_timestamps_mapped_to_nan
+                ).sort_index(ascending=True)
+            )
 
             df_coordinates = pd.DataFrame(
-                np.array(timestamps_mapped_to_coordinates.to_list()),
-                index=timestamps_mapped_to_coordinates.index,
+                np.array(all_timestamps_mapped_to_coordinates.to_list()),
+                index=all_timestamps_mapped_to_coordinates.index,
                 columns=["x", "y", "z"],
             )
             df_coordinates = df_coordinates.interpolate(
                 method="time", limit=10, limit_direction="both"
             )
-            df_coordinates = df_coordinates.drop(index=new_time_indexes[idx])
+            df_coordinates = df_coordinates[
+                df_coordinates.index.isin(rounded_time_index)
+            ]
             np_new_coordinates = df_coordinates.to_numpy().reshape(
                 (len(df_coordinates), 1, 3)
             )
 
             new_geom = copy.deepcopy(geom)
             new_geom.time_index = df_coordinates.index.to_numpy()
-            new_geom.start_time = new_start_time
-            new_geom.frames_per_second = new_frames_per_second
-            new_geom.num_frames = new_num_frames
+            new_geom.start_time = start_time
+            new_geom.frames_per_second = frames_per_second
+            new_geom.frame_width = frame_width
+            new_geom.frame_height = frame_height
+            new_geom.num_frames = np_new_coordinates.shape[0]
             new_geom.coordinates = np_new_coordinates
 
             num_points = new_geom.coordinates.shape[1]
             new_coordinates[
                 :,
                 new_coordinates_point_index : (
                     new_coordinates_point_index + num_points
                 ),
                 :,
             ] = new_geom.coordinates
 
             if isinstance(geom, GeomCollection):
                 for sub_geom in geom.geom_list:
                     new_sub_geom = copy.deepcopy(sub_geom)
-                    new_sub_geom.time_index = rounded_time_index
+                    new_sub_geom.time_index = new_geom.time_index
+                    new_sub_geom.start_time = new_geom.start_time
+                    new_sub_geom.frames_per_second = new_geom.frames_per_second
+                    new_sub_geom.num_frames = new_geom.num_frames
                     new_sub_geom.coordinate_indices = [
                         coordinate_index + new_coordinates_point_index
                         for coordinate_index in new_sub_geom.coordinate_indices
                     ]
                     new_geom_list.append(new_sub_geom)
             else:
-                new_geom.coordinates = None
-                new_geom.time_index = None
-                new_geom.start_time = None
-                new_geom.frames_per_second = None
-                new_geom.num_frames = None
-                new_geom.frame_width = None
-                new_geom.frame_height = None
                 new_geom.coordinate_indices = [
                     coordinate_index + new_coordinates_point_index
                     for coordinate_index in range(num_points)
                 ]
                 new_geom_list.append(new_geom)
 
             new_coordinates_point_index += num_points
@@ -694,27 +680,24 @@
         self.vertical_alignment = vertical_alignment
 
 
 class GeomCollection2D(Geom2D, GeomCollection):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def draw_matplotlib(self, axis):
+    def draw_matplotlib(self, axis, frame_index):
         for geom_index, geom in enumerate(self.geom_list):
-            geom.coordinates = self.coordinates.take(
-                geom.coordinate_indices, 1
-            )
-            geom.draw_matplotlib(axis)
+            geom.coordinates = self.coordinates.take(geom.coordinate_indices, 1)
+            geom.draw_matplotlib(axis, frame_index)
 
-    def draw_opencv(self, image):
-        new_image = image.copy()
+    def draw_opencv(self, image, frame_index):
         for geom_index, geom in enumerate(self.geom_list):
             geom.coordinates = self.coordinates.take(geom.coordinate_indices, 1)
-            new_image = geom.draw_opencv(new_image)
-        return new_image
+            image = geom.draw_opencv(image, frame_index)
+        return image
 
 
 class GeomCollection3D(Geom3D, GeomCollection):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def project(
@@ -735,18 +718,20 @@
                 distortion_coefficients=distortion_coefficients,
                 frame_width=frame_width,
                 frame_height=frame_height,
             )
 
         new_geom_list = [
             geom.project(
-                rotation_vector,
-                translation_vector,
-                camera_matrix,
-                distortion_coefficients,
+                rotation_vector=rotation_vector,
+                translation_vector=translation_vector,
+                camera_matrix=camera_matrix,
+                distortion_coefficients=distortion_coefficients,
+                frame_width=frame_width,
+                frame_height=frame_height,
             )
             for geom in self.geom_list
         ]
         return GeomCollection2D(
             coordinates=new_coordinates,
             geom_list=new_geom_list,
             time_index=self.time_index,
@@ -758,44 +743,54 @@
         )
 
 
 class Circle2D(Geom2D, Circle):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def draw_matplotlib(self, axis):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_matplotlib(self, axis, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Circle2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Circle2D requires coordinates to be of shape (N, 1, 2)"
             )
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
+            return
+
         axis.add_artist(
             plt.Circle(
-                xy=self.coordinates[0, 0, :],
+                xy=coordinates,
                 radius=self.radius,
                 linewidth=self.line_width,
                 edgecolor=self.color,
                 fill=self.fill,
                 facecolor=self.color,
                 alpha=self.alpha,
             )
         )
 
-    def draw_opencv(self, image):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_opencv(self, image, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Circle2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Circle2D requires coordinates to be of shape (N, 1, 2)"
             )
-        if np.any(np.isnan(self.coordinates)):
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
             return image
+
         new_image = cv_utils.draw_circle(
             image,
-            coordinates=self.coordinates[0, 0],
+            coordinates=coordinates,
             radius=self.radius,
             line_width=self.line_width,
-            color=self.line_color,
+            color=self.color,
             fill=self.fill,
             alpha=self.alpha,
         )
         return new_image
 
 
 class Circle3D(Geom3D, Circle):
@@ -810,18 +805,20 @@
         distortion_coefficients,
         frame_width=None,
         frame_height=None,
     ):
         new_coordinates = None
         if self.coordinates is not None:
             new_coordinates = self.project_coordinates(
-                rotation_vector,
-                translation_vector,
-                camera_matrix,
-                distortion_coefficients,
+                rotation_vector=rotation_vector,
+                translation_vector=translation_vector,
+                camera_matrix=camera_matrix,
+                distortion_coefficients=distortion_coefficients,
+                frame_width=frame_width,
+                frame_height=frame_height,
             )
         return Circle2D(
             coordinates=new_coordinates,
             coordinate_indices=self.coordinate_indices,
             time_index=self.time_index,
             start_time=self.start_time,
             frames_per_second=self.frames_per_second,
@@ -843,42 +840,52 @@
         )
 
 
 class Point2D(Geom2D, Point):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def draw_matplotlib(self, axis):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_matplotlib(self, axis, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Point2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Point2D requires coordinates to be of shape (N, 1, 2)"
             )
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
+            return
+
         s = None
         if self.size is not None:
             s = self.size**2
         axis.scatter(
-            self.coordinates[0, 0, 0],
-            self.coordinates[0, 0, 1],
+            coordinates[0],
+            coordinates[1],
             marker=self.marker,
             s=s,
             edgecolors=self.color,
             color=self.color,
             alpha=self.alpha,
         )
 
-    def draw_opencv(self, image):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_opencv(self, image, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Point2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Point2D requires coordinates to be of shape (N, 1, 2)"
             )
-        if np.any(np.isnan(self.coordinates)):
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
             return image
+
         new_image = cv_utils.draw_point(
             image,
-            coordinates=self.coordinates[0, 0],
+            coordinates=coordinates,
             marker=self.marker,
             marker_size=self.size,
             color=self.color,
             alpha=self.alpha,
         )
         return new_image
 
@@ -895,18 +902,20 @@
         distortion_coefficients,
         frame_width=None,
         frame_height=None,
     ):
         new_coordinates = None
         if self.coordinates is not None:
             new_coordinates = self.project_coordinates(
-                rotation_vector,
-                translation_vector,
-                camera_matrix,
-                distortion_coefficients,
+                rotation_vector=rotation_vector,
+                translation_vector=translation_vector,
+                camera_matrix=camera_matrix,
+                distortion_coefficients=distortion_coefficients,
+                frame_width=frame_width,
+                frame_height=frame_height,
             )
         return Point2D(
             coordinates=new_coordinates,
             coordinate_indices=self.coordinate_indices,
             time_index=self.time_index,
             start_time=self.start_time,
             frames_per_second=self.frames_per_second,
@@ -927,39 +936,49 @@
         )
 
 
 class Line2D(Geom2D, Line):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def draw_matplotlib(self, axis):
-        if self.coordinates.shape != (1, 2, 2):
+    def draw_matplotlib(self, axis, frame_index):
+        if self.coordinates.shape[1:] != (2, 2):
             raise ValueError(
-                "Draw method for Line2D requires coordinates to be of shape (1, 2, 2)"
+                "Draw method for Line2D requires coordinates to be of shape (N, 2, 2)"
             )
+
+        coordinates = self.coordinates[frame_index]
+
+        if np.any(np.isnan(coordinates)):
+            return
+
         axis.add_artist(
             plt.Line2D(
-                (self.coordinates[0, 0, 0], self.coordinates[0, 1, 0]),
-                (self.coordinates[0, 0, 1], self.coordinates[0, 1, 1]),
+                (coordinates[0, 0], coordinates[1, 0]),
+                (coordinates[0, 1], coordinates[1, 1]),
                 linewidth=self.line_width,
                 color=self.color,
                 alpha=self.alpha,
             )
         )
 
-    def draw_opencv(self, image):
-        if self.coordinates.shape != (1, 2, 2):
+    def draw_opencv(self, image, frame_index):
+        if self.coordinates.shape[1:] != (2, 2):
             raise ValueError(
-                "Draw method for Line2D requires coordinates to be of shape (1, 2, 2)"
+                "Draw method for Line2D requires coordinates to be of shape (N, 2, 2)"
             )
-        if np.any(np.isnan(self.coordinates)):
+
+        coordinates = self.coordinates[frame_index]
+
+        if np.any(np.isnan(coordinates)):
             return image
+
         new_image = cv_utils.draw_line(
             image,
-            coordinates=self.coordinates[0],
+            coordinates=coordinates,
             line_width=self.line_width,
             color=self.color,
             alpha=self.alpha,
         )
         return new_image
 
 
@@ -975,18 +994,20 @@
         distortion_coefficients,
         frame_width=None,
         frame_height=None,
     ):
         new_coordinates = None
         if self.coordinates is not None:
             new_coordinates = self.project_coordinates(
-                rotation_vector,
-                translation_vector,
-                camera_matrix,
-                distortion_coefficients,
+                rotation_vector=rotation_vector,
+                translation_vector=translation_vector,
+                camera_matrix=camera_matrix,
+                distortion_coefficients=distortion_coefficients,
+                frame_width=frame_width,
+                frame_height=frame_height,
             )
         return Line2D(
             coordinates=new_coordinates,
             coordinate_indices=self.coordinate_indices,
             time_index=self.time_index,
             start_time=self.start_time,
             frames_per_second=self.frames_per_second,
@@ -1006,42 +1027,50 @@
         )
 
 
 class Text2D(Geom2D, Text):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def draw_matplotlib(self, axis):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_matplotlib(self, axis, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Text2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Text2D requires coordinates to be of shape (N, 1, 2)"
             )
-        if np.any(np.isnan(self.coordinates)):
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
             return
+
         axis.text(
-            self.coordinates[0, 0, 0],
-            self.coordinates[0, 0, 1],
+            coordinates[0],
+            coordinates[1],
             self.text,
             color=self.color,
             alpha=self.alpha,
             horizontalalignment=self.horizontal_alignment,
             verticalalignment=self.vertical_alignment,
             clip_on=True,
         )
 
-    def draw_opencv(self, image):
-        if self.coordinates.shape != (1, 1, 2):
+    def draw_opencv(self, image, frame_index):
+        if self.coordinates.shape[1:] != (1, 2):
             raise ValueError(
-                "Draw method for Text2D requires coordinates to be of shape (1, 1, 2)"
+                "Draw method for Text2D requires coordinates to be of shape (N, 1, 2)"
             )
-        if np.any(np.isnan(self.coordinates)):
+
+        coordinates = self.coordinates[frame_index][0]
+
+        if np.any(np.isnan(coordinates)):
             return image
+
         new_image = cv_utils.draw_text(
             image,
-            anchor_coordinates=self.coordinates[0, 0],
+            anchor_coordinates=coordinates,
             text=self.text,
             horizontal_alignment=self.horizontal_alignment,
             vertical_alignment=self.vertical_alignment,
             color=self.color,
             alpha=self.alpha,
         )
         return new_image
@@ -1059,18 +1088,20 @@
         distortion_coefficients,
         frame_width=None,
         frame_height=None,
     ):
         new_coordinates = None
         if self.coordinates is not None:
             new_coordinates = self.project_coordinates(
-                rotation_vector,
-                translation_vector,
-                camera_matrix,
-                distortion_coefficients,
+                rotation_vector=rotation_vector,
+                translation_vector=translation_vector,
+                camera_matrix=camera_matrix,
+                distortion_coefficients=distortion_coefficients,
+                frame_width=frame_width,
+                frame_height=frame_height,
             )
         return Text2D(
             coordinates=new_coordinates,
             coordinate_indices=self.coordinate_indices,
             time_index=self.time_index,
             start_time=self.start_time,
             frames_per_second=self.frames_per_second,
```

### Comparing `wf_geom_render-0.4.0/pyproject.toml` & `wf_geom_render-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-geom-render"
-dynamic = ["version"]
+version = "0.5.0"
 
 [tool.poetry]
 name = "wf-geom-render"
-version = "0.4.0"
+version = "0.5.0"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 description = "A library for projecting 3D geoms into 2D videos"
 keywords = ["opencv", "cv"]
 repository = "https://github.com/WildflowerSchools/wf-geom-render"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
@@ -25,14 +25,15 @@
 numpy = ">=1.17"
 python = "^3.8"
 tqdm = ">=4.41.1"
 wf-cv-utils = ">=0.3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
+pylint = "^2.17.4"
 
 [tool.setuptools]
 py-modules = []
 
 [build-system]
 requires = ["poetry-core", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wf_geom_render-0.4.0/setup.py` & `wf_geom_render-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.1.2', 'numpy>=1.17', 'tqdm>=4.41.1', 'wf-cv-utils>=0.3.1']
 
 setup_kwargs = {
     'name': 'wf-geom-render',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'A library for projecting 3D geoms into 2D videos',
     'long_description': '# geom_render\n\nA library for projecting 3D geoms onto 2D videos\n',
     'author': 'Theodore Quinn',
     'author_email': 'ted.quinn@wildflowerschools.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/WildflowerSchools/wf-geom-render',
```

### Comparing `wf_geom_render-0.4.0/PKG-INFO` & `wf_geom_render-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-geom-render
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library for projecting 3D geoms into 2D videos
 Home-page: https://github.com/WildflowerSchools/wf-geom-render
 Keywords: opencv,cv
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

