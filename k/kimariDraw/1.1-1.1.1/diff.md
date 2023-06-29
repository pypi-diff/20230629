# Comparing `tmp/kimariDraw-1.1.tar.gz` & `tmp/kimariDraw-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariDraw-1.1.tar", last modified: Thu Jun 29 06:23:06 2023, max compression
+gzip compressed data, was "kimariDraw-1.1.1.tar", last modified: Thu Jun 29 06:37:25 2023, max compression
```

## Comparing `kimariDraw-1.1.tar` & `kimariDraw-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:23:06.752588 kimariDraw-1.1/
--rw-rw-rw-   0        0        0     1086 2023-06-28 14:34:53.000000 kimariDraw-1.1/LICENSE
--rw-rw-rw-   0        0        0      369 2023-06-29 06:23:06.751555 kimariDraw-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2430 2023-06-29 06:08:51.000000 kimariDraw-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 06:23:06.720556 kimariDraw-1.1/kimariDraw/
--rw-rw-rw-   0        0        0        0 2023-06-29 03:29:28.000000 kimariDraw-1.1/kimariDraw/__init__.py
--rw-rw-rw-   0        0        0      739 2023-06-29 05:58:56.000000 kimariDraw-1.1/kimariDraw/__main__.py
--rw-rw-rw-   0        0        0     1230 2023-06-28 16:53:47.000000 kimariDraw-1.1/kimariDraw/kd_data.py
--rw-rw-rw-   0        0        0     3692 2023-06-28 14:34:53.000000 kimariDraw-1.1/kimariDraw/kd_parser.py
--rw-rw-rw-   0        0        0     1820 2023-06-29 03:25:05.000000 kimariDraw-1.1/kimariDraw/kd_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:23:06.749554 kimariDraw-1.1/kimariDraw.egg-info/
--rw-rw-rw-   0        0        0      369 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 06:23:06.000000 kimariDraw-1.1/kimariDraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 06:23:06.753560 kimariDraw-1.1/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-06-29 06:22:51.000000 kimariDraw-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:37:25.475494 kimariDraw-1.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-28 14:34:53.000000 kimariDraw-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      371 2023-06-29 06:37:25.475494 kimariDraw-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2430 2023-06-29 06:08:51.000000 kimariDraw-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 06:37:25.459863 kimariDraw-1.1.1/kimariDraw/
+-rw-rw-rw-   0        0        0        0 2023-06-29 03:29:28.000000 kimariDraw-1.1.1/kimariDraw/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-06-29 06:37:08.000000 kimariDraw-1.1.1/kimariDraw/__main__.py
+-rw-rw-rw-   0        0        0     1230 2023-06-28 16:53:47.000000 kimariDraw-1.1.1/kimariDraw/kd_data.py
+-rw-rw-rw-   0        0        0      988 2023-06-29 06:37:08.000000 kimariDraw-1.1.1/kimariDraw/kd_file.py
+-rw-rw-rw-   0        0        0     2741 2023-06-29 06:37:08.000000 kimariDraw-1.1.1/kimariDraw/kd_parser.py
+-rw-rw-rw-   0        0        0     1820 2023-06-29 03:25:05.000000 kimariDraw-1.1.1/kimariDraw/kd_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-29 06:37:25.475494 kimariDraw-1.1.1/kimariDraw.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 06:37:25.000000 kimariDraw-1.1.1/kimariDraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 06:37:25.475494 kimariDraw-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-06-29 06:37:22.000000 kimariDraw-1.1.1/setup.py
```

### Comparing `kimariDraw-1.1/LICENSE` & `kimariDraw-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1/README.md` & `kimariDraw-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1/kimariDraw/__main__.py` & `kimariDraw-1.1.1/kimariDraw/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import argparse
-from kd_parser import *
-from kd_plot import *
-from kd_data import *
+
+from kimariDraw.kd_parser import KDFileParser
+from kimariDraw.kd_plot import kd_draw
+
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Draw energy profile plot using matplotlib')
     parser.add_argument('input_file', type=str, help='path to input data file')
     parser.add_argument('-s', '--save_name', type=str, default='figure', help='name of the output image file')
     return parser.parse_args()
 
+
 def main():
     args = parse_args()
     # 读取数据    
     data = KDFileParser(args.input_file).parse().get_kd_data()
     # 判断 save_name 是否为空
-    if args.save_name == None:
+    if args.save_name is None:
         kd_draw(data)
     else:
         kd_draw(data, args.save_name)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `kimariDraw-1.1/kimariDraw/kd_data.py` & `kimariDraw-1.1.1/kimariDraw/kd_data.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1/kimariDraw/kd_plot.py` & `kimariDraw-1.1.1/kimariDraw/kd_plot.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1/setup.py` & `kimariDraw-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='kimariDraw',
-    version='1.1',
+    version='1.1.1',
     description='The application is used to draw the Energy Profile Map',
     author='kimariyb',
     author_email='kimariyb@163.com',
     url='https://github.com/kimariyb/kimariDraw',
     install_requires=[
         'numpy',
         'matplotlib',
```

