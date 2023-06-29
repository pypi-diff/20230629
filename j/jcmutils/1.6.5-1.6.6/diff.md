# Comparing `tmp/jcmutils-1.6.5.tar.gz` & `tmp/jcmutils-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.6.5.tar", last modified: Thu Jun 29 08:30:13 2023, max compression
+gzip compressed data, was "jcmutils-1.6.6.tar", last modified: Thu Jun 29 08:40:57 2023, max compression
```

## Comparing `jcmutils-1.6.5.tar` & `jcmutils-1.6.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:30:13.343119 jcmutils-1.6.5/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.5/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:30:13.343119 jcmutils-1.6.5/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.5/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:30:13.343119 jcmutils-1.6.5/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.5/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)    17940 2023-06-29 08:29:21.000000 jcmutils-1.6.5/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.5/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.5/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.5/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:30:13.343119 jcmutils-1.6.5/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:30:13.000000 jcmutils-1.6.5/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 08:30:13.000000 jcmutils-1.6.5/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 08:30:13.000000 jcmutils-1.6.5/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:30:13.000000 jcmutils-1.6.5/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 08:30:13.000000 jcmutils-1.6.5/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:30:13.343119 jcmutils-1.6.5/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 08:29:30.000000 jcmutils-1.6.5/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.6.6/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:40:56.999254 jcmutils-1.6.6/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-05-17 04:08:25.000000 jcmutils-1.6.6/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)    17940 2023-06-29 08:38:54.000000 jcmutils-1.6.6/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.6.6/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-17 04:08:25.000000 jcmutils-1.6.6/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-06-29 08:40:56.999254 jcmutils-1.6.6/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-06-29 08:40:56.000000 jcmutils-1.6.6/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-06-29 08:40:56.999254 jcmutils-1.6.6/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-06-29 08:39:05.000000 jcmutils-1.6.6/setup.py
```

### Comparing `jcmutils-1.6.5/LICENSE` & `jcmutils-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.5/README.md` & `jcmutils-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.5/jcmutils/dataset_utils.py` & `jcmutils-1.6.6/jcmutils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 min_dist = dist
                 c = conners
 
         # compute the rotated bounding box of the largest contour
         x,y,w,h=cv2.boundingRect(c)
 
         # 延伸扩展边界，避免强截断
-        x += extend_length
+        x -= extend_length
         y -= extend_length
         w += extend_length*2
         h += extend_length*2
         
         # img=cv2.rectangle(defect_img,(x,y),(x+w,y+h),(0,255,0),2)
         # 根据左上角坐标和长宽计算矩形的四个角点坐标
         rect_points = [(x, y),
```

### Comparing `jcmutils-1.6.5/jcmutils/gen_sources.py` & `jcmutils-1.6.6/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.5/jcmutils/logger.py` & `jcmutils-1.6.6/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.5/jcmutils/solver.py` & `jcmutils-1.6.6/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.6.5/setup.py` & `jcmutils-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.6.5'
+VERSION = '1.6.6'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

