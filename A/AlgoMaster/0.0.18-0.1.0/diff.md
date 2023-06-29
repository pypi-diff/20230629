# Comparing `tmp/AlgoMaster-0.0.18.tar.gz` & `tmp/AlgoMaster-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoMaster-0.0.18.tar", last modified: Wed Jun 21 14:10:25 2023, max compression
+gzip compressed data, was "AlgoMaster-0.1.0.tar", last modified: Thu Jun 29 13:24:21 2023, max compression
```

## Comparing `AlgoMaster-0.0.18.tar` & `AlgoMaster-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:10:25.247494 AlgoMaster-0.0.18/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:10:25.177306 AlgoMaster-0.0.18/AlgoMaster/
--rw-rw-rw-   0        0        0       39 2023-06-19 16:54:03.000000 AlgoMaster-0.0.18/AlgoMaster/__init__.py
--rw-rw-rw-   0        0        0    27535 2023-06-21 10:03:10.000000 AlgoMaster-0.0.18/AlgoMaster/classifier.py
--rw-rw-rw-   0        0        0     2540 2023-06-21 09:37:36.000000 AlgoMaster-0.0.18/AlgoMaster/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:10:25.244495 AlgoMaster-0.0.18/AlgoMaster.egg-info/
--rw-rw-rw-   0        0        0     3397 2023-06-21 14:10:25.000000 AlgoMaster-0.0.18/AlgoMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-21 14:10:25.000000 AlgoMaster-0.0.18/AlgoMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:10:25.000000 AlgoMaster-0.0.18/AlgoMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 14:10:25.000000 AlgoMaster-0.0.18/AlgoMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 14:10:25.000000 AlgoMaster-0.0.18/AlgoMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3397 2023-06-21 14:10:25.246493 AlgoMaster-0.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     2349 2023-06-21 14:07:26.000000 AlgoMaster-0.0.18/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 14:10:25.248495 AlgoMaster-0.0.18/setup.cfg
--rw-rw-rw-   0        0        0     1718 2023-06-21 14:10:11.000000 AlgoMaster-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.356380 AlgoMaster-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.307354 AlgoMaster-0.1.0/AlgoMaster/
+-rw-rw-rw-   0        0        0       73 2023-06-21 14:23:59.000000 AlgoMaster-0.1.0/AlgoMaster/__init__.py
+-rw-rw-rw-   0        0        0    21345 2023-06-29 10:17:12.000000 AlgoMaster-0.1.0/AlgoMaster/classifier.py
+-rw-rw-rw-   0        0        0     3230 2023-06-29 06:17:21.000000 AlgoMaster-0.1.0/AlgoMaster/demo.py
+-rw-rw-rw-   0        0        0     2493 2023-06-28 17:05:15.000000 AlgoMaster-0.1.0/AlgoMaster/reg.py
+-rw-rw-rw-   0        0        0    31651 2023-06-29 11:09:26.000000 AlgoMaster-0.1.0/AlgoMaster/regressor.py
+-rw-rw-rw-   0        0        0       36 2023-06-29 05:46:33.000000 AlgoMaster-0.1.0/AlgoMaster/tempCodeRunnerFile.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:24:21.351358 AlgoMaster-0.1.0/AlgoMaster.egg-info/
+-rw-rw-rw-   0        0        0     5206 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 13:24:21.000000 AlgoMaster-0.1.0/AlgoMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5206 2023-06-29 13:24:21.355359 AlgoMaster-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4012 2023-06-29 11:10:52.000000 AlgoMaster-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:24:21.357360 AlgoMaster-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2790 2023-06-29 11:11:49.000000 AlgoMaster-0.1.0/setup.py
```

### Comparing `AlgoMaster-0.0.18/AlgoMaster/demo.py` & `AlgoMaster-0.1.0/AlgoMaster/demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,40 @@
-import numpy as np
 import pandas as pd
-from sklearn.preprocessing import StandardScaler
-from sklearn.model_selection import train_test_split
-from sklearn import svm
 from sklearn.metrics import accuracy_score
+from sklearn.linear_model import LogisticRegression
+from sklearn.model_selection import train_test_split
 from classifier import Classifier
-
 diabetes_dataset = pd.read_csv('F:\packagesPyPi\AlgoMaster\diabetes.csv')
 X = diabetes_dataset.drop(["Pregnancies","BloodPressure","SkinThickness","Outcome"], axis=1)
 Y = diabetes_dataset['Outcome']
-clg=Classifier(X,Y,0.2,42)
-print(clg.model_training())
-print(clg.ensemble_prediction(4))
+# X_train, X_test, Y_train, Y_test=train_test_split(X,Y,test_size=0.2,stratify=Y,random_state=30)
+# data=LogisticRegression()
+# data.fit(X_train,Y_train)
+# y_pred=data.predict(X_test)
+# acc = accuracy_score(Y_test, y_pred)
+# print("1st",acc)
+
+# X_train, X_test, Y_train, Y_test=train_test_split(X,Y,test_size=0.2,stratify=Y,random_state=30)
+# data=LogisticRegression()
+# data.fit(X_train,Y_train)
+# y_pred=data.predict(X_test)
+# acc = accuracy_score(Y_test, y_pred)
+# print("2nd",acc)
+
+# data=LogisticRegression()
+# data.fit(X_train,Y_train)
+# y_pred=data.predict(X_test)
+# acc = accuracy_score(Y_test, y_pred)
+# print("3rd",acc)
+clg=Classifier(X,Y,0.2,30)
+# print(clg.demo())
+# print(clg.model_training())
+# print(clg.ensemble_prediction(4))
 
 print(clg.hyperparameter_tuning())
-
 data=(148,0,33.6,0.627,50)
 # pred, acc=clg.AdaBoost_test(data)
 # print(pred)
 # print(acc)
 
 # pred,acc =clg.logistic_test(data)
 # print(pred)
@@ -68,49 +84,48 @@
 # print(pred)
 # print(acc)
 
 # pred,acc =clg.SVC_test(data)
 # print(pred)
 # print(acc)
 
-pred,acc=clg.logistic_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.knn_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.gaussian_nb_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.bernoulli_nb_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.bagging_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.extra_trees_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.ridge_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.sgd_hyperparameter(data)
+pred=clg.logistic_hyperparameter(data)
 print(pred)
-print(acc)
-pred,acc=clg.random_forest_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.xgb_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.ada_boost_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.gradient_boosting_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.decision_tree_hyperparameter(data)
-print(pred)
-print(acc)
-pred,acc=clg.svc_hyperparameter(data)
-print(pred)
-print(acc)
+# pred,acc=clg.knn_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.gaussian_nb_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.bernoulli_nb_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.bagging_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.extra_trees_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.ridge_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.sgd_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.random_forest_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.xgb_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.ada_boost_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.gradient_boosting_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.decision_tree_hyperparameter(data)
+# print(pred)
+# print(acc)
+# pred,acc=clg.svc_hyperparameter(data)
+# print(pred)
+# print(acc)
```

