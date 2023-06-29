# Comparing `tmp/gaitalytics-0.0.8b0.tar.gz` & `tmp/gaitalytics-0.0.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.0.8b0.tar", last modified: Wed Jun 28 13:11:04 2023, max compression
+gzip compressed data, was "gaitalytics-0.0.9b0.tar", last modified: Wed Jun 28 14:06:21 2023, max compression
```

## Comparing `gaitalytics-0.0.8b0.tar` & `gaitalytics-0.0.9b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 13:11:04.428912 gaitalytics-0.0.8b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.8b0/LICENSE
--rw-rw-rw-   0        0        0     1405 2023-06-28 13:11:04.428912 gaitalytics-0.0.8b0/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.8b0/README.md
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.0.8b0/pyproject.toml
--rw-rw-rw-   0        0        0      730 2023-06-28 13:11:04.428912 gaitalytics-0.0.8b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 13:11:04.375932 gaitalytics-0.0.8b0/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 13:11:04.414521 gaitalytics-0.0.8b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.0.8b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    22257 2023-06-28 07:52:44.000000 gaitalytics-0.0.8b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    12259 2023-06-28 13:10:13.000000 gaitalytics-0.0.8b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.0.8b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    13086 2023-06-28 07:52:44.000000 gaitalytics-0.0.8b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.8b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.0.8b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     7999 2023-06-28 10:09:03.000000 gaitalytics-0.0.8b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6139 2023-06-28 07:52:44.000000 gaitalytics-0.0.8b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0    14361 2023-06-28 08:00:17.000000 gaitalytics-0.0.8b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 13:11:04.428912 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     1405 2023-06-28 13:11:04.000000 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-28 13:11:04.000000 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 13:11:04.000000 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-28 13:11:04.000000 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 13:11:04.000000 gaitalytics-0.0.8b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.9b0/LICENSE
+-rw-rw-rw-   0        0        0     1405 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.9b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.0.9b0/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.892465 gaitalytics-0.0.9b0/src/
+drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.913998 gaitalytics-0.0.9b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.0.9b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    22257 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    12259 2023-06-28 13:10:13.000000 gaitalytics-0.0.9b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    13086 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.9b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.0.9b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     7999 2023-06-28 10:09:03.000000 gaitalytics-0.0.9b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6139 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0    14514 2023-06-28 14:05:27.000000 gaitalytics-0.0.9b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     1405 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.0.8b0/LICENSE` & `gaitalytics-0.0.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/PKG-INFO` & `gaitalytics-0.0.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gait_analysis
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaitalytics-0.0.8b0/README.md` & `gaitalytics-0.0.9b0/README.md`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/setup.cfg` & `gaitalytics-0.0.9b0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 3862  version = 0.0.8b
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 3962  version = 0.0.9b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
```

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/analysis.py` & `gaitalytics-0.0.9b0/src/gaitalytics/analysis.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/api.py` & `gaitalytics-0.0.9b0/src/gaitalytics/api.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/c3d.py` & `gaitalytics-0.0.9b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/cycle.py` & `gaitalytics-0.0.9b0/src/gaitalytics/cycle.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/emg.py` & `gaitalytics-0.0.9b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/events.py` & `gaitalytics-0.0.9b0/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/modelling.py` & `gaitalytics-0.0.9b0/src/gaitalytics/modelling.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/plot.py` & `gaitalytics-0.0.9b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics/utils.py` & `gaitalytics-0.0.9b0/src/gaitalytics/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,20 @@
             return f"{translated_label.name}.{point_type.name}.{direction.name}.{side.value}"
 
 
 class SubjectMeasures(yaml.YAMLObject):
     yaml_tag = u'!subject'
     yaml_loader = yaml.SafeLoader
 
-    def __init__(self, body_mass: float, body_height: float, left_leg_length: float, right_leg_length: float):
+    def __init__(self, body_mass: float, body_height: float, left_leg_length: float, right_leg_length: float, subject :str):
         self.body_mass = body_mass
         self.body_height = body_height
         self.left_leg_length = left_leg_length
         self.right_leg_length = right_leg_length
+        self.subject = subject
 
     def to_file(self, path_out: str):
         with open(f"{path_out}/subject.yml", "w") as f:
             yaml.dump(self, f)
 
     @staticmethod
     def from_file(file_path: str):
@@ -79,15 +80,16 @@
 
 
 def extract_subject(acq: btkAcquisition) -> SubjectMeasures:
     body_mass = acq.GetMetaData().GetChild("PROCESSING").GetChild("Bodymass").GetInfo().ToDouble()[0]
     body_height = acq.GetMetaData().GetChild("PROCESSING").GetChild("Height").GetInfo().ToDouble()[0]
     left_leg_length = acq.GetMetaData().GetChild("PROCESSING").GetChild("LLegLength").GetInfo().ToDouble()[0]
     right_leg_length = acq.GetMetaData().GetChild("PROCESSING").GetChild("RLegLength").GetInfo().ToDouble()[0]
-    subject = SubjectMeasures(body_mass, body_height, left_leg_length, right_leg_length)
+    name = acq.GetMetaData().GetChild("SUBJECTS").GetChild("NAMES").GetInfo().ToString()[0].strip()
+    subject = SubjectMeasures(body_mass, body_height, left_leg_length, right_leg_length, name)
     return subject
 
 
 class PointDataType(Enum):
     Marker = 0
     Angles = 1
     Forces = 2
```

### Comparing `gaitalytics-0.0.8b0/src/gaitalytics.egg-info/PKG-INFO` & `gaitalytics-0.0.9b0/src/gaitalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitalytics
-Version: 0.0.8b0
+Version: 0.0.9b0
 Summary: Library to analyse gait data captured with a mocap system
 Home-page: https://github.com/cereneo-foundation/gait_analysis
 Author: André Böni
 Author-email: andre.boeni@cereneo.foundation
 License: MIT
 Keywords: gait,analysis,c3d,mocap
 Classifier: Programming Language :: Python :: 3
```

