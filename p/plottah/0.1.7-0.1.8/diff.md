# Comparing `tmp/plottah-0.1.7.tar.gz` & `tmp/plottah-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.7.tar", max compression
+gzip compressed data, was "plottah-0.1.8.tar", max compression
```

## Comparing `plottah-0.1.7.tar` & `plottah-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1081 2023-06-29 10:06:25.944332 plottah-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/__init__.py
--rw-r--r--   0        0        0     2648 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/colors.py
--rw-r--r--   0        0        0     4841 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/config.py
--rw-r--r--   0        0        0       24 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     3821 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7563 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0    10631 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     3030 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-29 10:06:27.580359 plottah-0.1.7/plottah/utils.py
--rw-r--r--   0        0        0      529 2023-06-29 10:06:56.908714 plottah-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2015 1970-01-01 00:00:00.000000 plottah-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-06-29 11:03:06.506744 plottah-0.1.8/README.md
+-rw-r--r--   0        0        0       22 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/colors.py
+-rw-r--r--   0        0        0     4841 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/config.py
+-rw-r--r--   0        0        0       24 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     3821 2023-06-29 11:03:07.710757 plottah-0.1.8/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7563 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0    10631 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     3030 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-29 11:03:07.714757 plottah-0.1.8/plottah/utils.py
+-rw-r--r--   0        0        0      529 2023-06-29 11:03:46.395293 plottah-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 plottah-0.1.8/PKG-INFO
```

### Comparing `plottah-0.1.7/README.md` & `plottah-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 ### Development environment
 
 Clone the repo, give name plotting_analyis
 ```shell
 git clone git@github.com:nielsota/plottah.git plotting_analysis
 ```
+
+CD into the directory
 ```shell
 cd plotting_analysis
 ```
 
 Create a virtual environment by running:
 
 ```shell
@@ -49,9 +51,9 @@
 ```
 
 Next, update the config.yaml how you see fit, and then to generate the images run:
 ```shell
 python -m plottah
 ```
 
-See notebooks for examples on how to run code inline
+See notebooks for examples on how to run code inline during development
```

### Comparing `plottah-0.1.7/plottah/__main__.py` & `plottah-0.1.8/plottah/__main__.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/colors.py` & `plottah-0.1.8/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/config.py` & `plottah-0.1.8/plottah/config.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plot_builder/builders.py` & `plottah-0.1.8/plottah/plot_builder/builders.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.8/plottah/plot_handler/PlotHandler.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.8/plottah/plots/BinEventRatePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plots/DistPlot.py` & `plottah-0.1.8/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plots/PlotProtocol.py` & `plottah-0.1.8/plottah/plots/PlotProtocol.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/plots/RocCurvePlot.py` & `plottah-0.1.8/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/plottah/utils.py` & `plottah-0.1.8/plottah/utils.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.7/pyproject.toml` & `plottah-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plottah"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Niels Ota"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pre-commit = "^3.3.3"
```

### Comparing `plottah-0.1.7/PKG-INFO` & `plottah-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottah
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Niels Ota
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,14 +35,16 @@
 
 ### Development environment
 
 Clone the repo, give name plotting_analyis
 ```shell
 git clone git@github.com:nielsota/plottah.git plotting_analysis
 ```
+
+CD into the directory
 ```shell
 cd plotting_analysis
 ```
 
 Create a virtual environment by running:
 
 ```shell
@@ -75,10 +77,10 @@
 ```
 
 Next, update the config.yaml how you see fit, and then to generate the images run:
 ```shell
 python -m plottah
 ```
 
-See notebooks for examples on how to run code inline
+See notebooks for examples on how to run code inline during development
```

