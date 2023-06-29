# Comparing `tmp/kimariDraw-1.1.3.tar.gz` & `tmp/kimariDraw-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariDraw-1.1.3.tar", last modified: Thu Jun 29 14:54:02 2023, max compression
+gzip compressed data, was "kimariDraw-1.1.4.tar", last modified: Thu Jun 29 15:37:36 2023, max compression
```

## Comparing `kimariDraw-1.1.3.tar` & `kimariDraw-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.945016 kimariDraw-1.1.3/
--rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      371 2023-06-29 14:54:02.944013 kimariDraw-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.921955 kimariDraw-1.1.3/kimariDraw/
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.934990 kimariDraw-1.1.3/kimariDraw/Data/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Data/__init__.py
--rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.3/kimariDraw/Data/kd_data.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.940003 kimariDraw-1.1.3/kimariDraw/Parser/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Parser/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.3/kimariDraw/Parser/kd_file.py
--rw-rw-rw-   0        0        0     2710 2023-06-29 14:24:25.000000 kimariDraw-1.1.3/kimariDraw/Parser/kd_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.943011 kimariDraw-1.1.3/kimariDraw/Plot/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Plot/__init__.py
--rw-rw-rw-   0        0        0     1836 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Plot/kd_plot.py
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/__init__.py
--rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.932984 kimariDraw-1.1.3/kimariDraw.egg-info/
--rw-rw-rw-   0        0        0      371 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:54:02.945016 kimariDraw-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-29 14:26:07.000000 kimariDraw-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      371 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.161397 kimariDraw-1.1.4/kimariDraw/
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.175479 kimariDraw-1.1.4/kimariDraw/Data/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Data/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.4/kimariDraw/Data/kd_data.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.179491 kimariDraw-1.1.4/kimariDraw/Parser/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Parser/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.4/kimariDraw/Parser/kd_file.py
+-rw-rw-rw-   0        0        0     2710 2023-06-29 14:24:25.000000 kimariDraw-1.1.4/kimariDraw/Parser/kd_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.182499 kimariDraw-1.1.4/kimariDraw/Plot/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Plot/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-06-29 15:35:16.000000 kimariDraw-1.1.4/kimariDraw/Plot/kd_plot.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.172475 kimariDraw-1.1.4/kimariDraw.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-29 15:37:31.000000 kimariDraw-1.1.4/setup.py
```

### Comparing `kimariDraw-1.1.3/LICENSE` & `kimariDraw-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/README.md` & `kimariDraw-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/kimariDraw/Data/kd_data.py` & `kimariDraw-1.1.4/kimariDraw/Data/kd_data.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/kimariDraw/Parser/kd_file.py` & `kimariDraw-1.1.4/kimariDraw/Parser/kd_file.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/kimariDraw/Parser/kd_parser.py` & `kimariDraw-1.1.4/kimariDraw/Parser/kd_parser.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/kimariDraw/Plot/kd_plot.py` & `kimariDraw-1.1.4/kimariDraw/Plot/kd_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     num_y = data.get_num_y()
 
     # 创建画布和子图对象
     fig, ax = plt.subplots(figsize=data.figure_size)
 
     # 设置 x 轴和 y 轴的范围
     ax.set_xlim(0, np.max(num_x) + 1)
-    ax.set_ylim(np.min(num_y) * 0.9, np.max(num_y) * 1.1)
+    y_min = np.min(num_y) * 1.1 if np.min(num_y) < 0 else np.min(num_y) * 0.9
+    y_max = np.max(num_y) * 1.1 if np.max(num_y) > 0 else np.max(num_y) * 0.9
+    ax.set_ylim(y_min, y_max)
 
     # 绘制平台
     # 绘制数据点
     # for i in range(len(num_x)):
     #    ax.scatter(num_x[i], num_y[i])
 
     # 在每个数据点上绘制长度为0.4的水平线
```

### Comparing `kimariDraw-1.1.3/kimariDraw/main.py` & `kimariDraw-1.1.4/kimariDraw/main.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.3/setup.py` & `kimariDraw-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='kimariDraw',
-    version='1.1.3',
+    version='1.1.4',
     description='The application is used to draw the Energy Profile Map',
     author='kimariyb',
     author_email='kimariyb@163.com',
     url='https://github.com/kimariyb/kimariDraw',
     install_requires=[
         'numpy',
         'matplotlib',
```

