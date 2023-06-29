# Comparing `tmp/nexusformat-1.0.1.tar.gz` & `tmp/nexusformat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusformat-1.0.1.tar", last modified: Wed Mar 15 21:33:08 2023, max compression
+gzip compressed data, was "nexusformat-1.0.2.tar", last modified: Thu Jun 29 21:25:04 2023, max compression
```

## Comparing `nexusformat-1.0.1.tar` & `nexusformat-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.797746 nexusformat-1.0.1/
--rw-r--r--   0 rosborn  (938267710) 660979062      672 2022-12-02 18:44:50.000000 nexusformat-1.0.1/.gitattributes
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.755887 nexusformat-1.0.1/.github/
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.766970 nexusformat-1.0.1/.github/workflows/
--rw-r--r--   0 rosborn  (938267710) 660979062      616 2022-12-02 21:10:44.000000 nexusformat-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 rosborn  (938267710) 660979062      596 2022-12-02 18:44:50.000000 nexusformat-1.0.1/.gitignore
--rw-r--r--   0 rosborn  (938267710) 660979062     2380 2022-12-02 18:44:50.000000 nexusformat-1.0.1/COPYING
--rw-r--r--   0 rosborn  (938267710) 660979062     2750 2023-03-15 21:33:08.797960 nexusformat-1.0.1/PKG-INFO
--rw-r--r--   0 rosborn  (938267710) 660979062     1667 2022-12-02 18:44:50.000000 nexusformat-1.0.1/README.md
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.769750 nexusformat-1.0.1/conda-recipe/
--rw-r--r--   0 rosborn  (938267710) 660979062       51 2018-01-26 20:36:52.000000 nexusformat-1.0.1/conda-recipe/bld.bat
--rw-r--r--   0 rosborn  (938267710) 660979062      103 2018-01-26 20:36:52.000000 nexusformat-1.0.1/conda-recipe/build.sh
--rw-r--r--   0 rosborn  (938267710) 660979062      679 2023-03-15 20:15:34.000000 nexusformat-1.0.1/conda-recipe/meta.yaml
--rw-r--r--   0 rosborn  (938267710) 660979062      187 2022-12-02 18:44:50.000000 nexusformat-1.0.1/pyproject.toml
--rw-r--r--   0 rosborn  (938267710) 660979062     1568 2023-03-15 21:33:08.798721 nexusformat-1.0.1/setup.cfg
--rwxr-xr-x   0 rosborn  (938267710) 660979062      410 2022-12-02 18:44:50.000000 nexusformat-1.0.1/setup.py
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.757852 nexusformat-1.0.1/src/
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.772057 nexusformat-1.0.1/src/nexusformat/
--rw-r--r--   0 rosborn  (938267710) 660979062      395 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/__init__.py
--rw-r--r--   0 rosborn  (938267710) 660979062      160 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat/_version.py
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.780572 nexusformat-1.0.1/src/nexusformat/nexus/
--rw-r--r--   0 rosborn  (938267710) 660979062     1542 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/nexus/__init__.py
--rw-r--r--   0 rosborn  (938267710) 660979062     6160 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/nexus/completer.py
--rw-r--r--   0 rosborn  (938267710) 660979062     8339 2022-12-12 18:29:18.000000 nexusformat-1.0.1/src/nexusformat/nexus/lock.py
--rw-r--r--   0 rosborn  (938267710) 660979062    11754 2022-12-22 17:58:48.000000 nexusformat-1.0.1/src/nexusformat/nexus/plot.py
--rw-r--r--   0 rosborn  (938267710) 660979062   267793 2023-03-15 20:15:34.000000 nexusformat-1.0.1/src/nexusformat/nexus/tree.py
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.782942 nexusformat-1.0.1/src/nexusformat/notebooks/
--rw-r--r--   0 rosborn  (938267710) 660979062    17734 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/notebooks/nexusformat.ipynb
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.786576 nexusformat-1.0.1/src/nexusformat/scripts/
--rw-r--r--   0 rosborn  (938267710) 660979062        0 2014-12-17 16:52:32.000000 nexusformat-1.0.1/src/nexusformat/scripts/__init__.py
--rwxr-xr-x   0 rosborn  (938267710) 660979062      741 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/scripts/nexusformat.py
--rwxr-xr-x   0 rosborn  (938267710) 660979062     1492 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/scripts/nxconsolidate.py
--rwxr-xr-x   0 rosborn  (938267710) 660979062      986 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/scripts/nxdir.py
--rwxr-xr-x   0 rosborn  (938267710) 660979062     1436 2022-12-02 18:44:50.000000 nexusformat-1.0.1/src/nexusformat/scripts/nxduplicate.py
--rwxr-xr-x   0 rosborn  (938267710) 660979062     7538 2022-12-12 18:29:18.000000 nexusformat-1.0.1/src/nexusformat/scripts/nxstack.py
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.776661 nexusformat-1.0.1/src/nexusformat.egg-info/
--rw-r--r--   0 rosborn  (938267710) 660979062     2750 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/PKG-INFO
--rw-r--r--   0 rosborn  (938267710) 660979062     1126 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/SOURCES.txt
--rw-r--r--   0 rosborn  (938267710) 660979062        1 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/dependency_links.txt
--rw-r--r--   0 rosborn  (938267710) 660979062      257 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/entry_points.txt
--rw-r--r--   0 rosborn  (938267710) 660979062       47 2017-06-13 21:07:05.000000 nexusformat-1.0.1/src/nexusformat.egg-info/pbr.json
--rw-r--r--   0 rosborn  (938267710) 660979062       51 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/requires.txt
--rw-r--r--   0 rosborn  (938267710) 660979062       12 2023-03-15 21:33:08.000000 nexusformat-1.0.1/src/nexusformat.egg-info/top_level.txt
-drwxr-xr-x   0 rosborn  (938267710) 660979062        0 2023-03-15 21:33:08.797160 nexusformat-1.0.1/tests/
--rw-r--r--   0 rosborn  (938267710) 660979062     1476 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/conftest.py
--rw-r--r--   0 rosborn  (938267710) 660979062    12927 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_data.py
--rw-r--r--   0 rosborn  (938267710) 660979062     1409 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_entry_groups.py
--rw-r--r--   0 rosborn  (938267710) 660979062     3621 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_fields.py
--rw-r--r--   0 rosborn  (938267710) 660979062     2335 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_files.py
--rw-r--r--   0 rosborn  (938267710) 660979062     5117 2023-03-15 20:15:34.000000 nexusformat-1.0.1/tests/test_groups.py
--rw-r--r--   0 rosborn  (938267710) 660979062     7890 2022-12-12 18:29:18.000000 nexusformat-1.0.1/tests/test_links.py
--rw-r--r--   0 rosborn  (938267710) 660979062     4102 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_locks.py
--rw-r--r--   0 rosborn  (938267710) 660979062     1671 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_masks.py
--rw-r--r--   0 rosborn  (938267710) 660979062     1224 2022-12-02 18:44:50.000000 nexusformat-1.0.1/tests/test_paths.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.192444 nexusformat-1.0.2/
+-rw-r--r--   0 rosborn    (504) 660979062      672 2022-12-02 18:44:50.000000 nexusformat-1.0.2/.gitattributes
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.177369 nexusformat-1.0.2/.github/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.180510 nexusformat-1.0.2/.github/workflows/
+-rw-r--r--   0 rosborn    (504) 660979062      616 2022-12-02 21:10:44.000000 nexusformat-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 rosborn    (504) 660979062      596 2022-12-02 18:44:50.000000 nexusformat-1.0.2/.gitignore
+-rw-r--r--   0 rosborn    (504) 660979062     2380 2022-12-02 18:44:50.000000 nexusformat-1.0.2/COPYING
+-rw-r--r--   0 rosborn    (504) 660979062     2750 2023-06-29 21:25:04.192607 nexusformat-1.0.2/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     1667 2022-12-02 18:44:50.000000 nexusformat-1.0.2/README.md
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.182121 nexusformat-1.0.2/conda-recipe/
+-rw-r--r--   0 rosborn    (504) 660979062       51 2018-01-26 20:36:52.000000 nexusformat-1.0.2/conda-recipe/bld.bat
+-rw-r--r--   0 rosborn    (504) 660979062      103 2018-01-26 20:36:52.000000 nexusformat-1.0.2/conda-recipe/build.sh
+-rw-r--r--   0 rosborn    (504) 660979062      679 2023-06-27 18:23:19.000000 nexusformat-1.0.2/conda-recipe/meta.yaml
+-rw-r--r--   0 rosborn    (504) 660979062      187 2022-12-02 18:44:50.000000 nexusformat-1.0.2/pyproject.toml
+-rw-r--r--   0 rosborn    (504) 660979062     1568 2023-06-29 21:25:04.193226 nexusformat-1.0.2/setup.cfg
+-rwxr-xr-x   0 rosborn    (504) 660979062      410 2022-12-02 18:44:50.000000 nexusformat-1.0.2/setup.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.177751 nexusformat-1.0.2/src/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.182758 nexusformat-1.0.2/src/nexusformat/
+-rw-r--r--   0 rosborn    (504) 660979062      395 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062      160 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat/_version.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.185999 nexusformat-1.0.2/src/nexusformat/nexus/
+-rw-r--r--   0 rosborn    (504) 660979062     1542 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/nexus/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062     6255 2023-06-27 03:08:08.000000 nexusformat-1.0.2/src/nexusformat/nexus/completer.py
+-rw-r--r--   0 rosborn    (504) 660979062     8339 2022-12-12 18:29:18.000000 nexusformat-1.0.2/src/nexusformat/nexus/lock.py
+-rw-r--r--   0 rosborn    (504) 660979062    11754 2022-12-22 17:58:48.000000 nexusformat-1.0.2/src/nexusformat/nexus/plot.py
+-rw-r--r--   0 rosborn    (504) 660979062   267892 2023-06-29 19:16:15.000000 nexusformat-1.0.2/src/nexusformat/nexus/tree.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.187188 nexusformat-1.0.2/src/nexusformat/notebooks/
+-rw-r--r--   0 rosborn    (504) 660979062    17734 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/notebooks/nexusformat.ipynb
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.189227 nexusformat-1.0.2/src/nexusformat/scripts/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2014-12-17 16:52:32.000000 nexusformat-1.0.2/src/nexusformat/scripts/__init__.py
+-rwxr-xr-x   0 rosborn    (504) 660979062      741 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/scripts/nexusformat.py
+-rwxr-xr-x   0 rosborn    (504) 660979062     1492 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/scripts/nxconsolidate.py
+-rwxr-xr-x   0 rosborn    (504) 660979062      986 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/scripts/nxdir.py
+-rwxr-xr-x   0 rosborn    (504) 660979062     1436 2022-12-02 18:44:50.000000 nexusformat-1.0.2/src/nexusformat/scripts/nxduplicate.py
+-rwxr-xr-x   0 rosborn    (504) 660979062     7538 2022-12-12 18:29:18.000000 nexusformat-1.0.2/src/nexusformat/scripts/nxstack.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.184660 nexusformat-1.0.2/src/nexusformat.egg-info/
+-rw-r--r--   0 rosborn    (504) 660979062     2750 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     1126 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/SOURCES.txt
+-rw-r--r--   0 rosborn    (504) 660979062        1 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/dependency_links.txt
+-rw-r--r--   0 rosborn    (504) 660979062      257 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/entry_points.txt
+-rw-r--r--   0 rosborn    (504) 660979062       47 2017-06-13 21:07:05.000000 nexusformat-1.0.2/src/nexusformat.egg-info/pbr.json
+-rw-r--r--   0 rosborn    (504) 660979062       51 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/requires.txt
+-rw-r--r--   0 rosborn    (504) 660979062       12 2023-06-29 21:25:04.000000 nexusformat-1.0.2/src/nexusformat.egg-info/top_level.txt
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-06-29 21:25:04.192038 nexusformat-1.0.2/tests/
+-rw-r--r--   0 rosborn    (504) 660979062     1476 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/conftest.py
+-rw-r--r--   0 rosborn    (504) 660979062    12927 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_data.py
+-rw-r--r--   0 rosborn    (504) 660979062     1409 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_entry_groups.py
+-rw-r--r--   0 rosborn    (504) 660979062     3960 2023-05-08 21:26:19.000000 nexusformat-1.0.2/tests/test_fields.py
+-rw-r--r--   0 rosborn    (504) 660979062     2335 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_files.py
+-rw-r--r--   0 rosborn    (504) 660979062     5117 2023-03-15 20:15:34.000000 nexusformat-1.0.2/tests/test_groups.py
+-rw-r--r--   0 rosborn    (504) 660979062     7890 2022-12-12 18:29:18.000000 nexusformat-1.0.2/tests/test_links.py
+-rw-r--r--   0 rosborn    (504) 660979062     4102 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_locks.py
+-rw-r--r--   0 rosborn    (504) 660979062     1671 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_masks.py
+-rw-r--r--   0 rosborn    (504) 660979062     1224 2022-12-02 18:44:50.000000 nexusformat-1.0.2/tests/test_paths.py
```

### Comparing `nexusformat-1.0.1/.gitattributes` & `nexusformat-1.0.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/.github/workflows/ci.yml` & `nexusformat-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/.gitignore` & `nexusformat-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/COPYING` & `nexusformat-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/PKG-INFO` & `nexusformat-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusformat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API to access NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexusformat
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nexusformat-1.0.1/README.md` & `nexusformat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/conda-recipe/meta.yaml` & `nexusformat-1.0.2/conda-recipe/meta.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 package:
   name: nexusformat
-  version: "1.0.1"
+  version: "1.0.2"
 
 source:
   git_url: https://github.com/nexpy/nexusformat.git
-  git_tag: v1.0.1
+  git_tag: v1.0.2
 
 build:
   entry_points:
     - nxstack = nexusformat.scripts.nxstack:main
     - nxduplicate = nexusformat.scripts.nxduplicate:main
     - nexusformat = nexusformat.scripts.nexusformat:main
   number: 0
```

### Comparing `nexusformat-1.0.1/setup.cfg` & `nexusformat-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/nexus/__init__.py` & `nexusformat-1.0.2/src/nexusformat/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/nexus/completer.py` & `nexusformat-1.0.2/src/nexusformat/nexus/completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,19 @@
     command = re.split('[ !#$%&()*+,:;<=>?@^~]',
                        event.line)[-1].lstrip(punctuation)
     try:
         base = re_object_match.split(command)[1]
     except Exception:
         raise TryNext
 
-    if not isinstance(shell._ofind(base)['obj'], NXobject):
+    try:
+        obj = shell._ofind(base).obj
+    except AttributeError:
+        obj = shell._ofind(base).get('obj')
+    if not isinstance(obj, NXobject):
         raise TryNext
 
     try:
         return nxattr_completer(shell, command)
     except ValueError:
         pass
```

### Comparing `nexusformat-1.0.1/src/nexusformat/nexus/lock.py` & `nexusformat-1.0.2/src/nexusformat/nexus/lock.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/nexus/plot.py` & `nexusformat-1.0.2/src/nexusformat/nexus/plot.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/nexus/tree.py` & `nexusformat-1.0.2/src/nexusformat/nexus/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,19 +483,20 @@
                   not os.access(self._lockdir, os.W_OK)):
                 raise NeXusError(
                   f"Not permitted to create a lock file in '{self._lockdir}'")
             try:
                 self.acquire_lock()
                 self._file = self.h5.File(self._filename, mode, **kwargs)
                 self._file.close()
-                self.release_lock()
             except NeXusError as error:
                 raise error
             except Exception as error:
                 raise NeXusError(str(error))
+            finally:
+                self.release_lock()
 
     def __repr__(self):
         return (
           f'<NXFile "{Path(self._filename).name}" mode "{self._mode}">')
 
     def __getattr__(self, name):
         """Return an attribute of the h5py File if not defined by NXFile"""
@@ -3274,19 +3275,19 @@
                 step = self.nxdata[idx] - self.nxdata[idx-1]
                 if abs(diff/step) < 0.99:
                     idx = idx - 1
             except IndexError:
                 pass
         return int(np.clip(idx, 0, len(self.nxdata)-1))
 
-    def __array__(self):
+    def __array__(self, *args, **kwargs):
         """Cast the NXfield as a NumPy array."""
-        return np.asarray(self.nxdata)
+        return np.asarray(self.nxdata, *args, **kwargs)
 
-    def __array_wrap__(self, value):
+    def __array_wrap__(self, value, context=None):
         """Transform the array resulting from a ufunc to an NXfield."""
         return NXfield(value, name=self.nxname)
 
     def __int__(self):
         """Cast a scalar field as an integer."""
         return int(self.nxvalue)
 
@@ -4483,15 +4484,15 @@
         """
         if name.startswith('NX'):
             return self.component(name)
         elif name in self.entries:
             return self.entries[name]
         elif name in self.attrs:
             return self.attrs[name]
-        raise NeXusError("'"+name+"' not in "+self.nxpath)
+        raise AttributeError("'"+name+"' not in "+self.nxpath)
 
     def __setattr__(self, name, value):
         """Set an attribute as an object or regular Python attribute.
 
         Parameters
         ----------
         name : str
@@ -4863,16 +4864,16 @@
     def makelink(self, target, name=None, abspath=False):
         """Create a linked NXobject within the group.
 
         The root of the target and the child's group must be the same.
 
         Parameters
         ----------
-        target : str
-            Path to the parent object.
+        target : NXobject
+            Target object of the link.
         name : str, optional
             The name of the linked object, by default the same as the target.
         abspath : bool, optional
             True if the target is an absolute path, by default False
         """
         if isinstance(target, NXlink):
             raise NeXusError("Cannot link to an NXlink object")
@@ -5280,15 +5281,16 @@
 
         The value of the corresponding target attribute is returned, reading
         from the external file if necessary.
         """
         try:
             return getattr(self.nxlink, name)
         except Exception:
-            raise NeXusError(f"Cannot resolve the link to '{self._target}'")
+            raise AttributeError(
+                f"Cannot resolve the link to '{self._target}'")
 
     def __setattr__(self, name, value):
         """Set an attribute of the link target.
 
         This is not allowed when the target is in an external file.
 
         Parameters
```

### Comparing `nexusformat-1.0.1/src/nexusformat/notebooks/nexusformat.ipynb` & `nexusformat-1.0.2/src/nexusformat/notebooks/nexusformat.ipynb`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/scripts/nexusformat.py` & `nexusformat-1.0.2/src/nexusformat/scripts/nexusformat.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/scripts/nxconsolidate.py` & `nexusformat-1.0.2/src/nexusformat/scripts/nxconsolidate.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/scripts/nxdir.py` & `nexusformat-1.0.2/src/nexusformat/scripts/nxdir.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/scripts/nxduplicate.py` & `nexusformat-1.0.2/src/nexusformat/scripts/nxduplicate.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat/scripts/nxstack.py` & `nexusformat-1.0.2/src/nexusformat/scripts/nxstack.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/src/nexusformat.egg-info/PKG-INFO` & `nexusformat-1.0.2/src/nexusformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusformat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API to access NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexusformat
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nexusformat-1.0.1/src/nexusformat.egg-info/SOURCES.txt` & `nexusformat-1.0.2/src/nexusformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/conftest.py` & `nexusformat-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_data.py` & `nexusformat-1.0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_entry_groups.py` & `nexusformat-1.0.2/tests/test_entry_groups.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_fields.py` & `nexusformat-1.0.2/tests/test_fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -145,7 +145,22 @@
 def test_field_operations(peak1D):
 
     assert peak1D.sum() == peak1D.nxvalue.sum()
     assert np.isclose(peak1D.moment(1), 50.0, rtol=1e-3)
     assert np.isclose(peak1D.moment(2), 100.0, rtol=1e-3)
     assert np.isclose(peak1D.std(), 10.0, rtol=1e-3)
     assert np.isclose(peak1D.average(), peak1D.nxvalue.sum() / 101.0)
+
+
+@pytest.mark.parametrize(
+    "arr",
+    ["arr1D",
+     "arr2D",
+     "arr3D"])
+def test_numpy_conversion(arr, request):
+
+    arr = request.getfixturevalue(arr)
+    field = NXfield(arr)
+
+    assert np.array_equal(field, arr)
+    assert np.array_equal(np.array(field, dtype=np.float32), 
+                          arr.astype(np.float32))
```

### Comparing `nexusformat-1.0.1/tests/test_files.py` & `nexusformat-1.0.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_groups.py` & `nexusformat-1.0.2/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_links.py` & `nexusformat-1.0.2/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_locks.py` & `nexusformat-1.0.2/tests/test_locks.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_masks.py` & `nexusformat-1.0.2/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `nexusformat-1.0.1/tests/test_paths.py` & `nexusformat-1.0.2/tests/test_paths.py`

 * *Files identical despite different names*

