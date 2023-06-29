# Comparing `tmp/xobjects-0.2.6.tar.gz` & `tmp/xobjects-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xobjects-0.2.6.tar", last modified: Tue Jun  6 14:57:23 2023, max compression
+gzip compressed data, was "xobjects-0.2.7.tar", last modified: Thu Jun 29 15:32:27 2023, max compression
```

## Comparing `xobjects-0.2.6.tar` & `xobjects-0.2.7.tar`

### file list

```diff
@@ -1,51 +1,33 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.949040 xobjects-0.2.6/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.6/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-06 14:57:23.949144 xobjects-0.2.6/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.6/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-06-06 14:57:23.949625 xobjects-0.2.6/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1231 2023-03-23 11:04:29.000000 xobjects-0.2.6/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.932472 xobjects-0.2.6/tests/
--rw-r--r--   0 giadarol   (503) staff       (20)      724 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_align.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7262 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3641 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_buffer.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16680 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)      743 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_chunk.py
--rw-r--r--   0 giadarol   (503) staff       (20)     9220 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     7409 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_kernel.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2915 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_linked_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4614 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_nplike_arrays.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8856 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)      944 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_scalars.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1160 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_strides.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1264 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_string.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6677 2023-04-03 19:20:50.000000 xobjects-0.2.6/tests/test_struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)      692 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_to_json.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3202 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1540 2023-03-23 11:04:29.000000 xobjects-0.2.6/tests/test_unionref.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.946418 xobjects-0.2.6/xobjects/
--rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.6/xobjects/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/_patch_pyopencl_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-06 14:56:28.000000 xobjects-0.2.6/xobjects/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/array.py
--rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21990 2023-05-30 19:14:00.000000 xobjects-0.2.6/xobjects/context.py
--rw-r--r--   0 giadarol   (503) staff       (20)    28428 2023-06-06 14:53:24.000000 xobjects-0.2.6/xobjects/context_cpu.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23940 2023-03-29 07:05:06.000000 xobjects-0.2.6/xobjects/context_cupy.py
--rw-r--r--   0 giadarol   (503) staff       (20)    17221 2023-03-29 07:05:06.000000 xobjects-0.2.6/xobjects/context_pyopencl.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.6/xobjects/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12701 2023-06-06 14:53:24.000000 xobjects-0.2.6/xobjects/hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/linkedarray.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/scalar.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/specialize_source.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/string.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16447 2023-05-30 19:14:00.000000 xobjects-0.2.6/xobjects/struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.2.6/xobjects/test_helpers.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.6/xobjects/union.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:57:23.948888 xobjects-0.2.6/xobjects.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)     1022 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       27 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-06-06 14:57:23.000000 xobjects-0.2.6/xobjects.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-29 15:32:27.633958 xobjects-0.2.7/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.7/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-29 15:32:27.634052 xobjects-0.2.7/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.7/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-06-29 15:32:27.639800 xobjects-0.2.7/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1246 2023-06-29 15:31:45.000000 xobjects-0.2.7/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-29 15:32:27.632324 xobjects-0.2.7/xobjects/
+-rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.7/xobjects/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/_patch_pyopencl_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-29 15:31:58.000000 xobjects-0.2.7/xobjects/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21990 2023-05-30 19:14:00.000000 xobjects-0.2.7/xobjects/context.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    28693 2023-06-29 15:31:45.000000 xobjects-0.2.7/xobjects/context_cpu.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    24248 2023-06-29 15:31:45.000000 xobjects-0.2.7/xobjects/context_cupy.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    17376 2023-06-29 15:31:45.000000 xobjects-0.2.7/xobjects/context_pyopencl.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.7/xobjects/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12701 2023-06-06 14:53:24.000000 xobjects-0.2.7/xobjects/hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/linkedarray.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/scalar.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/specialize_source.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16447 2023-05-30 19:14:00.000000 xobjects-0.2.7/xobjects/struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.2.7/xobjects/test_helpers.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.7/xobjects/union.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-29 15:32:27.633786 xobjects-0.2.7/xobjects.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-06-29 15:32:27.000000 xobjects-0.2.7/xobjects.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      646 2023-06-29 15:32:27.000000 xobjects-0.2.7/xobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-29 15:32:27.000000 xobjects-0.2.7/xobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       39 2023-06-29 15:32:27.000000 xobjects-0.2.7/xobjects.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-06-29 15:32:27.000000 xobjects-0.2.7/xobjects.egg-info/top_level.txt
```

### Comparing `xobjects-0.2.6/LICENSE` & `xobjects-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/PKG-INFO` & `xobjects-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.6
+Version: 0.2.7
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.2.6/setup.py` & `xobjects-0.2.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,10 +29,10 @@
     download_url="https://pypi.python.org/pypi/xobjects",
     project_urls={
         "Bug Tracker": "https://github.com/xsuite/xsuite/issues",
         "Documentation": "https://xsuite.readthedocs.io/",
         "Source Code": "https://github.com/xsuite/xobjects",
     },
     extras_require={
-        "tests": ["pytest"],
+        "tests": ["pytest", "pytest-mock"],
     },
 )
```

### Comparing `xobjects-0.2.6/xobjects/__init__.py` & `xobjects-0.2.7/xobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/_patch_pyopencl_array.py` & `xobjects-0.2.7/xobjects/_patch_pyopencl_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/array.py` & `xobjects-0.2.7/xobjects/array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/capi.py` & `xobjects-0.2.7/xobjects/capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/context.py` & `xobjects-0.2.7/xobjects/context.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/context_cpu.py` & `xobjects-0.2.7/xobjects/context_cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import uuid
 from pathlib import Path
 from typing import Callable, Dict, List, Sequence, Tuple
 
 from .general import _print
 
 import numpy as np
+import scipy as sp
 
 from .context import (
     Kernel,
     ModuleNotAvailable,
     SourceType,
     XBuffer,
     XContext,
@@ -531,14 +532,24 @@
         Module containing all the numpy features. Numpy members should be accessed
         through ``nplike_lib`` to keep compatibility with the other contexts.
 
         """
 
         return np
 
+    @property
+    def splike_lib(self):
+        """
+        Module containing all the scipy features. Numpy members should be accessed
+        through ``splike_lib`` to keep compatibility with the other contexts.
+
+        """
+
+        return sp
+
     def synchronize(self):
         """
         Ensures that all computations submitted to the context are completed.
         No action is performed by this function in the CPU context. The method
         is provided so that the CPU context has an identical API to the GPU ones.
         """
         pass
```

### Comparing `xobjects-0.2.6/xobjects/context_cupy.py` & `xobjects-0.2.7/xobjects/context_cupy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 from .linkedarray import BaseLinkedArray
 from .specialize_source import specialize_source
 
 log = logging.getLogger(__name__)
 
 try:
     import cupy
+    import cupyx.scipy
+    import cupyx.scipy.interpolate
+    import cupyx.scipy.signal
+    import cupyx.scipy.special
+    import cupyx.scipy.stats
     from cupyx.scipy import fftpack as cufftp
 
     _enabled = True
 except ImportError:
     log.info("cupy is not installed, ContextCupy will not be available")
     cupy = ModuleNotAvailable(
         message=("cupy is not installed. " "ContextCupy is not available!")
@@ -496,14 +501,21 @@
     @property
     def nplike_lib(self):
         """
         Module containing all the numpy features supported by cupy.
         """
         return cupy
 
+    @property
+    def splike_lib(self):
+        """
+        Module containing all the scipy features supported by cupy.
+        """
+        return cupyx.scipy
+
     def synchronize(self):
         """
         Ensures that all computations submitted to the context are completed.
         Equivalent to ``cupy.cuda.stream.get_current_stream().synchronize()``
         """
         cupy.cuda.stream.get_current_stream().synchronize()
```

### Comparing `xobjects-0.2.6/xobjects/context_pyopencl.py` & `xobjects-0.2.7/xobjects/context_pyopencl.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,21 @@
     def nplike_lib(self):
         """
         Module containing all the numpy features supported by PyOpenCL (optionally
         with patches to operate with non-contiguous arrays).
         """
         return cla
 
+    @property
+    def splike_lib(self):
+        """
+        Scipy features are not available through openCL
+        """
+        raise NotImplementedError
+
     def synchronize(self):
         """
         Ensures that all computations submitted to the context are completed.
         No action is performed by this function in the Pyopencl context. The method
         is provided so that the Pyopencl context has an identical API to the Cupy one.
         """
         pass
```

### Comparing `xobjects-0.2.6/xobjects/hybrid_class.py` & `xobjects-0.2.7/xobjects/hybrid_class.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/linkedarray.py` & `xobjects-0.2.7/xobjects/linkedarray.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/ref.py` & `xobjects-0.2.7/xobjects/ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/scalar.py` & `xobjects-0.2.7/xobjects/scalar.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/specialize_source.py` & `xobjects-0.2.7/xobjects/specialize_source.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/string.py` & `xobjects-0.2.7/xobjects/string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/struct.py` & `xobjects-0.2.7/xobjects/struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/test_helpers.py` & `xobjects-0.2.7/xobjects/test_helpers.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/typeutils.py` & `xobjects-0.2.7/xobjects/typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects/union.py` & `xobjects-0.2.7/xobjects/union.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.6/xobjects.egg-info/PKG-INFO` & `xobjects-0.2.7/xobjects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.6
+Version: 0.2.7
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

