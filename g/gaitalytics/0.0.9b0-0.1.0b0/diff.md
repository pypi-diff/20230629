# Comparing `tmp/gaitalytics-0.0.9b0.tar.gz` & `tmp/gaitalytics-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitalytics-0.0.9b0.tar", last modified: Wed Jun 28 14:06:21 2023, max compression
+gzip compressed data, was "gaitalytics-0.1.0b0.tar", last modified: Thu Jun 29 09:25:02 2023, max compression
```

## Comparing `gaitalytics-0.0.9b0.tar` & `gaitalytics-0.1.0b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/
--rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.0.9b0/LICENSE
--rw-rw-rw-   0        0        0     1405 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-06-21 04:53:15.000000 gaitalytics-0.0.9b0/README.md
--rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.0.9b0/pyproject.toml
--rw-rw-rw-   0        0        0      730 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.892465 gaitalytics-0.0.9b0/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.913998 gaitalytics-0.0.9b0/src/gaitalytics/
--rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.0.9b0/src/gaitalytics/__init__.py
--rw-rw-rw-   0        0        0    22257 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/analysis.py
--rw-rw-rw-   0        0        0    12259 2023-06-28 13:10:13.000000 gaitalytics-0.0.9b0/src/gaitalytics/api.py
--rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/c3d.py
--rw-rw-rw-   0        0        0    13086 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/cycle.py
--rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.0.9b0/src/gaitalytics/emg.py
--rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.0.9b0/src/gaitalytics/events.py
--rw-rw-rw-   0        0        0     7999 2023-06-28 10:09:03.000000 gaitalytics-0.0.9b0/src/gaitalytics/modelling.py
--rw-rw-rw-   0        0        0     6139 2023-06-28 07:52:44.000000 gaitalytics-0.0.9b0/src/gaitalytics/plot.py
--rw-rw-rw-   0        0        0    14514 2023-06-28 14:05:27.000000 gaitalytics-0.0.9b0/src/gaitalytics/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 14:06:21.923509 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/
--rw-rw-rw-   0        0        0     1405 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 14:06:21.000000 gaitalytics-0.0.9b0/src/gaitalytics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/
+-rw-rw-rw-   0        0        0     1096 2023-04-25 17:34:59.000000 gaitalytics-0.1.0b0/LICENSE
+-rw-rw-rw-   0        0        0     5555 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     5031 2023-06-29 08:31:56.000000 gaitalytics-0.1.0b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-06-21 07:51:06.000000 gaitalytics-0.1.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0      728 2023-06-29 09:25:02.038627 gaitalytics-0.1.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.003369 gaitalytics-0.1.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.019876 gaitalytics-0.1.0b0/src/gaitalytics/
+-rw-rw-rw-   0        0        0        0 2023-06-21 08:57:09.000000 gaitalytics-0.1.0b0/src/gaitalytics/__init__.py
+-rw-rw-rw-   0        0        0    27232 2023-06-29 07:53:14.000000 gaitalytics-0.1.0b0/src/gaitalytics/analysis.py
+-rw-rw-rw-   0        0        0    12671 2023-06-29 07:53:14.000000 gaitalytics-0.1.0b0/src/gaitalytics/api.py
+-rw-rw-rw-   0        0        0     3226 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/c3d.py
+-rw-rw-rw-   0        0        0    13086 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/cycle.py
+-rw-rw-rw-   0        0        0     3340 2023-06-20 15:51:04.000000 gaitalytics-0.1.0b0/src/gaitalytics/emg.py
+-rw-rw-rw-   0        0        0    15989 2023-06-28 13:09:43.000000 gaitalytics-0.1.0b0/src/gaitalytics/events.py
+-rw-rw-rw-   0        0        0     8394 2023-06-29 09:07:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/modelling.py
+-rw-rw-rw-   0        0        0     6139 2023-06-28 07:52:44.000000 gaitalytics-0.1.0b0/src/gaitalytics/plot.py
+-rw-rw-rw-   0        0        0    14514 2023-06-28 14:05:27.000000 gaitalytics-0.1.0b0/src/gaitalytics/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:25:02.034889 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/
+-rw-rw-rw-   0        0        0     5555 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 09:25:01.000000 gaitalytics-0.1.0b0/src/gaitalytics.egg-info/top_level.txt
```

### Comparing `gaitalytics-0.0.9b0/LICENSE` & `gaitalytics-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/setup.cfg` & `gaitalytics-0.1.0b0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6169 7461 6c79 7469 6373 0d0a   = gaitalytics..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 3962  version = 0.0.9b
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 3062  version = 0.1.0b
 00000030: 6574 610d 0a61 7574 686f 7220 3d20 416e  eta..author = An
 00000040: 6472 c3a9 2042 c3b6 6e69 0d0a 6175 7468  dr.. B..ni..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6e64 7265  or_email = andre
 00000060: 2e62 6f65 6e69 4063 6572 656e 656f 2e66  .boeni@cereneo.f
 00000070: 6f75 6e64 6174 696f 6e0d 0a75 726c 203d  oundation..url =
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 6365 7265 6e65 6f2d 666f 756e  com/cereneo-foun
-000000a0: 6461 7469 6f6e 2f67 6169 745f 616e 616c  dation/gait_anal
-000000b0: 7973 6973 0d0a 6465 7363 7269 7074 696f  ysis..descriptio
-000000c0: 6e20 3d20 4c69 6272 6172 7920 746f 2061  n = Library to a
-000000d0: 6e61 6c79 7365 2067 6169 7420 6461 7461  nalyse gait data
-000000e0: 2063 6170 7475 7265 6420 7769 7468 2061   captured with a
-000000f0: 206d 6f63 6170 2073 7973 7465 6d0d 0a6c   mocap system..l
-00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000110: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000120: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-00000130: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000140: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000150: 0d0a 6b65 7977 6f72 6473 203d 2067 6169  ..keywords = gai
-00000160: 742c 2061 6e61 6c79 7369 732c 2063 3364  t, analysis, c3d
-00000170: 2c20 6d6f 6361 700d 0a6c 6963 656e 7365  , mocap..license
-00000180: 203d 204d 4954 0d0a 636c 6173 7369 6669   = MIT..classifi
-00000190: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001e0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-000001f0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000200: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000210: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000220: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
-00000230: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-00000240: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000250: 6573 203d 200d 0a09 7061 6e64 6173 0d0a  es = ...pandas..
-00000260: 0970 7979 616d 6c0d 0a09 6d61 7470 6c6f  .pyyaml...matplo
-00000270: 746c 6962 0d0a 096e 756d 7079 0d0a 0973  tlib...numpy...s
-00000280: 6369 7079 0d0a 0d0a 5b6f 7074 696f 6e73  cipy....[options
-00000290: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000002a0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000002b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-000002c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-000002d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
+000000a0: 6461 7469 6f6e 2f67 6169 7461 6c79 7469  dation/gaitalyti
+000000b0: 6373 0d0a 6465 7363 7269 7074 696f 6e20  cs..description 
+000000c0: 3d20 4c69 6272 6172 7920 746f 2061 6e61  = Library to ana
+000000d0: 6c79 7365 2067 6169 7420 6461 7461 2063  lyse gait data c
+000000e0: 6170 7475 7265 6420 7769 7468 2061 206d  aptured with a m
+000000f0: 6f63 6170 2073 7973 7465 6d0d 0a6c 6f6e  ocap system..lon
+00000100: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+00000110: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
+00000120: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000130: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+00000140: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000150: 6b65 7977 6f72 6473 203d 2067 6169 742c  keywords = gait,
+00000160: 2061 6e61 6c79 7369 732c 2063 3364 2c20   analysis, c3d, 
+00000170: 6d6f 6361 700d 0a6c 6963 656e 7365 203d  mocap..license =
+00000180: 204d 4954 0d0a 636c 6173 7369 6669 6572   MIT..classifier
+00000190: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001b0: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
+000001c0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001d0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001e0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
+000001f0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000200: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
+00000210: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
+00000220: 6972 203d 200d 0a09 3d73 7263 0d0a 7061  ir = ...=src..pa
+00000230: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000240: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000250: 203d 200d 0a09 7061 6e64 6173 0d0a 0970   = ...pandas...p
+00000260: 7979 616d 6c0d 0a09 6d61 7470 6c6f 746c  yyaml...matplotl
+00000270: 6962 0d0a 096e 756d 7079 0d0a 0973 6369  ib...numpy...sci
+00000280: 7079 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  py....[options.p
+00000290: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000002a0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+000002b0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002c0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002d0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/analysis.py` & `gaitalytics-0.1.0b0/src/gaitalytics/analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,37 +5,41 @@
 from pandas import DataFrame, concat
 from scipy import signal
 
 import gaitalytics.utils
 
 
 class AbstractAnalysis(ABC):
-    def __init__(self, data_list: Dict[str, gaitalytics.utils.BasicCyclePoint]):
+    def __init__(self, data_list: Dict[str, gaitalytics.utils.BasicCyclePoint],
+                 configs: gaitalytics.utils.ConfigProvider):
         self._data_list: Dict[str, gaitalytics.utils.BasicCyclePoint] = data_list
+        self._configs = configs
 
-    def analyse(self) -> DataFrame:
+    def analyse(self, **kwargs) -> DataFrame:
         pass
 
 
 class AbstractCycleAnalysis(AbstractAnalysis, ABC):
 
     def __init__(self, data_list: Dict[str, gaitalytics.utils.BasicCyclePoint],
+                 configs: gaitalytics.utils.ConfigProvider,
                  data_type: gaitalytics.utils.PointDataType):
-        super().__init__(data_list)
+        super().__init__(data_list, configs)
         self._point_data_type = data_type
 
     @abstractmethod
     def _do_analysis(self, data: DataFrame) -> DataFrame:
         pass
 
     def _filter_keys(self, key: str) -> bool:
         """ Check if its the right point data """
         return f".{self._point_data_type.name}." in key
 
-    def analyse(self, by_phase=True) -> DataFrame:
+    def analyse(self, **kwargs) -> DataFrame:
+        by_phase = kwargs.get("by_phase", True)
         results = None
         for key in self._data_list:  # TODO change quick fix
             if self._filter_keys(key):
                 raw_point = self._data_list[key]
                 data = raw_point.data_table
                 if not by_phase:
                     result = self._do_analysis(data)
@@ -59,16 +63,16 @@
                 else:
                     results = concat([results, result])
         return results.pivot(columns="metric")
 
 
 class JointForcesCycleAnalysis(AbstractCycleAnalysis):
 
-    def __init__(self, data_list: Dict):
-        super().__init__(data_list, gaitalytics.utils.PointDataType.Forces)
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
+        super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Forces)
 
     def _filter_keys(self, key: str) -> bool:
         if super()._filter_keys(key):
             splits = key.split(".")
             return splits[3].lower() in splits[0]
         return False
 
@@ -83,16 +87,16 @@
         results['forces_sd'] = data.std(axis=1)
         results['forces_amplitude'] = rom_max - rom_min
         return results
 
 
 class JointMomentsCycleAnalysis(AbstractCycleAnalysis):
 
-    def __init__(self, data_list: Dict):
-        super().__init__(data_list, gaitalytics.utils.PointDataType.Moments)
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
+        super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Moments)
 
     def _filter_keys(self, key: str) -> bool:
         if super()._filter_keys(key):
             splits = key.split(".")
             return splits[3].lower() in splits[0]
         return False
 
@@ -107,16 +111,16 @@
         results['moments_sd'] = data.std(axis=1)
         results['power_amplitude'] = rom_max - rom_min
         return results
 
 
 class JointPowerCycleAnalysis(AbstractCycleAnalysis):
 
-    def __init__(self, data_list: Dict):
-        super().__init__(data_list, gaitalytics.utils.PointDataType.Power)
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
+        super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Power)
 
     def _filter_keys(self, key: str) -> bool:
         if super()._filter_keys(key):
             splits = key.split(".")
             if splits[3].lower() in splits[0]:
                 return gaitalytics.utils.AxesNames.z.name is splits[2]
         return False
@@ -132,16 +136,16 @@
         results['power_sd'] = data.std(axis=1)
         results['power_amplitude'] = rom_max - rom_min
         return results
 
 
 class JointAnglesCycleAnalysis(AbstractCycleAnalysis):
 
-    def __init__(self, data_list: Dict):
-        super().__init__(data_list, gaitalytics.utils.PointDataType.Angles)
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
+        super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Angles)
 
     def _filter_keys(self, key: str) -> bool:
         if super()._filter_keys(key):
             splits = key.split(".")
             return splits[3].lower() in splits[0]
         return False
 
@@ -158,24 +162,103 @@
         velocity = data.diff(axis=1)
         results['angle_velocity_max'] = velocity.max(axis=1)
         results['angle_velocity_min'] = velocity.min(axis=1)
         results['angle_velocity_sd'] = velocity.std(axis=1)
         return results
 
 
+class CMosAnalysis(AbstractCycleAnalysis):
+
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider):
+        super().__init__(data_list, configs, gaitalytics.utils.PointDataType.Marker)
+
+    def _filter_keys(self, key: str) -> bool:
+        if super()._filter_keys(key):
+            useful = self._configs.MARKER_MAPPING.right_cmos.name in key
+            useful = self._configs.MARKER_MAPPING.left_cmos.name in key or useful
+            return useful
+        return False
+
+    def _do_analysis(self, data: DataFrame) -> DataFrame:
+        results = DataFrame(index=data.index)
+
+        results['cmos_mean'] = data.mean(axis=1)
+        results['cmos_max'] = data.max(axis=1)
+        results['cmos_min'] = data.min(axis=1)
+        results['cmos_sd'] = data.std(axis=1)
+
+        return results
+
+
+class MosAnalysis(AbstractAnalysis):
+
+    def analyse(self, **kwargs) -> DataFrame:
+        left_cmos_ap = self._data_list[
+            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.left_cmos,
+                                                        gaitalytics.utils.PointDataType.Marker,
+                                                        gaitalytics.utils.AxesNames.y,
+                                                        gaitalytics.utils.GaitEventContext.LEFT)]
+        left_cmos_ml = self._data_list[
+            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.left_cmos,
+                                                        gaitalytics.utils.PointDataType.Marker,
+                                                        gaitalytics.utils.AxesNames.x,
+                                                        gaitalytics.utils.GaitEventContext.LEFT)]
+
+        right_cmos_ap = self._data_list[
+            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_cmos,
+                                                        gaitalytics.utils.PointDataType.Marker,
+                                                        gaitalytics.utils.AxesNames.y,
+                                                        gaitalytics.utils.GaitEventContext.RIGHT)]
+        right_cmos_ml = self._data_list[
+            gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_cmos,
+                                                        gaitalytics.utils.PointDataType.Marker,
+                                                        gaitalytics.utils.AxesNames.x,
+                                                        gaitalytics.utils.GaitEventContext.RIGHT)]
+
+        left_ap = self._extract_mos_frames(left_cmos_ap, "left", "ap")
+        left_ml = self._extract_mos_frames(left_cmos_ml, "left", "ml")
+        right_ap = self._extract_mos_frames(right_cmos_ap, "right", "ap")
+        right_ml = self._extract_mos_frames(right_cmos_ml, "right", "ml")
+        result = left_ap.merge(left_ml, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
+        result = result.merge(right_ap, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
+        result = result.merge(right_ml, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
+
+
+        result['metric'] = "Mos"
+        return result.pivot(columns="metric")
+
+    @staticmethod
+    def _extract_mos_frames(cmos: gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER, side, direction):
+        hs_label = f"{direction}_hs_{side}"
+        to_label = f"{direction}_to_{side}"
+        hs_contra_label = f"{direction}_hs_contra_{side}"
+        to_contra_label = f"{direction}_to_contra_{side}"
+        column_label = [hs_label, to_label, hs_contra_label, to_contra_label]
+
+        result = DataFrame(index=cmos.data_table.index)
+        result[hs_label] = cmos.data_table[0].to_list()
+        for cycle_number in cmos.event_frames.index.to_list():
+            to_frame = cmos.event_frames[gaitalytics.utils.BasicCyclePoint.FOOT_OFF].loc[cycle_number]
+            hs_contra_frame = cmos.event_frames[gaitalytics.utils.BasicCyclePoint.FOOT_STRIKE_CONTRA].loc[cycle_number]
+            to_contra_frame = cmos.event_frames[gaitalytics.utils.BasicCyclePoint.FOOT_OFF_CONTRA].loc[cycle_number]
+            result.loc[cycle_number, to_label] = cmos.data_table.loc[cycle_number, to_frame]
+            result.loc[cycle_number, hs_contra_label] = cmos.data_table.loc[cycle_number, hs_contra_frame]
+            result.loc[cycle_number, to_contra_label] = cmos.data_table.loc[cycle_number, to_contra_frame]
+        return result
+
+
 class SpatioTemporalAnalysis(AbstractAnalysis):
 
-    def __init__(self, configs: gaitalytics.utils.ConfigProvider, data_list: Dict, body_height: float = 1800,
+    def __init__(self, data_list: Dict, configs: gaitalytics.utils.ConfigProvider, body_height: float = 1800,
                  frequency: int = 100):
-        super().__init__(data_list)
-        self._configs = configs
+        super().__init__(data_list, configs)
         self._frequency = frequency
         self._body_height = body_height
 
-    def analyse(self) -> DataFrame:
+    def analyse(self, **kwargs) -> DataFrame:
         subject = self._data_list[
             gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_heel,
                                                         gaitalytics.utils.PointDataType.Marker,
                                                         gaitalytics.utils.AxesNames.x,
                                                         gaitalytics.utils.GaitEventContext.RIGHT)].subject
         step_length = self._calculate_length(subject)
         durations = self._calculate_durations()
@@ -262,15 +345,15 @@
                                                         gaitalytics.utils.AxesNames.y,
                                                         gaitalytics.utils.GaitEventContext.LEFT)]
         right_durations = self._side_duration_calculation(right_heel_progression, "right")
         left_durations = self._side_duration_calculation(left_heel_progression, "left")
 
         return concat([left_durations, right_durations], axis=1)
 
-    def _side_duration_calculation(self, progression: DataFrame, side: str) -> DataFrame:
+    def _side_duration_calculation(self, progression: gaitalytics.utils.BasicCyclePoint, side: str) -> DataFrame:
         c_dur_label = f"cycle_duration_s_{side}"
         s_dur_label = f"step_duration_s_{side}"
         sw_dur_label = f"swing_duration_p_{side}"
         st_dur_label = f"stance_duration_p_{side}"
         columns = [c_dur_label, s_dur_label, sw_dur_label, st_dur_label]
         durations = DataFrame(index=progression.data_table.index, columns=columns)
         for cycle_number in progression.data_table.index.to_series():
@@ -345,18 +428,17 @@
     # max_hip_vertical_amplitude = np.zeros(len(data))  # BH%
 
 
 class MinimalClearingDifference(AbstractAnalysis):
 
     def __init__(self, data_list: Dict[str, gaitalytics.utils.BasicCyclePoint],
                  configs: gaitalytics.utils.ConfigProvider):
-        super().__init__(data_list)
-        self._configs = configs
+        super().__init__(data_list, configs)
 
-    def analyse(self) -> DataFrame:
+    def analyse(self, **kwargs) -> DataFrame:
         right_toe = self._data_list[
             gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.right_meta_2,
                                                         gaitalytics.utils.PointDataType.Marker,
                                                         gaitalytics.utils.AxesNames.z,
                                                         gaitalytics.utils.GaitEventContext.RIGHT)]
         left_toe = self._data_list[gaitalytics.utils.ConfigProvider.define_key(self._configs.MARKER_MAPPING.left_meta_2,
                                                                                gaitalytics.utils.PointDataType.Marker,
```

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/api.py` & `gaitalytics-0.1.0b0/src/gaitalytics/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,67 +28,75 @@
 
 ANALYSIS_MOMENTS = "moments"
 ANALYSIS_ANGLES = "angles"
 ANALYSIS_POWERS = "powers"
 ANALYSIS_FORCES = "forces"
 ANALYSIS_TOE_CLEARANCE = "toe_clearance"
 ANALYSIS_SPATIO_TEMP = "spatiotemporal"
+ANALYSIS_CMOS = "cmos"
+ANALYSIS_MOS = "mos"
 ANALYSIS_LIST = (ANALYSIS_MOMENTS,
                  ANALYSIS_ANGLES,
                  ANALYSIS_POWERS,
                  ANALYSIS_FORCES,
                  ANALYSIS_SPATIO_TEMP,
-                 ANALYSIS_TOE_CLEARANCE)
+                 ANALYSIS_TOE_CLEARANCE,
+                 ANALYSIS_CMOS,
+                 ANALYSIS_MOS)
 
 
 def analyse_data(cycle_data: Dict[str, gaitalytics.utils.BasicCyclePoint],
                  config: gaitalytics.utils.ConfigProvider,
-                 methode: List[str] = ANALYSIS_LIST) -> DataFrame:
+                 methode: List[str] = ANALYSIS_LIST, **kwargs) -> DataFrame:
     """
     runs specified analysis and concatenates into one frame
     :param cycle_data: unnormalised cycle data
     :param config: configs from marker and model mapping
     :param methode: list of methods, 'moments' api.ANALYSIS_MOMENTS, 'angles' api.ANALYSIS_ANGLES,
         'powers' api.ANALYSIS_POWERS, 'forces' api.ANALYSIS_FORCES, 'spatiotemporal' api.ANALYSIS_SPATIO_TEMP,
-        'toe_clearance' api.ANALYSIS_TOE_CLEARANCE
+        'toe_clearance' api.ANALYSIS_TOE_CLEARANCE, 'cmos' api.ANALYSIS_CMOS
     :return: results of analysis
     """
     if not all(item in ANALYSIS_LIST for item in methode):
         raise KeyError(f"{methode} are not a valid anomaly checker")
 
     methods: List[gaitalytics.analysis.AbstractAnalysis] = []
     if ANALYSIS_ANGLES in methode:
-        methods.append(gaitalytics.analysis.JointAnglesCycleAnalysis(cycle_data))
+        methods.append(gaitalytics.analysis.JointAnglesCycleAnalysis(cycle_data, config))
     if ANALYSIS_MOMENTS in methode:
-        methods.append(gaitalytics.analysis.JointMomentsCycleAnalysis(cycle_data))
+        methods.append(gaitalytics.analysis.JointMomentsCycleAnalysis(cycle_data, config))
     if ANALYSIS_POWERS in methode:
-        methods.append(gaitalytics.analysis.JointPowerCycleAnalysis(cycle_data))
+        methods.append(gaitalytics.analysis.JointPowerCycleAnalysis(cycle_data, config))
     if ANALYSIS_FORCES in methode:
-        methods.append(gaitalytics.analysis.JointForcesCycleAnalysis(cycle_data))
+        methods.append(gaitalytics.analysis.JointForcesCycleAnalysis(cycle_data, config))
     if ANALYSIS_SPATIO_TEMP in methode:
-        methods.append(gaitalytics.analysis.SpatioTemporalAnalysis(config, cycle_data))
+        methods.append(gaitalytics.analysis.SpatioTemporalAnalysis(cycle_data, config))
     if ANALYSIS_TOE_CLEARANCE in methode:
         methods.append(gaitalytics.analysis.MinimalClearingDifference(cycle_data, config))
+    if ANALYSIS_CMOS in methode:
+        methods.append(gaitalytics.analysis.CMosAnalysis(cycle_data, config))
+    if ANALYSIS_MOS in methode:
+        methods.append(gaitalytics.analysis.MosAnalysis(cycle_data, config))
 
     results = None
     for methode in methods:
-        result = methode.analyse()
+        result = methode.analyse(**kwargs)
         if results is None:
             results = result
         else:
             results = results.merge(result, on=gaitalytics.utils.BasicCyclePoint.CYCLE_NUMBER)
 
     return results
 
 
 def check_gait_event(c3d_file_path: str,
                      output_path: str,
                      anomaly_checker: List[str] = GAIT_EVENT_CHECKER_LIST):
     """
-    Checks events aditionally
+    Checks events additionally
     with given anomaly_checker method and saves it in output_path with '*_anomaly.txt' extension
     :param c3d_file_path: path of c3d file with modelled filtered data '.3.c3d'
     :param output_path: path to dir to store c3d file with events
     :param anomaly_checker: list of anomaly checkers, "context" api.GAIT_EVENT_CHECKER_CONTEXT,
        "spacing" api.GAIT_EVENT_CHECKER_SPACING
     """
     if not os.path.isfile(c3d_file_path):
```

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/c3d.py` & `gaitalytics-0.1.0b0/src/gaitalytics/c3d.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/cycle.py` & `gaitalytics-0.1.0b0/src/gaitalytics/cycle.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/emg.py` & `gaitalytics-0.1.0b0/src/gaitalytics/emg.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/events.py` & `gaitalytics-0.1.0b0/src/gaitalytics/events.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/modelling.py` & `gaitalytics-0.1.0b0/src/gaitalytics/modelling.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 
     def __init__(self, side: str, configs: gaitalytics.utils.ConfigProvider,
                  dominant_leg_length: float, belt_speed: float):
         self._configs = configs
         self._dominant_leg_length = dominant_leg_length
         self._belt_speed = belt_speed
         self._side = side
-        super().__init__(f"{side}cMoS", gaitalytics.utils.PointDataType.Marker)
+        if side == "Left":
+            label = self._configs.MARKER_MAPPING.left_cmos.value
+        else:
+            label = self._configs.MARKER_MAPPING.right_cmos.value
+        super().__init__(label, gaitalytics.utils.PointDataType.Marker)
 
     def _calculate_point(self, acq: btkAcquisition) -> np.ndarray:
         com = acq.GetPoint(self._configs.MARKER_MAPPING.com.value).GetValues()
         if self._side == "Left":
             lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.left_lat_malleoli.value).GetValues()
             contra_lat_malleoli = acq.GetPoint(self._configs.MARKER_MAPPING.right_lat_malleoli.value).GetValues()
             meta_2 = acq.GetPoint(self._configs.MARKER_MAPPING.left_meta_2.value).GetValues()
@@ -70,14 +74,19 @@
              second_meta_head_marker: np.ndarray,
              second_meta_head_marker_contra: np.ndarray,
              dominant_leg_length: float,
              belt_speed: float,
              acq: btkAcquisition,
              side: str,
              show: bool = True) -> np.ndarray:
+        # AP axis is inverted
+        com[:, 1] *= -1
+        second_meta_head_marker[:, 1] *= -1
+        second_meta_head_marker_contra[:, 1] *= -1
+
         if side == "Left":
             contra_side = "Right"
         else:
             contra_side = "Left"
         distance_from_x_com_to_bos = np.zeros((len(com), 3))
 
         # preparing events for the MOS calculation
@@ -105,15 +114,15 @@
                     cycle_event = f"{foot} {type_of_event}"
                     # determining the event to know the base of support we have to use for the calculation
                     itr += 1
             else:
                 break
 
             # calculating the x_com
-            x_com = [com[i,0] + (com_v[i, 0]/sqrt_leg_speed), com[i,1] + (com_v[i, 1] + belt_speed) / sqrt_leg_speed]
+            x_com = [com[i, 0] + (com_v[i, 0]/sqrt_leg_speed), com[i, 1] + (belt_speed+com_v[i, 1]) / sqrt_leg_speed]
             # still miss the treadmill speed (need velocity of belt in AP and ML axis too)
             # x_com = [COM[i, 0], COM[i, 1]]
             # calculating the distance between the x_com and the BOS
             # 4 cases : Left Heel Strike, Left Toe Off, Right Heel Strike, Right Toe Off
             """
                         MOSant
                             ^
@@ -134,14 +143,17 @@
                 mos = [x_com[0] - lat_malleoli_marker[i, 0],
                        second_meta_head_marker[i, 1] - x_com[1]]
             elif cycle_event == f"{contra_side} Foot Strike":
                 mos = [lat_malleoli_marker_contra[i, 0] - x_com[0],
                        second_meta_head_marker_contra[i, 1] - x_com[1]]
             else:
                 mos = [0, 0]
+
+            if side == "Left":
+                mos[0] = mos[0] * -1
             distance_from_x_com_to_bos[i, 0] = mos[0]
             distance_from_x_com_to_bos[i, 1] = mos[1]
         if show:
             self._show(distance_from_x_com_to_bos, side)
         return distance_from_x_com_to_bos
 
     def _show(self, distance_from_xCOM_to_BOS, side):
```

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/plot.py` & `gaitalytics-0.1.0b0/src/gaitalytics/plot.py`

 * *Files identical despite different names*

### Comparing `gaitalytics-0.0.9b0/src/gaitalytics/utils.py` & `gaitalytics-0.1.0b0/src/gaitalytics/utils.py`

 * *Files identical despite different names*

