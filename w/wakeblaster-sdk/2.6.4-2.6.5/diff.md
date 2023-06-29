# Comparing `tmp/wakeblaster-sdk-2.6.4.tar.gz` & `tmp/wakeblaster-sdk-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wakeblaster-sdk-2.6.4.tar", last modified: Tue Jun 20 12:23:26 2023, max compression
+gzip compressed data, was "dist\wakeblaster-sdk-2.6.5.tar", last modified: Thu Jun 29 08:33:51 2023, max compression
```

## Comparing `wakeblaster-sdk-2.6.4.tar` & `wakeblaster-sdk-2.6.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:26.000000 wakeblaster-sdk-2.6.4/
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/
--rw-rw-rw-   0        0        0     5546 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/flow_case_maker.py
--rw-rw-rw-   0        0        0     3806 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/tab_file_parser.py
--rw-rw-rw-   0        0        0      561 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/energytoolbox/util.py
--rw-rw-rw-   0        0        0     6717 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_dependencies.py
--rw-rw-rw-   0        0        0     7198 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_simulation.py
--rw-rw-rw-   0        0        0     1514 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/wind_frequency_matrix.py
--rw-rw-rw-   0        0        0     1954 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/yield_calculator.py
--rw-rw-rw-   0        0        0      525 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/__init__.py
--rw-rw-rw-   0        0        0      734 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0       84 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/README.md
--rw-rw-rw-   0        0        0       64 2023-06-20 12:23:26.000000 wakeblaster-sdk-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     3204 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/
--rw-rw-rw-   0        0        0     2629 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/example.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/
--rw-rw-rw-   0        0        0  1170512 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/flow-plane.h5
--rw-rw-rw-   0        0        0     6158 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/Lillgrund.json
--rw-rw-rw-   0        0        0      444 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/simulator-config.json
--rw-rw-rw-   0        0        0     2608 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg
--rw-rw-rw-   0        0        0       39 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/
--rw-rw-rw-   0        0        0    13810 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/converters.py
--rw-rw-rw-   0        0        0     4854 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/submit.py
--rw-rw-rw-   0        0        0    11435 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeRequest.py
--rw-rw-rw-   0        0        0     3434 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeResult.py
--rw-rw-rw-   0        0        0       52 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/__init__.py
--rw-rw-rw-   0        0        0     8314 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/flow_plane_plots.py
--rw-rw-rw-   0        0        0    25630 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/sdk.py
--rw-rw-rw-   0        0        0      584 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-20 12:23:24.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      734 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1043 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       49 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/energytoolbox/
+-rw-rw-rw-   0        0        0     5546 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/flow_case_maker.py
+-rw-rw-rw-   0        0        0     3806 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/tab_file_parser.py
+-rw-rw-rw-   0        0        0      561 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.5/energytoolbox/util.py
+-rw-rw-rw-   0        0        0     6717 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.5/energytoolbox/wakeblaster_dependencies.py
+-rw-rw-rw-   0        0        0     7198 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/wakeblaster_simulation.py
+-rw-rw-rw-   0        0        0     1514 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/wind_frequency_matrix.py
+-rw-rw-rw-   0        0        0     1954 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/yield_calculator.py
+-rw-rw-rw-   0        0        0      525 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/energytoolbox/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.5/README.md
+-rw-rw-rw-   0        0        0       64 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     3204 2023-06-29 08:33:42.000000 wakeblaster-sdk-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/
+-rw-rw-rw-   0        0        0     2629 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/example.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/
+-rw-rw-rw-   0        0        0  1170512 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/flow-plane.h5
+-rw-rw-rw-   0        0        0     6158 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/Lillgrund.json
+-rw-rw-rw-   0        0        0      444 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/simulator-config.json
+-rw-rw-rw-   0        0        0     2608 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/SWT-2.3-93m.wtg
+-rw-rw-rw-   0        0        0       39 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblasterexamples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/
+-rw-rw-rw-   0        0        0    13810 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/converters.py
+-rw-rw-rw-   0        0        0     4854 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/submit.py
+-rw-rw-rw-   0        0        0    11435 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/wakeRequest.py
+-rw-rw-rw-   0        0        0     3434 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/wakeResult.py
+-rw-rw-rw-   0        0        0       52 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/emd/__init__.py
+-rw-rw-rw-   0        0        0     8314 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/flow_plane_plots.py
+-rw-rw-rw-   0        0        0    25630 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/sdk.py
+-rw-rw-rw-   0        0        0      584 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblastersdk/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:33:51.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      734 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1043 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       49 2023-06-29 08:33:50.000000 wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/top_level.txt
```

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/flow_case_maker.py` & `wakeblaster-sdk-2.6.5/energytoolbox/flow_case_maker.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/tab_file_parser.py` & `wakeblaster-sdk-2.6.5/energytoolbox/tab_file_parser.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/util.py` & `wakeblaster-sdk-2.6.5/energytoolbox/util.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_dependencies.py` & `wakeblaster-sdk-2.6.5/energytoolbox/wakeblaster_dependencies.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_simulation.py` & `wakeblaster-sdk-2.6.5/energytoolbox/wakeblaster_simulation.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/wind_frequency_matrix.py` & `wakeblaster-sdk-2.6.5/energytoolbox/wind_frequency_matrix.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/yield_calculator.py` & `wakeblaster-sdk-2.6.5/energytoolbox/yield_calculator.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/energytoolbox/__init__.py` & `wakeblaster-sdk-2.6.5/energytoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/PKG-INFO` & `wakeblaster-sdk-2.6.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: wakeblaster-sdk
-Version: 2.6.4
+Version: 2.6.5
 Summary: The WakeBlaster SDK
 Home-page: http://www.wakeblaster.net
-Author: ProPlanEn Ltd.
+Author: ProPlanEn GmbH
 Author-email: wakeblaster@proplanen.net
 License: UNKNOWN
 Description: # WakeBlaster SDK
         
         For more information, see https://proplanen.info/wakeblaster.
         
 Keywords: wakeblaster windfarm modelling simulation
```

### Comparing `wakeblaster-sdk-2.6.4/setup.py` & `wakeblaster-sdk-2.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # The project's main homepage.
     url='http://www.wakeblaster.net',
     
     version=__version__,
 
     # Author details
-    author='ProPlanEn Ltd.',
+    author='ProPlanEn GmbH',
     author_email='wakeblaster@proplanen.net',
 
     # Choose your license
     # license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

### Comparing `wakeblaster-sdk-2.6.4/wakeblasterexamples/example.py` & `wakeblaster-sdk-2.6.5/wakeblasterexamples/example.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/flow-plane.h5` & `wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/flow-plane.h5`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/Lillgrund.json` & `wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/Lillgrund.json`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg` & `wakeblaster-sdk-2.6.5/wakeblasterexamples/examples/SWT-2.3-93m.wtg`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/converters.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/emd/converters.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/submit.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/emd/submit.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeRequest.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/emd/wakeRequest.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeResult.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/emd/wakeResult.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/flow_plane_plots.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/flow_plane_plots.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/sdk.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/sdk.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblastersdk/__init__.py` & `wakeblaster-sdk-2.6.5/wakeblastersdk/__init__.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/PKG-INFO` & `wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.2
 Name: wakeblaster-sdk
-Version: 2.6.4
+Version: 2.6.5
 Summary: The WakeBlaster SDK
 Home-page: http://www.wakeblaster.net
-Author: ProPlanEn Ltd.
+Author: ProPlanEn GmbH
 Author-email: wakeblaster@proplanen.net
 License: UNKNOWN
 Description: # WakeBlaster SDK
         
         For more information, see https://proplanen.info/wakeblaster.
         
 Keywords: wakeblaster windfarm modelling simulation
```

### Comparing `wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/SOURCES.txt` & `wakeblaster-sdk-2.6.5/wakeblaster_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

