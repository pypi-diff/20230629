# Comparing `tmp/vhs-0.0.2.tar.gz` & `tmp/vhs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhs-0.0.2.tar", last modified: Thu Jun 29 13:17:22 2023, max compression
+gzip compressed data, was "vhs-0.0.3.tar", last modified: Thu Jun 29 15:51:17 2023, max compression
```

## Comparing `vhs-0.0.2.tar` & `vhs-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.101917 vhs-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.093917 vhs-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-29 13:17:11.000000 vhs-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 13:17:11.000000 vhs-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 13:17:11.000000 vhs-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 13:17:11.000000 vhs-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 13:17:22.097917 vhs-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 13:17:11.000000 vhs-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/docs/source/_extra/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 13:17:11.000000 vhs-0.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 13:17:11.000000 vhs-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:17:22.101917 vhs-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 13:17:11.000000 vhs-0.0.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-29 13:17:11.000000 vhs-0.0.2/test/test_vhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/vhs/
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-29 13:17:11.000000 vhs-0.0.2/vhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:17:21.000000 vhs-0.0.2/vhs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:11.000000 vhs-0.0.2/vhs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:17:22.097917 vhs-0.0.2/vhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 13:17:22.000000 vhs-0.0.2/vhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.940033 vhs-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.932033 vhs-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-29 15:51:04.000000 vhs-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-29 15:51:04.000000 vhs-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 15:51:04.000000 vhs-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 15:51:04.000000 vhs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 15:51:17.940033 vhs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-29 15:51:04.000000 vhs-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-29 15:51:04.000000 vhs-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-29 15:51:04.000000 vhs-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/docs/source/_extra/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 15:51:04.000000 vhs-0.0.3/docs/source/_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-29 15:51:04.000000 vhs-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 15:51:04.000000 vhs-0.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 15:51:04.000000 vhs-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:51:17.940033 vhs-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-29 15:51:04.000000 vhs-0.0.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-29 15:51:04.000000 vhs-0.0.3/test/test_vhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.936033 vhs-0.0.3/vhs/
+-rw-r--r--   0 runner    (1001) docker     (123)    22762 2023-06-29 15:51:04.000000 vhs-0.0.3/vhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:04.000000 vhs-0.0.3/vhs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:51:17.940033 vhs-0.0.3/vhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 15:51:17.000000 vhs-0.0.3/vhs.egg-info/top_level.txt
```

### Comparing `vhs-0.0.2/.github/workflows/ci.yaml` & `vhs-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/.gitignore` & `vhs-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/LICENSE` & `vhs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/PKG-INFO` & `vhs-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Write terminal GIFs as code for integration testing and demoing your CLI tools, now with python
 Author-email: Tamika Nomara <taminomara@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tamika Nomara
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vhs-0.0.2/README.md` & `vhs-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/docs/Makefile` & `vhs-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/docs/make.bat` & `vhs-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/docs/source/conf.py` & `vhs-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/pyproject.toml` & `vhs-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/test/test_vhs.py` & `vhs-0.0.3/test/test_vhs.py`

 * *Files identical despite different names*

### Comparing `vhs-0.0.2/vhs/__init__.py` & `vhs-0.0.3/vhs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,50 +24,53 @@
 Then resolve VHS binary and run it:
 
 .. code-block:: python
 
     import vhs
 
     vhs_runner = vhs.resolve()
-    vhs_runner.run('./example.tape', './example.gif')
+    vhs_runner.run("./example.tape", "./example.gif")
 
 
 Reference
 ---------
 
 The entry point of the package is the :func:`resolve` function.
 It searches for an installed VHS, checks its version, downloads
 a new one if necessary, and returns a :class:`Vhs` object
 through which you can invoke the found VHS binary:
 
 .. autofunction:: resolve
 
+.. autofunction:: default_cache_path
+
 .. autoclass:: Vhs
    :members:
 
 In case of an error, VHS raises a :class:`VhsError` or its subclass:
 
 .. autoclass:: VhsError
 
 .. autoclass:: VhsRunError
 
 By default, the :func:`resolve` function silently detects or installs VHS,
 without printing anything (it may emit warning log messages
-to the ``'vhs'`` logger).
+to the ``"vhs"`` logger).
 
 You can display installation progress by passing a :class:`ProgressReporter`.
 Specifically, there's :class:`DefaultProgressReporter` which will cover
 most basic cases:
 
 .. autoclass:: ProgressReporter
    :members:
 
 .. autoclass:: DefaultProgressReporter
 
 """
+
 import datetime
 import logging
 import os
 import pathlib
 import platform
 import re
 import shutil
@@ -355,15 +358,15 @@
     def write(self, msg: str):
         self.stream.write(msg)
         self.stream.flush()
 
 
 def resolve(
     *,
-    cache_path: _t.Optional[pathlib.Path] = None,
+    cache_path: _t.Optional[_PathLike] = None,
     min_version: str = "0.5.0",
     quiet: bool = True,
     env: _t.Optional[_t.Dict[str, str]] = None,
     cwd: _t.Optional[_PathLike] = None,
     install: bool = True,
     reporter: ProgressReporter = ProgressReporter(),
     timeout: int = 15,
@@ -405,15 +408,15 @@
         resolved VHS installation.
     :raises VhsError:
         VHS not available or installation failed.
 
     """
 
     if cache_path is None:
-        cache_path = pathlib.Path(tempfile.gettempdir()) / "python_vhs_cache"
+        cache_path = default_cache_path()
     else:
         cache_path = pathlib.Path(cache_path)
 
     _logger.debug("using vhs cache path: %s", cache_path)
 
     if retry is None:
         retry = urllib3.Retry(10, backoff_factor=0.1)
@@ -431,14 +434,25 @@
         _path=path,
         _quiet=quiet,
         _env=env,
         _cwd=cwd,
     )
 
 
+def default_cache_path() -> pathlib.Path:
+    """
+    Return default path where VHS binaries should be downloaded to.
+
+    Currently it is equal to ``pathlib.Path(tempfile.gettempdir()) / "python_vhs_cache"``.
+
+    """
+
+    return pathlib.Path(tempfile.gettempdir()) / "python_vhs_cache"
+
+
 def _get_path(env: _t.Optional[_t.Dict[str, str]]) -> str:
     path = (env or {}).get("PATH", None)
     if path is None:
         path = os.environ.get("PATH", None)
     if path is None:
         try:
             path = os.confstr("CS_PATH")  # type: ignore
```

### Comparing `vhs-0.0.2/vhs.egg-info/PKG-INFO` & `vhs-0.0.3/vhs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vhs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Write terminal GIFs as code for integration testing and demoing your CLI tools, now with python
 Author-email: Tamika Nomara <taminomara@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tamika Nomara
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

