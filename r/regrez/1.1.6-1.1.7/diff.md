# Comparing `tmp/regrez-1.1.6.tar.gz` & `tmp/regrez-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-1.1.6.tar", last modified: Thu Jun 29 12:38:48 2023, max compression
+gzip compressed data, was "regrez-1.1.7.tar", last modified: Thu Jun 29 12:43:10 2023, max compression
```

## Comparing `regrez-1.1.6.tar` & `regrez-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.236747 regrez-1.1.6/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:38:48.226174 regrez-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-06-27 18:39:50.000000 regrez-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.124079 regrez-1.1.6/regrez/
--rw-rw-rw-   0        0        0       23 2023-06-29 12:37:40.000000 regrez-1.1.6/regrez/__init__.py
--rw-rw-rw-   0        0        0     2639 2023-06-27 12:04:53.000000 regrez-1.1.6/regrez/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.214965 regrez-1.1.6/regrez.egg-info/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 12:38:48.237756 regrez-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 12:38:30.000000 regrez-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:43:10.774982 regrez-1.1.7/
+-rw-rw-rw-   0        0        0     1478 2023-06-29 12:43:10.771179 regrez-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-06-29 12:42:33.000000 regrez-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 12:43:10.683781 regrez-1.1.7/regrez/
+-rw-rw-rw-   0        0        0       28 2023-06-29 12:41:43.000000 regrez-1.1.7/regrez/__init__.py
+-rw-rw-rw-   0        0        0     2640 2023-06-29 12:41:58.000000 regrez-1.1.7/regrez/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:43:10.759777 regrez-1.1.7/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1478 2023-06-29 12:43:10.000000 regrez-1.1.7/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-29 12:43:10.000000 regrez-1.1.7/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:43:10.000000 regrez-1.1.7/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 12:43:10.000000 regrez-1.1.7/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 12:43:10.000000 regrez-1.1.7/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:43:10.776930 regrez-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-29 12:42:48.000000 regrez-1.1.7/setup.py
```

### Comparing `regrez-1.1.6/PKG-INFO` & `regrez-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.1.6
+Version: 1.1.7
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
 
 ```
-from regrez import Model
+from regrez import Models
 
-m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
+m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
 ```
 
 After that, you can train your model using `m.Train()` and test using `m.Test(list_that_will_be_used_for_testing)`. Alternatively, there is a function called `m.TrainAndTest()` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use `m.Visualize()` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.1.6/README.md` & `regrez-1.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
 
 ```
-from regrez import Model
+from regrez import Models
 
-m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
+m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
 ```
 
 After that, you can train your model using `m.Train()` and test using `m.Test(list_that_will_be_used_for_testing)`. Alternatively, there is a function called `m.TrainAndTest()` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use `m.Visualize()` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.1.6/regrez/main.py` & `regrez-1.1.7/regrez/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import numpy as np
 from sklearn import linear_model
 from sklearn.metrics import r2_score
 class ModelNotTrainedException(Exception):
     "You tried to test the model before training it."
     pass
-class Model:
+class Simple:
     def __init__(self, csv_path, label_x, label_y):
         self.csv = csv_path
         self.x_label = label_x
         self.y_label = label_y
         self.file = pd.read_csv(self.csv)
         self.data = self.file[[self.x_label, self.y_label]]
         self.coef = 0
```

### Comparing `regrez-1.1.6/regrez.egg-info/PKG-INFO` & `regrez-1.1.7/regrez.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.1.6
+Version: 1.1.7
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
@@ -15,14 +15,14 @@
 Description-Content-Type: text/markdown
 
 This is a simple Python package that aims to make using linear regression easier for programmers. For now, it only provides a simple linear regresion calculation that is based on one independent variable.
 
 You can create a linear regression model as following:
 
 ```
-from regrez import Model
+from regrez import Models
 
-m = Model("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
+m = Models.Simple("path/to/csv", "label for column that'll be used for x axis", "label for column that'll be used for y axis")
 ```
 
 After that, you can train your model using `m.Train()` and test using `m.Test(list_that_will_be_used_for_testing)`. Alternatively, there is a function called `m.TrainAndTest()` you can use if you only want to see how accurate would the model work. It separates 20% of the data for testing, trains the model with the rest of it, tests the model with separated data and shows how accurate your model is. You can use `m.Visualize()` after training if you want to see a plot showing both data points and the line to see how relative your variables are.
```

### Comparing `regrez-1.1.6/setup.py` & `regrez-1.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.6' 
+VERSION = '1.1.7' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
```

