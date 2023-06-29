# Comparing `tmp/sam_ml-py-0.7.1.tar.gz` & `tmp/sam_ml-py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.7.1.tar", last modified: Tue Jun 27 20:01:25 2023, max compression
+gzip compressed data, was "sam_ml-py-0.7.2.tar", last modified: Thu Jun 29 12:13:21 2023, max compression
```

## Comparing `sam_ml-py-0.7.1.tar` & `sam_ml-py-0.7.2.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.425649 sam_ml-py-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-27 20:01:25.425649 sam_ml-py-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.421649 sam_ml-py-0.7.1/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.421649 sam_ml-py-0.7.1/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.421649 sam_ml-py-0.7.1/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.425649 sam_ml-py-0.7.1/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:25.425649 sam_ml-py-0.7.1/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-27 20:01:25.000000 sam_ml-py-0.7.1/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-27 20:01:25.000000 sam_ml-py-0.7.1/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:01:25.000000 sam_ml-py-0.7.1/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 20:01:25.000000 sam_ml-py-0.7.1/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 20:01:25.000000 sam_ml-py-0.7.1/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 20:01:25.425649 sam_ml-py-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-27 20:01:15.000000 sam_ml-py-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.540483 sam_ml-py-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 12:13:21.540483 sam_ml-py-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.532483 sam_ml-py-0.7.2/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.532483 sam_ml-py-0.7.2/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.536483 sam_ml-py-0.7.2/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.536483 sam_ml-py-0.7.2/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.536483 sam_ml-py-0.7.2/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-29 12:13:21.000000 sam_ml-py-0.7.2/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 12:13:21.000000 sam_ml-py-0.7.2/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:13:21.000000 sam_ml-py-0.7.2/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-29 12:13:21.000000 sam_ml-py-0.7.2/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 12:13:21.000000 sam_ml-py-0.7.2/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-29 12:13:21.540483 sam_ml-py-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:21.540483 sam_ml-py-0.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-29 12:13:11.000000 sam_ml-py-0.7.2/test/test_models.py
```

### Comparing `sam_ml-py-0.7.1/LICENSE` & `sam_ml-py-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/PKG-INFO` & `sam_ml-py-0.7.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.7.1/README.md` & `sam_ml-py-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/config/logging.py` & `sam_ml-py-0.7.2/sam_ml/config/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         elif log_level == "warning":
             logger.setLevel(logging.WARNING)
         elif log_level == "error":
             logger.setLevel(logging.ERROR)
         else:
             raise ValueError("not supported content of global variable SAM_ML_LOG_LEVEL")
     except:
+        os.environ["SAM_ML_LOG_LEVEL"] = "info"
         logger.setLevel(logging.INFO)
 
     c_handler = logging.StreamHandler(sys.stdout)
 
     c_format = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     c_handler.setFormatter(c_format)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/data/embeddings.py` & `sam_ml-py-0.7.2/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/data/feature_selection.py` & `sam_ml-py-0.7.2/sam_ml/data/feature_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import pandas as pd
 import statsmodels.api as sm
 from sklearn.decomposition import PCA
 from sklearn.ensemble import ExtraTreesClassifier
-from sklearn.feature_selection import (RFE, RFECV, SelectFromModel,
-                                       SelectKBest, SequentialFeatureSelector,
-                                       chi2)
+from sklearn.feature_selection import (
+    RFE,
+    RFECV,
+    SelectFromModel,
+    SelectKBest,
+    SequentialFeatureSelector,
+    chi2,
+)
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import LinearSVC
 
 from sam_ml.config import setup_logger
 
 logger = setup_logger(__name__)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/data/sampling.py` & `sam_ml-py-0.7.2/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/data/scaler.py` & `sam_ml-py-0.7.2/sam_ml/data/scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import pandas as pd
-from sklearn.preprocessing import (MaxAbsScaler, MinMaxScaler, Normalizer,
-                                   PowerTransformer, QuantileTransformer,
-                                   RobustScaler, StandardScaler)
+from sklearn.preprocessing import (
+    MaxAbsScaler,
+    MinMaxScaler,
+    Normalizer,
+    PowerTransformer,
+    QuantileTransformer,
+    RobustScaler,
+    StandardScaler,
+)
 
 from sam_ml.config import setup_logger
 
 logger = setup_logger(__name__)
 
 
 class Scaler:
```

### Comparing `sam_ml-py-0.7.1/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.7.2/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/AdaBoostClassifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from ConfigSpace import Beta, Categorical, ConfigurationSpace, Float, Integer
-from sklearn.ensemble import (AdaBoostClassifier, GradientBoostingClassifier,
-                              RandomForestClassifier)
+from sklearn.ensemble import (
+    AdaBoostClassifier,
+    GradientBoostingClassifier,
+    RandomForestClassifier,
+)
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
 from .main_classifier import Classifier
 
 
@@ -41,8 +44,17 @@
             seed=42,
             space={
             "estimator": Categorical("estimator", core_estimator, default=core_estimator[2]),
             "n_estimators": Integer("n_estimators", (10, 3000), log=True, default=50),
             "learning_rate": Float("learning_rate", (0.005, 2), distribution=Beta(10, 5), default=1),
             "algorithm": Categorical("algorithm", ["SAMME.R", "SAMME"], default="SAMME.R"),
             })
+        
+        # workaround for now -> Problems with estimator parameter and JSON format (in smac_search)
+        self.smac_grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (10, 3000), log=True, default=50),
+            "learning_rate": Float("learning_rate", (0.005, 2), distribution=Beta(10, 5), default=1),
+            "algorithm": Categorical("algorithm", ["SAMME.R", "SAMME"], default="SAMME.R"),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/ExtraTreesClassifier.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,60 @@
-import warnings
-
-from ConfigSpace import Beta, Categorical, ConfigurationSpace, Float, Integer
-from sklearn.ensemble import (BaggingClassifier, GradientBoostingClassifier,
-                              RandomForestClassifier)
-from sklearn.linear_model import LogisticRegression
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.svm import SVC
-from sklearn.tree import DecisionTreeClassifier
+from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
+from sklearn.ensemble import ExtraTreesClassifier
 
 from .main_classifier import Classifier
 
-warnings. filterwarnings('ignore')
-
 
-class BC(Classifier):
-    """ BaggingClassifier Wrapper class """
+class ETC(Classifier):
+    """ ExtraTreesClassifier Wrapper class """
 
     def __init__(
         self,
-        model_name: str = "BaggingClassifier",
-        random_state: int = 42,
+        model_name: str = "ExtraTreesClassifier",
         n_jobs: int = -1,
+        random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
-            estimator: base estimator from which the boosted ensemble is built (default: DecisionTreeClassifier with max_depth=1)
-            n_estimator: number of boosting stages to perform
-            max_samples: the number of samples to draw from X to train each base estimator
-            max_features: the number of features to draw from X to train each base estimator
-            bootstrap: whether samples are drawn with replacement. If False, sampling without replacement is performed
-            bootstrap_features: whether features are drawn with replacement
+            n_estimators: Number of trees
+            max_depth: Maximum number of levels in tree
+            n_jobs: how many cores shall be used (-1 means all)
+            random_state: random_state for model
+            verbose: log level (higher number --> more logs)
+            warm_start: work with previous fit and add more estimator
+
+            max_features: Number of features to consider at every split
+            min_samples_split: Minimum number of samples required to split a node
+            min_samples_leaf: Minimum number of samples required at each leaf node
+            bootstrap: Method of selecting samples for training each tree
+            criterion: function to measure the quality of a split
         """
-        model_type = "BC"
-        model = BaggingClassifier(
-            random_state=random_state,
+        model_type = "ETC"
+        model = ExtraTreesClassifier(
             n_jobs=n_jobs,
+            random_state=random_state,
             **kwargs,
         )
-        if type(model.estimator) == RandomForestClassifier:
-            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for j in (100, 50, 20, 10, 5) for i in range(1,11)]
-        elif type(model.estimator) == DecisionTreeClassifier or model.estimator is None:
-            core_estimator = [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]
-        else:
-            core_estimator = [SVC(probability=True, kernel='linear'), GradientBoostingClassifier(), KNeighborsClassifier(), LogisticRegression()]
-
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "estimator": Categorical("estimator", core_estimator, default=core_estimator[3]),
-            "n_estimators": Integer("n_estimators", (3, 3000), distribution=Beta(1, 15), default=10),
-            "max_samples": Float("max_samples", (0.1, 1), default=1),
-            "max_features": Categorical("max_features", [0.5, 0.9, 1.0, 2, 4], default=1.0),
-            "bootstrap": Categorical("bootstrap", [True, False], default=True),
-            "bootstrap_features": Categorical("bootstrap_features", [True, False], default=False),
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
+            "bootstrap": Categorical("bootstrap", [True, False], default=False),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
+            })
+        
+        # workaround for now -> Problems with Normal distribution (in smac_search)
+        self.smac_grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
+            "bootstrap": Categorical("bootstrap", [True, False], default=False),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.7.2/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.7.2/sam_ml/models/ClassifierTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         @param:
             x_train, y_train, x_test, y_test: Data to train and evaluate models
 
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")    
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
             saves metrics in dict self.scores and also outputs them
         """
         try:
             for key in tqdm(self.models.keys(), desc="Crossvalidation"):
                 tscore, ttime = self.models[key].train(x_train, y_train, console_out=False)
@@ -259,15 +259,15 @@
 
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
             
             small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
             saves metrics in dict self.scores and also outputs them
         """
 
         try:
             for key in tqdm(self.models.keys(), desc="Crossvalidation"):
@@ -338,15 +338,15 @@
 
             n_trails: number of parameter sets to test
 
             scoring: metrics to evaluate the models
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
             secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
 
             small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
 
             cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
 
             leave_loadbar: shall the loading bar of the randomCVsearch of each individual model be visible after training (True - load bar will still be visible)
         """
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.7.2/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.7.2/sam_ml/models/RandomForestClassifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-from ConfigSpace import Categorical, ConfigurationSpace, Float, Integer, Normal
-from sklearn.ensemble import GradientBoostingClassifier
+from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
+from sklearn.ensemble import RandomForestClassifier
 
 from .main_classifier import Classifier
 
 
-class GBM(Classifier):
-    """ GradientBoostingMachine Wrapper class """
+class RFC(Classifier):
+    """ RandomForestClassifier Wrapper class """
 
     def __init__(
         self,
-        model_name: str = "GradientBoostingMachine",
+        model_name: str = "RandomForestClassifier",
+        n_jobs: int = -1, 
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
-            n_estimator: number of boosting stages to perform
-            criterion: function to measure the quality of a split
+            n_estimators: Number of trees in random forest
             max_depth: Maximum number of levels in tree
+            n_jobs: how many cores shall be used (-1 means all)
+            random_state: random_state for model
+            verbose: log level (higher number --> more logs)
+            warm_start: work with previous fit and add more estimator
+
+            max_features: Number of features to consider at every split
             min_samples_split: Minimum number of samples required to split a node
             min_samples_leaf: Minimum number of samples required at each leaf node
-            max_features: number of features to consider when looking for the best split
-            subsample: fraction of samples to be used for fitting the individual base learners
-            loss: The loss function to be optimized. 'deviance' refers to deviance (= logistic regression) for classification with probabilistic outputs. For loss 'exponential' gradient boosting recovers the AdaBoost algorithm
-            learning_rate: shrinks the contribution of each tree by learning rate
-
-            warm_start: work with previous fit and add more estimator
-            random_state: random_state for model
+            bootstrap: Method of selecting samples for training each tree
+            criterion: function to measure the quality of a split
         """
-        model_type = "GBM"
-        model = GradientBoostingClassifier(random_state=random_state, **kwargs,)
+        model_type = "RFC"
+        model = RandomForestClassifier(
+            n_jobs=n_jobs,
+            random_state=random_state,
+            **kwargs,
+        )
         grid = ConfigurationSpace(
             seed=42,
             space={
-            "n_estimators": Integer("n_estimators", (20, 1500), log=True, default=100),
-            "max_depth": Integer("max_depth", (1, 15), distribution=Normal(5, 3), default=3),
-            "min_samples_split": Integer("min_samples_split", (2, 100), log=True, default=2),
-            "min_samples_leaf": Integer("min_samples_leaf", (1, 100), log=True, default=1),
-            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"], default="auto"),
-            "subsample": Float("subsample", (0.7, 1), default=1),
-            "criterion": Categorical("criterion", ["friedman_mse", "squared_error"], default="friedman_mse"),
-            "loss": Categorical("loss", ["log_loss", "deviance"], default="log_loss"),
-            "learning_rate": Float("learning_rate", (0.005, 0.3), log=True, default=0.1),
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
+            "bootstrap": Categorical("bootstrap", [True, False], default=True),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
+            })
+        
+        # workaround for now -> Problems with Normal distribution (in smac_search)
+        self.smac_grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True, default=100),
+            "max_depth": Integer("max_depth", (3, 15), default=5),
+            "min_samples_split": Integer("min_samples_split", (2, 10), default=2),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4), default=1),
+            "bootstrap": Categorical("bootstrap", [True, False], default=True),
+            "criterion": Categorical("criterion", ["gini", "entropy"], default="gini"),
             })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.7.2/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from ConfigSpace import (Categorical, ConfigurationSpace, Float,
-                         ForbiddenAndConjunction, ForbiddenEqualsClause)
+from ConfigSpace import (
+    Categorical,
+    ConfigurationSpace,
+    Float,
+    ForbiddenAndConjunction,
+    ForbiddenEqualsClause,
+)
 from sklearn.svm import LinearSVC
 
 from .main_classifier import Classifier
 
 
 class LSVC(Classifier):
     """ LinearSupportVectorClassifier Wrapper class """
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.7.2/sam_ml/models/LogisticRegression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import numpy as np
-from ConfigSpace import (Categorical, ConfigurationSpace, EqualsCondition,
-                         Float, ForbiddenAndConjunction, ForbiddenEqualsClause,
-                         ForbiddenInClause)
+from ConfigSpace import (
+    Categorical,
+    ConfigurationSpace,
+    EqualsCondition,
+    Float,
+    ForbiddenAndConjunction,
+    ForbiddenEqualsClause,
+    ForbiddenInClause,
+)
 from sklearn.linear_model import LogisticRegression
 
 from .main_classifier import Classifier
 
 
 class LR(Classifier):
     """ LogisticRegression Wrapper class """
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.7.2/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.7.2/sam_ml/models/XGBoostClassifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,11 +33,25 @@
             'reg_alpha' : Integer('reg_alpha', (0, 180), default=0),
             'reg_lambda' : Float('reg_lambda', (0, 1), default=1),
             'colsample_bytree' : Float('colsample_bytree', (0.5, 1), default=1),
             'min_child_weight' : Integer('min_child_weight', (0, 10), default=1),
             'n_estimators': Integer("n_estimators", bounds=(50, 750), distribution=Normal(150, 100), default=100),
             "learning_rate": Float("learning_rate", bounds=(0.001, 0.30), log=True, default=0.1),
             })
+        
+        # workaround for now -> Problems with Normal distribution (in smac_search)
+        self.smac_grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "max_depth": Integer("max_depth", (3, 10), default=6),
+            "gamma": Float('gamma', (0, 9), default=0),
+            'reg_alpha' : Integer('reg_alpha', (0, 180), default=0),
+            'reg_lambda' : Float('reg_lambda', (0, 1), default=1),
+            'colsample_bytree' : Float('colsample_bytree', (0.5, 1), default=1),
+            'min_child_weight' : Integer('min_child_weight', (0, 10), default=1),
+            'n_estimators': Integer("n_estimators", bounds=(50, 750), default=100),
+            "learning_rate": Float("learning_rate", bounds=(0.001, 0.30), log=True, default=0.1),
+            })
         super().__init__(model, model_name, model_type, grid)
 
     def feature_importance(self):
         super().feature_importance()
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/__init__.py` & `sam_ml-py-0.7.2/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/main_classifier.py` & `sam_ml-py-0.7.2/sam_ml/models/main_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 from statistics import mean
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from ConfigSpace import Configuration, ConfigurationSpace
 from matplotlib import pyplot as plt
-from sklearn.metrics import (accuracy_score, classification_report,
-                             make_scorer, precision_score, recall_score)
+from sklearn.metrics import (
+    accuracy_score,
+    classification_report,
+    make_scorer,
+    precision_score,
+    recall_score,
+)
 from sklearn.model_selection import cross_validate
 from smac import HyperparameterOptimizationFacade, Scenario
 from tqdm.auto import tqdm
 
 from sam_ml.config import setup_logger
 
 from .main_model import Model
@@ -112,15 +117,15 @@
 
             avg: average to use for precision and recall score (e.g. "micro", None, "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
 
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return: dictionary with keys with scores: 'accuracy', 'precision', 'recall', 's_score', 'l_score'
         """
         pred = self.predict(x_test)
 
         # Calculate Accuracy, Precision and Recall Metrics
         accuracy = accuracy_score(y_test, pred)
@@ -163,15 +168,15 @@
         @param:
             x_test, y_test: Data to evaluate model
             scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
 
             avg: average to use for precision and recall score (e.g. "micro", None, "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return: score as float
         """
         pred = self.predict(x_test)
 
         # Calculate score
         if scoring == "accuracy":
@@ -195,27 +200,27 @@
         y: pd.Series,
         cv_num: int = 10,
         avg: str = "macro",
         pos_label: Union[int, str] = -1,
         console_out: bool = True,
         secondary_scoring: str = None,
         strength: int = 3,
-    ) -> Union[dict[str, float], pd.DataFrame]:
+    ) -> dict[str, float]:
         """
         @param:
             X, y: data to cross validate on
             cv_num: number of different splits
 
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
 
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
             dictionary with "accuracy", "precision", "recall", "s_score", "l_score", train_score", "train_time"
         """
         logger.debug(f"cross validation {self.model_name} - started")
 
         precision_scorer = make_scorer(precision_score, average=avg, pos_label=pos_label)
@@ -292,15 +297,15 @@
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. pos_label is used by s_score/l_score
 
             leave_loadbar: shall the loading bar of the training be visible after training (True - load bar will still be visible)
             console_out: shall the result be printed into the console
 
             secondary_scoring: weights the scoring (only for 's_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for 's_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for 's_score'/'l_score')
 
         @return:
             dictionary with "accuracy", "precision", "recall", "s_score", "l_score", train_score", "train_time"
         """
         logger.debug(f"cross validation {self.model_name} - started")
 
         predictions = []
@@ -396,43 +401,47 @@
         scoring: str = "accuracy",
         avg: str = "macro",
         pos_label: Union[int, str] = -1,
         secondary_scoring: str = None,
         strength: int = 3,
         small_data_eval: bool = False,
         walltime_limit: float = 600,
+        log_level: int = 20,
     ) -> Configuration:
         """
         @params:
             x_train: DataFrame with train features
             y_train: Series with labels
 
             n_trails: max number of parameter sets to test
             cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
 
             scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
             secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
 
             small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
             
             walltime_limit: the maximum time in seconds that SMAC is allowed to run
 
+            log_level: 10 - DEBUG, 20 - INFO, 30 - WARNING, 40 - ERROR, 50 - CRITICAL (SMAC3 library log levels)
+
         @return: ConfigSpace.Configuration with best hyperparameters (can be used like dict)
         """
         logger.debug("starting smac_search")
-        # NormalInteger in grid are not supported and Classifier in Categorical
-        if self.model_type in ("RFC", "ABC", "BC", "ETC", "GBM", "XGBC"):
-            logger.error(f"The model type '{self.model_type}' is currently not supported")
-            return {}
+        # NormalInteger in grid are not supported and Classifier in Categorical (using workaround for now)
+        if self.model_type in ("RFC", "ETC", "GBM", "XGBC", "ABC", "BC"):
+            grid = self.smac_grid
+        else:
+            grid = self.grid
 
         scenario = Scenario(
-            self.grid,
+            grid,
             n_trials=n_trails,
             deterministic=True,
             walltime_limit=walltime_limit,
         )
 
         initial_design = HyperparameterOptimizationFacade.get_initial_design(scenario, n_configs=5)
         logger.debug(f"initial_design: {initial_design.select_configurations()}")
@@ -450,14 +459,15 @@
 
         # use SMAC to find the best hyperparameters
         smac = HyperparameterOptimizationFacade(
             scenario,
             grid_train,
             initial_design=initial_design,
             overwrite=True,  # If the run exists, we overwrite it; alternatively, we can continue from last state
+            logging_level=log_level,
         )
 
         incumbent = smac.optimize()
         logger.debug("finished smac_search")
         return incumbent
 
     def randomCVsearch(
@@ -481,15 +491,15 @@
 
             n_trails: number of parameter sets to test
 
             scoring: metrics to evaluate the models ("accuracy", "precision", "recall", "s_score", "l_score")
             avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
             pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
             secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+            strength: higher strength means a higher weight for the preferred secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
 
             small_data_eval: if True: trains model on all datapoints except one and does this for all datapoints (recommended for datasets with less than 150 datapoints)
 
             cv_num: number of different splits per crossvalidation (only used when small_data_eval=False)
 
             leave_loadbar: shall the loading bar of the different parameter sets be visible after training (True - load bar will still be visible)
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/main_model.py` & `sam_ml-py-0.7.2/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.7.1/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.7.2/sam_ml/models/main_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+from contextlib import suppress
 from typing import Union
 
 import pandas as pd
 
 from sam_ml.config import setup_logger
 from sam_ml.data import Embeddings_builder, Sampler, Scaler, Selector
 
@@ -24,14 +25,16 @@
             sampling: type of "data.sampling.Sampler" or Sampler class object for sampling the train data (None for no sampling)
             model: Classifier class object or tuple (model, model_type, hyperparameter grid)
             model_name: name of the model
         """
         self._classifier: tuple
 
         if issubclass(type(model), Classifier):
+            with suppress(BaseException):
+                self.smac_grid = model.smac_grid
             super().__init__(model.model, model_name, model.model_type, model.grid)
             self._classifier = (model.model, model.model_type, model.grid)
         else:
             super().__init__(model[0], model_name, model[1], model[2])
             self._classifier = model
 
         if vectorizer in Embeddings_builder.params()["vec"]:
```

### Comparing `sam_ml-py-0.7.1/sam_ml/models/scorer.py` & `sam_ml-py-0.7.2/sam_ml/models/scorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             'precision': take precision more into account
             'recall': take recall more into account
         
         pos_label:
             pos_label > 0: take <scoring> in class <pos_label> more into account
             pos_label = -1: handle all classes the same
 
-        strength: higher strength means a higher weight for the prefered scoring/pos_label
+        strength: higher strength means a higher weight for the preferred scoring/pos_label
 
         score_func: function to use for scoring (default: samuel_function)
 
     @return:
         score as float between 0 and 1
     """
     prec = precision_score(y_true, y_pred, average=None)
```

### Comparing `sam_ml-py-0.7.1/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.7.2/sam_ml_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.7.1/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.7.2/sam_ml_py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 sam_ml/__init__.py
 sam_ml/config/__init__.py
 sam_ml/config/logging.py
 sam_ml/data/__init__.py
 sam_ml/data/embeddings.py
 sam_ml/data/feature_selection.py
@@ -33,8 +34,10 @@
 sam_ml/models/main_model.py
 sam_ml/models/main_pipeline.py
 sam_ml/models/scorer.py
 sam_ml_py.egg-info/PKG-INFO
 sam_ml_py.egg-info/SOURCES.txt
 sam_ml_py.egg-info/dependency_links.txt
 sam_ml_py.egg-info/requires.txt
-sam_ml_py.egg-info/top_level.txt
+sam_ml_py.egg-info/top_level.txt
+test/__init__.py
+test/test_models.py
```

### Comparing `sam_ml-py-0.7.1/setup.py` & `sam_ml-py-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.7.1",
+    version="0.7.2",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

