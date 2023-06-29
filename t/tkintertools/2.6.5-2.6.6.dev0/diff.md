# Comparing `tmp/tkintertools-2.6.5.tar.gz` & `tmp/tkintertools-2.6.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.5.tar", last modified: Fri Jun 16 17:36:10 2023, max compression
+gzip compressed data, was "tkintertools-2.6.6.dev0.tar", last modified: Thu Jun 29 09:43:34 2023, max compression
```

## Comparing `tkintertools-2.6.5.tar` & `tkintertools-2.6.6.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.472603 tkintertools-2.6.5/
--rw-rw-rw-   0        0        0     9257 2023-06-12 07:55:24.000000 tkintertools-2.6.5/LICENSE.txt
--rw-rw-rw-   0        0        0    28817 2023-06-16 17:36:10.470597 tkintertools-2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0    28252 2023-06-16 17:34:58.000000 tkintertools-2.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 17:36:10.472603 tkintertools-2.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-06-16 17:04:04.000000 tkintertools-2.6.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.460519 tkintertools-2.6.5/tkintertools/
--rw-rw-rw-   0        0        0     2859 2023-06-16 17:07:18.000000 tkintertools-2.6.5/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    62351 2023-06-16 16:33:00.000000 tkintertools-2.6.5/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.5/tkintertools/constants.py
--rw-rw-rw-   0        0        0    21400 2023-06-16 17:26:13.000000 tkintertools-2.6.5/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.467935 tkintertools-2.6.5/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    28817 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/
+-rw-rw-rw-   0        0        0     9267 2023-06-20 19:03:57.000000 tkintertools-2.6.6.dev0/LICENSE.txt
+-rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:34.022947 tkintertools-2.6.6.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     8428 2023-06-29 09:04:12.000000 tkintertools-2.6.6.dev0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:43:34.023952 tkintertools-2.6.6.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-06-29 06:36:36.000000 tkintertools-2.6.6.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.010671 tkintertools-2.6.6.dev0/tkintertools/
+-rw-rw-rw-   0        0        0     2863 2023-06-29 07:57:18.000000 tkintertools-2.6.6.dev0/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62351 2023-06-28 20:32:13.000000 tkintertools-2.6.6.dev0/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.6.dev0/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    21734 2023-06-29 07:51:40.000000 tkintertools-2.6.6.dev0/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:34.020749 tkintertools-2.6.6.dev0/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9062 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 09:43:33.000000 tkintertools-2.6.6.dev0/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.5/LICENSE.txt` & `tkintertools-2.6.6.dev0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
    1， 请您补充如下声明中的空白，包括软件名、软件的首次发表年份以及您作为版权人的名字；
 
    2， 请您在软件包的一级目录下创建以"LICENSE"为名的文件，将整个许可证文本放入该文件中；
 
    3， 请将如下声明文本放入每个源文件的头部注释中。
 
-Copyright (c) 2022 小康2022
+Copyright (c) 2022-2023 小康2022
 
 tkintertools is licensed under Mulan PSL v2.
 
 You can use this software according to the terms and conditions of the Mulan PSL v2.
 
 You may obtain a copy of Mulan PSL v2 at:
 
@@ -122,15 +122,15 @@
 
    i. Fill in the blanks in following statement, including insert your software name, the year of the first publication of your software, and your name identified as the copyright owner;
 
    ii. Create a file named "LICENSE" which contains the whole context of this License in the first directory of your software package;
 
    iii. Attach the statement to the appropriate annotated syntax at the beginning of each source file.
 
-Copyright (c) 2022 Xiaokang2022
+Copyright (c) 2022-2023 Xiaokang2022
 
 tkintertools is licensed under Mulan PSL v2.
 
 You can use this software according to the terms and conditions of the Mulan PSL v2.
 
 You may obtain a copy of Mulan PSL v2 at:
```

### Comparing `tkintertools-2.6.5/setup.py` & `tkintertools-2.6.6.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-""" 上传 pypi """
+""" 上传 PyPi """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version='2.6.5',
+    version='2.6.6.dev',
+    description='An auxiliary module of the tkinter module.',
+    long_description=open('README.md', encoding='utf-8').read(),
     author='Xiaokang2022',
-    license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
-    description='An auxiliary module of the tkinter module',
-    long_description=open('README.md', encoding='utf-8').read(),
-    long_description_content_type='text/markdown',
+    maintainer='Xiaokang2022',
+    maintainer_email='2951256653@qq.com',
     url='https://github.com/Xiaokang2022/tkintertools',
     packages=setuptools.find_packages(),
+    license='MulanPSL-2.0',
+    keywords=['tkinter', 'tkintertools', 'GUI'],
+    long_description_content_type='text/markdown',
     python_requires='>=3.8',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
-    keywords=['tkinter', 'tkintertools', 'GUI'],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
 
 # python setup.py sdist bdist_wheel [打包]
 # python -m twine upload dist/* [上传]
```

### Comparing `tkintertools-2.6.5/tkintertools/__init__.py` & `tkintertools-2.6.6.dev0/tkintertools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.5'
+__version__ = '2.6.6.dev'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
```

### Comparing `tkintertools-2.6.5/tkintertools/__main__.py` & `tkintertools-2.6.6.dev0/tkintertools/__main__.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.5/tkintertools/constants.py` & `tkintertools-2.6.6.dev0/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.5/tkintertools/tools_3d.py` & `tkintertools-2.6.6.dev0/tkintertools/tools_3d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """ 3D support """
 
 import math  # 数学支持
 import statistics  # 数据统计
+from abc import ABCMeta, abstractmethod  # 抽象类
 from tkinter import Event  # 类型提示
 from typing import Iterable  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
 from .constants import *
 
 
 def translate(coords, dx=0, dy=0, dz=0):
     # type: (list[float], float, float, float) -> None
     """
     ### 平移
     将一个空间三维中的点进行平移\n
     ---
     `coords`: 被平移点的空间坐标列表\n
-    `dx`: x方向位移\n
-    `dy`: y方向位移\n
-    `dz`: z方向位移\n
+    `dx`: x 方向位移\n
+    `dy`: y 方向位移\n
+    `dz`: z 方向位移\n
     """
     coords[0] += dx
     coords[1] += dy
     coords[2] += dz
 
 
 def rotate(coords, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
     # type: (list[float], float, float, float, ..., Iterable[float]) -> None
     """
     ### 旋转
     将一个空间三维中的点以另一个点为旋转中心进行旋转\n
     ---
     `coords`: 被旋转点的空间坐标列表\n
-    `dx`: x方向旋转弧度\n
-    `dy`: y方向旋转弧度\n
-    `dz`: z方向旋转弧度\n
+    `dx`: x 方向旋转弧度\n
+    `dy`: y 方向旋转弧度\n
+    `dz`: z 方向旋转弧度\n
     `center`: 旋转中心的空间坐标列表\n
     """
     sx, sy, sz = math.sin(dx), math.sin(dy), math.sin(dz)
     cx, cy, cz = math.cos(dx), math.cos(dy), math.cos(dz)
 
     matrix = [[cz*cy, cz*sy*sx-sz*cx, cz*sy*cx+sz*sx],
               [sz*cy, sz*sy*sx+cz*cx, sz*sy*cx-cz*sx],
@@ -54,17 +55,17 @@
 def scale(coords, kx=1, ky=1, kz=1, *, center=None):
     # type: (list[float], float, float, float, ..., Iterable[float] | None) -> None
     """
     ### 缩放
     将一个空间三维中的点以另一个点为缩放中心进行位置缩放\n
     ---
     `coords`: 被缩放点的空间坐标列表\n
-    `dx`: x方向缩放比例\n
-    `dy`: y方向缩放比例\n
-    `dz`: z方向缩放比例\n
+    `dx`: x 方向缩放比例\n
+    `dy`: y 方向缩放比例\n
+    `dz`: z 方向缩放比例\n
     `center`: 缩放中心的空间坐标列表\n
     """
     for i, k in zip(range(3), (kx, ky, kz)):
         coords[i] += (coords[i] - center[i]) * (k - 1)
 
 
 class Canvas_3D(Canvas):
@@ -78,51 +79,55 @@
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=True,  # type: bool
         camera_distance=CAMERA_DISTANCE,  # type: float
-        dx=None,  # type: float | None
-        dy=None,  # type: float | None
         **kw
     ):  # type: (...) -> None
         """
         `master`: 父控件\n
         `width`: 画布宽度\n
         `height`: 画布高度\n
         `x`: 画布左上角的横坐标\n
         `y`: 画布左上角的纵坐标\n
         `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
         `expand`: 画布内控件是否能缩放\n
         `keep`: 画布比例是否保持不变\n
-        `camera_distance`: 3d绘图时相机与原点的距离，默认值为1000\n
-        `dx`: 画面在横坐标方向的偏移，None表示居中\n
-        `dy`: 画面在纵坐标方向的偏移，None表示居中\n
+        `camera_distance`: 3D 绘图时相机与原点的距离，默认值为 1000\n
         `**kw`: 与 tkinter.Canvas 类的参数相同\n
         """
         Canvas.__init__(self, master, width, height, x, y,
                         lock=lock, expand=expand, keep=keep, **kw)
         self.distance = camera_distance
-        self.dx = width / 2 if dx is None else dx
-        self.dy = height / 2 if dy is None else dy
         self._items_3d = []  # type: list[Point | Line | Side]
         self._geos = []  # type: list[Geometry]
+        self.configure(  # 使画布视野居中
+            scrollregion=(-self.width[1]/2, -self.height[1]/2, self.width[1]/2, self.height[1]/2))
+
+    def zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
+        # override: 保持画布视野居中
+        Canvas.zoom(self, rate_x, rate_y)
+        half_width, half_height = self.width[1]/2, self.height[1]/2
+        self.configure(scrollregion=(-half_width, -
+                       half_height, half_width, half_height))
 
     def items_3d(self):  # type: () -> tuple[Point | Line | Side]
-        """ 返回`Canvas_3d`类的`items_3d`元组 """
+        """ 返回 `Canvas_3d` 类的 `items_3d` 元组 """
         return tuple(self._items_3d)
 
     def geos(self):  # type: () -> tuple[Geometry]
-        """ 返回`Canvas_3d`类的`geos`元组 """
+        """ 返回 `Canvas_3d` 类的 `geos` 元组 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
         """ 空间位置排序 """
-        self._items_3d.sort(key=lambda item: item.camera_distance())
+        self._items_3d.sort(key=lambda item: (
+            not isinstance(item, Point), item.camera_distance()))
         for item in self._items_3d:
             self.lower(item.item)
 
 
 class Space(Canvas_3D):
     """ 三维空间 """
 
@@ -134,23 +139,41 @@
         x=None,  # type: int | None
         y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=True,  # type: bool
         camera_distance=CAMERA_DISTANCE,  # type: float
-        dx=None,  # type: float | None
-        dy=None,  # type: float | None
-        origin_color='',  # type: str
+        origin_size=POINT_SIZE,  # type: float
+        origin_width=POINT_WIDTH,  # type: float
+        origin_fill='',  # type: str
+        origin_outline='',  # type: str
         **kw
     ):  # type: (...) -> None
+        """
+        `master`: 父控件\n
+        `width`: 画布宽度\n
+        `height`: 画布高度\n
+        `x`: 画布左上角的横坐标\n
+        `y`: 画布左上角的纵坐标\n
+        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
+        `expand`: 画布内控件是否能缩放\n
+        `keep`: 画布比例是否保持不变\n
+        `camera_distance`: 3D 绘图时相机与原点的距离，默认值为 1000\n
+        `origin_size`: 原点大小\n
+        `origin_width`: 原点轮廓宽度\n
+        `origin_fill`: 原点内部填充颜色\n
+        `origin_outline`: 原点轮廓颜色\n
+        `**kw`: 与 `tkinter.Canvas` 类的参数相同\n
+        """
         Canvas_3D.__init__(self, master, width, height, x, y, lock=lock, expand=expand,
-                           keep=keep, camera_distance=camera_distance, dx=dx, dy=dy, **kw)
-        self._origin = Point(self, [0, 0, 0], size=1,
-                             fill=origin_color, outline=origin_color)
+                           keep=keep, camera_distance=camera_distance, **kw)
+        self._origin = Point(self, [0, 0, 0], size=origin_size, width=origin_width,
+                             fill=origin_fill, outline=origin_outline)
+        self._items_3d.clear()
         self.space_sort()
         self.bind('<B3-Motion>', self._translate)
         self.bind('<Button-3>', lambda _: self._translate(_, True))
         self.bind('<ButtonRelease-3>', lambda _: self._translate(_, False))
         self.bind('<B1-Motion>', self._rotate)
         self.bind('<Button-1>', lambda _: self._rotate(_, True))
         self.bind('<ButtonRelease-1>', lambda _: self._rotate(_, False))
@@ -166,354 +189,341 @@
         if flag is True:  # 按下
             cache[:] = [event.x, event.y]
             return self.configure(cursor='fleur')
         elif flag is False:  # 松开
             return self.configure(cursor='arrow')
         dx, dy = event.x-cache[0], event.y-cache[1]
         cache[:] = [event.x, event.y]
-        for item in self._geos+[self._origin]:
-            item.translate(0, dx, dy)
+        for item in self._items_3d+[self._origin]:
+            item.translate(
+                0, dx*self.width[0]/self.width[1], dy*self.height[0]/self.height[1])
             item.update()
         self.space_sort()
 
     def _rotate(self, event, flag=None, cache=[]):
         # type: (Event, bool | None, list[float]) -> None
         """ 旋转视角 """
         if flag is True:
             cache[:] = [event.x, event.y]
             return self.configure(cursor='fleur')
         elif flag is False:
             return self.configure(cursor='arrow')
         dx, dy = event.x-cache[0], event.y-cache[1]
         cache[:] = [event.x, event.y]
-        for item in self._geos+[self._origin]:
-            item.rotate(0, -dy/self.dx*math.pi, dx /
-                        self.dy*math.pi, center=self._origin.coords)
+        for item in self._items_3d:
+            item.rotate(0, -2*dy/self.width[1]*math.tau, 2*dx /
+                        self.height[1]*math.tau, center=self._origin.coords)
             item.update()
         self.space_sort()
 
     def _zoom(self, event, flag=None):  # type: (Event, bool | None) -> None
         """ 缩放视角 """
         if flag is not None:
             event.delta = flag
         k = 1.1 if event.delta > 0 else 0.9
-        for item in self.geos():
+        for item in self._items_3d:
             item.scale(k, k, k, center=self._origin.coords)
             item.update()
         self.space_sort()
 
 
-class _Point:
+class _3D_Object(metaclass=ABCMeta):
+    """ 3D 对象抽象元类 """
+
+    @abstractmethod
+    def translate(self, dx=0, dy=0, dz=0):
+        """
+        平移\n
+        `dx`: x 轴方向位移距离\n
+        `dy`: y 轴方向位移距离\n
+        `dz`: z 轴方向位移距离\n
+        """
+
+    @abstractmethod
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+        """
+        旋转\n
+        `dx`: 绕x 轴方向旋转弧度\n
+        `dy`: 绕y 轴方向旋转弧度\n
+        `dz`: 绕z 轴方向旋转弧度\n
+        `center`: 旋转中心\n
+        """
+
+    @abstractmethod
+    def scale(self, kx=1, ky=1, kz=1, *, center=None):
+        """
+        缩放\n
+        `kx`: x 轴方向缩放比例\n
+        `ky`: y 轴方向缩放比例\n
+        `kz`: z 轴方向缩放比例\n
+        `center`: 缩放中心，默认为几何中心\n
+        """
+
+    @abstractmethod
+    def project(self, distance):
+        """
+        投影\n
+        `distance`: 对象与观察者的距离\n
+        """
+
+
+class _Point(_3D_Object):
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """ 平移 """
         translate(self.coords, dx, dy, dz)
 
     def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
-        """ 旋转 """
         rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """ 缩放 """
         scale(self.coords, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[float]
-        """ 投影 """
         relative_dis = distance - self.coords[0]
         if relative_dis <= 1e-16:
-            return [float('INF')]*2  # BUG
+            return [float('INF')]*2  # BUG: 目前超出范围只能让其消失
         k = distance/relative_dis
         return [self.coords[1]*k, self.coords[2]*k]
 
 
-class _Line:
+class _Line(_3D_Object):
     """ 线 """
 
     def __init__(
         self,
-        point1,  # type: list[float]
-        point2,  # type: list[float]
+        point_start,  # type: list[float]
+        point_end,  # type: list[float]
     ):  # type: (...) -> None
-        self.coords = [point1, point2]
+        self.coords = [point_start, point_end]
         self.points = [_Point(point) for point in self.coords]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """ 平移 """
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
     def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
-        """ 旋转 """
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """ 缩放 """
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[float]]
-        """ 投影 """
         return [point.project(distance) for point in self.points]
 
 
-class _Side:
+class _Side(_3D_Object):
     """ 面 """
 
     def __init__(self, *points):  # type: (list[float]) -> None
         self.coords = list(points)
         self.lines = [_Line(points[ind-1], points[ind])
                       for ind in range(len(points))]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """ 平移 """
         for coord in self.coords:
             translate(coord, dx, dy, dz)
 
     def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
-        """ 旋转 """
         for coord in self.coords:
             rotate(coord, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """ 缩放 """
         if center is None:
             center = [statistics.mean(axis) for axis in zip(*self.coords)]
         for coord in self.coords:
             scale(coord, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[list[list[float]]]
-        """ 投影 """
         return [line.project(distance) for line in self.lines]
 
 
 class Point(_Point):
     """ 点 """
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D
-        coords,  # type: list[float]
+        canvas,  # type: Canvas_3D | Space
+        coords,  # type: Iterable[float]
         *,
         size=POINT_SIZE,  # type: float
         width=POINT_WIDTH,  # type: float
         fill=COLOR_POINT_FILL,  # type: str
         outline=COLOR_POINT_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `coords`: 点的空间坐标\n
         `size`: 点的大小\n
         `width`: 点轮廓的宽度\n
         `fill`: 点内部的填充颜色\n
         `outline`: 点轮廓的颜色\n
         """
-        _Point.__init__(self, coords)
+        _Point.__init__(self, list(coords))
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.size = size
         self.width = width
         self.fill = fill
         self.item = canvas.create_oval(
             -1, -1, -1, -1, fill=fill, outline=outline, width=width)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
         x, y = self.project(self.canvas.distance)
-        kx, ky = self.canvas.rx, self.canvas.ry
-        x += self.canvas.dx
-        y += self.canvas.dy
-        self.canvas.coords(
-            self.item, (x-self.size)*kx, (y-self.size)*ky, (x+self.size)*kx, (y+self.size)*ky)
+        self.canvas.coords(self.item, (x-self.size)*self.canvas.rx, (y-self.size) *
+                           self.canvas.ry, (x+self.size)*self.canvas.rx, (y+self.size)*self.canvas.ry)
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return math.hypot(self.canvas.distance-self.coords[0], self.coords[1], self.coords[2])
+        return math.dist([self.canvas.distance, 0, 0], self.coords)
 
 
 class Line(_Line):
     """ 线 """
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D
-        point1,  # type: list[float]
-        point2,  # type: list[float]
+        canvas,  # type: Canvas_3D | Space
+        point_start,  # type: Iterable[float]
+        point_end,  # type: Iterable[float]
         *,
         width=LINE_WDITH,  # type: float
         fill=COLOR_LINE_FILL,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
-        `point1`: 起点坐标\n
-        `point2`: 终点坐标\n
+        `point_start`: 起点坐标\n
+        `point_end`: 终点坐标\n
         `width`: 线的宽度\n
         `fill`: 线的颜色\n
         """
-        _Line.__init__(self, point1, point2)
+        _Line.__init__(self, list(point_start), list(point_end))
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
-        kx, ky = self.canvas.rx, self.canvas.ry
-        data = self.project(self.canvas.distance)
-        for point in data:
-            point[0] += self.canvas.dx
-            point[1] += self.canvas.dy
-        self.canvas.coords(
-            self.item, *[coord*(ky if i else kx) for point in data for i, coord in enumerate(point)])
+        self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
+                           for point in self.project(self.canvas.distance) for i, coord in enumerate(point)])
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return statistics.mean(math.hypot(self.canvas.distance-coord[0], coord[1], coord[2]) for coord in self.coords)
+        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
 
 
 class Side(_Side):
     """ 面 """
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D
-        *points,  # type: list[float]
+        canvas,  # type: Canvas_3D | Space
+        *points,  # type: Iterable[float]
         width=SIDE_WIDTH,  # type: float
         fill=COLOR_SIDE_FILL,  # type: str
         outline=COLOR_SIDE_OUTLINE,  # type: str
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
         `points`: 各点的空间坐标\n
         `width`: 面轮廓的宽度\n
         `fill`: 面内部的填充颜色\n
         `outline`: 面轮廓的颜色\n
         """
-        _Side.__init__(self, *points)
+        _Side.__init__(self, *[list(point) for point in points])
         canvas._items_3d.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.outline = outline
         self.item = canvas.create_polygon(
             -1, -1, -1, -1, width=width, fill=fill, outline=outline)
         self.update()
 
     def update(self) -> None:
         """ 更新 """
-        kx, ky = self.canvas.rx, self.canvas.ry
-        data = self.project(self.canvas.distance)
-        for line in data:
-            for point in line:
-                point[0] += self.canvas.dx
-                point[1] += self.canvas.dy
-        self.canvas.coords(
-            self.item, *[coord*(ky if i else kx) for line in data for point in line for i, coord in enumerate(point)])
+        self.canvas.coords(self.item, *[coord*(self.canvas.ry if i else self.canvas.rx)
+                           for line in self.project(self.canvas.distance) for point in line for i, coord in enumerate(point)])
 
     def camera_distance(self):  # type: () -> float
         """ 与相机距离 """
-        return statistics.mean(math.hypot(self.canvas.distance-coord[0], coord[1], coord[2]) for coord in self.coords)
+        return statistics.mean(math.dist([self.canvas.distance, 0, 0], coord) for coord in self.coords)
 
 
 class Geometry:
     """ 几何体 """
 
-    def __init__(self, canvas, *sides):  # type: (Canvas_3D, _Side) -> None
+    def __init__(
+        self,
+        canvas,  # type: Canvas_3D | Space
+        *sides,  # type: Side
+    ):  # type: (...) -> None
         """
         `canvas`: 显示的画布\n
-        `sides`: 平面类`Side`\n
+        `sides`: 组成几何体的面\n
         """
         canvas._geos.append(self)
         self.canvas = canvas
-        self.coords = []  # type: list[list[float]]
-        self.sides = []  # type: list[Side]
-        if sides:
-            self.append(*sides)
+        self.sides = list(sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
-        """
-        平移\n
-        `dx`: x轴方向位移距离\n
-        `dy`: y轴方向位移距离\n
-        `dz`: z轴方向位移距离\n
-        """
-        coords = [coord for side in self.sides for coord in side.coords]
-        for ind, coord in enumerate(coords):
-            if coord not in coords[:ind]:
-                translate(coord, dx, dy, dz)
+        for side in self.sides:
+            side.translate(dx, dy, dz)
 
     def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
-        """
-        旋转\n
-        `dx`: 绕x轴方向旋转弧度\n
-        `dy`: 绕y轴方向旋转弧度\n
-        `dz`: 绕z轴方向旋转弧度\n
-        `center`: 旋转中心\n
-        """
-        coords = [coord for side in self.sides for coord in side.coords]
-        for ind, coord in enumerate(coords):
-            if coord not in coords[:ind]:
-                rotate(coord, dx, dy, dz, center=center)
+        for side in self.sides:
+            side.rotate(dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
-        """
-        缩放\n
-        `kx`: x轴方向缩放比例\n
-        `ky`: y轴方向缩放比例\n
-        `kz`: z轴方向缩放比例\n
-        `center`: 缩放中心，默认为几何中心\n
-        """
-        if center is None:  # NOTE: 对凹面几何体无效
-            center = [statistics.mean(axis) for axis in zip(*self.coords)]
-        coords = [coord for side in self.sides for coord in side.coords]
-        for ind, coord in enumerate(coords):
-            if coord not in coords[:ind]:
-                scale(coord, kx, ky, kz, center=center)
+        if center is None:  # BUG: 公式对凹面几何体不成立
+            center = [statistics.mean(axis) for axis in zip(
+                *set(tuple(coord) for side in self.sides for coord in side.coords))]
+        for side in self.sides:
+            side.scale(kx, ky, kz, center=center)
 
     def update(self):  # type: () -> None
         """ 更新几何体 """
         for side in self.sides:
             side.update()
 
     def append(self, *sides):  # type: (Side) -> None
         """
         添加面\n
         `sides`: `Side`类\n
         """
         for side in sides:
-            for line in side.lines:
-                for point in line.points:
-                    if point not in self.coords:
-                        self.coords.append(point)
             self.sides.append(side)
 
 
 class Cuboid(Geometry):
     """ 长方体 """
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D
+        canvas,  # type: Canvas_3D | Space
         x,  # type: float
         y,  # type: float
         z,  # type: float
         length,  # type: float
         width,  # type: float
         height,  # type: float
         *,
@@ -537,64 +547,59 @@
         `color_left`: 左侧面颜色\n
         `color_right`: 右侧面颜色\n
         `color_front`: 正面颜色\n
         `color_back`: 后面颜色\n
         """
         canvas._geos.append(self)
         self.canvas = canvas
-        self.coords = [[x+l, y+w, z+h]
-                       for l in (0, length)
-                       for w in (0, width)
-                       for h in (0, height)]
+        coords = [[x+l, y+w, z+h]
+                  for l in (0, length)
+                  for w in (0, width)
+                  for h in (0, height)]
         self.sides = [
-            Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[3], self.coords[2], fill=color_back),
-            Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[5], self.coords[4], fill=color_left),
-            Side(canvas, self.coords[0], self.coords[2],
-                 self.coords[6], self.coords[4], fill=color_up),
-            Side(canvas, self.coords[1], self.coords[3],
-                 self.coords[7], self.coords[5], fill=color_down),
-            Side(canvas, self.coords[2], self.coords[3],
-                 self.coords[7], self.coords[6], fill=color_right),
-            Side(canvas, self.coords[4], self.coords[5],
-                 self.coords[7], self.coords[6], fill=color_front),
+            Side(canvas, coords[0], coords[1],
+                 coords[3], coords[2], fill=color_back),
+            Side(canvas, coords[0], coords[1],
+                 coords[5], coords[4], fill=color_left),
+            Side(canvas, coords[0], coords[2],
+                 coords[6], coords[4], fill=color_up),
+            Side(canvas, coords[1], coords[3],
+                 coords[7], coords[5], fill=color_down),
+            Side(canvas, coords[2], coords[3],
+                 coords[7], coords[6], fill=color_right),
+            Side(canvas, coords[4], coords[5],
+                 coords[7], coords[6], fill=color_front),
         ]
 
 
 class Tetrahedron(Geometry):
     """ 四面体 """
 
     def __init__(
         self,
-        canvas,  # type: Canvas_3D
-        p1,  # type: Iterable[float]
-        p2,  # type: Iterable[float]
-        p3,  # type: Iterable[float]
-        p4,  # type: Iterable[float]
+        canvas,  # type: Canvas_3D | Space
+        point_1,  # type: Iterable[float]
+        point_2,  # type: Iterable[float]
+        point_3,  # type: Iterable[float]
+        point_4,  # type: Iterable[float]
         *,
         colors=('',)*4  # type: Iterable[str]
     ):  # type: (...) -> None
         """
         `canvas`: 父画布\n
-        `p1`: 第一个顶点\n
-        `p2`: 第二个顶点\n
-        `p3`: 第三个顶点\n
-        `p4`: 第四个顶点\n
+        `point_1`: 第一个顶点\n
+        `point_2`: 第二个顶点\n
+        `point_3`: 第三个顶点\n
+        `point_4`: 第四个顶点\n
         `colors`: 颜色序列\n
         """
         canvas._geos.append(self)
         self.canvas = canvas
-        self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
-            Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[2], fill=colors[0]),
-            Side(canvas, self.coords[0], self.coords[1],
-                 self.coords[3], fill=colors[1]),
-            Side(canvas, self.coords[0], self.coords[2],
-                 self.coords[3], fill=colors[2]),
-            Side(canvas, self.coords[1], self.coords[2],
-                 self.coords[3], fill=colors[3]),
+            Side(canvas, point_1, point_2, point_3, fill=colors[0]),
+            Side(canvas, point_1, point_2, point_4, fill=colors[1]),
+            Side(canvas, point_1, point_3, point_4, fill=colors[2]),
+            Side(canvas, point_2, point_3, point_4, fill=colors[3]),
         ]
 
 
 __all__ = [name for name in globals() if '__' not in name]
```

