# Comparing `tmp/jcmutils-1.6.3.tar.gz` & `tmp/jcmutils-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.6.3.tar", last modified: Thu Jun 29 08:10:47 2023, max compression
+gzip compressed data, was "jcmutils-1.6.4.tar", last modified: Thu Jun 29 08:16:52 2023, max compression
```

## Comparing `jcmutils-1.6.3.tar` & `jcmutils-1.6.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:10:47.598101 jcmutils-1.6.3/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.3/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:10:47.594101 jcmutils-1.6.3/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.3/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:10:47.594101 jcmutils-1.6.3/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.3/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    17941 2023-06-29 08:10:16.000000 jcmutils-1.6.3/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.3/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.3/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.3/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:10:47.594101 jcmutils-1.6.3/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:10:47.000000 jcmutils-1.6.3/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 08:10:47.000000 jcmutils-1.6.3/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 08:10:47.000000 jcmutils-1.6.3/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:10:47.000000 jcmutils-1.6.3/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 08:10:47.000000 jcmutils-1.6.3/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:10:47.598101 jcmutils-1.6.3/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 08:10:26.000000 jcmutils-1.6.3/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:16:52.073908 jcmutils-1.6.4/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.4/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:16:52.073908 jcmutils-1.6.4/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.4/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:16:52.069908 jcmutils-1.6.4/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.4/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    17941 2023-06-29 08:16:01.000000 jcmutils-1.6.4/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.4/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.4/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.4/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:16:52.069908 jcmutils-1.6.4/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:16:51.000000 jcmutils-1.6.4/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 08:16:51.000000 jcmutils-1.6.4/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 08:16:51.000000 jcmutils-1.6.4/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:16:51.000000 jcmutils-1.6.4/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 08:16:51.000000 jcmutils-1.6.4/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:16:52.073908 jcmutils-1.6.4/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 08:16:31.000000 jcmutils-1.6.4/setup.py
```

### Comparing `jcmutils-1.6.3/LICENSE` & `jcmutils-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.3/README.md` & `jcmutils-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.3/jcmutils/dataset_utils.py` & `jcmutils-1.6.4/jcmutils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         
         width_lower_border = 0.6*(periodic_x/source_density)/output_image.shape[1]
         height_lower_border = 0.6*(periodic_y/source_density)/output_image.shape[0]
         width_lower_warn = 0.9*(periodic_x/source_density)/output_image.shape[1]
         height_lower_warn = 0.9*(periodic_y/source_density)/output_image.shape[0]
         width_upper_warn = 1.8*(periodic_x/source_density)/output_image.shape[1]
         height_upper_warn = 1.8*(periodic_y/source_density)/output_image.shape[0]
-        width_upper_border = 2.1*(periodic_x/source_density)/output_image.shape[1]
-        height_upper_border = 2.1*(periodic_y/source_density)/output_image.shape[0]
+        width_upper_border = 2.5*(periodic_x/source_density)/output_image.shape[1]
+        height_upper_border = 2.5*(periodic_y/source_density)/output_image.shape[0]
         # 大致检测结果正确性
         if width <=width_lower_border or height <=height_lower_border :
             logger.error(f"false mixed image detected,key-{self.origin_key} was detected too small width or height. the width is {width},height is {height},which is smaller than ({width_lower_border},{height_lower_border}) , try a smaller signal_level")
             raise Exception("error detected , please read log")
         if width <= width_lower_warn or height <=height_lower_warn:
             logger.warning(f"key-{self.origin_key} mixed image smaller than ({width_lower_warn},{height_lower_warn}) maybe a little bit strage , please check")
         if width >= width_upper_warn or height >= height_upper_warn:
```

### Comparing `jcmutils-1.6.3/jcmutils/gen_sources.py` & `jcmutils-1.6.4/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.3/jcmutils/logger.py` & `jcmutils-1.6.4/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.3/jcmutils/solver.py` & `jcmutils-1.6.4/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.3/setup.py` & `jcmutils-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.6.3'
+VERSION = '1.6.4'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

