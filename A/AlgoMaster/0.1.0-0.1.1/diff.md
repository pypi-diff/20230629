# Comparing `tmp/AlgoMaster-0.1.0.tar.gz` & `tmp/AlgoMaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoMaster-0.1.0.tar", last modified: Thu Jun 29 13:24:21 2023, max compression
+gzip compressed data, was "AlgoMaster-0.1.1.tar", last modified: Thu Jun 29 13:33:06 2023, max compression
```

## Comparing `AlgoMaster-0.1.0.tar` & `AlgoMaster-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.356380 AlgoMaster-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.307354 AlgoMaster-0.1.0/AlgoMaster/
--rw-rw-rw-   0        0        0       73 2023-06-21 14:23:59.000000 AlgoMaster-0.1.0/AlgoMaster/__init__.py
--rw-rw-rw-   0        0        0    21345 2023-06-29 10:17:12.000000 AlgoMaster-0.1.0/AlgoMaster/classifier.py
--rw-rw-rw-   0        0        0     3230 2023-06-29 06:17:21.000000 AlgoMaster-0.1.0/AlgoMaster/demo.py
--rw-rw-rw-   0        0        0     2493 2023-06-28 17:05:15.000000 AlgoMaster-0.1.0/AlgoMaster/reg.py
--rw-rw-rw-   0        0        0    31651 2023-06-29 11:09:26.000000 AlgoMaster-0.1.0/AlgoMaster/regressor.py
--rw-rw-rw-   0        0        0       36 2023-06-29 05:46:33.000000 AlgoMaster-0.1.0/AlgoMaster/tempCodeRunnerFile.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.351358 AlgoMaster-0.1.0/AlgoMaster.egg-info/
--rw-rw-rw-   0        0        0     5206 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5206 2023-06-29 13:24:21.355359 AlgoMaster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4012 2023-06-29 11:10:52.000000 AlgoMaster-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 13:24:21.357360 AlgoMaster-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2790 2023-06-29 11:11:49.000000 AlgoMaster-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:33:06.060912 AlgoMaster-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-29 13:33:06.029910 AlgoMaster-0.1.1/AlgoMaster/
+-rw-rw-rw-   0        0        0       73 2023-06-21 14:23:59.000000 AlgoMaster-0.1.1/AlgoMaster/__init__.py
+-rw-rw-rw-   0        0        0    21345 2023-06-29 10:17:12.000000 AlgoMaster-0.1.1/AlgoMaster/classifier.py
+-rw-rw-rw-   0        0        0     3230 2023-06-29 06:17:21.000000 AlgoMaster-0.1.1/AlgoMaster/demo.py
+-rw-rw-rw-   0        0        0     2493 2023-06-28 17:05:15.000000 AlgoMaster-0.1.1/AlgoMaster/reg.py
+-rw-rw-rw-   0        0        0    31651 2023-06-29 11:09:26.000000 AlgoMaster-0.1.1/AlgoMaster/regressor.py
+-rw-rw-rw-   0        0        0       36 2023-06-29 05:46:33.000000 AlgoMaster-0.1.1/AlgoMaster/tempCodeRunnerFile.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:33:06.055911 AlgoMaster-0.1.1/AlgoMaster.egg-info/
+-rw-rw-rw-   0        0        0     5343 2023-06-29 13:33:05.000000 AlgoMaster-0.1.1/AlgoMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-29 13:33:05.000000 AlgoMaster-0.1.1/AlgoMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:33:05.000000 AlgoMaster-0.1.1/AlgoMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:33:05.000000 AlgoMaster-0.1.1/AlgoMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 13:33:05.000000 AlgoMaster-0.1.1/AlgoMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5343 2023-06-29 13:33:06.058913 AlgoMaster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4012 2023-06-29 11:10:52.000000 AlgoMaster-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:33:06.060912 AlgoMaster-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2746 2023-06-29 13:32:20.000000 AlgoMaster-0.1.1/setup.py
```

### Comparing `AlgoMaster-0.1.0/AlgoMaster/classifier.py` & `AlgoMaster-0.1.1/AlgoMaster/classifier.py`

 * *Files identical despite different names*

### Comparing `AlgoMaster-0.1.0/AlgoMaster/demo.py` & `AlgoMaster-0.1.1/AlgoMaster/demo.py`

 * *Files identical despite different names*

### Comparing `AlgoMaster-0.1.0/AlgoMaster/reg.py` & `AlgoMaster-0.1.1/AlgoMaster/reg.py`

 * *Files identical despite different names*

### Comparing `AlgoMaster-0.1.0/AlgoMaster/regressor.py` & `AlgoMaster-0.1.1/AlgoMaster/regressor.py`

 * *Files identical despite different names*

### Comparing `AlgoMaster-0.1.0/AlgoMaster.egg-info/PKG-INFO` & `AlgoMaster-0.1.1/AlgoMaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.1.0
-Summary: The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.
+Version: 0.1.1
+Summary: The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.The Classifier class streamlines classification tasks by offering a well-organized framework for model selection, hyperparameter tuning, 
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: machine learning,classifiers,logistic regression,k-nearest neighbors,naive Bayes,random forests,support vector machines,ensemble methods,hyperparameter tuning,performance evaluation,comparison,multiple classifiersadvantages,Regression class,regression analysis, Python,model training,evaluation,hyperparameter tuning,encapsulating,regression algorithms,metrics,simplifies,building,comparing,regression models,accurate predictions,insights
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `AlgoMaster-0.1.0/PKG-INFO` & `AlgoMaster-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.1.0
-Summary: The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.
+Version: 0.1.1
+Summary: The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.The Classifier class streamlines classification tasks by offering a well-organized framework for model selection, hyperparameter tuning, 
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: machine learning,classifiers,logistic regression,k-nearest neighbors,naive Bayes,random forests,support vector machines,ensemble methods,hyperparameter tuning,performance evaluation,comparison,multiple classifiersadvantages,Regression class,regression analysis, Python,model training,evaluation,hyperparameter tuning,encapsulating,regression algorithms,metrics,simplifies,building,comparing,regression models,accurate predictions,insights
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `AlgoMaster-0.1.0/README.md` & `AlgoMaster-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `AlgoMaster-0.1.0/setup.py` & `AlgoMaster-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,23 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = '''
 
-        The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.
-        The Classifier class streamlines classification tasks by offering a well-organized framework for model selection, hyperparameter tuning, 
+        The Regression class simplifies regression analysis by providing a convenient and flexible approach for model training, evaluation, and hyperparameter tuning.The Classifier class streamlines classification tasks by offering a well-organized framework for model selection, hyperparameter tuning, 
         and performance evaluation with diverse classifiers.
 
 '''
 LONG_DESCRIPTION = '''
-        The Regression class provides a convenient and flexible way to perform regression analysis in Python, 
-    allowing for easy model training, evaluation, and hyperparameter tuning. By encapsulating various regression algorithms and metrics, 
-    it simplifies the process of building and comparing regression models, ultimately aiding in accurate predictions and insights.
-        The "Classifier" class provides a convenient and organized way to perform various machine learning classification tasks, 
-    including model selection, hyperparameter tuning, and performance evaluation, with a wide range of classifiers. 
-    It encapsulates common functionality and enables easy comparison of multiple classifiers, making it a useful tool for classification tasks.'''
+        The Regression class provides a convenient and flexible way to perform regression analysis in Python, allowing for easy model training, evaluation, and hyperparameter tuning. By encapsulating various regression algorithms and metrics, it simplifies the process of building and comparing regression models, ultimately aiding in accurate predictions and insights.The "Classifier" class provides a convenient and organized way to perform various machine learning classification tasks, including model selection, hyperparameter tuning, and performance evaluation, with a wide range of classifiers. It encapsulates common functionality and enables easy comparison of multiple classifiers, making it a useful tool for classification tasks.'''
 
 # Setting up
 setup(
     name="AlgoMaster",
     version=VERSION,
     author="sajo sam",
     author_email="<sajosamambalakara@gmail.com>",
```

