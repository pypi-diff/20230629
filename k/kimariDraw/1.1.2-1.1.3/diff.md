# Comparing `tmp/kimariDraw-1.1.2.tar.gz` & `tmp/kimariDraw-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariDraw-1.1.2.tar", last modified: Thu Jun 29 06:50:27 2023, max compression
+gzip compressed data, was "kimariDraw-1.1.3.tar", last modified: Thu Jun 29 14:54:02 2023, max compression
```

## Comparing `kimariDraw-1.1.2.tar` & `kimariDraw-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.817810 kimariDraw-1.1.2/
--rw-rw-rw-   0        0        0     1086 2023-06-28 14:34:53.000000 kimariDraw-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      371 2023-06-29 06:50:27.816809 kimariDraw-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2430 2023-06-29 06:08:51.000000 kimariDraw-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.791040 kimariDraw-1.1.2/kimariDraw/
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.805040 kimariDraw-1.1.2/kimariDraw/Data/
--rw-rw-rw-   0        0        0        0 2023-06-29 06:44:59.000000 kimariDraw-1.1.2/kimariDraw/Data/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-06-28 16:53:47.000000 kimariDraw-1.1.2/kimariDraw/Data/kd_data.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.811040 kimariDraw-1.1.2/kimariDraw/Parser/
--rw-rw-rw-   0        0        0        0 2023-06-29 06:45:16.000000 kimariDraw-1.1.2/kimariDraw/Parser/__init__.py
--rw-rw-rw-   0        0        0      976 2023-06-29 06:50:08.000000 kimariDraw-1.1.2/kimariDraw/Parser/kd_file.py
--rw-rw-rw-   0        0        0     2748 2023-06-29 06:46:54.000000 kimariDraw-1.1.2/kimariDraw/Parser/kd_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.814810 kimariDraw-1.1.2/kimariDraw/Plot/
--rw-rw-rw-   0        0        0        0 2023-06-29 06:45:29.000000 kimariDraw-1.1.2/kimariDraw/Plot/__init__.py
--rw-rw-rw-   0        0        0     1836 2023-06-29 06:50:08.000000 kimariDraw-1.1.2/kimariDraw/Plot/kd_plot.py
--rw-rw-rw-   0        0        0        0 2023-06-29 03:29:28.000000 kimariDraw-1.1.2/kimariDraw/__init__.py
--rw-rw-rw-   0        0        0      777 2023-06-29 06:46:54.000000 kimariDraw-1.1.2/kimariDraw/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 06:50:27.801039 kimariDraw-1.1.2/kimariDraw.egg-info/
--rw-rw-rw-   0        0        0      371 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 06:50:27.000000 kimariDraw-1.1.2/kimariDraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 06:50:27.818808 kimariDraw-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-29 06:50:23.000000 kimariDraw-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.945016 kimariDraw-1.1.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-26 16:23:56.000000 kimariDraw-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      371 2023-06-29 14:54:02.944013 kimariDraw-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2550 2023-06-29 14:24:48.000000 kimariDraw-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.921955 kimariDraw-1.1.3/kimariDraw/
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.934990 kimariDraw-1.1.3/kimariDraw/Data/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Data/__init__.py
+-rw-rw-rw-   0        0        0     1145 2023-06-29 14:20:48.000000 kimariDraw-1.1.3/kimariDraw/Data/kd_data.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.940003 kimariDraw-1.1.3/kimariDraw/Parser/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Parser/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-06-29 14:24:18.000000 kimariDraw-1.1.3/kimariDraw/Parser/kd_file.py
+-rw-rw-rw-   0        0        0     2710 2023-06-29 14:24:25.000000 kimariDraw-1.1.3/kimariDraw/Parser/kd_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.943011 kimariDraw-1.1.3/kimariDraw/Plot/
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Plot/__init__.py
+-rw-rw-rw-   0        0        0     1836 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/Plot/kd_plot.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-06-29 13:22:39.000000 kimariDraw-1.1.3/kimariDraw/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:54:02.932984 kimariDraw-1.1.3/kimariDraw.egg-info/
+-rw-rw-rw-   0        0        0      371 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 14:54:02.000000 kimariDraw-1.1.3/kimariDraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:54:02.945016 kimariDraw-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-29 14:26:07.000000 kimariDraw-1.1.3/setup.py
```

### Comparing `kimariDraw-1.1.2/LICENSE` & `kimariDraw-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.2/README.md` & `kimariDraw-1.1.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 <div align="center">
     <img src="figure/logo.png" width="250px"  alt=""/>
 </div>
 
 ---
 
-kimariDraw 是一个用于绘制化学反应能量折线图的 Python 命令行程序，使用 Matplotlib 和 Numpy 库实现绘图功能。其目的是为了更方便的绘制出化学反应能量折线图，特别是在每周的组会上，需要绘制化学反应能量折线图
+kimariDraw 是一个用于绘制化学反应能量折线图的 Python 命令行程序，使用 Matplotlib 和 Numpy 库实现绘图功能。其目的是为了更方便的绘制出化学反应能量折线图，特别是在每周的组会上，需要你绘制化学反应能量折线图的时候，kimariDraw 能快速的帮你制作出化学反应能量折线图。
 
 ## 安装
 
-你可以通过以下命令使用 pip 安装 kimariDraw：
+你可以通过以下命令使用 pip 安装 kimariDraw，除此之外还需要确保已经安装了 Matplotlib 和 Numpy。
 
 ```bash
 pip install kimariDraw
+pip install Numpy
+pip install Matplotlib
 ```
 
-除此之外，还可以直接从 Github 上 clone:
+除此之外，还可以直接从 Github 上 clone（不推荐，因为这样得到的是源码）。
 
 ```bash
 git clone https://github.com/kimariyb/kimariDraw.git
 ```
 
 ## 使用
 
-使用 kimariDraw 绘制折线图需要一个符合 .kd 格式的文件。该文件应包含绘制折线图所需的数据和参数。以下是一个 .kd 文件的示例：
+使用 kimariDraw 绘制折线图需要一个 .kd 格式的文件。该文件应包含绘制折线图所需的数据和参数。以下是一个 .kd 文件的示例：
 
 ```basic
-# 文件头格式，文件头必须以 # 开头，包含键值对，以 : 分隔，例如 # UNIT = kj/mol，key 不区分大小写。
-# UNIT: 能量单位，例如 kJ/mol
-# TEMPERATURE: 温度，例如 298，默认为开尔文温度
-# FIGURE_SIZE: 画布大小，例如 8,6
-# COLOR_THEME: 颜色主题，例如 nature
-# FONT_FAMILY: 坐标字体，例如 Times New Roman
-# SIVE_IMAGE: 保存的图片格式，例如 PNG
-
-# 数据行格式，数据行格式以 BEGIN 开头，用逗号分隔，表示反应进度和能量
-# 数据行每行包含两个浮点数第一个数表示反应进度，后面的数表示能量
-# 数据行以 END 开头的行结束
-
-# 示例
-# # UNIT = Hartree
-# # TEMPERATURE = 398
-# # FIGURE_SIZE = 8, 4
-# # COLOR_THEME = science
-# # FONT_FAMILY = Arial
-# # SAVE_IMAGE = png
-# #
-# # BEGIN
-# # 1, 375.5
-# # 2, 405.5
-# # 3, 323.7
-# # 4, 457.8
-# # 5, 300.6
-# # 6, 346.9
-# # END
+# UNIT = Hartree
+# FIGURE_SIZE = 8, 4
+# COLOR_THEME = science
+# FONT_FAMILY = Arial
+# SAVE_IMAGE = png
+
+BEGIN
+1, 375.5
+2, 405.5
+3, 323.7
+4, 457.8
+5, 300.6
+6, 346.9
+END
 ```
 
+在示例中，以 `#` 开头的是文件的文件头，其包含了单位、画布的大小、颜色以及字体等参数，以 `=` 分隔。`BEGIN` 和 `END` 之间表示的数据行，数据行每行包含两个数，用逗号分隔，分别表示反应进度和能量。反应进度必须从 1 开始。注意，文件头和数据行的中间必须存在一个空格。
+
+- `UNIT:` 能量单位，例如 kJ/mol
+- `FIGURE_SIZE:` 画布大小，例如 8,6
+- `COLOR_THEME:` 颜色主题，例如 nature
+- `FONT_FAMILY:` 坐标字体，例如 Times New Roman
+- `SIVE_IMAGE:` 保存的图片格式，例如 PNG
+
 使用 kimariDraw 绘制折线图的命令如下：
 
 ```bash
 kimariDraw <filename>
 ```
 
-其中 <filename> 是一个 .kd 格式的文件。
+其中 `<filename>` 是一个 `.kd` 格式的文件。
 
-假如要运行 example 目录下的 test2.kd 文件，并且生成 test.png 则可以输入以下指令：
+假如要运行 example 目录下的 `test2.kd` 文件，并且生成 `test.png` 则可以输入以下指令：
 
 ```bash
 kimariDraw ./example/test2.kd -s test
 ```
 
 则可以在当前目录下得到 test.png:
 
@@ -77,12 +73,12 @@
 
 kimariDraw 支持以下命令行参数：
 
 - `-s`, `--save_name`：指定输出文件名，默认为 figure.png
 
 ## 作者
 
-kimariDraw 是由 kimariyb 开发的。
+**kimariDraw 是由 kimariyb 开发的。**
 
 ## 许可证
 
 kimariDraw 使用 MIT 许可证。详细信息请参考 LICENSE 文件。
```

### Comparing `kimariDraw-1.1.2/kimariDraw/Data/kd_data.py` & `kimariDraw-1.1.3/kimariDraw/Data/kd_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import numpy as np
 
 
 class KDData:
 
-    def __init__(self, unit, temperature, figure_size, color_theme, font_family, save_image, num_data):
+    def __init__(self, unit, figure_size, color_theme, font_family, save_image, num_data):
         self.unit = unit
-        self.temperature = temperature
         self.figure_size = figure_size
         self.color_theme = color_theme
         self.font_family = font_family
         self.save_image = save_image
         self.num_Data = num_data
 
     def __str__(self):
-        return f"KDData(unit={self.unit}, temperature={self.temperature}, figure_size={self.figure_size}, color_theme={self.color_theme}, font_family={self.font_family}, save_image={self.save_image}, num_data={self.num_Data})"
+        return f"KDData(unit={self.unit}, figure_size={self.figure_size}, color_theme={self.color_theme}, font_family={self.font_family}, save_image={self.save_image}, num_data={self.num_Data})"
 
     def get_num_x(self):
         """
         Returns the number of x-axis values
         """
         x = []
         for item in self.num_Data:
```

### Comparing `kimariDraw-1.1.2/kimariDraw/Parser/kd_file.py` & `kimariDraw-1.1.3/kimariDraw/Parser/kd_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,15 @@
         return f"Header: {self.header}\nData: {self.data}"
 
     def get_kd_data(self):
         """
         返回 KDDate 对象的数据列表
         """
         unit = self.header["unit"]
-        temperature = self.header["temperature"]
         figure_size = self.header["figure_size"]
         color_theme = self.header["color_theme"]
         font_family = self.header["font_family"]
         save_image = self.header["save_image"]
         num_data = self.data
 
-        kd_data = KDData(unit, temperature, figure_size, color_theme, font_family, save_image, num_data)
+        kd_data = KDData(unit, figure_size, color_theme, font_family, save_image, num_data)
         return kd_data
```

### Comparing `kimariDraw-1.1.2/kimariDraw/Parser/kd_parser.py` & `kimariDraw-1.1.3/kimariDraw/Parser/kd_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,27 +48,26 @@
         """
         解析文件，返回头部字典和数据列表
         """
         if not self._validate():
             raise ValueError('Invalid KD file format')
 
         header = {'unit': None,
-                  'temperature': None,
                   'figure_size': None,
                   'color_theme': None,
                   'font_family': None,
                   'save_image': None}
 
         data = []
 
         with open(self.filepath, 'r', encoding="utf-8") as f:
             lines = f.readlines()
 
         # 解析文件头
-        for line in lines[:6]:
+        for line in lines[:5]:
             key, value = line[2:].strip().split(' = ')
             if key == 'FIGURE_SIZE':
                 width, height = map(int, value.split(','))
                 header[key.lower()] = (width, height)
             else:
                 header[key.lower()] = value
 
@@ -81,7 +80,8 @@
                 x_str, y_str = line.strip().split(',')
                 x, y = float(x_str), float(y_str)
                 data.append((x, y))
             elif line.strip() == 'BEGIN':
                 data_started = True
 
         return header, data
+
```

### Comparing `kimariDraw-1.1.2/kimariDraw/Plot/kd_plot.py` & `kimariDraw-1.1.3/kimariDraw/Plot/kd_plot.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.2/kimariDraw/main.py` & `kimariDraw-1.1.3/kimariDraw/main.py`

 * *Files identical despite different names*

### Comparing `kimariDraw-1.1.2/setup.py` & `kimariDraw-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='kimariDraw',
-    version='1.1.2',
+    version='1.1.3',
     description='The application is used to draw the Energy Profile Map',
     author='kimariyb',
     author_email='kimariyb@163.com',
     url='https://github.com/kimariyb/kimariDraw',
     install_requires=[
         'numpy',
         'matplotlib',
```

