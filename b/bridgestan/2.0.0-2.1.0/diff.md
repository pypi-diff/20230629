# Comparing `tmp/bridgestan-2.0.0.tar.gz` & `tmp/bridgestan-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgestan-2.0.0.tar", last modified: Wed May  3 16:14:12 2023, max compression
+gzip compressed data, was "bridgestan-2.1.0.tar", last modified: Thu Jun 29 16:08:39 2023, max compression
```

## Comparing `bridgestan-2.0.0.tar` & `bridgestan-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 16:14:12.305067 bridgestan-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 16:13:14.000000 bridgestan-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/bridgestan/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 16:13:39.000000 bridgestan-2.0.0/bridgestan/__version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/bridgestan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 16:13:14.000000 bridgestan-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 16:14:12.305067 bridgestan-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 16:13:14.000000 bridgestan-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_stanmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-29 16:08:38.996098 bridgestan-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 16:06:07.000000 bridgestan-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.992098 bridgestan-2.1.0/bridgestan/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 16:08:01.000000 bridgestan-2.1.0/bridgestan/__version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25802 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 16:06:07.000000 bridgestan-2.1.0/bridgestan/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/bridgestan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 16:08:38.000000 bridgestan-2.1.0/bridgestan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 16:06:07.000000 bridgestan-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 16:08:38.996098 bridgestan-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 16:06:07.000000 bridgestan-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:38.996098 bridgestan-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25485 2023-06-29 16:06:07.000000 bridgestan-2.1.0/test/test_stanmodel.py
```

### Comparing `bridgestan-2.0.0/PKG-INFO` & `bridgestan-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.0.0/bridgestan/compile.py` & `bridgestan-2.1.0/bridgestan/compile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import platform
 import subprocess
 from pathlib import Path
 from typing import List
+import warnings
 
 from .__version import __version__
-from .download import CURRENT_BRIDGESTAN, get_bridgestan_src
+from .download import CURRENT_BRIDGESTAN, HOME_BRIDGESTAN, get_bridgestan_src
 from .util import validate_readable
 
 
 def verify_bridgestan_path(path: str) -> None:
     folder = Path(path).resolve()
     if not folder.exists():
         raise ValueError(
@@ -55,14 +56,20 @@
             verify_bridgestan_path(path)
         except ValueError:
             print(
                 "Bridgestan not found at location specified by $BRIDGESTAN "
                 f"environment variable, downloading version {__version__} to {path}"
             )
             get_bridgestan_src()
+            num_files = len(list(HOME_BRIDGESTAN.iterdir()))
+            if num_files >= 5:
+                warnings.warn(
+                    f"Found {num_files} different versions of Bridgestan in {HOME_BRIDGESTAN}. "
+                    "Consider deleting old versions to save space."
+                )
             print("Done!")
 
     return path
 
 
 def generate_so_name(model: Path):
     name = model.stem
```

### Comparing `bridgestan-2.0.0/bridgestan/download.py` & `bridgestan-2.1.0/bridgestan/download.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.0.0/bridgestan/model.py` & `bridgestan-2.1.0/bridgestan/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             if they were created *before* this model.
         :raises FileNotFoundError or PermissionError: If ``model_lib`` is not readable or
             ``model_data`` is specified and not a path to a readable file.
         :raises RuntimeError: If there is an error instantiating the
             model from C++.
         """
         validate_readable(model_lib)
-        if  model_data is not None and model_data.endswith(".json"):
+        if model_data is not None and model_data.endswith(".json"):
             validate_readable(model_data)
             with open(model_data, "r") as f:
                 model_data = f.read()
 
         self.lib_path = model_lib
         self.stanlib = ctypes.CDLL(self.lib_path)
```

### Comparing `bridgestan-2.0.0/bridgestan.egg-info/PKG-INFO` & `bridgestan-2.1.0/bridgestan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
```

### Comparing `bridgestan-2.0.0/test/test_compile.py` & `bridgestan-2.1.0/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.0.0/test/test_stanmodel.py` & `bridgestan-2.1.0/test/test_stanmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     np.testing.assert_equal("stdnormal_model", b.name())
 
 
 def test_model_info():
     std_so = str(STAN_FOLDER / "stdnormal" / "stdnormal_model.so")
     b = bs.StanModel(std_so)
     assert "STAN_OPENCL" in b.model_info()
-    assert "BridgeStan version: 1." in b.model_info()
+    assert "BridgeStan version: 2." in b.model_info()
 
 
 def test_param_num():
     full_so = str(STAN_FOLDER / "full" / "full_model.so")
     b = bs.StanModel(full_so)
     np.testing.assert_equal(1, b.param_num())
     np.testing.assert_equal(1, b.param_num(include_tp=False))
@@ -642,15 +642,16 @@
     pos = 0
     for n in range(1, 11):
         np.testing.assert_string_equal(names_unc[pos], f"Omega.{n}")
         pos += 1
 
 
 def test_stdout_capture():
-    import contextlib, io
+    import contextlib
+    import io
 
     theta = 0.1
 
     m = bs.StanModel(
         str(STAN_FOLDER / "print" / "print_model.so"), capture_stan_prints=False
     )
 
@@ -670,15 +671,16 @@
 
     lines = f.getvalue().splitlines()
     assert lines[0] == "Hello from Python!"
     assert lines[1] == "Hi from Stan!"
     assert lines[2] == f"theta = {theta}"
 
     # test re-entrancy
-    import ctypes, threading
+    import ctypes
+    import threading
 
     # define a new, sillier, callback which lets us test thread safety
     x = 0
 
     @ctypes.CFUNCTYPE(None, ctypes.POINTER(ctypes.c_char), ctypes.c_int)
     def callback(s, n):
         nonlocal x
@@ -706,15 +708,15 @@
     """Recompile simple_model with autodiff hessian enable, then clean-up/restore it after test"""
 
     stanfile = STAN_FOLDER / "simple" / "simple.stan"
     lib = bs.compile.generate_so_name(stanfile)
     lib.unlink(missing_ok=True)
     res = bs.compile_model(stanfile, make_args=["BRIDGESTAN_AD_HESSIAN=true"])
 
-    yield res
+    yield str(res)
 
     lib.unlink(missing_ok=True)
     bs.compile_model(stanfile, make_args=["STAN_THREADS=true"])
 
 
 @pytest.mark.ad_hessian
 def test_hessian_autodiff(recompile_simple):
```

