# Comparing `tmp/jwave-0.1.3.tar.gz` & `tmp/jwave-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwave-0.1.3.tar", max compression
+gzip compressed data, was "jwave-0.1.4.tar", max compression
```

## Comparing `jwave-0.1.3.tar` & `jwave-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rwxr-xr-x   0        0        0     7652 2023-06-28 09:22:58.524655 jwave-0.1.3/LICENSE
--rwxr-xr-x   0        0        0     5131 2023-06-28 09:22:58.524655 jwave-0.1.3/README.md
--rwxr-xr-x   0        0        0       19 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/__about__.py
--rwxr-xr-x   0        0        0      885 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/__init__.py
--rw-r--r--   0        0        0      768 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/__init__.py
--rw-r--r--   0        0        0     1951 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/conversion.py
--rw-r--r--   0        0        0    10119 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/operators.py
--rw-r--r--   0        0        0     4561 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/pml.py
--rwxr-xr-x   0        0        0     1186 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/spectral.py
--rw-r--r--   0        0        0    20569 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/time_harmonic.py
--rwxr-xr-x   0        0        0    19105 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/acoustics/time_varying.py
--rw-r--r--   0        0        0       85 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/extras/__init__.py
--rw-r--r--   0        0        0     3029 2023-06-28 09:22:58.560656 jwave-0.1.3/jwave/extras/export.py
--rwxr-xr-x   0        0        0    19433 2023-06-28 09:22:58.564656 jwave-0.1.3/jwave/geometry.py
--rwxr-xr-x   0        0        0     1423 2023-06-28 09:22:58.564656 jwave-0.1.3/jwave/phantoms.py
--rwxr-xr-x   0        0        0     8798 2023-06-28 09:22:58.564656 jwave-0.1.3/jwave/signal_processing.py
--rw-r--r--   0        0        0      835 2023-06-28 09:22:58.564656 jwave-0.1.3/jwave/transformations.py
--rwxr-xr-x   0        0        0     6265 2023-06-28 09:22:58.564656 jwave-0.1.3/jwave/utils.py
--rw-r--r--   0        0        0     2944 2023-06-28 09:22:58.564656 jwave-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 jwave-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2023-06-29 13:52:05.889147 jwave-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     5137 2023-06-29 13:52:05.889147 jwave-0.1.4/README.md
+-rwxr-xr-x   0        0        0      885 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/__init__.py
+-rw-r--r--   0        0        0     1951 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/conversion.py
+-rw-r--r--   0        0        0    10119 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/operators.py
+-rw-r--r--   0        0        0     4561 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/pml.py
+-rwxr-xr-x   0        0        0     1186 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/spectral.py
+-rw-r--r--   0        0        0    20569 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/time_harmonic.py
+-rwxr-xr-x   0        0        0    18960 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/acoustics/time_varying.py
+-rw-r--r--   0        0        0       85 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/extras/__init__.py
+-rw-r--r--   0        0        0     2455 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/extras/export.py
+-rwxr-xr-x   0        0        0    21345 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/geometry.py
+-rwxr-xr-x   0        0        0     1417 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/phantoms.py
+-rwxr-xr-x   0        0        0     9165 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/signal_processing.py
+-rwxr-xr-x   0        0        0     7368 2023-06-29 13:52:05.929145 jwave-0.1.4/jwave/utils.py
+-rw-r--r--   0        0        0     2926 2023-06-29 13:52:05.929145 jwave-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 jwave-0.1.4/PKG-INFO
```

### Comparing `jwave-0.1.3/LICENSE` & `jwave-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/README.md` & `jwave-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <img src="docs/assets/images/jwave_logo.png" alt="logo"></img>
 </div>
 
 # j-Wave: Differentiable acoustic simulations in JAX
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](LICENSE)
-[![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml)
+[![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/ci_tests.yml)
 [![codecov](https://codecov.io/gh/ucl-bug/jwave/branch/main/graph/badge.svg?token=6J03OMVJS1)](https://codecov.io/gh/ucl-bug/jwave)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ucl-bug/jwave/main?labpath=docs%2Fnotebooks%2Fivp%2Fhomogeneous_medium.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xAHAognF1v9un6GNvaGPSfdVeCDK8l9z?usp=sharing)
 
 [Install](#install) | [Tutorials](https://ucl-bug.github.io/jwave/notebooks/ivp/homogeneous_medium.html) | [Documentation](https://ucl-bug.github.io/jwave) | [Changelog](HISTORY.md)
 
 j-Wave is a library of simulators for acoustic applications. It is heavily inspired by [k-Wave](http://www.k-wave.org/)—a substantial portion of j-Wave is a port of k-Wave in JAX—and it's intended to be used as a collection of modular blocks that can be easily incorporated into any machine learning pipeline.
```

### Comparing `jwave-0.1.3/jwave/__init__.py` & `jwave-0.1.4/jwave/__init__.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/__init__.py` & `jwave-0.1.4/jwave/acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/conversion.py` & `jwave-0.1.4/jwave/acoustics/conversion.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/operators.py` & `jwave-0.1.4/jwave/acoustics/operators.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/pml.py` & `jwave-0.1.4/jwave/acoustics/pml.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/spectral.py` & `jwave-0.1.4/jwave/acoustics/spectral.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/time_harmonic.py` & `jwave-0.1.4/jwave/acoustics/time_harmonic.py`

 * *Files identical despite different names*

### Comparing `jwave-0.1.3/jwave/acoustics/time_varying.py` & `jwave-0.1.4/jwave/acoustics/time_varying.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from jaxdf.operators import (diag_jacobian, functional, shift_operator,
                              sum_over_dims)
 
 from jwave.acoustics.spectral import kspace_op
 from jwave.geometry import (Medium, MediumAllScalars, MediumOnGrid, Sources,
                             TimeAxis)
 from jwave.signal_processing import smooth
-from jwave.transformations import CheckpointType
 
 from .pml import td_pml_on_grid
 
 Any = TypeVar("Any")
 
 
 def _shift_rho(rho0, direction, dx):
@@ -325,15 +324,15 @@
     medium: MediumOnGrid,
     time_axis: TimeAxis,
     *,
     sources=None,
     sensors=None,
     u0=None,
     p0=None,
-    checkpoint: CheckpointType = CheckpointType.NONE,
+    checkpoint: bool = True,
     max_unroll_checkpoint: int = 10,
     smooth_initial=True,
     params=None,
 ):
     r"""Simulate the wave propagation operator.
 
     Args:
@@ -427,15 +426,15 @@
                                      c_ref=c_ref,
                                      dt=dt)
         rho = pml_rho * (pml_rho * rho + dt * drho)
 
         p = pressure_from_density(rho, medium)
         return [p, u, rho], sensors(p, u, rho)
 
-    if checkpoint == CheckpointType.STEP:
+    if checkpoint:
         scan_fun = jax_checkpoint(scan_fun)
 
     _, ys = scan(scan_fun, fields, output_steps)
 
     return ys
 
 
@@ -476,15 +475,15 @@
     medium: Union[MediumAllScalars, MediumOnGrid],
     time_axis: TimeAxis,
     *,
     sources=None,
     sensors=None,
     u0=None,
     p0=None,
-    checkpoint: CheckpointType = CheckpointType.NONE,
+    checkpoint: bool = True,
     max_unroll_checkpoint: int = 10,
     smooth_initial=True,
     params=None,
 ):
     r"""Simulates the wave propagation operator using the PSTD method. This
     implementation is equivalent to the `kspaceFirstOrderND` function in the
     k-Wave Toolbox.
@@ -585,15 +584,15 @@
                                      params=params["fourier"])
         rho = pml_rho * (pml_rho * rho + dt * drho)
 
         p = pressure_from_density(rho, medium)
         return [p, u, rho], sensors(p, u, rho)
 
     # Define the scanning function according to the checkpoint type
-    if checkpoint == CheckpointType.STEP:
+    if checkpoint:
         scan_fun = jax_checkpoint(scan_fun)
 
     _, ys = scan(scan_fun, fields, output_steps)
 
     return ys
```

### Comparing `jwave-0.1.3/jwave/extras/export.py` & `jwave-0.1.4/jwave/extras/export.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,78 +8,66 @@
 # j-Wave is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with j-Wave. If not, see <https://www.gnu.org/licenses/>.
+from typing import Union
 
-import os
-
-try:
-    import imageio
-    from tqdm import trange
-except ImportError:
-    raise ImportError(
-        "Please install imageio and tqdm to use use the extras module.")
-
-import matplotlib.pyplot as plt
+import numpy as np
 from jaxdf import Field
+from matplotlib import colormaps, colors
 
 
 def save_video(
     fields: Field,
     filename: str,
-    fps=30,
-    vmin=None,
-    vmax=None,
+    fps: int = 30,
+    vmin: Union[None, float] = None,
+    vmax: Union[None, float] = None,
     cmap="RdBu_r",
     aspect="equal",
+    codec="mp4v",
 ):
-    r"""Saves a video of the fields to an mp4 file. **Unix only**. It
-    requires ffmpeg and the package `imageio` to be installed.
+    try:
+        import cv2
+    except ImportError:
+        raise ImportError(
+            "Please install opencv-python to use the save_video function.")
+
+    try:
+        from tqdm import trange
+    except ImportError:
+        # Define a fallback function if tqdm is not available.
+        def trange(*args, **kwargs):
+            return range(*args, **kwargs)
+
+    # Define the colormap
+    cmap = colormaps[cmap]
+
+    # Define a video writer
+    fourcc = cv2.VideoWriter_fourcc(*codec)
+
+    # Assuming the field shape is known
+    frame_height, frame_width, _ = fields[0].on_grid.shape
+    writer = cv2.VideoWriter(filename, fourcc, fps,
+                             (frame_width, frame_height))
 
-    Args:
-      fields (Field): The fields to save. It needs to be a Field object
-        with a time dimension, represented as a leading index. It must be
-        therefore possible to iterate over the time dimension using
-        ``for field in fields``, or generally being able to access the
-        fields as ``fields[i]``.
-      filename (str): The name of the file to save the video to.
-      fps (int, optional): The number of frames per second. Defaults to 30.
-      vmin (float, optional): The minimum value of the color scale. If None,
-        the minimum value of the fields at each time step is used. Defaults
-        to None.
-      vmax (float, optional): The maximum value of the color scale. If None,
-        the maximum value of the fields at each time step is used. Defaults
-        to None.
-      cmap (str, optional): The matplotlib colormap to use. Defaults to
-        'RdBu_r'.
-      aspect (str, optional): The aspect ratio of the plot. Defaults to
-        'equal'.
-    """
-    # Make a temporary directory in /tmp
-    tmp_dir = os.path.join("/tmp", "jwave_video")
-
-    # Clean the directory if it exists
-    if os.path.exists(tmp_dir):
-        os.system(f"rm -rf {tmp_dir}")
-    os.mkdir(tmp_dir)
-
-    # Saves all images in the temporary director
     for i in trange(fields.params.shape[0]):
-        img_data = fields[i].on_grid
-        plt.imshow(img_data, cmap=cmap, vmin=vmin, vmax=vmax, aspect=aspect)
-        plt.colorbar()
-        # Save with leading zeros
-        plt.savefig(f"{tmp_dir}/frame_{i:08}.png")
-        plt.close()
-
-    # Create the video
-    writer = imageio.get_writer(filename, fps=fps)
-    for filename in sorted(os.listdir(tmp_dir)):
-        frame = imageio.imread(os.path.join(tmp_dir, filename))
-        writer.append_data(frame)
-    writer.close()
+        img_data = fields[i].on_grid[:, :, 0]
+        norm = colors.Normalize(vmin=vmin,
+                                vmax=vmax) if vmin and vmax else None
+        img_data = cmap(norm(img_data)) if norm else cmap(img_data)
+
+        # Convert from RGBA to BGR and ignore the alpha channel
+        img_data = cv2.cvtColor((img_data[:, :, :3] * 255).astype(np.uint8),
+                                cv2.COLOR_RGBA2BGR)
+
+        # If aspect ratio is not 'equal', resize the image according to the given aspect ratio
+        if aspect != 'equal':
+            aspect_ratio = tuple(map(int, aspect.split(':')))
+            img_data = cv2.resize(img_data, aspect_ratio)
+
+        writer.write(img_data)
 
-    # Clean up
-    os.system(f"rm -rf {tmp_dir}")
+    writer.release()
```

### Comparing `jwave-0.1.3/jwave/geometry.py` & `jwave-0.1.4/jwave/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with j-Wave. If not, see <https://www.gnu.org/licenses/>.
 
 import math
 from dataclasses import dataclass
 from typing import List, Tuple, Union
-from numpy.typing import ArrayLike
 
 import numpy as np
 from jax import numpy as jnp
 from jax.tree_util import register_pytree_node_class
 from jaxdf import Field, FourierSeries, OnGrid
 from jaxdf.geometry import Domain
 from jaxdf.operators import dot_product, functional
@@ -107,35 +106,35 @@
         all_params = [
             "domain", "sound_speed", "density", "attenuation", "pml_size"
         ]
         strings = list(map(lambda x: show_param(x), all_params))
         return "Medium:\n - " + "\n - ".join(strings)
 
 
-def _points_on_circle(n: int,
-                      radius: float,
-                      centre: Tuple[float, float],
-                      cast_int: bool = True,
-                      angle: float = 0.0,
-                      max_angle: float = 2 * np.pi):
+def points_on_circle(
+        n: int,
+        radius: float,
+        centre: Tuple[float, float],
+        cast_int: bool = True,
+        angle: float = 0.0,
+        max_angle: float = 2 * np.pi) -> Tuple[List[float], List[float]]:
     """
     Generate points on a circle.
 
     Args:
-    n (int): Number of points.
-    radius (float): Radius of the circle.
-    centre (tuple): Centre coordinates of the circle (x, y).
-    cast_int (bool, optional): If True, points will be rounded and converted to integers. Default is True.
-    angle (float, optional): Starting angle in radians. Default is 0.
-    max_angle (float, optional): Maximum angle to reach in radians. Default is 2*pi (full circle).
+        n (int): Number of points.
+        radius (float): Radius of the circle.
+        centre (tuple): Centre coordinates of the circle (x, y).
+        cast_int (bool, optional): If True, points will be rounded and converted to integers. Default is True.
+        angle (float, optional): Starting angle in radians. Default is 0.
+        max_angle (float, optional): Maximum angle to reach in radians. Default is 2*pi (full circle).
 
     Returns:
-    x, y (tuple): Lists of x and y coordinates of the points.
+        x, y (tuple): Lists of x and y coordinates of the points.
     """
-
     angles = np.linspace(0, max_angle, n, endpoint=False)
     x = (radius * np.cos(angles + angle) + centre[0]).tolist()
     y = (radius * np.sin(angles + angle) + centre[1]).tolist()
     if cast_int:
         x = list(map(int, x))
         y = list(map(int, y))
     return x, y
@@ -145,16 +144,16 @@
 class MediumType(Medium):
     """A type for Medium objects that depends on the discretization of its components"""
 
 
 @type_of.dispatch
 def type_of(m: Medium):
     return MediumType[type(m.sound_speed),
-    type(m.density),
-    type(m.attenuation)]
+                      type(m.density),
+                      type(m.attenuation)]
 
 
 MediumAllScalars = MediumType[object, object, object]
 """A type for Medium objects that have all scalar components"""
 
 MediumFourierSeries = Union[
     MediumType[FourierSeries, object, object],
@@ -167,43 +166,43 @@
     MediumType[OnGrid, object, object],
     MediumType[object, OnGrid, object],
     MediumType[object, object, OnGrid],
 ]
 """A type for Medium objects that have at least one OnGrid component"""
 
 
-def _unit_fibonacci_sphere(
+def unit_fibonacci_sphere(
         samples: int = 128) -> List[Tuple[float, float, float]]:
     """
     Generate evenly distributed points on the surface
     of a unit sphere using the Fibonacci Sphere method.
 
     From https://stackoverflow.com/questions/9600801/evenly-distributing-n-points-on-a-sphere
 
     Args:
-    samples (int, optional): The number of points to generate.
-        Default is 128.
+        samples (int, optional): The number of points to generate.
+            Default is 128.
 
     Returns:
-    points (list): A list of tuples representing the (x, y, z)
-        coordinates of the points on the sphere.
+        points (list): A list of tuples representing the (x, y, z)
+            coordinates of the points on the sphere.
     """
     points = []
-    phi = math.pi * (3.0 - math.sqrt(5.0))  # golden angle in radians
+    phi = math.pi * (3.0 - math.sqrt(5.0))    # golden angle in radians
     for i in range(samples):
-        y = 1 - (i / float(samples - 1)) * 2  # y goes from 1 to -1
-        radius = math.sqrt(1 - y * y)  # radius at y
-        theta = phi * i  # golden angle increment
+        y = 1 - (i / float(samples - 1)) * 2    # y goes from 1 to -1
+        radius = math.sqrt(1 - y * y)    # radius at y
+        theta = phi * i    # golden angle increment
         x = math.cos(theta) * radius
         z = math.sin(theta) * radius
         points.append((x, y, z))
     return points
 
 
-def _fibonacci_sphere(
+def fibonacci_sphere(
         n: int,
         radius: float,
         centre: Union[Tuple[float, float, float], np.ndarray],
         cast_int: bool = True) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Generate evenly distributed points on the surface of
     a sphere using the Fibonacci Sphere method.
@@ -215,44 +214,85 @@
         the center of the sphere.
     cast_int (bool, optional): If True, points will be rounded
         and converted to integers. Default is True.
 
     Returns:
     x, y, z (tuple): The x, y, and z coordinates of the points on the sphere.
     """
-    points = _unit_fibonacci_sphere(n)
+    points = unit_fibonacci_sphere(n)
     points = np.array(points)
     points = points * radius + centre
     if cast_int:
         points = points.astype(int)
     return points[:, 0], points[:, 1], points[:, 2]
 
 
-def _circ_mask(N, radius, centre):
+def circ_mask(N: Tuple[int, int], radius: float,
+              centre: Union[List[float], Tuple[float, float]]) -> np.ndarray:
+    """
+    Generate a 2D binary mask representing a circle within a 2D grid.
+
+    The mask is an ndarray of size N with 1s inside the circle (defined by a given
+    centre and radius) and 0s outside.
+
+    Args:
+        N (Tuple[int, int]): The shape of the output mask (size of the grid).
+            It should be in the format (x_size, y_size).
+        radius (float): The radius of the circle.
+        centre (Union[List[float], Tuple[float, float]]): The coordinates of
+            the centre of the circle in the format (x, y).
+
+    Returns:
+        mask (np.ndarray): The 2D mask as a numpy ndarray of integers.
+            The shape of the mask is N. Values inside the circle are 1, and values
+            outside the circle are 0.
+    """
     x, y = np.mgrid[0:N[0], 0:N[1]]
-    dist_from_centre = np.sqrt((x - centre[0]) ** 2 + (y - centre[1]) ** 2)
+    dist_from_centre = np.sqrt((x - centre[0])**2 + (y - centre[1])**2)
     mask = (dist_from_centre < radius).astype(int)
     return mask
 
 
-def _sphere_mask(N, radius, centre):
+def sphere_mask(
+        N: Tuple[int, int, int], radius: float,
+        centre: Union[List[float], Tuple[float, float, float]]) -> np.ndarray:
+    """
+    Generate a 3D binary mask representing a sphere within a 3D grid.
+
+    The mask is an ndarray of size N with 1s inside the sphere (defined by a given
+    centre and radius) and 0s outside.
+
+    Args:
+        N (Tuple[int, int, int]): The shape of the output mask (size of the grid).
+            It should be in the format (x_size, y_size, z_size).
+        radius (float): The radius of the sphere.
+        centre (Union[List[float], Tuple[float, float, float]]): The coordinates of the
+            centre of the sphere in the format (x, y, z).
+
+    Returns:
+        mask (np.ndarray): The 3D mask as a numpy ndarray of integers. The shape of
+            the mask is N. Values inside the sphere are 1, and values outside the
+            sphere are 0.
+    """
     x, y, z = np.mgrid[0:N[0], 0:N[1], 0:N[2]]
-    dist_from_centre = np.sqrt((x - centre[0]) ** 2 + (y - centre[1]) ** 2 +
-                               (z - centre[2]) ** 2)
+    dist_from_centre = np.sqrt((x - centre[0])**2 + (y - centre[1])**2 +
+                               (z - centre[2])**2)
     mask = (dist_from_centre < radius).astype(int)
     return mask
 
 
 @register_pytree_node_class
 class Sources:
     r"""Sources structure
 
     Attributes:
       positions (Tuple[List[int]): source positions
       signals (List[jnp.ndarray]): source signals
+      dt (float): time step
+      domain (Domain): domain
 
     !!! example
 
       ```python
       x_pos = [10,20,30,40]
       y_pos = [30,30,30,30]
       signal = jnp.sin(jnp.linspace(0,10,100))
@@ -324,15 +364,15 @@
         self.mask = mask
         self.signal = signal
         self.dt = dt
         self.domain = domain
 
     def tree_flatten(self):
         children = (self.mask, self.signal, self.dt)
-        aux = (self.domain,)
+        aux = (self.domain, )
         return (children, aux)
 
     @classmethod
     def tree_unflatten(cls, aux, children):
         mask, signal, dt = children
         domain = aux[0]
         a = cls(mask, signal, dt, domain)
@@ -427,15 +467,15 @@
     positions: Tuple[tuple]
 
     def __init__(self, positions):
         self.positions = positions
 
     def tree_flatten(self):
         children = None
-        aux = (self.positions,)
+        aux = (self.positions, )
         return (children, aux)
 
     @classmethod
     def tree_unflatten(cls, aux, children):
         positions = aux[0]
         return cls(positions)
 
@@ -458,52 +498,58 @@
         Args:
           u (Field): The field to be sampled.
         """
         if len(self.positions) == 1:
             return p.on_grid[self.positions[0]]
         elif len(self.positions) == 2:
             return p.on_grid[self.positions[0],
-            self.positions[1]]  # type: ignore
+                             self.positions[1]]    # type: ignore
         elif len(self.positions) == 3:
             return p.on_grid[self.positions[0], self.positions[1],
-            self.positions[2]]  # type: ignore
+                             self.positions[2]]    # type: ignore
         else:
             raise ValueError(
                 "Sensors positions must be 1, 2 or 3 dimensional. Not {}".
                 format(len(self.positions)))
 
 
-def _bli_function(x0: jnp.ndarray, x: jnp.ndarray, n: int, include_imag: bool = False) -> jnp.ndarray:
+def bli_function(x0: jnp.ndarray,
+                 x: jnp.ndarray,
+                 n: int,
+                 include_imag: bool = False) -> jnp.ndarray:
     """
     The function used to compute the band limited interpolation function.
 
     Args:
         x0 (jnp.ndarray): Position of the sensors along the axis.
         x (jnp.ndarray): Grid positions.
         n (int): Size of the grid
         include_imag (bool): Include the imaginary component?
 
     Returns:
-    jnp.ndarray: The values of the function at the grid positions.
+        jnp.ndarray: The values of the function at the grid positions.
     """
-    dx = jnp.where((x - x0[:, None]) == 0, 1, x - x0[:, None])  # https://github.com/google/jax/issues/1052
+    dx = jnp.where(
+        (x - x0[:, None]) == 0, 1,
+        x - x0[:, None])    # https://github.com/google/jax/issues/1052
     dx_nonzero = (x - x0[:, None]) != 0
 
     if n % 2 == 0:
         y = jnp.sin(jnp.pi * dx) / \
             jnp.tan(jnp.pi * dx / n) / n
         y -= jnp.sin(jnp.pi * x0[:, None]) * jnp.sin(jnp.pi * x) / n
         if include_imag:
             y += 1j * jnp.cos(jnp.pi * x0[:, None]) * jnp.sin(jnp.pi * x) / n
     else:
         y = jnp.sin(jnp.pi * dx) / \
             jnp.sin(jnp.pi * dx / n) / n
 
     # Deal with case of precisely on grid.
-    y = y * jnp.all(dx_nonzero, axis=1)[:, None] + (1 - dx_nonzero) * (~jnp.all(dx_nonzero, axis=1)[:, None])
+    y = y * jnp.all(dx_nonzero, axis=1)[:, None] + (1 - dx_nonzero) * (
+        ~jnp.all(dx_nonzero, axis=1)[:, None])
     return y
 
 
 @register_pytree_node_class
 class BLISensors:
     """ Band-limited interpolant (off-grid) sensors.
 
@@ -521,27 +567,27 @@
 
     def __init__(self, positions: Tuple[jnp.ndarray], n: Tuple[int]):
         self.positions = positions
         self.n = n
 
         # Calculate the band-limited interpolant weights if not provided.
         x = jnp.arange(n[0])[None]
-        self.bx = jnp.expand_dims(_bli_function(positions[0], x, n[0]),
+        self.bx = jnp.expand_dims(bli_function(positions[0], x, n[0]),
                                   axis=range(2, 2 + len(n)))
 
         if len(n) > 1:
             y = jnp.arange(n[1])[None]
-            self.by = jnp.expand_dims(_bli_function(positions[1], y, n[1]),
+            self.by = jnp.expand_dims(bli_function(positions[1], y, n[1]),
                                       axis=range(2, 2 + len(n) - 1))
         else:
             self.by = None
 
         if len(n) > 2:
             z = jnp.arange(n[2])[None]
-            self.bz = jnp.expand_dims(_bli_function(positions[2], z, n[2]),
+            self.bz = jnp.expand_dims(bli_function(positions[2], z, n[2]),
                                       axis=range(2, 2 + len(n) - 2))
         else:
             self.bz = None
 
     def tree_flatten(self):
         children = self.positions,
         aux = self.n,
@@ -590,15 +636,15 @@
     t_end: float
 
     def __init__(self, dt, t_end):
         self.dt = dt
         self.t_end = t_end
 
     def tree_flatten(self):
-        children = (None,)
+        children = (None, )
         aux = (self.dt, self.t_end)
         return (children, aux)
 
     @classmethod
     def tree_unflatten(cls, aux, children):
         dt, t_end = aux
         return cls(dt, t_end)
@@ -624,11 +670,11 @@
               it is automatically calculated as the time required to travel
               from one corner of the domain to the opposite one.
         """
         dt = cfl * min(medium.domain.dx) / functional(medium.sound_speed)(
             np.max)
         if t_end is None:
             t_end = np.sqrt(
-                sum((x[-1] - x[0]) ** 2
+                sum((x[-1] - x[0])**2
                     for x in medium.domain.spatial_axis)) / functional(
-                medium.sound_speed)(np.min)
+                        medium.sound_speed)(np.min)
         return TimeAxis(dt=float(dt), t_end=float(t_end))
```

### Comparing `jwave-0.1.3/jwave/phantoms.py` & `jwave-0.1.4/jwave/phantoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with j-Wave. If not, see <https://www.gnu.org/licenses/>.
 
 from jax import numpy as jnp
 
-from jwave.geometry import _circ_mask
+from jwave.geometry import circ_mask
 
 
 def three_circles(N: tuple) -> jnp.ndarray:
     """
     Generate a 3-circle phantom.
 
     Args:
@@ -27,14 +27,14 @@
 
     Returns:
         jnp.ndarray: The phantom.
     """
     assert len(N) == 2, "N must be of length 2"
 
     radius = sum(N) / float(len(N))
-    mask1 = _circ_mask(N, radius * 0.05,
-                       (int(N[0] / 2 + N[0] / 8), int(N[1] / 2)))
-    mask2 = _circ_mask(N, radius * 0.1,
-                       (int(N[0] / 2 - N[0] / 8), int(N[1] / 2 + N[1] / 6)))
-    mask3 = _circ_mask(N, radius * 0.15, (int(N[0] / 2), int(N[1] / 2)))
+    mask1 = circ_mask(N, radius * 0.05,
+                      (int(N[0] / 2 + N[0] / 8), int(N[1] / 2)))
+    mask2 = circ_mask(N, radius * 0.1,
+                      (int(N[0] / 2 - N[0] / 8), int(N[1] / 2 + N[1] / 6)))
+    mask3 = circ_mask(N, radius * 0.15, (int(N[0] / 2), int(N[1] / 2)))
     p0 = 5.0 * mask1 + 3.0 * mask2 + 4.0 * mask3
     return jnp.expand_dims(p0, -1)
```

### Comparing `jwave-0.1.3/jwave/signal_processing.py` & `jwave-0.1.4/jwave/signal_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,22 @@
     Returns:
         jnp.ndarray: Upsampled signal
     """
     if upsample == 1:
         return x
 
     def _single_upsample(x):
-        """adds zeros at appropriate cut values"""
         new_size = list(map(lambda x: x * upsample, x.shape))
         Fx = jnp.fft.fftshift(jnp.fft.fftn(x))
         new_Fx = jnp.zeros(new_size, dtype=Fx.dtype)
-        cuts = [int((upsample - 1) * x / 2 / upsample) for x in new_size]
-        slices = tuple([slice(cut, -cut) for cut in cuts])
+        cuts = [(new_dim - old_dim) // 2
+                for old_dim, new_dim in zip(Fx.shape, new_size)]
+        slices = tuple([
+            slice(cut, cut + old_dim) for cut, old_dim in zip(cuts, Fx.shape)
+        ])
         new_Fx = new_Fx.at[slices].set(Fx)
         return jnp.fft.ifftn(jnp.fft.ifftshift(new_Fx)) * (upsample**x.ndim)
 
     if discard_last:
         _single_upsample = vmap(_single_upsample, in_axes=(-1, ), out_axes=-1)
 
     return _single_upsample(x)
@@ -131,14 +133,22 @@
         dt (float): [description]
         center_freq (float): $f_0$
         warmup_cycles (float, optional): $\sigma$. Defaults to 3.
 
     Returns:
         jnp.ndarray: [description]
     """
+    # Raise ValueError if the center frequency is negative
+    if center_freq <= 0:
+        raise ValueError(
+            f"Center frequency must be positive, got {center_freq}")
+
+    # Raise an error if the signal is not 1D
+    if signal.ndim != 1:
+        raise ValueError(f"Signal must be 1D, got {signal.ndim}D")
 
     t = jnp.arange(signal.shape[0]) * dt
     period = 1 / center_freq
     ramp_length = warmup_cycles * period
     return signal * jnp.where(t < ramp_length, (t / ramp_length), 1.0)
 
 
@@ -172,15 +182,15 @@
 
     Returns:
         jnp.ndarray: [description]
     """
     return signal * jnp.exp(-((time - mu)**2) / sigma**2)
 
 
-def smoothing_filter(sample_input) -> Callable:
+def smoothing_filter(sample_input: jnp.ndarray) -> Callable:
     r"""Returns a smoothing filter based on the blackman window, which
     works on a signal similar to the one provided as input. The filter
     is amenable to jax transformations.
 
     Args:
         sample_input (jnp.ndarray): Example signal
 
@@ -200,15 +210,15 @@
             filter_kernel = jnp.fft.fftshift(jnp.outer(*axis))
         elif len(axis) == 3:
             filter_kernel_2d = jnp.outer(*axis[1:])
             third_component = jnp.expand_dims(jnp.expand_dims(axis[0], 1), 2)
             filter_kernel = third_component * filter_kernel_2d
 
     # Different filtering functions for real and complex data
-    if sample_input.dtype != jnp.complex64 or sample_input.dtype != jnp.complex128:
+    if sample_input.dtype != jnp.complex64 and sample_input.dtype != jnp.complex128:
         Fx = eval_shape(jnp.fft.rfft, sample_input)
         filter_kernel = filter_kernel[..., :Fx.shape[-1]]
 
         def smooth_fun(x):
             return jnp.fft.irfftn(filter_kernel * jnp.fft.rfftn(x)).real
 
     else:
```

### Comparing `jwave-0.1.3/jwave/utils.py` & `jwave-0.1.4/jwave/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with j-Wave. If not, see <https://www.gnu.org/licenses/>.
 
+import warnings
 from typing import Tuple, Union
 
 import numpy as np
 from jax import numpy as jnp
 from jaxdf import Field
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
@@ -108,46 +109,71 @@
 def is_numeric(x):
     """
     Check if x is a numeric value, including complex.
     """
     return isinstance(x, (int, float, complex))
 
 
-def plot_complex_field(field: Field, figsize=(15, 8), max_intensity=None):
+def display_complex_field(
+        field: Union[Field, jnp.ndarray, np.ndarray],
+        figsize: Tuple[int, int] = (15, 8),
+        max_intensity: Union[float, None] = None) -> Tuple[Figure, np.ndarray]:
     """
-    Plots a complex field.
+    Displays the real and absolute value of a complex field.
 
     Args:
-      field (jnp.ndarray): Complex field to plot.
-      figsize (tuple): Figure size.
-      max_intensity (float): Maximum intensity to plot.
-        Defaults to the maximum value in the field.
+      field (Union[Field, jnp.ndarray, np.ndarray]): Complex field to plot.
+      figsize (Tuple[int, int]): Figure size.
+      max_intensity (Union[float, None]): Maximum intensity to plot.
+        If None, the maximum intensity is set to the maximum absolute value of the field.
+        Defaults to None.
 
     Returns:
-      matplotlib.pyplot.figure: Figure object.
-      matplotlib.pyplot.axes: Axes object.
+      Tuple[matplotlib.pyplot.figure, matplotlib.pyplot.axes]: Tuple of Figure object and Axes object.
     """
     fig, axes = plt.subplots(1, 2, figsize=figsize)
     if isinstance(field, Field):
         field = field.on_grid
 
     if max_intensity is None:
         max_intensity = jnp.amax(jnp.abs(field))
 
-    axes[0].imshow(field.real,
-                   vmin=-max_intensity,
-                   vmax=max_intensity,
-                   cmap="seismic")
+    im1 = axes[0].imshow(field.real,
+                         vmin=-max_intensity,
+                         vmax=max_intensity,
+                         cmap="seismic")
     axes[0].set_title("Real wavefield")
-    axes[1].imshow(jnp.abs(field), vmin=0, vmax=max_intensity, cmap="magma")
+    im2 = axes[1].imshow(jnp.abs(field),
+                         vmin=0,
+                         vmax=max_intensity,
+                         cmap="magma")
     axes[1].set_title("Wavefield magnitude")
 
+    # Add colorbars
+    divider1 = make_axes_locatable(axes[0])
+    cax1 = divider1.append_axes("right", size="5%", pad=0.05)
+    plt.colorbar(im1, cax=cax1)
+
+    divider2 = make_axes_locatable(axes[1])
+    cax2 = divider2.append_axes("right", size="5%", pad=0.05)
+    plt.colorbar(im2, cax=cax2)
+
     return fig, axes
 
 
+def plot_complex_field(
+        field: Union[Field, jnp.ndarray, np.ndarray],
+        figsize: Tuple[int, int] = (15, 8),
+        max_intensity: Union[float, None] = None) -> Tuple[Figure, np.ndarray]:
+    warnings.warn(
+        "plot_complex_field is deprecated, use display_complex_field instead",
+        DeprecationWarning)
+    return display_complex_field(field, figsize, max_intensity)
+
+
 def show_field(
     x: Field,
     title: str = "",
     figsize: Tuple[int, int] = (8, 6),
     vmax: Union[float, int, None] = None,
     aspect: str = "auto",
 ):
```

### Comparing `jwave-0.1.3/pyproject.toml` & `jwave-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwave"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fast and differentiable acoustic simulations in JAX."
 authors = [
   "Antonio Stanziola <a.stanziola@ucl.ac.uk>",
   "Simon Arridge",
   "Ben T. Cox",
   "Bradley E. Treeby",
 ]
@@ -66,17 +66,16 @@
 mkdocs-jupyter = "^0.24.1"
 mkdocs-macros-plugin = "^1.0.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
 mkdocstrings-python = "^1.1.2"
 python-kacl = "^0.4.6"
 pymdown-extensions = "^10.0.1"
 plumkdocs = "0.0.2"
-imageio = "^2.31.1"
 tqdm = "^4.65.0"
-imageio-ffmpeg = "^0.4.8"
+opencv-python = "^4.7.0.72"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tools.isort]
 src_paths = ["jwave", "tests"]
```

### Comparing `jwave-0.1.3/PKG-INFO` & `jwave-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwave
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fast and differentiable acoustic simulations in JAX.
 License: LGPL-3.0-only
 Keywords: jax,acoustics,simulation,ultrasound,differentiable-programming
 Author: Antonio Stanziola
 Author-email: a.stanziola@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: GPU
@@ -40,15 +40,15 @@
 <img src="docs/assets/images/jwave_logo.png" alt="logo"></img>
 </div>
 
 # j-Wave: Differentiable acoustic simulations in JAX
 
 [![Support](https://dcbadge.vercel.app/api/server/VtUb4fFznt?style=flat)](https://discord.gg/VtUb4fFznt)
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](LICENSE)
-[![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/tests.yml)
+[![Continous Integration](https://github.com/ucl-bug/jwave/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/ucl-bug/jwave/actions/workflows/ci_tests.yml)
 [![codecov](https://codecov.io/gh/ucl-bug/jwave/branch/main/graph/badge.svg?token=6J03OMVJS1)](https://codecov.io/gh/ucl-bug/jwave)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ucl-bug/jwave/main?labpath=docs%2Fnotebooks%2Fivp%2Fhomogeneous_medium.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1xAHAognF1v9un6GNvaGPSfdVeCDK8l9z?usp=sharing)
 
 [Install](#install) | [Tutorials](https://ucl-bug.github.io/jwave/notebooks/ivp/homogeneous_medium.html) | [Documentation](https://ucl-bug.github.io/jwave) | [Changelog](HISTORY.md)
 
 j-Wave is a library of simulators for acoustic applications. It is heavily inspired by [k-Wave](http://www.k-wave.org/)—a substantial portion of j-Wave is a port of k-Wave in JAX—and it's intended to be used as a collection of modular blocks that can be easily incorporated into any machine learning pipeline.
```

