# Comparing `tmp/webcam-1.7.tar.gz` & `tmp/webcam-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.7.tar", last modified: Wed Jun 28 13:58:44 2023, max compression
+gzip compressed data, was "webcam-1.8.tar", last modified: Thu Jun 29 12:12:36 2023, max compression
```

## Comparing `webcam-1.7.tar` & `webcam-1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:58:44.635107 webcam-1.7/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.7/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-06-28 13:58:44.632830 webcam-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-28 13:58:44.636109 webcam-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-06-28 13:58:40.000000 webcam-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:58:44.572967 webcam-1.7/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.7/webcam/__init__.py
--rw-rw-rw-   0        0        0    15431 2023-06-28 13:58:31.000000 webcam-1.7/webcam/_perspective_manager.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.7/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.7/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    24481 2023-06-28 12:32:18.000000 webcam-1.7/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:58:44.630830 webcam-1.7/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-06-28 13:58:44.000000 webcam-1.7/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-28 13:58:44.000000 webcam-1.7/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:58:44.000000 webcam-1.7/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-28 13:58:44.000000 webcam-1.7/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-28 13:58:44.000000 webcam-1.7/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.430014 webcam-1.8/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.8/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-29 12:12:36.428120 webcam-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:12:36.430014 webcam-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-29 12:12:02.000000 webcam-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.396885 webcam-1.8/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.8/webcam/__init__.py
+-rw-rw-rw-   0        0        0    16742 2023-06-29 11:22:04.000000 webcam-1.8/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.8/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.8/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    25157 2023-06-29 12:11:46.000000 webcam-1.8/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.426075 webcam-1.8/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.7/LICENSE` & `webcam-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.7/PKG-INFO` & `webcam-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.7
+Version: 1.8
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.7/README.md` & `webcam-1.8/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.7/setup.py` & `webcam-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.7',
+    version='1.8',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.7/webcam/_perspective_manager.py` & `webcam-1.8/webcam/_perspective_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,130 +28,73 @@
         self.inverse_homography_matrix = np.linalg.inv(self.homography_matrix)
 
         self.crop_boundaries = crop_boundaries
         self.boundaries_color = boundaries_color
 
     @property
     def output_w(self) -> int:
-        w, h = self.after_warp_image_shape(w=self.default_w, h=self.default_h)
+        w, h = self.calculate_output_shape(w=self.default_w, h=self.default_h)
         return w
 
     @property
     def output_h(self) -> int:
-        w, h = self.after_warp_image_shape(w=self.default_w, h=self.default_h)
+        w, h = self.calculate_output_shape(w=self.default_w, h=self.default_h)
         return h
 
-    @lru_cache(maxsize=32)
-    def __build_corners(self, w: float|int, h: float|int):
-        assert w == self.default_w and h == self.default_h, \
-            f'By the moment, that is assumed that h and w are kept since the initialization. ' \
-            f'Changing them could lead to unexpected results. '
-        w, h = float(w), float(h)
-        return np.array(((0., 0.), (w - 1., 0.), (w - 1., h - 1.), (0., h - 1.)), dtype=np.float32)
-
-    # Cache this function as most of times it will be always called with the same arguments
-    @lru_cache(maxsize=16)
-    def after_warp_image_shape(self, w: int, h: int, cropping_boundaries: bool | None = None) -> tuple[int, int]:
-        """
-        Gets the new width and height that an image with width w, and height w will have after warping.
-        It will depend on the defined self.homography_matrix and the value of cropping_boundaries.
-        :param w: int. The width of the input image
-        :param h: int. The height of the input image
-        :param cropping_boundaries: int. If crop boundaries to hide black borders or not. If None, the value of
-                                    self.crop_boundaries will be used.
-        :return: tuple[int, int]. width and height of the image that .warp() will produce for an input image with
-                                  of width w and height h.
-        """
-        if cropping_boundaries is None:
-            cropping_boundaries = self.crop_boundaries
-
-        # Get the new position for the four image corners
-        warped_corners = self.__output_corners(w=w, h=h)
-        # Get the four x coords and the four y coords
-        x_coords, y_coords =  warped_corners[:, 0], warped_corners[:, 1]
-        # If cropping boundaries, let's delete from here the larger and shorter limits, to ensure no black borders
-        if cropping_boundaries:
-            # Now they will contain only two coords, as we will crop largest limits to shortest ones.
-            x_coords, y_coords = np.sort(x_coords)[1:-1], np.sort(y_coords)[1:-1]
-        # Get the output width and height
-        w_after_warp = int(np.ceil(np.max(x_coords)) - np.floor(np.min(x_coords)))
-        h_after_warp = int(np.ceil(np.max(y_coords)) - np.floor(np.min(y_coords)))
-        return w_after_warp, h_after_warp
-
     def warp(self, image: np.ndarray) -> np.ndarray:
         """
         Warp the image to generate the required perspective correction
         :param image: np.ndarray. Image to warp
         :return: np.ndarray. The output warped image
         """
         h, w = image.shape[:2]
-        w_after_warp, h_after_warp = self.after_warp_image_shape(w=w, h=h, cropping_boundaries=False)
+        w_after_warp, h_after_warp = self.calculate_output_shape(w=w, h=h, cropping_boundaries=False)
 
         warped_image = cv2.warpPerspective(
             src=image,
             M=self.homography_matrix,
             dsize=(w_after_warp, h_after_warp),
             borderMode=cv2.BORDER_CONSTANT,
             borderValue=self.boundaries_color
         )
 
         if self.crop_boundaries:
-            warped_corners = self.__output_corners(w=w, h=h)
-            # Keep only the second and third x coords, as they are the left and right limits
-            x_min, x_max = np.sort(warped_corners[:, 0])[1:-1]
-            # Keep only the second and third y coords, as they are the top and bottom limits
-            y_min, y_max = np.sort(warped_corners[:, 1])[1:-1]
-            x_min, x_max = int(np.floor(x_min)), int(np.ceil(x_max))
-            y_min, y_max = int(np.floor(y_min)), int(np.ceil(y_max))
-
-            assert y_min >= 0 and x_min >=0, f"Cropping coords can't be negatives. Got x={x_min}, y={y_max}"
-            assert y_max > y_min and x_max > x_min, f"x_max and y_max must be larger than x_min and y_min."\
-                                                    f"Got x_min={x_min}, x_max={x_max}, y_min={y_min} and y_max={y_max}"
-
+            x_min, y_min, x_max, y_max = self.__get_crop_bbox_xyxy(h=h, w=w)
             warped_image = warped_image[y_min:y_max, x_min:x_max]
 
         return warped_image
 
+    # Cache this function as most of times it will be always called with the same arguments
     @lru_cache(maxsize=16)
-    def __output_corners(self, w: int, h: int) -> np.ndarray:
+    def calculate_output_shape(self, w: int, h: int, cropping_boundaries: bool | None = None) -> tuple[int, int]:
         """
-        Get the corners of the output image after warping an image with width w and height h.
+        Gets the new width and height that an image with width w, and height w will have after warping.
+        It will depend on the defined self.homography_matrix and the value of cropping_boundaries.
         :param w: int. The width of the input image
         :param h: int. The height of the input image
-        :return: np.ndarray. The corners of the output image after warping an image with width w and height h.
+        :param cropping_boundaries: int. If crop boundaries to hide black borders or not. If None, the value of
+                                    self.crop_boundaries will be used.
+        :return: tuple[int, int]. width and height of the image that .warp() will produce for an input image with
+                                  of width w and height h.
         """
-        # Calculate the positions for each one of the four corners determined by w and h
-        corners = self.__build_corners(w=w, h=h)
-        # Get the new position for the four image corners
-        warped_corners = cv2.perspectiveTransform(corners[None, ...], self.homography_matrix)[0]
-        assert np.isclose(np.min(warped_corners), 0., atol=1e-3), f"Minimum warped corner should be 0. Got {np.min(warped_corners)}"
-        return np.clip(warped_corners, a_min=0., a_max=None)
+        if cropping_boundaries is None:
+            cropping_boundaries = self.crop_boundaries
 
-    def __apply_non_negative_translation_to_homography_matrix(self, m: np.ndarray, w: int, h: int) -> np.ndarray:
-        """
-        Apply a translation to the given homography matrix to ensure that the minimum x and y coordinates
-        are at (0,0) after transformation.
-        :param m: np.ndarray. The matrix to be translated.
-        :return: np.ndarray. The translated matrix.
-        """
-        corners = self.__build_corners(w=w, h=h)
         # Get the new position for the four image corners
-        warped_corners = cv2.perspectiveTransform(corners[None, ...], m)[0]
-
-        # Get the minimum x and y coordinates
-        x_min = np.min(warped_corners[:, 0])
-        y_min = np.min(warped_corners[:, 1])
-
-        # Create a translation matrix to move the minimum x and y coordinates to (0,0)
-        translation_matrix = np.array(((1., 0., -x_min), (0., 1., -y_min), (0., 0., 1.)), dtype=np.float32)
-
-        # Combine the original matrix with the translation matrix
-        combined_matrix = np.dot(a=translation_matrix, b=m)
-
-        return combined_matrix
+        warped_corners = self.__output_corners(w=w, h=h)
+        # Get the four x coords and the four y coords
+        x_coords, y_coords =  warped_corners[:, 0], warped_corners[:, 1]
+        # If cropping boundaries, let's delete from here the larger and shorter limits, to ensure no black borders
+        if cropping_boundaries:
+            # Now they will contain only two coords, as we will crop largest limits to shortest ones.
+            x_coords, y_coords = np.sort(x_coords)[1:-1], np.sort(y_coords)[1:-1]
+        # Get the output width and height
+        w_after_warp = int(np.ceil(np.max(x_coords)) - np.floor(np.min(x_coords)))
+        h_after_warp = int(np.ceil(np.max(y_coords)) - np.floor(np.min(y_coords)))
+        return w_after_warp, h_after_warp
 
 
     # ------------------------------ CALCULATE MAGNIFICATION FACTOR ------------------------------
 
     @lru_cache(maxsize=64)
     def get_hw_magnification_at_point(self, x:int|float, y:int|float) -> tuple[float, float]:
         """
@@ -259,13 +202,94 @@
         if isinstance(points_xy, (tuple, list)):
             points_xy = np.array(points_xy, dtype=np.float32)
         assert isinstance(points_xy, np.ndarray), "Line must be either a tuple, a list or a numpy array."
         points_xy = points_xy.reshape(-1, 2)
         n_points, coords = points_xy.shape
         assert coords == 2, f"Expected 2 coordinates per point, but got {coords}."
 
+        if self.crop_boundaries:
+            x_min, y_min, x_max, y_max = self.__get_crop_bbox_xyxy(h=self.default_h, w=self.default_w)
+            points_xy += (x_min, y_min)
         # Transform the line back to the input space using the inverse homography matrix
         points_transformed = np.dot(self.inverse_homography_matrix, np.c_[points_xy, np.ones(n_points)].T)
         points_transformed /= points_transformed[2]
         points_transformed = points_transformed[:2].T
 
         return points_transformed
+
+
+    # ------------------------------- AUXILIARY METHODS -------------------------------
+
+    def __apply_non_negative_translation_to_homography_matrix(self, m: np.ndarray, w: int, h: int) -> np.ndarray:
+        """
+        Apply a translation to the given homography matrix to ensure that the minimum x and y coordinates
+        are at (0,0) after transformation.
+        :param m: np.ndarray. The matrix to be translated.
+        :return: np.ndarray. The translated matrix.
+        """
+        corners = self.__build_corners(w=w, h=h)
+        # Get the new position for the four image corners
+        warped_corners = cv2.perspectiveTransform(corners[None, ...], m)[0]
+
+        # Get the minimum x and y coordinates
+        x_min = np.min(warped_corners[:, 0])
+        y_min = np.min(warped_corners[:, 1])
+
+        # Create a translation matrix to move the minimum x and y coordinates to (0,0)
+        translation_matrix = np.array(((1., 0., -x_min), (0., 1., -y_min), (0., 0., 1.)), dtype=np.float32)
+
+        # Combine the original matrix with the translation matrix
+        combined_matrix = np.dot(a=translation_matrix, b=m)
+
+        return combined_matrix
+
+    @lru_cache(maxsize=16)
+    def __get_crop_bbox_xyxy(self, h: int | float, w: int | float,
+                             return_as_int: bool = True) -> tuple[int|float, int|float, int|float, int|float]:
+        """
+        Get the bounding box of the warped image that excludes the black borders. The returned bounding box is in the
+        format x_min, y_min, x_max, y_max.
+        :param h: int|float. Height of the image.
+        :param w: int|float. Width of the image.
+        :param return_as_int: bool. Whether to return the bounding box as integers or floats. Default: True. Set to
+        False if you want subpixel precision.
+        :return: tuple[int, int, int, int]. The bounding box of the warped image that excludes the black borders.
+        """
+        warped_corners = self.__output_corners(w=w, h=h)
+        # Keep only the second and third x coords, as they are the left and right limits
+        x_min, x_max = np.sort(warped_corners[:, 0])[1:-1]
+        # Keep only the second and third y coords, as they are the top and bottom limits
+        y_min, y_max = np.sort(warped_corners[:, 1])[1:-1]
+        if return_as_int:
+            x_min, x_max = int(np.floor(x_min)), int(np.ceil(x_max))
+            y_min, y_max = int(np.floor(y_min)), int(np.ceil(y_max))
+        assert y_min >= 0 and x_min >= 0, f"Cropping coords can't be negatives. Got x={x_min}, y={y_max}"
+        assert y_max > y_min and x_max > x_min, f"x_max and y_max must be larger than x_min and y_min." \
+                                                f"Got x_min={x_min}, x_max={x_max}, y_min={y_min} and y_max={y_max}"
+        return x_min, y_min, x_max, y_max
+
+    @lru_cache(maxsize=16)
+    def __output_corners(self, w: int, h: int) -> np.ndarray:
+        """
+        Get the corners of the output image after warping an image with width w and height h.
+        :param w: int. The width of the input image
+        :param h: int. The height of the input image
+        :return: np.ndarray. The corners of the output image after warping an image with width w and height h.
+        """
+        # Calculate the positions for each one of the four corners determined by w and h
+        corners = self.__build_corners(w=w, h=h)
+        # Get the new position for the four image corners
+        warped_corners = cv2.perspectiveTransform(corners[None, ...], self.homography_matrix)[0]
+        assert np.isclose(np.min(warped_corners), 0., atol=1e-3), f"Minimum warped corner should be 0. Got {np.min(warped_corners)}"
+        return np.clip(warped_corners, a_min=0., a_max=None)
+
+    @lru_cache(maxsize=32)
+    def __build_corners(self, w: float | int, h: float | int) -> np.ndarray:
+        """
+        Build the corners of the image as a numpy array of shape (4, 2). In the format x1y1, x2y2, x3y3, x4y4.
+        :param w: int|float. Width of the image.
+        :param h: int|float. Height of the image.
+        :return: np.ndarray. The corners of the image, as float32. Shape (4, 2). Format x1y1, x2y2, x3y3, x4y4.
+        """
+        w, h = float(w), float(h)
+        return np.array(((0., 0.), (w - 1., 0.), (w - 1., h - 1.), (0., h - 1.)), dtype=np.float32)
+
```

### Comparing `webcam-1.7/webcam/_video_webcam.py` & `webcam-1.8/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.7/webcam/_webcam_background.py` & `webcam-1.8/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.7/webcam/webcam.py` & `webcam-1.8/webcam/webcam.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         homography_matrix: np.ndarray | list[list[float], ...] | None = None,
         crop_on_warping: bool = True
     ):
         """
         Initialize the WebcamReader.
 
         :param src: int or str. The index of the webcam or its path.
-        :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
-        :param w: int or None. Desired width of the frames. If None and `_h` is provided, the aspect ratio will be preserved.
+        :param h: int or None. Desired height of the frames. If None and `_input_w` is provided, the aspect ratio will be preserved.
+        :param w: int or None. Desired width of the frames. If None and `_input_h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         :param on_aspect_ratio_lost: str. What to do if the aspect ratio of the frames is different from the desired aspect ratio. Valid values are: 'crop' and 'resize'.
         :param homography_matrix: np.ndarray or list[list[float], ...] or None. The homography matrix to warp the frames with.
         If passed, frames will be warped before any other processing.
@@ -70,47 +70,48 @@
             self.cap = cv2.VideoCapture(src) if not run_in_background else _WebcamBackground(src=src).start()
         self.as_bgr = as_bgr
 
         if homography_matrix is None:
             self.perspective_manager = None
         else:
             self.perspective_manager = _PerspectiveManager(homography_matrix=homography_matrix,
-                                                          default_h=int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
-                                                          default_w=int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
+                                                          default_h=self._input_h,
+                                                          default_w=self._input_w,
                                                           crop_boundaries=crop_on_warping)
 
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h=h, w=w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
         self.start_timestamp = time.time()
         self.max_frame_rate = max_frame_rate
         self.last_frame_timestamp = self.start_timestamp
 
 
 
     @property
-    def _h(self) -> int:
-        h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        if self.perspective_manager is None:
-            return h
-        w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
-        corrected_w, corrected_h = self.perspective_manager.after_warp_image_shape(w=w, h=h)
-        return corrected_h
+    def _input_h(self) -> int:
+        return int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+
+    @property
+    def _input_w(self) -> int:
+        return int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
 
     @property
-    def _w(self) -> int:
-        w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+    def __pre_resize_w(self) -> int:
         if self.perspective_manager is None:
-            return w
-        h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        corrected_w, corrected_h = self.perspective_manager.after_warp_image_shape(w=w, h=h)
-        return corrected_w
+            return self._input_w
+        return self.perspective_manager.output_w
 
+    @property
+    def __pre_resize_h(self) -> int:
+        if self.perspective_manager is None:
+            return self._input_h
+        return self.perspective_manager.output_h
 
     @property
     def h(self) -> int:
         return self.frame_size_hw[0]
 
     @property
     def w(self) -> int:
@@ -166,68 +167,52 @@
         :return: The next frame in the video.
         """
         # While webcam is open
         while self.cap.isOpened():
             yield self.read_next_frame()
         raise StopIteration
 
-    def _calculate_and_set_desired_resolution(self, h: int | None = None, w: int | None = None) -> tuple[int, int]:
-        """
-        Calculate and set the optimal webcam resolution based on the desired width and height.
-        The resolution will only change if the new resolution is natively supported by the webcam
-        and maintains the maximum available aspect ratio.
-
-        :param h: int or None. Desired height of the frames.
-        :param w: int or None. Desired width of the frames.
-        :return: tuple. The final frame size (height, width).
-        """
-        # Set webcam to its maximum supported resolution
-        max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
-
-        if h is None and w is None:
-            return max_h, max_w
-
-        # Calculate the missing dimension while keeping the aspect ratio if only one dimension is provided
-        if h is None or w is None:
-            h, w = self.calculate_frame_size_keeping_aspect_ratio(h=h, w=w)
-
-        # Change the resolution if supported (and keeps the maximum aspect ratio if only one dimension was provided)
-        if self._is_resolution_natively_supported(h=h, w=w):
-            self._set_webcam_resolution(h=h, w=w)
-
-        return h, w
-
     def _set_webcam_resolution(self, h: int, w: int) -> Tuple[int, int]:
         """
         Set the webcam resolution to the specified height and width and return the actual frame size set by the webcam.
 
         :param h: int. Desired height of the frames.
         :param w: int. Desired width of the frames.
         :return: tuple. The final frame size (height, width) after attempting to set the desired resolution.
         """
-        self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
-        self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
 
-        return self._h, self._w
+        # Set the webcam resolution
+        self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
+        self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
+        # Get the actual resolution set by the webcam
+        return self._input_h, self._input_w
 
     def _is_resolution_natively_supported(self, h: int, w: int):
-        current_h, current_w = self._h, self._w
+        """
+        Check if the webcam supports the specified resolution natively.
+        :param h: int. Desired height of the frames.
+        :param w: int. Desired width of the frames.
+        :return: bool. True if the webcam supports the specified resolution natively.
+        """
+        assert isinstance(h, int) and isinstance(w, int), f"Invalid resolution: {h}x{w}. Expected integers. " \
+                                                          f"Got {type(h)}x{type(w)}."
+        current_h, current_w = self._input_h, self._input_w
         supported_h, supported_w = self._set_webcam_resolution(h=h, w=w)
         new_h, new_w = self._set_webcam_resolution(h=current_h, w=current_w)
         assert new_h == current_h and new_w == current_w, f"Webcam resolution could not be restored to {current_h}x{current_w}."
         return supported_h == h and supported_w == w
 
     def _max_available_resolution(self) -> Tuple[int, int]:
         """
         Get the maximum allowed webcam resolution without changing the current resolution.
 
         :return: tuple. The maximum allowed webcam resolution (height, width).
         """
         # Store the current resolution
-        current_h, current_w = self._h, self._w
+        current_h, current_w = self._input_h, self._input_w
 
         # Set the webcam resolution to an extremely high value and get the resulting maximum allowed resolution
         max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
 
         # Restore the original resolution
         self._set_webcam_resolution(h=current_h, w=current_w)
 
@@ -331,27 +316,27 @@
         :param x: int or float or None. The x coordinate of the pixel.
         :param y: int or float or None. The y coordinate of the pixel.
         :return: float. The magnification of the pixel at (x, y).
         """
 
         # Calculate the homography magnification if appliable
         if self.perspective_manager is not None:
-            x = self._w // 2 if x is None else x
-            y = self._h // 2 if y is None else y
-
+            x = self.__pre_resize_w // 2 if x is None else x
+            y = self.__pre_resize_h // 2 if y is None else y
             magnification_h, magnification_w = self.perspective_manager.get_hw_magnification_at_point(x=x, y=y)
-            input_h, input_w = self.perspective_manager.output_h, self.perspective_manager.output_w
         # Or use the default magnification
         else:
             magnification_h, magnification_w = 1.0, 1.0
-            input_h, input_w = self._h, self._w
+
+        input_h, input_w = self.__pre_resize_h, self.__pre_resize_w
 
         # Calculate the pixel magnification for each axis when adjusting size
-        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h, input_w, magnification_h,
-                                                                                      magnification_w)
+        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h=input_h, input_w=input_w,
+                                                                                      pre_magnification_h=magnification_h,
+                                                                                      pre_magnification_w=magnification_w)
 
         # Return the magnification of the pixel at (x, y)
         return magnification_h, magnification_w
 
     def get_line_hw_magnification(self, line_xyxy: np.ndarray | tuple[int|float, int|float, int|float, int|float],
                                   space: str = OUTPUT) \
             -> tuple[float, float]:
@@ -363,51 +348,76 @@
         :return: tuple. The magnification factor for the line.
         """
         if space == OUTPUT:
             line_xyxy = self.output_space_points_to_input_space(points_xy=line_xyxy)
 
         # Calculate the homography magnification if appliable
         if self.perspective_manager is not None:
-            magnification_h, magnification_w = self.perspective_manager.get_hw_magnification_for_line(xyxy_line=line_xyxy,
-                                                                                                      space=INPUT)
-            input_h, input_w = self.perspective_manager.output_h, self.perspective_manager.output_w
+            magnification_h, magnification_w = self.perspective_manager.get_hw_magnification_for_line(xyxy_line=line_xyxy, space=INPUT)
         # Or use the default magnification
         else:
             magnification_h, magnification_w = 1.0, 1.0
-            input_h, input_w = self._h, self._w
 
-        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h=input_h, input_w=input_w,
+        magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h=self.__pre_resize_h,
+                                                                                      input_w=self.__pre_resize_w,
                                                                                       pre_magnification_h=magnification_h,
                                                                                       pre_magnification_w=magnification_w)
 
         return magnification_h, magnification_w
 
 
 
     # --------------- AUXILIARY METHODS ---------------
-    def calculate_frame_size_keeping_aspect_ratio(self, h:int | None, w:int|None) -> tuple[int, int]:
+    def _calculate_frame_size_keeping_aspect_ratio(self, h: int | None, w: int | None) -> tuple[int, int]:
         """
         When only one of the frame size dimensions is given, the other one is calculated keeping the
         aspect ratio with the original video.
 
-        :param h: int or None. Height of the frame. If None, _w must be provided.
-        :param w: int or None. Width of the frame. If None, _h must be provided.
+        :param h: int or None. Height of the frame. If None, _input_w must be provided.
+        :param w: int or None. Width of the frame. If None, _input_h must be provided.
         :return: The height and width of the frame.
         """
 
         if h is None and w is not None:
-            h = int(round(self._h * w / self._w))
+            h = int(round(self.__pre_resize_h * w / self.__pre_resize_w))
         elif h is not None and w is None:
-            w = int(round(self._w * h / self._h))
+            w = int(round(self.__pre_resize_w * h / self.__pre_resize_h))
         else:
             raise ValueError(f'Only one of the frame size dimensions must be provided.'
-                             f' Got _h={h} and _w={w}.')
-        assert h is not None and w is not None, f'Both _h and _w should have been calculated. Got _h={h} and _w={w}.'
+                             f' Got _input_h={h} and _input_w={w}.')
+        assert h is not None and w is not None, f'Both _input_h and _input_w should have been calculated. Got _input_h={h} and _input_w={w}.'
+        return h, w
+
+    def _calculate_and_set_desired_resolution(self, h: int | None = None, w: int | None = None) -> tuple[int, int]:
+        """
+        Calculate and set the optimal webcam resolution based on the desired width and height.
+        The resolution will only change if the new resolution is natively supported by the webcam
+        and maintains the maximum available aspect ratio.
+
+        :param h: int or None. Desired height of the frames.
+        :param w: int or None. Desired width of the frames.
+        :return: tuple. The final frame size (height, width).
+        """
+        # Set webcam to its maximum supported resolution
+        max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
+
+        if h is None and w is None:
+            return max_h, max_w
+
+        # Calculate the missing dimension while keeping the aspect ratio if only one dimension is provided
+        if h is None or w is None:
+            h, w = self._calculate_frame_size_keeping_aspect_ratio(h=h, w=w)
+
+        # Change the resolution if supported (and keeps the maximum aspect ratio if only one dimension was provided)
+        if self._is_resolution_natively_supported(h=h, w=w):
+            self._set_webcam_resolution(h=h, w=w)
+
         return h, w
 
+
     @lru_cache(maxsize=64)
     def __calculate_resizing_magnification_hw(self, input_h: int, input_w: int, pre_magnification_h: float = 1.0,
                                               pre_magnification_w: float = 1.0) -> tuple[float, float]:
         """
         Calculate the pixel magnification for each axis when adjusting size
         :param input_h: int. The input height.
         :param input_w: int. The input width.
@@ -425,14 +435,17 @@
             magnification_w = pre_magnification_w * resize_ratio
         else:
             raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}."
                              f" Valid values are '{RESIZE}' and '{CROP}'.")
 
         return magnification_h, magnification_w
 
+
+    # -------------------------- REVERSE TRANSFORMATIONS --------------------------
+
     def output_space_points_to_input_space(self, points_xy: np.ndarray | tuple[float | int, ...] | list[float | int, ...]) ->\
             np.ndarray:
         """
         Transform the given points from output space to input space.
 
         :param points_xy: np.ndarray. Points to be transformed. It has shape (N, 2), where N is the number of points.
         :return: np.ndarray. The transformed points. It has shape (N, 2).
@@ -507,14 +520,16 @@
 
         # Translate the points
         points_xy[:, 0] += x1
         points_xy[:, 1] += y1
 
         return points_xy
 
+# -------------------------- BUILT-IN METHODS --------------------------
+
     def __iter__(self):
         return self
 
     def __next__(self):
         return self.read_next_frame()
 
     def __del__(self):
```

### Comparing `webcam-1.7/webcam.egg-info/PKG-INFO` & `webcam-1.8/webcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.7
+Version: 1.8
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

