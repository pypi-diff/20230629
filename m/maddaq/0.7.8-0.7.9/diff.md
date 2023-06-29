# Comparing `tmp/maddaq-0.7.8.tar.gz` & `tmp/maddaq-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.8.tar", last modified: Mon Jun 19 14:59:29 2023, max compression
+gzip compressed data, was "maddaq-0.7.9.tar", last modified: Thu Jun 29 14:19:24 2023, max compression
```

## Comparing `maddaq-0.7.8.tar` & `maddaq-0.7.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.339249 maddaq-0.7.8/
--rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-19 14:59:29.338836 maddaq-0.7.8/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4786 2023-06-19 14:58:03.000000 maddaq-0.7.8/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.332092 maddaq-0.7.8/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.8/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7804 2023-05-25 17:24:23.000000 maddaq-0.7.8/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.8/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.8/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.8/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-05-29 09:45:06.000000 maddaq-0.7.8/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.338255 maddaq-0.7.8/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.8/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.8/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.8/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.8/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     9493 2023-05-29 09:52:27.000000 maddaq-0.7.8/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.8/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.8/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-19 14:59:29.334849 maddaq-0.7.8/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-06-19 14:59:29.000000 maddaq-0.7.8/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-05-29 09:45:06.000000 maddaq-0.7.8/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-06-19 14:59:29.339385 maddaq-0.7.8/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-29 14:19:24.889883 maddaq-0.7.9/
+-rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-29 14:19:24.889503 maddaq-0.7.9/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4786 2023-06-19 14:58:03.000000 maddaq-0.7.9/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-29 14:19:24.883703 maddaq-0.7.9/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.9/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7804 2023-05-25 17:24:23.000000 maddaq-0.7.9/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.9/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.9/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.9/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      482 2023-06-29 14:19:19.000000 maddaq-0.7.9/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-29 14:19:24.888924 maddaq-0.7.9/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.9/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.9/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.9/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.9/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    10022 2023-06-29 14:11:18.000000 maddaq-0.7.9/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.9/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.9/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-06-29 14:19:24.885844 maddaq-0.7.9/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     5220 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-06-29 14:19:24.000000 maddaq-0.7.9/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-06-29 14:13:25.000000 maddaq-0.7.9/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-06-29 14:19:24.889998 maddaq-0.7.9/setup.cfg
```

### Comparing `maddaq-0.7.8/PKG-INFO` & `maddaq-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.8
+Version: 0.7.9
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.8/README.md` & `maddaq-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/GTimer.py` & `maddaq-0.7.9/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/MadDAQData.py` & `maddaq-0.7.9/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/MadDAQModule.py` & `maddaq-0.7.9/maddaq/MadDAQModule.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/Progress.py` & `maddaq-0.7.9/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/ScanManager.py` & `maddaq-0.7.9/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.9/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/cmmds/file_info.py` & `maddaq-0.7.9/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.9/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.9/maddaq/cmmds/getSpectrum.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,16 @@
         if options.mid in keys:
             mid = options.mid
         else:
             mid = keys[0]
 
         print("\n## Looking at data from module {}.".format(mid))
         md = maddaq.modules[mid]
+        md.seed_cut = options.seed_cut
+        md.neigh_cut = options.neigh_cut
 
         # Show pedeswtals and noise
         if options.show_ped:
             show_pedestals(md)
 
         # Create the iterator
         if options.scan_point is not None:
@@ -182,15 +184,15 @@
         prg = ShowProgress(maddaq.nevts, width=24)
         prg.start()
 
         for evt in maddaq_iter:
             data = md.process_event(evt)
             if data is not None:
                 for C, E in data:
-                    if E > options.thrs:
+                    if E > options.thrs and E < options.max_E:
                         amplitude.append(E)
 
             prg.increase(show=True)
 
         amplitudes.append(get_E(amplitude))
         prg.stop()
         print("")
@@ -290,20 +292,25 @@
                         action=CommaSeparatedListAction,
                         help="Event number to start showing")
     parser.add_argument("--scan-point", dest="scan_point", type=int, default=None,
                         help="Scan point number to visit")
     parser.add_argument("--nbin", default=50, type=int, help="Number of bins in histogram.")
     parser.add_argument("--logY", default=False, action="store_true", help="Log axis")
     parser.add_argument("--thrs", default=0.0, type=float, help="Min E to show in histogram")
+    parser.add_argument("--max_E", default=sys.float_info.max, type=float, help="Max E to show in histogram")
     parser.add_argument("--two_peaks", default=False, action="store_true", help="Min E to show in histogram")
     parser.add_argument("--no-fit", dest="fit", default=True, action="store_false")
     parser.add_argument("--show-ped", action="store_true", default=False, dest="show_ped")
     parser.add_argument("--mid", dest="mid", default=-1, type=int, help="The module ID")
     parser.add_argument("--calib", default=None, help="The energy calibration file. X:adc, Y:energy")
     parser.add_argument("--time", default=False, action="store_true", help="Normalize to duration of run when reading various files")
+    parser.add_argument("--seed_cut", dest="seed_cut", default=3.5, type=float,
+                        help="Threshold of charge for a cluster seed")
+    parser.add_argument("--neigh_cut", dest="neigh_cut", default=1.5, type=float,
+                        help="Threshold of charge to add a neighbour to a cluster")
 
     options = parser.parse_args()
 
     if len(options.files) == 0:
         print("I need an input file")
         sys.exit()
```

### Comparing `maddaq-0.7.8/maddaq/cmmds/read_data.py` & `maddaq-0.7.9/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq/cmmds/show_data.py` & `maddaq-0.7.9/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.9/maddaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.8
+Version: 0.7.9
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.8/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.9/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.8/pyproject.toml` & `maddaq-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

