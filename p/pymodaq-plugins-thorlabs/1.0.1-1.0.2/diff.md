# Comparing `tmp/pymodaq_plugins_thorlabs-1.0.1.tar.gz` & `tmp/pymodaq_plugins_thorlabs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_thorlabs-1.0.1.tar", last modified: Mon Jun 12 15:28:57 2023, max compression
+gzip compressed data, was "pymodaq_plugins_thorlabs-1.0.2.tar", last modified: Thu Jun 29 09:43:29 2023, max compression
```

## Comparing `pymodaq_plugins_thorlabs-1.0.1.tar` & `pymodaq_plugins_thorlabs-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.575821 pymodaq_plugins_thorlabs-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.579820 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.583821 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-12 15:28:45.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:28:57.579820 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 15:28:57.000000 pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.907349 pymodaq_plugins_thorlabs-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.907349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Elliptec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8158 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.911349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-29 09:43:11.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/powermeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:43:29.907349 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-29 09:43:29.000000 pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_thorlabs-1.0.1/LICENSE` & `pymodaq_plugins_thorlabs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_thorlabs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-1.0.1/README.rst` & `pymodaq_plugins_thorlabs-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/setup.py` & `pymodaq_plugins_thorlabs-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Kinesis_KPA101.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeter.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TLPMPowermeterInst.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_DCx.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Thorlabs_TSI.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/kinesis.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/kinesis.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs/hardware/powermeter.py` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs/hardware/powermeter.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-thorlabs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Set of PyMoDAQ plugins for instruments from Thorlabs (Kinesis K10CR1 (stepper rotation actuator), Kinesis Flipper, Kinesis KSP100, DCx camera...)
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_thorlabs
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_thorlabs-1.0.1/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt` & `pymodaq_plugins_thorlabs-1.0.2/src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/pymodaq_plugins_thorlabs.egg-info/PKG-INFO
 src/pymodaq_plugins_thorlabs.egg-info/SOURCES.txt
 src/pymodaq_plugins_thorlabs.egg-info/dependency_links.txt
 src/pymodaq_plugins_thorlabs.egg-info/entry_points.txt
 src/pymodaq_plugins_thorlabs.egg-info/requires.txt
 src/pymodaq_plugins_thorlabs.egg-info/top_level.txt
 src/pymodaq_plugins_thorlabs/daq_move_plugins/__init__.py
+src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Elliptec.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_K10CR1.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_Kinesis.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisFlipper.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_KinesisIntegratedStepper.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_MFF101_pylablib.py
 src/pymodaq_plugins_thorlabs/daq_move_plugins/daq_move_PRM1Z8_pylablib.py
 src/pymodaq_plugins_thorlabs/daq_viewer_plugins/__init__.py
```

