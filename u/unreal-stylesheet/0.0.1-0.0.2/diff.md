# Comparing `tmp/unreal-stylesheet-0.0.1.tar.gz` & `tmp/unreal-stylesheet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unreal-stylesheet-0.0.1.tar", last modified: Thu Jun 29 09:44:37 2023, max compression
+gzip compressed data, was "unreal-stylesheet-0.0.2.tar", last modified: Thu Jun 29 13:09:52 2023, max compression
```

## Comparing `unreal-stylesheet-0.0.1.tar` & `unreal-stylesheet-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.778216 unreal-stylesheet-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.774216 unreal-stylesheet-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.774216 unreal-stylesheet-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-29 09:44:37.778216 unreal-stylesheet-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:44:37.778216 unreal-stylesheet-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.774216 unreal-stylesheet-0.0.1/unreal_stylesheet/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.778216 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/arrow-down-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/arrow-up-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/cross-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/progress-pattern.svg
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/radio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/triangle-down-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/triangle-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/triangle-right-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/triangle-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/uncheck.svg
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons/unradio.svg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons.qrc
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/icons.rcc
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ue.qss
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ue.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.778216 unreal-stylesheet-0.0.1/unreal_stylesheet/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ui/editor.ui
--rw-r--r--   0 runner    (1001) docker     (123)    38505 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ui/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ui/progress.ui
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-06-29 09:44:14.000000 unreal-stylesheet-0.0.1/unreal_stylesheet/ui/tree.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:44:37.774216 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-29 09:44:37.000000 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-29 09:44:37.000000 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:44:37.000000 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 09:44:37.000000 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 09:44:37.000000 unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.636468 unreal-stylesheet-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.628468 unreal-stylesheet-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.632468 unreal-stylesheet-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-29 13:09:52.636468 unreal-stylesheet-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:09:52.636468 unreal-stylesheet-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.632468 unreal-stylesheet-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.632468 unreal-stylesheet-0.0.2/tests/sample_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/sample_ui/editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    38505 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/sample_ui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/sample_ui/progress.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/sample_ui/tree.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/tests/test_qt_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.632468 unreal-stylesheet-0.0.2/unreal_stylesheet/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.636468 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/arrow-down-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/arrow-up-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/cross-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/progress-pattern.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/radio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/triangle-down-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/triangle-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/triangle-right-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/triangle-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/uncheck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons/unradio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/icons.rcc
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/ue.qss
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-06-29 13:09:38.000000 unreal-stylesheet-0.0.2/unreal_stylesheet/ue.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:09:52.636468 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-29 13:09:52.000000 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-29 13:09:52.000000 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:09:52.000000 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 13:09:52.000000 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 13:09:52.000000 unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/top_level.txt
```

### Comparing `unreal-stylesheet-0.0.1/.github/workflows/python-publish.yml` & `unreal-stylesheet-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/LICENSE` & `unreal-stylesheet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/PKG-INFO` & `unreal-stylesheet-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unreal-stylesheet
-Version: 0.0.1
+Version: 0.0.2
 Summary: style qt like unreal 5
 Author: Xingyu Lei, Hannes Delbeke
 License: MIT License
         
         Copyright (c) 2022 Xingyu Lei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,23 +21,23 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/hannesdelbeke/unrealStylesheet
-Project-URL: Source, https://github.com/hannesdelbeke/unrealStylesheet
-Keywords: qt,unreal,unrealengine,engine,pyside,pyside2,pyside6,PyQt5,PyQt6,stylesheet,dark,night,theme,darkmode
+Project-URL: Homepage, https://github.com/leixingyu/unrealStylesheet
+Project-URL: Source, https://github.com/leixingyu/unrealStylesheet
+Keywords: qt,unreal,unrealengine,engine,pyside,pyside2,pyside6,PyQt5,PyQt6,stylesheet,dark,night,theme,darkmode,ui
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Unreal Stylesheet ![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)
+# Unreal Stylesheet [![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)](https://pypi.org/project/unreal-stylesheet/)
 
  A Qt stylesheet designed to make your tools look native in Unreal Engine 5  
 
 <img src="https://i.imgur.com/y7UP7k3.jpg" alt="main" width="100%"/>  
 
 ## Installation
 PIP install the [latest release](https://pypi.org/project/unreal-stylesheet/) from PYPi (recommended):
```

### Comparing `unreal-stylesheet-0.0.1/README.md` & `unreal-stylesheet-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Unreal Stylesheet ![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)
+# Unreal Stylesheet [![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)](https://pypi.org/project/unreal-stylesheet/)
 
  A Qt stylesheet designed to make your tools look native in Unreal Engine 5  
 
 <img src="https://i.imgur.com/y7UP7k3.jpg" alt="main" width="100%"/>  
 
 ## Installation
 PIP install the [latest release](https://pypi.org/project/unreal-stylesheet/) from PYPi (recommended):
```

### Comparing `unreal-stylesheet-0.0.1/pyproject.toml` & `unreal-stylesheet-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 authors = [
     {name = "Xingyu Lei"},
     {name = "Hannes Delbeke"},
 ]
 description = "style qt like unreal 5"
 readme = "README.md"
 requires-python = ">=3.4"
-keywords = ["qt", "unreal", "unrealengine", "engine", "pyside", "pyside2", "pyside6", "PyQt5", "PyQt6", "stylesheet", "dark", "night", "theme", "darkmode"]
+keywords = ["qt", "unreal", "unrealengine", "engine", "pyside", "pyside2", "pyside6", "PyQt5", "PyQt6", "stylesheet", "dark", "night", "theme", "darkmode", "ui"]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"']
 #dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
 
 [project.urls]
-Homepage = "https://github.com/hannesdelbeke/unrealStylesheet"
-Source = "https://github.com/hannesdelbeke/unrealStylesheet"
+Homepage = "https://github.com/leixingyu/unrealStylesheet"
+Source = "https://github.com/leixingyu/unrealStylesheet"
```

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons/check.svg` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons/check.svg`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons/cross-white.svg` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons/cross-white.svg`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons/cross.svg` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons/progress-pattern.svg` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons/progress-pattern.svg`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons.qrc` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons.qrc`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/icons.rcc` & `unreal-stylesheet-0.0.2/unreal_stylesheet/icons.rcc`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ue.qss` & `unreal-stylesheet-0.0.2/unreal_stylesheet/ue.qss`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ue.scss` & `unreal-stylesheet-0.0.2/unreal_stylesheet/ue.scss`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ui/editor.ui` & `unreal-stylesheet-0.0.2/tests/sample_ui/editor.ui`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ui/main.ui` & `unreal-stylesheet-0.0.2/tests/sample_ui/main.ui`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ui/progress.ui` & `unreal-stylesheet-0.0.2/tests/sample_ui/progress.ui`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet/ui/tree.ui` & `unreal-stylesheet-0.0.2/tests/sample_ui/tree.ui`

 * *Files identical despite different names*

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/PKG-INFO` & `unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unreal-stylesheet
-Version: 0.0.1
+Version: 0.0.2
 Summary: style qt like unreal 5
 Author: Xingyu Lei, Hannes Delbeke
 License: MIT License
         
         Copyright (c) 2022 Xingyu Lei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,23 +21,23 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/hannesdelbeke/unrealStylesheet
-Project-URL: Source, https://github.com/hannesdelbeke/unrealStylesheet
-Keywords: qt,unreal,unrealengine,engine,pyside,pyside2,pyside6,PyQt5,PyQt6,stylesheet,dark,night,theme,darkmode
+Project-URL: Homepage, https://github.com/leixingyu/unrealStylesheet
+Project-URL: Source, https://github.com/leixingyu/unrealStylesheet
+Keywords: qt,unreal,unrealengine,engine,pyside,pyside2,pyside6,PyQt5,PyQt6,stylesheet,dark,night,theme,darkmode,ui
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Unreal Stylesheet ![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)
+# Unreal Stylesheet [![PyPI](https://img.shields.io/pypi/v/unreal_stylesheet?color=blue)](https://pypi.org/project/unreal-stylesheet/)
 
  A Qt stylesheet designed to make your tools look native in Unreal Engine 5  
 
 <img src="https://i.imgur.com/y7UP7k3.jpg" alt="main" width="100%"/>  
 
 ## Installation
 PIP install the [latest release](https://pypi.org/project/unreal-stylesheet/) from PYPi (recommended):
```

### Comparing `unreal-stylesheet-0.0.1/unreal_stylesheet.egg-info/SOURCES.txt` & `unreal-stylesheet-0.0.2/unreal_stylesheet.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/python-publish.yml
+tests/requirements.txt
+tests/test_qt_wrappers.py
+tests/sample_ui/editor.ui
+tests/sample_ui/main.ui
+tests/sample_ui/progress.ui
+tests/sample_ui/tree.ui
 unreal_stylesheet/__init__.py
 unreal_stylesheet/icons.qrc
 unreal_stylesheet/icons.rcc
 unreal_stylesheet/main.py
 unreal_stylesheet/ue.qss
 unreal_stylesheet/ue.scss
 unreal_stylesheet.egg-info/PKG-INFO
@@ -23,12 +30,8 @@
 unreal_stylesheet/icons/progress-pattern.svg
 unreal_stylesheet/icons/radio.svg
 unreal_stylesheet/icons/triangle-down-white.svg
 unreal_stylesheet/icons/triangle-down.svg
 unreal_stylesheet/icons/triangle-right-white.svg
 unreal_stylesheet/icons/triangle-right.svg
 unreal_stylesheet/icons/uncheck.svg
-unreal_stylesheet/icons/unradio.svg
-unreal_stylesheet/ui/editor.ui
-unreal_stylesheet/ui/main.ui
-unreal_stylesheet/ui/progress.ui
-unreal_stylesheet/ui/tree.ui
+unreal_stylesheet/icons/unradio.svg
```

