# Comparing `tmp/webcam-1.8.tar.gz` & `tmp/webcam-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.8.tar", last modified: Thu Jun 29 12:12:36 2023, max compression
+gzip compressed data, was "webcam-1.9.tar", last modified: Thu Jun 29 12:42:37 2023, max compression
```

## Comparing `webcam-1.8.tar` & `webcam-1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.430014 webcam-1.8/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.8/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-06-29 12:12:36.428120 webcam-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 12:12:36.430014 webcam-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-06-29 12:12:02.000000 webcam-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.396885 webcam-1.8/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.8/webcam/__init__.py
--rw-rw-rw-   0        0        0    16742 2023-06-29 11:22:04.000000 webcam-1.8/webcam/_perspective_manager.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.8/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.8/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    25157 2023-06-29 12:11:46.000000 webcam-1.8/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:12:36.426075 webcam-1.8/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 12:12:36.000000 webcam-1.8/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.220170 webcam-1.9/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.9/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-29 12:42:37.218893 webcam-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:42:37.220170 webcam-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-29 12:42:32.000000 webcam-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.171483 webcam-1.9/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.9/webcam/__init__.py
+-rw-rw-rw-   0        0        0    16742 2023-06-29 11:22:04.000000 webcam-1.9/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.9/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.9/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    24581 2023-06-29 12:41:23.000000 webcam-1.9/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:42:37.213900 webcam-1.9/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-29 12:42:37.000000 webcam-1.9/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-29 12:42:37.000000 webcam-1.9/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:42:37.000000 webcam-1.9/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-29 12:42:37.000000 webcam-1.9/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 12:42:37.000000 webcam-1.9/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.8/LICENSE` & `webcam-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.8/PKG-INFO` & `webcam-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.8
+Version: 1.9
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.8/README.md` & `webcam-1.9/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.8/setup.py` & `webcam-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.8',
+    version='1.9',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.8/webcam/_perspective_manager.py` & `webcam-1.9/webcam/_perspective_manager.py`

 * *Files identical despite different names*

### Comparing `webcam-1.8/webcam/_video_webcam.py` & `webcam-1.9/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.8/webcam/_webcam_background.py` & `webcam-1.9/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.8/webcam/webcam.py` & `webcam-1.9/webcam/webcam.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from __future__ import annotations
 
 from functools import lru_cache
 
 import cv2
 import numpy as np
 import time
-from typing import Tuple
 
 import os
 
 from webcam._video_webcam import _VideoWebcam
 from webcam._webcam_background import _WebcamBackground
 from webcam._perspective_manager import _PerspectiveManager
 
@@ -83,63 +82,61 @@
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
         self.start_timestamp = time.time()
         self.max_frame_rate = max_frame_rate
         self.last_frame_timestamp = self.start_timestamp
 
-
-
     @property
     def _input_h(self) -> int:
         return int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
 
     @property
     def _input_w(self) -> int:
         return int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
 
     @property
-    def __pre_resize_w(self) -> int:
-        if self.perspective_manager is None:
-            return self._input_w
-        return self.perspective_manager.output_w
-
-    @property
-    def __pre_resize_h(self) -> int:
-        if self.perspective_manager is None:
-            return self._input_h
-        return self.perspective_manager.output_h
-
-    @property
     def h(self) -> int:
         return self.frame_size_hw[0]
 
     @property
     def w(self) -> int:
         return self.frame_size_hw[1]
 
-    @property
-    def pixel_magnification(self) -> float:
-        m_h, m_w = self.get_magnification_hw(x=None, y=None)
-        return (m_h + m_w) / 2
-
-    @property
-    def pixel_magnification_h(self) -> float:
-        m_h, m_w = self.get_magnification_hw(x=None, y=None)
-        return m_h
-
-    @property
-    def pixel_magnification_w(self) -> float:
-        m_h, m_w = self.get_magnification_hw(x=None, y=None)
-        return m_w
 
     @property
     def current_timestamp_seconds(self):
         return time.time() - self.start_timestamp
 
+    def read(self, transform: bool = True) -> tuple[bool, np.ndarray|None]:
+        """
+        Read a frame from the webcam.
+
+        If the webcam's returned frame size is different from the user-set size, the frame is automatically resized.
+
+        :return: tuple. A boolean indicating whether the frame was read successfully, and the frame itself.
+        """
+        ret, frame = self.cap.read()
+
+        if ret and transform:
+            # Adjust the perspective (if needed). If homography matrix is not defined it will do nothing
+            if self.perspective_manager is not None:
+                frame = self.perspective_manager.warp(image=frame)
+            # Get the height and width of the frame
+            h, w = frame.shape[:2]
+            # Resize the frame if the webcam's returned frame size is different from the user-set size
+            if (h, w) != (self.h, self.w):
+                frame = self.__adjust_image_shape(frame=frame, h=self.h, w=self.w)
+
+        # Convert the frame from BGR to RGB format if necessary
+        if ret and not self.as_bgr:
+            cv2.cvtColor(src=frame, code=cv2.COLOR_BGR2RGB, dst=frame)
+
+        return ret, frame
+
     def read_next_frame(self) -> np.ndarray:
         """
         Read the next frame from the video. (Skipping the frames_offset if it is greater than one.)
         """
         batch_size = 1 if self.batch_size is None else self.batch_size
         frames = []
         for i in range(batch_size):
@@ -151,95 +148,32 @@
         if self.max_frame_rate is not None:
             # Sleep to simulate the frame rate (0.8 is a magic number, just to compensate the execution resuming time)
             time.sleep(max(0, (1/self.max_frame_rate)*0.8 - (time.time() - self.last_frame_timestamp)))
             self.last_frame_timestamp = time.time()
 
         return frames[0] if self.batch_size is None else np.stack(frames, axis=0)
 
-
-    def read_video_iterator(self, from_start: bool = False) -> np.ndarray:
-        """
-        Yields the frames of the video. If simulate_frame_rate is not None,
-         the frames are yielded at the given simulated frame rate. That is, skipping real_frame_rate / simulate_frame_rate
-         at each iteration.
-
-        :param from_start: If True, the iterator will start from the beginning of the video.
-
-        :return: The next frame in the video.
-        """
-        # While webcam is open
-        while self.cap.isOpened():
-            yield self.read_next_frame()
-        raise StopIteration
-
-    def _set_webcam_resolution(self, h: int, w: int) -> Tuple[int, int]:
-        """
-        Set the webcam resolution to the specified height and width and return the actual frame size set by the webcam.
-
-        :param h: int. Desired height of the frames.
-        :param w: int. Desired width of the frames.
-        :return: tuple. The final frame size (height, width) after attempting to set the desired resolution.
-        """
-
-        # Set the webcam resolution
-        self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
-        self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
-        # Get the actual resolution set by the webcam
-        return self._input_h, self._input_w
-
-    def _is_resolution_natively_supported(self, h: int, w: int):
-        """
-        Check if the webcam supports the specified resolution natively.
-        :param h: int. Desired height of the frames.
-        :param w: int. Desired width of the frames.
-        :return: bool. True if the webcam supports the specified resolution natively.
-        """
-        assert isinstance(h, int) and isinstance(w, int), f"Invalid resolution: {h}x{w}. Expected integers. " \
-                                                          f"Got {type(h)}x{type(w)}."
-        current_h, current_w = self._input_h, self._input_w
-        supported_h, supported_w = self._set_webcam_resolution(h=h, w=w)
-        new_h, new_w = self._set_webcam_resolution(h=current_h, w=current_w)
-        assert new_h == current_h and new_w == current_w, f"Webcam resolution could not be restored to {current_h}x{current_w}."
-        return supported_h == h and supported_w == w
-
-    def _max_available_resolution(self) -> Tuple[int, int]:
-        """
-        Get the maximum allowed webcam resolution without changing the current resolution.
-
-        :return: tuple. The maximum allowed webcam resolution (height, width).
-        """
-        # Store the current resolution
-        current_h, current_w = self._input_h, self._input_w
-
-        # Set the webcam resolution to an extremely high value and get the resulting maximum allowed resolution
-        max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
-
-        # Restore the original resolution
-        self._set_webcam_resolution(h=current_h, w=current_w)
-
-        return max_h, max_w
-
-    def _adjust_image_shape(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
+    def __adjust_image_shape(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
         """
         Adjust the shape of the frame according to the on_aspect_ratio_lost parameter.
 
         :param frame: np.ndarray. The input frame.
         :param h: int. Desired height of the frame.
         :param w: int. Desired width of the frame.
         :return: np.ndarray. The adjusted frame.
         """
         if self.on_aspect_ratio_lost == RESIZE:
             return cv2.resize(src=frame, dsize=(w, h))
         elif self.on_aspect_ratio_lost == CROP:
-            return self._resize_and_center_crop(frame=frame, h=h, w=w)
+            return self.__resize_and_center_crop(frame=frame, h=h, w=w)
         else:
             raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}. "
                                 f"Valid values are: {RESIZE}, {CROP}.")
 
-    def _resize_and_center_crop(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
+    def __resize_and_center_crop(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
         """
         Resize and center crop the input frame to the desired dimensions, while preserving the original aspect ratio.
 
         :param frame: np.ndarray. The input frame to be resized and cropped.
         :param h: int. The desired height of the output frame.
         :param w: int. The desired width of the output frame.
         :return: np.ndarray. The resized and center-cropped frame.
@@ -261,40 +195,14 @@
         # Calculate the position of the center crop
         y1, x1 = (new_h - h) // 2, (new_w - w) // 2
         y2, x2 = y1 + h, x1 + w
 
         # Crop the frame
         return frame[y1:y2, x1:x2]
 
-    def read(self, transform: bool = True) -> tuple[bool, np.ndarray|None]:
-        """
-        Read a frame from the webcam.
-
-        If the webcam's returned frame size is different from the user-set size, the frame is automatically resized.
-
-        :return: tuple. A boolean indicating whether the frame was read successfully, and the frame itself.
-        """
-        ret, frame = self.cap.read()
-
-        if ret and transform:
-            # Adjust the perspective (if needed). If homography matrix is not defined it will do nothing
-            if self.perspective_manager is not None:
-                frame = self.perspective_manager.warp(image=frame)
-            # Get the height and width of the frame
-            h, w = frame.shape[:2]
-            # Resize the frame if the webcam's returned frame size is different from the user-set size
-            if (h, w) != (self.h, self.w):
-                frame = self._adjust_image_shape(frame=frame, h=self.h, w=self.w)
-
-        # Convert the frame from BGR to RGB format if necessary
-        if ret and not self.as_bgr:
-            cv2.cvtColor(src=frame, code=cv2.COLOR_BGR2RGB, dst=frame)
-
-        return ret, frame
-
     def stop(self):
         self.cap.stop()
 
     def get(self, propId):
         return self.cap.get(propId=propId)
 
     def set(self, propId, value):
@@ -303,14 +211,137 @@
     def release(self):
         self.cap.release()
 
     def isOpened(self):
         return self.cap.isOpened()
 
 
+    # --------------- AUXILIARY METHODS ---------------
+    @property
+    def __pre_resize_w(self) -> int:
+        if self.perspective_manager is None:
+            return self._input_w
+        return self.perspective_manager.output_w
+
+    @property
+    def __pre_resize_h(self) -> int:
+        if self.perspective_manager is None:
+            return self._input_h
+        return self.perspective_manager.output_h
+
+    def _calculate_frame_size_keeping_aspect_ratio(self, h: int | None, w: int | None) -> tuple[int, int]:
+        """
+        When only one of the frame size dimensions is given, the other one is calculated keeping the
+        aspect ratio with the original video.
+
+        :param h: int or None. Height of the frame. If None, _input_w must be provided.
+        :param w: int or None. Width of the frame. If None, _input_h must be provided.
+        :return: The height and width of the frame.
+        """
+
+        if h is None and w is not None:
+            h = int(round(self.__pre_resize_h * w / self.__pre_resize_w))
+        elif h is not None and w is None:
+            w = int(round(self.__pre_resize_w * h / self.__pre_resize_h))
+        else:
+            raise ValueError(f'Only one of the frame size dimensions must be provided.'
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
+        return h, w
+
+    def _set_webcam_resolution(self, h: int, w: int) -> tuple[int, int]:
+        """
+        Set the webcam resolution to the specified height and width and return the actual frame size set by the webcam.
+
+        :param h: int. Desired height of the frames.
+        :param w: int. Desired width of the frames.
+        :return: tuple. The final frame size (height, width) after attempting to set the desired resolution.
+        """
+
+        # Set the webcam resolution
+        self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
+        self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
+        # Get the actual resolution set by the webcam
+        return self._input_h, self._input_w
+
+    def _is_resolution_natively_supported(self, h: int, w: int):
+        """
+        Check if the webcam supports the specified resolution natively.
+        :param h: int. Desired height of the frames.
+        :param w: int. Desired width of the frames.
+        :return: bool. True if the webcam supports the specified resolution natively.
+        """
+        assert isinstance(h, int) and isinstance(w, int), f"Invalid resolution: {h}x{w}. Expected integers. " \
+                                                          f"Got {type(h)}x{type(w)}."
+        current_h, current_w = self._input_h, self._input_w
+        supported_h, supported_w = self._set_webcam_resolution(h=h, w=w)
+        new_h, new_w = self._set_webcam_resolution(h=current_h, w=current_w)
+        assert new_h == current_h and new_w == current_w, f"Webcam resolution could not be restored to {current_h}x{current_w}."
+        return supported_h == h and supported_w == w
+
+    def _max_available_resolution(self) -> tuple[int, int]:
+        """
+        Get the maximum allowed webcam resolution without changing the current resolution.
+
+        :return: tuple. The maximum allowed webcam resolution (height, width).
+        """
+        # Store the current resolution
+        current_h, current_w = self._input_h, self._input_w
+
+        # Set the webcam resolution to an extremely high value and get the resulting maximum allowed resolution
+        max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
+
+        # Restore the original resolution
+        self._set_webcam_resolution(h=current_h, w=current_w)
+
+        return max_h, max_w
+
+
+
+    # ---------------------------- PIXEL MAGNIFICATION -----------------------------
+    @property
+    def pixel_magnification(self) -> float:
+        return (self.pixel_magnification_h + self.pixel_magnification_w) / 2
+
+    @property
+    def pixel_magnification_h(self) -> float:
+        m_h, m_w = self.get_magnification_hw(x=None, y=None)
+        return m_h
+
+    @property
+    def pixel_magnification_w(self) -> float:
+        m_h, m_w = self.get_magnification_hw(x=None, y=None)
+        return m_w
+
     @lru_cache(maxsize=64)
     def get_magnification_hw(self, x: int | float | None = None, y: int | float | None = None) -> float:
         """
         Calculate the magnification of the pixel at (x, y). If x and y are not given, the magnification of the
         center pixel is calculated. (x, y) coordinates are only relevant if the perspective is adjusted.
 
         :param x: int or float or None. The x coordinate of the pixel.
@@ -360,64 +391,14 @@
         magnification_h, magnification_w = self.__calculate_resizing_magnification_hw(input_h=self.__pre_resize_h,
                                                                                       input_w=self.__pre_resize_w,
                                                                                       pre_magnification_h=magnification_h,
                                                                                       pre_magnification_w=magnification_w)
 
         return magnification_h, magnification_w
 
-
-
-    # --------------- AUXILIARY METHODS ---------------
-    def _calculate_frame_size_keeping_aspect_ratio(self, h: int | None, w: int | None) -> tuple[int, int]:
-        """
-        When only one of the frame size dimensions is given, the other one is calculated keeping the
-        aspect ratio with the original video.
-
-        :param h: int or None. Height of the frame. If None, _input_w must be provided.
-        :param w: int or None. Width of the frame. If None, _input_h must be provided.
-        :return: The height and width of the frame.
-        """
-
-        if h is None and w is not None:
-            h = int(round(self.__pre_resize_h * w / self.__pre_resize_w))
-        elif h is not None and w is None:
-            w = int(round(self.__pre_resize_w * h / self.__pre_resize_h))
-        else:
-            raise ValueError(f'Only one of the frame size dimensions must be provided.'
-                             f' Got _input_h={h} and _input_w={w}.')
-        assert h is not None and w is not None, f'Both _input_h and _input_w should have been calculated. Got _input_h={h} and _input_w={w}.'
-        return h, w
-
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
-            h, w = self._calculate_frame_size_keeping_aspect_ratio(h=h, w=w)
-
-        # Change the resolution if supported (and keeps the maximum aspect ratio if only one dimension was provided)
-        if self._is_resolution_natively_supported(h=h, w=w):
-            self._set_webcam_resolution(h=h, w=w)
-
-        return h, w
-
-
     @lru_cache(maxsize=64)
     def __calculate_resizing_magnification_hw(self, input_h: int, input_w: int, pre_magnification_h: float = 1.0,
                                               pre_magnification_w: float = 1.0) -> tuple[float, float]:
         """
         Calculate the pixel magnification for each axis when adjusting size
         :param input_h: int. The input height.
         :param input_w: int. The input width.
```

### Comparing `webcam-1.8/webcam.egg-info/PKG-INFO` & `webcam-1.9/webcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.8
+Version: 1.9
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

