# Comparing `tmp/kimariDraw-1.1.4.tar.gz` & `tmp/kimariDraw-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariDraw-1.1.4.tar", last modified: Thu Jun 29 15:37:36 2023, max compression
+gzip compressed data, was "kimariDraw-1.1.5.tar", last modified: Thu Jun 29 16:04:47 2023, max compression
```

## Comparing `kimariDraw-1.1.4.tar` & `kimariDraw-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/
--rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      371 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.161397 kimariDraw-1.1.4/kimariDraw/
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.175479 kimariDraw-1.1.4/kimariDraw/Data/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Data/__init__.py
--rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.4/kimariDraw/Data/kd_data.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.179491 kimariDraw-1.1.4/kimariDraw/Parser/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Parser/__init__.py
--rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.4/kimariDraw/Parser/kd_file.py
--rw-rw-rw-   0        0        0     2710 2023-06-29 14:24:25.000000 kimariDraw-1.1.4/kimariDraw/Parser/kd_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.182499 kimariDraw-1.1.4/kimariDraw/Plot/
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/Plot/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-06-29 15:35:16.000000 kimariDraw-1.1.4/kimariDraw/Plot/kd_plot.py
--rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/__init__.py
--rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.4/kimariDraw/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 15:37:36.172475 kimariDraw-1.1.4/kimariDraw.egg-info/
--rw-rw-rw-   0        0        0      371 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 15:37:36.000000 kimariDraw-1.1.4/kimariDraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 15:37:36.184504 kimariDraw-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-29 15:37:31.000000 kimariDraw-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.781459 kimariDraw-1.1.5/
+-rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      371 2023-06-29 16:04:47.781459 kimariDraw-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.758398 kimariDraw-1.1.5/kimariDraw/
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.773439 kimariDraw-1.1.5/kimariDraw/Data/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Data/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.5/kimariDraw/Data/kd_data.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.777449 kimariDraw-1.1.5/kimariDraw/Parser/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Parser/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.5/kimariDraw/Parser/kd_file.py
+-rw-rw-rw-   0        0        0     2708 2023-06-29 15:59:51.000000 kimariDraw-1.1.5/kimariDraw/Parser/kd_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.779455 kimariDraw-1.1.5/kimariDraw/Plot/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/Plot/__init__.py
+-rw-rw-rw-   0        0        0     2117 2023-06-29 15:59:14.000000 kimariDraw-1.1.5/kimariDraw/Plot/kd_plot.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.5/kimariDraw/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:04:47.770430 kimariDraw-1.1.5/kimariDraw.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 16:04:47.000000 kimariDraw-1.1.5/kimariDraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 16:04:47.782462 kimariDraw-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-29 16:02:14.000000 kimariDraw-1.1.5/setup.py
```

### Comparing `kimariDraw-1.1.4/LICENSE` & `kimariDraw-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.4/README.md` & `kimariDraw-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.4/kimariDraw/Data/kd_data.py` & `kimariDraw-1.1.5/kimariDraw/Data/kd_data.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.4/kimariDraw/Parser/kd_file.py` & `kimariDraw-1.1.5/kimariDraw/Parser/kd_file.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.4/kimariDraw/Parser/kd_parser.py` & `kimariDraw-1.1.5/kimariDraw/Parser/kd_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
                 x_str, y_str = line.strip().split(',')
                 x, y = float(x_str), float(y_str)
                 data.append((x, y))
             elif line.strip() == 'BEGIN':
                 data_started = True
 
         return header, data
-
```

### Comparing `kimariDraw-1.1.4/kimariDraw/Plot/kd_plot.py` & `kimariDraw-1.1.5/kimariDraw/Plot/kd_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,30 @@
     num_y = data.get_num_y()
 
     # 创建画布和子图对象
     fig, ax = plt.subplots(figsize=data.figure_size)
 
     # 设置 x 轴和 y 轴的范围
     ax.set_xlim(0, np.max(num_x) + 1)
-    y_min = np.min(num_y) * 1.1 if np.min(num_y) < 0 else np.min(num_y) * 0.9
-    y_max = np.max(num_y) * 1.1 if np.max(num_y) > 0 else np.max(num_y) * 0.9
+    y_min = np.min(num_y) * 1.25 if np.min(num_y) < 0 else np.min(num_y) * 0.75
+    y_max = np.max(num_y) * 1.25 if np.max(num_y) > 0 else np.max(num_y) * 0.75
     ax.set_ylim(y_min, y_max)
 
     # 绘制平台
     # 绘制数据点
     # for i in range(len(num_x)):
     #    ax.scatter(num_x[i], num_y[i])
 
-    # 在每个数据点上绘制长度为0.4的水平线
+    # 在每个数据点上绘制长度为 0.4 的水平线
     for i, (x, y) in enumerate(zip(num_x, num_y)):
         ax.plot([x - 0.2, x + 0.2], [y, y], color='black', linewidth=3)
-        ax.text(x, y * 1.01, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10)
+        if abs(y) > 100:
+            ax.text(x, y + 2, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10)
+        else:
+            ax.text(x, y + 0.5, f"{y:.1f}", ha='center', va='bottom', fontweight='bold', fontsize=10)
 
     for i in range(len(num_x) - 1):
         ax.plot([num_x[i]+0.2, num_x[i+1]-0.2], [num_y[i], num_y[i+1]],  color='black', linewidth=1, linestyle='--')
 
     # 设置 x 轴和 y 轴标签
     y_label = "Free Energy" + f" ({data.unit})"
     ax.set_xlabel("Reaction Coordinate", fontweight='bold', fontsize=14)
```

### Comparing `kimariDraw-1.1.4/kimariDraw/main.py` & `kimariDraw-1.1.5/kimariDraw/main.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.4/setup.py` & `kimariDraw-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='kimariDraw',
-    version='1.1.4',
+    version='1.1.5',
     description='The application is used to draw the Energy Profile Map',
     author='kimariyb',
     author_email='kimariyb@163.com',
     url='https://github.com/kimariyb/kimariDraw',
     install_requires=[
         'numpy',
         'matplotlib',
@@ -18,8 +18,8 @@
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     python_requires='>=3.9'
-)
+)
```

