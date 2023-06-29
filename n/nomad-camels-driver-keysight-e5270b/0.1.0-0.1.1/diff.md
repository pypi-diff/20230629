# Comparing `tmp/nomad_camels_driver_keysight_e5270b-0.1.0.tar.gz` & `tmp/nomad_camels_driver_keysight_e5270b-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels_driver_keysight_e5270b-0.1.0.tar", last modified: Wed Jun 28 13:33:58 2023, max compression
+gzip compressed data, was "nomad_camels_driver_keysight_e5270b-0.1.1.tar", last modified: Thu Jun 29 09:01:15 2023, max compression
```

## Comparing `nomad_camels_driver_keysight_e5270b-0.1.0.tar` & `nomad_camels_driver_keysight_e5270b-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:33:58.090653 nomad_camels_driver_keysight_e5270b-0.1.0/
--rw-rw-rw-   0        0        0    27028 2023-04-13 14:09:42.000000 nomad_camels_driver_keysight_e5270b-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      913 2023-06-28 13:33:58.088814 nomad_camels_driver_keysight_e5270b-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-24 10:18:28.000000 nomad_camels_driver_keysight_e5270b-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 13:33:58.069819 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/
--rw-rw-rw-   0        0        0    12846 2023-06-28 09:30:35.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b.py
--rw-rw-rw-   0        0        0     8775 2023-06-13 07:27:03.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config.py
--rw-rw-rw-   0        0        0     7882 2023-04-24 07:35:17.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config_channel.py
--rw-rw-rw-   0        0        0    33729 2023-06-28 09:30:35.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_ophyd.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:33:58.086787 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/
--rw-rw-rw-   0        0        0      913 2023-06-28 13:33:58.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-06-28 13:33:58.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:33:58.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 13:33:58.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2023-06-28 13:33:58.000000 nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      709 2023-06-28 13:24:48.000000 nomad_camels_driver_keysight_e5270b-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 13:33:58.090653 nomad_camels_driver_keysight_e5270b-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 09:01:15.710181 nomad_camels_driver_keysight_e5270b-0.1.1/
+-rw-rw-rw-   0        0        0    27028 2023-04-13 14:09:42.000000 nomad_camels_driver_keysight_e5270b-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      935 2023-06-29 09:01:15.710181 nomad_camels_driver_keysight_e5270b-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-28 14:25:08.000000 nomad_camels_driver_keysight_e5270b-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 09:01:15.700184 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/
+-rw-rw-rw-   0        0        0    12881 2023-06-29 08:57:43.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b.py
+-rw-rw-rw-   0        0        0     8775 2023-06-13 07:27:03.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config.py
+-rw-rw-rw-   0        0        0     7882 2023-04-24 07:35:17.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config_channel.py
+-rw-rw-rw-   0        0        0    33729 2023-06-28 09:30:35.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_ophyd.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:01:15.700184 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/
+-rw-rw-rw-   0        0        0      935 2023-06-29 09:01:15.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-06-29 09:01:15.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:01:15.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 09:01:15.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       36 2023-06-29 09:01:15.000000 nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      720 2023-06-29 09:00:24.000000 nomad_camels_driver_keysight_e5270b-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:01:15.710181 nomad_camels_driver_keysight_e5270b-0.1.1/setup.cfg
```

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/LICENSE.txt` & `nomad_camels_driver_keysight_e5270b-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/PKG-INFO` & `nomad_camels_driver_keysight_e5270b-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nomad_camels_driver_keysight_e5270b
-Version: 0.1.0
+Version: 0.1.1
 Summary: Device driver for the Keysight E5270B Precision IV Analyzer.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
-Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html
+Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NOMAD-CAMELS Driver for Keysight E5270B
 
 Driver of the Keysight E5270B written for the measurement software [NOMAD-CAMELS](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 
 ## Documentation
 
-For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html).
+For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html).
```

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b.py` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             config_dict.pop(r)
         return config_dict
 
     def get_channels(self):
         channels = copy.deepcopy(super().get_channels())
         removes = []
         for i in range(1, 9):
-            if not self.config[f'active{i}']:
+            if f'active{i}' not in self.config or not self.config[f'active{i}']:
                 for key in self.channels:
                     if key.endswith(str(i)):
                         removes.append(key)
         for r in removes:
             channels.pop(r)
         return channels
```

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config.py` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config_channel.py` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_config_channel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b/keysight_e5270b_ophyd.py` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b/keysight_e5270b_ophyd.py`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/PKG-INFO` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nomad-camels-driver-keysight-e5270b
-Version: 0.1.0
+Version: 0.1.1
 Summary: Device driver for the Keysight E5270B Precision IV Analyzer.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
-Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html
+Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # NOMAD-CAMELS Driver for Keysight E5270B
 
 Driver of the Keysight E5270B written for the measurement software [NOMAD-CAMELS](https://fau-lap.github.io/NOMAD-CAMELS/).
 
 
 ## Documentation
 
-For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html).
+For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html).
```

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/nomad_camels_driver_keysight_e5270b.egg-info/SOURCES.txt` & `nomad_camels_driver_keysight_e5270b-0.1.1/nomad_camels_driver_keysight_e5270b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels_driver_keysight_e5270b-0.1.0/pyproject.toml` & `nomad_camels_driver_keysight_e5270b-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels_driver_keysight_e5270b"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "Device driver for the Keysight E5270B Precision IV Analyzer."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
@@ -18,8 +18,8 @@
 dependencies = [
     "pyvisa",
     "pyvisa-py"
 ]
 
 [project.urls]
 "GitHub Page" = "https://github.com/FAU-LAP/NOMAD-CAMELS"
-"Documentation" = "https://fau-lap.github.io/NOMAD-CAMELS/docs/instruments.html"
+"Documentation" = "https://fau-lap.github.io/NOMAD-CAMELS/doc/instruments/instruments.html"
```

