# Comparing `tmp/commonroad-openscenario-converter-0.0.3.tar.gz` & `tmp/commonroad-openscenario-converter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-openscenario-converter-0.0.3.tar", last modified: Wed May 17 13:36:37 2023, max compression
+gzip compressed data, was "commonroad-openscenario-converter-0.0.4.tar", last modified: Thu Jun 29 07:11:18 2023, max compression
```

## Comparing `commonroad-openscenario-converter-0.0.3.tar` & `commonroad-openscenario-converter-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4237 2023-05-17 09:16:36.000000 commonroad-openscenario-converter-0.0.3/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1752 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-05-17 13:36:37.000000 commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/top_level.txt
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error_analyzer.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/result.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.510572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/analysis.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5787 2023-05-09 09:30:26.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/converter.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1375 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22393 2023-05-10 07:31:51.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/osc2cr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3076 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/result.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/serializable.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/__init__.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/common.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/abs_rel.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6758 2023-05-09 08:57:31.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/general.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/obstacle_info.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/pps.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/statistics.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      483 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/ending_cause.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5956 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3533 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/sim_wrapper.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14812 2023-05-16 09:23:37.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/storyboard_element.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-05-17 13:32:43.000000 commonroad-openscenario-converter-0.0.3/setup.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-17 13:36:37.514572 commonroad-openscenario-converter-0.0.3/tests/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.3/tests/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.3/tests/test_conversion.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.3/tests/test_udp.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4250 2023-06-29 07:07:14.000000 commonroad-openscenario-converter-0.0.4/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1794 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/top_level.txt
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-30 08:29:14.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/enum_analyzer.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/error.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/result.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/analysis.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5792 2023-05-30 08:36:11.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/converter.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1921 2023-05-30 09:16:52.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    21898 2023-06-15 13:14:23.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/osc2cr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3075 2023-05-30 08:36:55.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/result.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/serializable.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/__init__.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/common.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/abs_rel.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     7617 2023-06-15 13:24:49.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/general.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1820 2023-06-29 06:45:10.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/logger.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-06-15 13:20:59.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/obstacle_info.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/pps_builder.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/statistics.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      483 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/ending_cause.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5956 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3570 2023-05-30 10:40:12.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/sim_wrapper.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13375 2023-06-15 13:01:18.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/storyboard_element.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-06-29 07:09:38.000000 commonroad-openscenario-converter-0.0.4/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/tests/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.4/tests/test_conversion.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.4/tests/test_udp.py
```

### Comparing `commonroad-openscenario-converter-0.0.3/LICENSE` & `commonroad-openscenario-converter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/PKG-INFO` & `commonroad-openscenario-converter-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.3/README.md` & `commonroad-openscenario-converter-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CommonROAD-OpenSCENARIO Converter
-![image info](./docs/figures/converter-banner.gif)
+![image info](./docs/figures/converter-banner.png)
 
 Automatic Traffic Scenario Conversion between [OpenSCENARIO](https://www.asam.net/standards/detail/openscenario/)
 and [CommonRoad](commonroad.in.tum.de/). Currently, only the conversion from **O**pen**SC**ENARIO to **C**ommon**R**OAD (osc2cr) is developed.<br>
 [![Linux](https://svgshare.com/i/Zhy.svg?style=plastic)](https://svgshare.com/i/Zhy.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
@@ -60,20 +60,20 @@
 and to [Sebastian Maierhofer](https://www.ce.cit.tum.de/air/people/sebastian-maierhofer-msc/)
 for maintaining the converter from OpenDRIVE to lanelets.
 We gratefully acknowledge partial financial support by the German Federal Ministry for Digital and Transport (BMDV) 
 within the project _Cooperative Autonomous Driving with Safety Guarantees_
 ([KoSi](https://www.ce.cit.tum.de/air/research/kosi/)).
 
 ### Citation
-If you use `commonroad-openscenario-converter` for academic work, we highly encourage you to cite our paper:
+If you use `commonroad-openscenario-converter` for academic work, we highly encourage you to cite our [paper](https://arxiv.org/pdf/2305.10080.pdf):
 ```text
-@InProceedings{osc2cr,
-      title     = {Automatic Traffic Scenario Conversion from OpenSCENARIO to CommonRoad},
-      author    = {Yuanfei Lin, Michael Ratzel, and Matthias Althoff},
-      booktitle = {coming soon},     
-      pages     = {}, 
-      year      = {2023},
+@article{osc2cr,
+  title={Automatic Traffic Scenario Conversion from OpenSCENARIO to CommonRoad},
+  author={Yuanfei Lin, Michael Ratzel, and Matthias Althoff},
+  archivePrefix={arXiv},
+  journal={arXiv preprint arXiv:2305.10080},
+  year={2023}}
 }
 ```
 If you use this project's code in industry, we'd love to hear from you as well; 
 feel free to reach out to [Yuanfei Lin](mailto:yuanfei.lin@tum.de) directly.
```

### Comparing `commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/PKG-INFO` & `commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-openscenario-converter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converter between OpenSCENARIO and CommonRoad formats
 Author: Yuanfei Lin, Michael Ratzel
 Author-email: yuanfei.lin@tum.de
 License: BSD 3-Clause
 Keywords: scenario description,autonomous driving
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `commonroad-openscenario-converter-0.0.3/commonroad_openscenario_converter.egg-info/SOURCES.txt` & `commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 commonroad_openscenario_converter.egg-info/SOURCES.txt
 commonroad_openscenario_converter.egg-info/dependency_links.txt
 commonroad_openscenario_converter.egg-info/requires.txt
 commonroad_openscenario_converter.egg-info/top_level.txt
 osc_cr_converter/__init__.py
 osc_cr_converter/analyzer/__init__.py
 osc_cr_converter/analyzer/base.py
+osc_cr_converter/analyzer/enum_analyzer.py
 osc_cr_converter/analyzer/error.py
-osc_cr_converter/analyzer/error_analyzer.py
 osc_cr_converter/analyzer/result.py
 osc_cr_converter/batch/__init__.py
 osc_cr_converter/batch/analysis.py
 osc_cr_converter/batch/converter.py
 osc_cr_converter/converter/__init__.py
 osc_cr_converter/converter/base.py
 osc_cr_converter/converter/osc2cr.py
@@ -22,16 +22,17 @@
 osc_cr_converter/converter/serializable.py
 osc_cr_converter/udp_driver/__init__.py
 osc_cr_converter/udp_driver/common.py
 osc_cr_converter/utility/__init__.py
 osc_cr_converter/utility/abs_rel.py
 osc_cr_converter/utility/configuration.py
 osc_cr_converter/utility/general.py
+osc_cr_converter/utility/logger.py
 osc_cr_converter/utility/obstacle_info.py
-osc_cr_converter/utility/pps.py
+osc_cr_converter/utility/pps_builder.py
 osc_cr_converter/utility/statistics.py
 osc_cr_converter/utility/visualization.py
 osc_cr_converter/wrapper/__init__.py
 osc_cr_converter/wrapper/base/__init__.py
 osc_cr_converter/wrapper/base/ending_cause.py
 osc_cr_converter/wrapper/base/scenario_object.py
 osc_cr_converter/wrapper/base/sim_wrapper.py
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/base.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/error.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/analyzer/error_analyzer.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/enum_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 from enum import Enum
 from typing import Type
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/analysis.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/analysis.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/batch/converter.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import os
 import pickle
 import re
@@ -124,15 +124,15 @@
         for dir_path, dirs, files in os.walk(directory):
             if not recursively and os.path.abspath(dir_path) != abs_directory:
                 continue
             for file in files:
                 if file_matcher.match(file) is not None:
                     self.file_list.append(os.path.join(dir_path, file))
 
-    def run_batch_conversion(self, num_worker: Optional[int]=0, timeout: Optional[int] = None):
+    def run_batch_conversion(self, num_worker: Optional[int] = None, timeout: Optional[int] = None):
         """
         Run the batch conversion
 
         :param num_worker:int: If None or leq than 0, it will default to all available processors
         :timeout:int: If present a single conversion run will time out if this amount of seconds passed
         """
         assert Serializable.storage_dir is not None
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/osc2cr.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/osc2cr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,56 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import math
 import os
 import re
 import time
 import warnings
+import logging
 import xml.etree.ElementTree as ElementTree
 from dataclasses import dataclass
-from enum import auto, Enum
 from os import path
 from typing import Optional, List, Dict, Tuple, Union, Set
 
 from commonroad.geometry.shape import Rectangle, Circle
 from commonroad.prediction.prediction import TrajectoryPrediction
 from commonroad.scenario.obstacle import DynamicObstacle, ObstacleType
 from commonroad.scenario.scenario import Scenario, Tag
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.trajectory import Trajectory
-from commonroad.common.util import Interval
 from commonroad.common.file_writer import CommonRoadFileWriter
 from commonroad.common.file_writer import OverwriteExistingFile
 from crdesigner.map_conversion.map_conversion_interface import opendrive_to_commonroad
 from scenariogeneration.xosc import Vehicle
 
-from osc_cr_converter.converter.base import Converter
+from osc_cr_converter.converter.base import Converter, EFailureReason
 from osc_cr_converter.analyzer.base import Analyzer
 from osc_cr_converter.analyzer.error import AnalyzerErrorResult
 from osc_cr_converter.analyzer.result import AnalyzerResult
-from osc_cr_converter.analyzer.error_analyzer import EAnalyzer
+from osc_cr_converter.analyzer.enum_analyzer import EAnalyzer
 from osc_cr_converter.wrapper.base.ending_cause import ESimEndingCause
 from osc_cr_converter.wrapper.esmini.esmini_wrapper_provider import EsminiWrapperProvider
 from osc_cr_converter.wrapper.base.scenario_object import ScenarioObjectState, SimScenarioObjectState
 from osc_cr_converter.wrapper.base.sim_wrapper import SimWrapper, WrapperSimResult
 from osc_cr_converter.converter.result import Osc2CrConverterResult
 from osc_cr_converter.utility.statistics import ConversionStatistics
 from osc_cr_converter.utility.obstacle_info import ObstacleExtraInfoFinder
-from osc_cr_converter.utility.pps import PPSBuilder
+from osc_cr_converter.utility.pps_builder import PPSBuilder
 from osc_cr_converter.utility.general import trim_scenario, dataclass_is_complete
 from osc_cr_converter.utility.configuration import ConverterParams
-from osc_cr_converter.utility.abs_rel import AbsRel
+import osc_cr_converter.utility.logger as util_logger
 
-
-class EFailureReason(Enum):
-    """
-    The enum of reasons why the conversion failed
-    """
-    SCENARIO_FILE_INVALID_PATH = auto()
-    SCENARIO_FILE_IS_CATALOG = auto()
-    SCENARIO_FILE_IS_PARAMETER_VALUE_DISTRIBUTION = auto()
-    SCENARIO_FILE_CONTAINS_NO_STORYBOARD = auto()
-    SIMULATION_FAILED_CREATING_OUTPUT = auto()
-    NO_DYNAMIC_BEHAVIOR_FOUND = auto()
+# Configure the logging module
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Osc2CrConverter(Converter):
     """
     The main class of the OpenSCENARIO to CommonRoad conversion
     """
@@ -69,20 +59,20 @@
         self.author: str = config.scenario.author              # Author of the scenario
         self.affiliation: str = config.scenario.affiliation    # Affiliation of the author of the scenario
         self.source: str = config.scenario.source              # Source of the scenario
         self.tags: Set[Tag] = config.scenario.tags             # Tags of the scenario
 
         self.dt_cr: float = config.scenario.dt_cr              # Time step size of the CommonRoad scenario
 
-        self.config = config
+        self.config: ConverterParams = config                  # Configurations
 
         # The used SimWrapper implementation
         self.sim_wrapper: SimWrapper = EsminiWrapperProvider(config).provide_esmini_wrapper()
         # The used PPSBuilder instance
-        self.pps_builder: PPSBuilder = self._initialize_planning_problem_set()
+        self.pps_builder: PPSBuilder = config.initialize_planning_problem_set()
 
         # indicating whether the openDRIVE map defined in the openSCENARIO is used
         self.use_implicit_odr_file: bool = config.esmini.use_implicit_odr_file
         # indicating whether the huge mag contained in the scenario is trimmed
         self.trim_scenario: bool = config.scenario.trim_scenario
         # indicating whether the ego vehicle is kept or not in the saved scenario
         self.keep_ego_vehicle: bool = config.scenario.keep_ego_vehicle
@@ -93,27 +83,14 @@
         # analyzers of the scenario with CommonRoad tools
         self.analyzers: Union[Dict[EAnalyzer, Optional[Analyzer]], List[EAnalyzer]] = {}
 
         self.dt_sim: Optional[float] = config.esmini.dt_sim  # User-defined time step size for esmini simulation
         self.odr_file_override: Optional[str] = config.esmini.odr_file_override  # User-defined OpenDRIVE map to be used
         self.ego_filter: Optional[re.Pattern, str] = config.esmini.ego_filter  # Pattern of recognizing the ego vehicle
 
-    @staticmethod
-    def _initialize_planning_problem_set():
-        planning_problem_set = PPSBuilder()
-        planning_problem_set.time_interval = AbsRel(Interval(-10, 0), AbsRel.EUsage.REL_ADD)
-        planning_problem_set.pos_length = AbsRel(50, AbsRel.EUsage.ABS)
-        planning_problem_set.pos_width = AbsRel(10, AbsRel.EUsage.ABS)
-        planning_problem_set.pos_rotation = AbsRel(0, AbsRel.EUsage.REL_ADD)
-        planning_problem_set.pos_center_x = AbsRel(0, AbsRel.EUsage.REL_ADD)
-        planning_problem_set.pos_center_y = AbsRel(0, AbsRel.EUsage.REL_ADD)
-        planning_problem_set.velocity_interval = AbsRel(Interval(-5, 5), AbsRel.EUsage.REL_ADD)
-        planning_problem_set.orientation_interval = None
-        return planning_problem_set
-
     def get_analyzer_objects(self) -> Dict[EAnalyzer, Analyzer]:
         if self.analyzers is None:
             return {}
         elif isinstance(self.analyzers, list):
             return {e_analyzer: e_analyzer.analyzer_type() for e_analyzer in self.analyzers}
         elif isinstance(self.analyzers, dict):
             ret = {}
@@ -128,58 +105,59 @@
             -> Union[Scenario, EFailureReason]:
         """
         The main function, that runs the simulation wrapper (SimWrapper) and converts its results.
         :param source_file: the given openSCENARIO source file
         :return converted results if converted successfully. Otherwise, the reason for the failure.
         """
         self.config.general.name_xosc = os.path.basename(source_file).split('.')[0]
-        print(f"* Converting the OpenSCENARIO file: {self.config.general.name_xosc}.xosc")
+        util_logger.print_and_log_info(logger,
+                                       f"* Converting the OpenSCENARIO file: {self.config.general.name_xosc}.xosc")
 
         assert dataclass_is_complete(self)
 
         xosc_file = path.abspath(source_file)
 
         implicit_opendrive_path = self._pre_parse_scenario(xosc_file)
 
         if isinstance(implicit_opendrive_path, EFailureReason):
             self.conversion_result = implicit_opendrive_path
-            print(f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
             return self.conversion_result
 
         start_time = time.time()
         scenario, xodr_file, xodr_conversion_error = self._create_basic_scenario(implicit_opendrive_path)
         runtime = time.time() - start_time
-        print(f"*\t Map conversion takes {runtime:.2f} s")
+        util_logger.print_and_log_info(logger, f"*\t Map conversion takes {runtime:.2f} s")
 
         if isinstance(scenario, EFailureReason):
             self.conversion_result = scenario
-            print(f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
             return self.conversion_result
 
         if self.view_scenario:
             self.sim_wrapper.view_scenario(source_file, self.config.esmini.window_size)
         if self.render_to_gif:
             self.sim_wrapper.render_scenario_to_gif(source_file,
                                                     self.config.general.path_output + self.config.general.name_xosc
                                                     + ".gif")
 
         dt_sim = self.dt_sim if self.dt_sim is not None else self.dt_cr / 10
         res: WrapperSimResult = self.sim_wrapper.simulate_scenario(xosc_file, dt_sim)
         if res.ending_cause is ESimEndingCause.FAILURE:
             self.conversion_result = EFailureReason.SIMULATION_FAILED_CREATING_OUTPUT
-            print(f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
             return self.conversion_result
         if len(res.states) == 0:
             self.conversion_result = EFailureReason.NO_DYNAMIC_BEHAVIOR_FOUND
-            print(f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
             return self.conversion_result
         sim_time = res.sim_time
         runtime += res.runtime
         ending_cause = res.ending_cause
-        print(f"*\t Esmini simulation takes {res.runtime:.2f} s")
+        util_logger.print_and_log_info(logger, f"*\t Esmini simulation takes {res.runtime:.2f} s")
 
         start_time = time.time()
 
         ego_vehicle, ego_vehicle_found_with_filter = self._find_ego_vehicle(list(res.states.keys()))
         keep_ego_vehicle = self.keep_ego_vehicle
 
         obstacles_extra_info = ObstacleExtraInfoFinder(xosc_file, set(res.states.keys())).run()
@@ -199,16 +177,16 @@
         if len(scenario.lanelet_network.lanelets) > 0:
             scenario.assign_obstacles_to_lanelets()
 
         if self.trim_scenario:
             scenario = trim_scenario(scenario, deep_copy=False)
         pps = self.pps_builder.build(obstacles[ego_vehicle])
         runtime += time.time() - start_time
-        print(f"*\t Other conversion tasks take {time.time() - start_time:.2f} s")
-        print(f"* {self.config.general.name_xosc} is successfully converted 🏆!")
+        util_logger.print_and_log_info(logger, f"*\t Other conversion tasks take {time.time() - start_time:.2f} s")
+        util_logger.print_and_log_info(logger, f"* {self.config.general.name_xosc} is successfully converted 🏆!")
 
         if self.config.debug.write_to_xml:
             self.write_to_xml(scenario, pps)
 
         self.conversion_result = Osc2CrConverterResult(
             statistics=self.build_statistics(
                 obstacles=obstacles,
@@ -367,15 +345,15 @@
         used_states = [ScenarioObjectState.build_interpolated(states, t, obstacle_extra_info) for t in used_timestamps]
 
         obstacle_type = states[0].get_obstacle_type()
         if obstacle_type == ObstacleType.PEDESTRIAN:
             # for pedestrian, we consider an overapproximated circular area.
             # see: Koschi, Markus, et al. "Set-based prediction of pedestrians in urban environments considering
             # formalized traffic rules." IEEE ITSC, 2018
-            shape = Circle(max(states[0].get_object_length(), states[0].get_object_width())/2.)
+            shape = Circle(max(states[0].get_object_length()/2., states[0].get_object_width())/2.)
         else:
             shape = Rectangle(states[0].get_object_length(), states[0].get_object_width())
 
         trajectory = Trajectory(
             first_used_time_step,
             [state.to_cr_state(i + first_used_time_step) for i, state in enumerate(used_states)]
         )
@@ -427,21 +405,21 @@
         :param ego_vehicle_found_with_filter: the way of ego creation
         :param keep_ego_vehicle: whether the ego vehicle is kept
         :param ending_cause: why simulation is finished
         :param sim_time: simulation time in total
         :param runtime: runtime of converting the scenario
         :return: statistics
         """
-        string = "# ===========  Conversion Statistics  =========== #\n"
-        string += f"# Nr of obstacles: {len(obstacles)}\n"
-        string += f"# Scenario duration: {sim_time:.2f} s\n"
-        string += f"# The ego vehicle is removed \n" if not keep_ego_vehicle else "# the ego vehicle is kept \n"
-        string += f"# The ending cause {ending_cause.name}\n"
-        string += "# ============================================== #"
-        print(string)
+        util_logger.print_and_log_info(logger, "# ===========  Conversion Statistics  ========== #")
+        util_logger.print_and_log_info(logger, f"#\t Nr of obstacles: {len(obstacles)}")
+        util_logger.print_and_log_info(logger, f"#\t Scenario duration: {sim_time:.2f} s")
+        util_logger.print_and_log_info(logger, f"#\t The ego vehicle is removed"
+                                               f"" if not keep_ego_vehicle else "#\t the ego vehicle is kept")
+        util_logger.print_and_log_info(logger, f"#\t The ending cause {ending_cause.name}")
+        util_logger.print_and_log_info(logger, "# ============================================== #")
         return ConversionStatistics(
             num_obstacle_conversions=len(obstacles),
             failed_obstacle_conversions=[o_name for o_name, o in obstacles.items() if o is None],
             ego_vehicle=ego_vehicle,
             ego_vehicle_found_with_filter=ego_vehicle_found_with_filter,
             ego_vehicle_removed=not keep_ego_vehicle,
             sim_ending_cause=ending_cause,
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/result.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 from dataclasses import dataclass
 from multiprocessing import Lock
 from os import path
@@ -14,15 +14,15 @@
 from commonroad.common.file_reader import CommonRoadFileReader
 from commonroad.common.file_writer import CommonRoadFileWriter, OverwriteExistingFile
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.scenario import Scenario
 
 from osc_cr_converter.analyzer.error import AnalyzerErrorResult
 from osc_cr_converter.analyzer.result import AnalyzerResult
-from osc_cr_converter.analyzer.error_analyzer import EAnalyzer
+from osc_cr_converter.analyzer.enum_analyzer import EAnalyzer
 from osc_cr_converter.utility.statistics import ConversionStatistics
 from osc_cr_converter.converter.serializable import Serializable
 
 
 @dataclass(frozen=True)
 class Osc2CrConverterResult(Serializable):
     """
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/converter/serializable.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/serializable.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/udp_driver/common.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/common.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/abs_rel.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/abs_rel.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/configuration.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import dataclasses
 import inspect
 from dataclasses import dataclass, field
 from typing import Union, Any, Dict, List, Optional
+from datetime import datetime
 import pathlib
 import re
 import os
+import logging
 from omegaconf import OmegaConf
 
-from osc_cr_converter.wrapper.esmini.storyboard_element import EStoryBoardElementLevel
-
 from commonroad.scenario.scenario import Tag
+from commonroad.common.util import Interval
+
+from osc_cr_converter.utility.pps_builder import PPSBuilder
+from osc_cr_converter.utility.abs_rel import AbsRel
 
 
 def _dict_to_params(dict_params: Dict[str, Any], cls: Any) -> Any:
     """
     Converts dictionary to parameter class.
 
     :param dict_params: Dictionary containing parameters.
@@ -106,14 +110,17 @@
 
     # path of the root
     # name of the OpenSCENARIO file and its path
     name_xosc: str = ''
 
     # path for the output files
     path_output_abs: str = os.path.normpath(os.path.join(os.path.dirname(__file__), "../..")) + "/output/"
+    # path for logging information
+    path_output_log: str = path_output_abs + 'log/'
+    string_date_time = datetime.now().strftime("%Y_%m_%d_%H-%M-%S")
 
     def __init__(self):
         super().__init__()
         os.makedirs(self.path_output_abs, exist_ok=True)
 
     @property
     def path_output(self):
@@ -134,14 +141,17 @@
     write_to_xml: bool = False
 
     # plotting limits for axis
     plot_limit: Union[List[Union[int, float]], None] = None
     # with which time steps
     time_steps: Union[List[int], None] = None
 
+    # logging level
+    logging_level: str = logging.INFO
+
 
 @dataclass
 class EsminiParams(BaseParam):
     """Parameters specifying the esmini settings"""
 
     @dataclass(frozen=True)
     class WindowSize:
@@ -156,19 +166,14 @@
     # version
     version: str = "default"  # we use v2.29.3 as default version
 
     # lower and upper time limits for the simulation duration
     min_time: float = 5.
     max_time: float = 60.
 
-    # additional time interval after the completion of the last triggered
-    # act or storyboard (defined by the ignore level)
-    grace_period: float = 1.0
-    ignore_level: EStoryBoardElementLevel = EStoryBoardElementLevel.ACT
-
     # logging information
     log_to_console: bool = False
     log_to_file: bool = True
 
     # run the simulation using this random seed
     random_seed: int = 0
 
@@ -209,7 +214,20 @@
 @dataclass
 class ConverterParams(BaseParam):
     """Configuration parameters for OpenSCENARIO2CommonRoad converter."""
     general: GeneralParams = field(default_factory=GeneralParams)
     debug: DebugParams = field(default_factory=DebugParams)
     esmini: EsminiParams = field(default_factory=EsminiParams)
     scenario: ScenarioParams = field(default_factory=ScenarioParams)
+
+    @staticmethod
+    def initialize_planning_problem_set():
+        planning_problem_set = PPSBuilder()
+        planning_problem_set.time_interval = AbsRel(Interval(-10, 0), AbsRel.EUsage.REL_ADD)
+        planning_problem_set.pos_length = AbsRel(50, AbsRel.EUsage.ABS)
+        planning_problem_set.pos_width = AbsRel(10, AbsRel.EUsage.ABS)
+        planning_problem_set.pos_rotation = AbsRel(0, AbsRel.EUsage.REL_ADD)
+        planning_problem_set.pos_center_x = AbsRel(0, AbsRel.EUsage.REL_ADD)
+        planning_problem_set.pos_center_y = AbsRel(0, AbsRel.EUsage.REL_ADD)
+        planning_problem_set.velocity_interval = AbsRel(Interval(-5, 5), AbsRel.EUsage.REL_ADD)
+        planning_problem_set.orientation_interval = None
+        return planning_problem_set
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/general.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/obstacle_info.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/obstacle_info.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/pps.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/pps_builder.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/statistics.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/statistics.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/utility/visualization.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/scenario_object.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/scenario_object.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/base/sim_wrapper.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/sim_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         :param scenario_path Path to the .xosc scenario file
         :param window_size Wanted size of the rendering window
         """
         warnings.warn(f"{self.__class__} did not implement to view scenario")
 
     def render_scenario_to_gif(self, scenario_path: str, gif_file_path: str, fps: int = 30,
-                               gif_size=None) -> bool:
+                               gif_size: Optional[EsminiParams.WindowSize] = None) -> bool:
         """
         Create a gif of an XOSC file.
 
         :param scenario_path Path to the .xosc scenario file
         :param gif_file_path Path to the .gif product
         :param fps Frames per second of the gif
         :param gif_size Size of the gif
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.0.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import ctypes as ct
 import logging
 import math
@@ -16,15 +16,14 @@
 import warnings
 from multiprocessing import Lock
 from os import path
 from sys import platform
 from typing import Optional, List, Dict, Union
 
 import imageio
-from commonroad.common.validity import is_real_number
 
 from osc_cr_converter.wrapper.base.ending_cause import ESimEndingCause
 from osc_cr_converter.wrapper.esmini.esmini_scenario_object import SEStruct
 from osc_cr_converter.wrapper.esmini.storyboard_element import EStoryBoardElementState, \
     EStoryBoardElementLevel, StoryBoardElement
 from osc_cr_converter.wrapper.base.sim_wrapper import SimWrapper, WrapperSimResult
 from osc_cr_converter.utility.configuration import ConverterParams, EsminiParams
@@ -48,27 +47,25 @@
     _sim_end_detected_time: Optional[float]
 
     def __init__(self, esmini_bin_path: str, config: ConverterParams):
         super().__init__(config=config)
         self._esmini_lib_bin_path = esmini_bin_path
 
         self.min_time = config.esmini.min_time
-        self.grace_period = config.esmini.grace_period
-        self.ignored_level = config.esmini.ignore_level
-        self.random_seed = config.esmini.ignore_level
+        self.random_seed = config.esmini.random_seed
 
         self.log_to_console = config.esmini.log_to_console
         self.log_to_file = config.esmini.log_to_file
 
         self._reset()
 
     @property
     def min_time(self) -> float:
         """
-        Minimum simulation time that is used if grace_period is not None
+        Minimum simulation time.
         """
         return self._min_time
 
     @min_time.setter
     def min_time(self, new_min_time: Optional[float]):
         if new_min_time is None:
             self._min_time = 0.0
@@ -111,40 +108,14 @@
             self._esmini_lib.SE_SetSeed.argtypes = [ct.c_uint]
             self._esmini_lib.SE_GetObjectName.restype = ct.c_char_p
 
         else:
             warnings.warn(f"<EsminiWrapper/esmini_lib> Path {new_esmini_lib_bin_path} does not exist")
 
     @property
-    def grace_period(self) -> Optional[float]:
-        """
-        If no OpenSCENARIO element is active for this amount of time, and min_time has already passed. Ending the
-        simulation
-        """
-        return self._grace_period
-
-    @grace_period.setter
-    def grace_period(self, new_grace_time: Optional[float]):
-        if new_grace_time is None or is_real_number(new_grace_time):
-            self._grace_period = new_grace_time
-        else:
-            warnings.warn(f"<EsminiWrapper/grace_period> Tried to set to non real number value {new_grace_time}.")
-
-    @property
-    def ignored_level(self) -> Optional[EStoryBoardElementLevel]:
-        """
-        For the end detection using the grace_period ignore any active elements of this level or higher
-        """
-        return self._ignored_level
-
-    @ignored_level.setter
-    def ignored_level(self, new_ignored_level: Optional[EStoryBoardElementLevel]):
-        self._ignored_level = new_ignored_level
-
-    @property
     def random_seed(self) -> int:
         """
         Run the simulation using this random seed, default is 0
         """
         return self._random_seed
 
     @random_seed.setter
@@ -179,23 +150,18 @@
     def log_to_file(self, new_log_to_file: Union[None, bool, str]):
         if new_log_to_file is None:
             self._log_to_file = None
         elif isinstance(new_log_to_file, bool):
             if new_log_to_file:
                 log_dir = os.path.dirname(os.path.realpath(__file__)) + "/../../../output/log"
                 os.makedirs(log_dir, exist_ok=True)  # create directory if it doesn't exist
-                self._log_to_file = os.path.join(log_dir,
-                                                 "{}.txt".format(datetime.now().isoformat(sep="_", timespec="seconds")))
-                warnings.warn(f"Using default log file {self._log_to_file}")
+                self._log_to_file = os.path.join(self.config.general.path_output_log,
+                                                 f"esmini_{self.config.general.string_date_time}.log")
             else:
                 self._log_to_file = None
-        elif path.exists(path.dirname(new_log_to_file)):
-            self._log_to_file = path.abspath(new_log_to_file)
-        else:
-            warnings.warn(f"<EsminiWrapper/log_to_file> Logging dir {path.dirname(new_log_to_file)} does not exist.")
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["_esmini_lib"]
 
         del state["_all_sim_elements"]
         del state["_scenario_engine_initialized"]
@@ -233,27 +199,27 @@
                 states={self._get_scenario_object_name(object_id): states for object_id, states in
                         all_states.items()},
                 sim_time=sim_time,
                 runtime=runtime,
                 ending_cause=cause
             )
 
-    def view_scenario(self, scenario_path: str, window_size=None):
+    def view_scenario(self, scenario_path: str, window_size: Optional[EsminiParams.WindowSize] = None):
         with EsminiWrapper.__lock:
             if not self._initialize_scenario_engine(scenario_path, viewer_mode=1, use_threading=True):
                 warnings.warn("<EsminiWrapper/view_scenario> Failed to initialize scenario engine")
                 return
             if window_size is not None:
                 self._set_set_window_size(window_size)
             while self._sim_finished() is None:
                 self._sim_step(None)
             self._close_scenario_engine()
 
     def render_scenario_to_gif(self, scenario_path: str, gif_file_path: str, fps: int = 30,
-                               window_size=None) -> bool:
+                               window_size: Optional[EsminiParams.WindowSize] = None) -> bool:
         with EsminiWrapper.__lock:
             if not self._initialize_scenario_engine(scenario_path, viewer_mode=7, use_threading=False):
                 warnings.warn("<EsminiWrapper/render_scenario_to_gif> Failed to initialize scenario engine")
                 return False
             if window_size is not None:
                 self._set_set_window_size(window_size)
             image_regex = re.compile(r"screen_shot_\d{5,}\.tga")
@@ -333,15 +299,15 @@
         if not self._first_frame_run:
             return None
         now = self.esmini_lib.SE_GetSimulationTime()
         if self.esmini_lib.SE_GetQuitFlag() == 1:
             self._log("{:.3f}: esmini requested quitting -> Scenario finished completely ".format(now))
             return ESimEndingCause.SCENARIO_FINISHED_BY_SIMULATOR
         if now >= self.max_time:
-            self._log("{:.3f}: Max Execution tim reached ".format(now))
+            self._log("{:.3f}: Max Execution time reached ".format(now))
             return ESimEndingCause.MAX_TIME_REACHED
         return None
 
     def _get_scenario_object_states(self) -> Optional[Dict[int, SEStruct]]:
         if not self._scenario_engine_initialized:
             raise RuntimeError("Scenario Engine not initialized")
         try:
```

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/osc_cr_converter/wrapper/esmini/storyboard_element.py` & `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/storyboard_element.py`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.3/setup.py` & `commonroad-openscenario-converter-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='commonroad-openscenario-converter',
-      version='0.0.3',
+      version='0.0.4',
       description='Converter between OpenSCENARIO and CommonRoad formats',
       keywords="scenario description, autonomous driving",
       author='Yuanfei Lin, Michael Ratzel',
       author_email='yuanfei.lin@tum.de',
       license='BSD 3-Clause',
       packages=find_packages(),
       install_requires=[
-          'commonroad-io>=2023.1',
+          'commonroad-io==2023.1',
           'commonroad-scenario-designer>=0.7.0',
           'matplotlib>=3.5.2',
           'imageio>=2.28.1',
           'numpy>=1.19.0',
           'tqdm>=4.65.0',
           'scenariogeneration>=0.9.0',
           'protobuf>=3.19'
```

### Comparing `commonroad-openscenario-converter-0.0.3/tests/test_conversion.py` & `commonroad-openscenario-converter-0.0.4/tests/test_conversion.py`

 * *Files identical despite different names*

