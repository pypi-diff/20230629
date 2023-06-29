# Comparing `tmp/cla-1.1.6.tar.gz` & `tmp/cla-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cla-1.1.6.tar", last modified: Sun Jun 25 05:39:42 2023, max compression
+gzip compressed data, was "cla-1.1.7.tar", last modified: Thu Jun 29 08:06:04 2023, max compression
```

## Comparing `cla-1.1.6.tar` & `cla-1.1.7.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.659752 cla-1.1.6/
--rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.1.6/LICENCE
--rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4563 2023-06-25 05:39:42.659752 cla-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.399722 cla-1.1.6/cla/
--rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.1.6/cla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.607727 cla-1.1.6/cla/gui/
--rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-1.1.6/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.6/cla/gui/__init__.py
--rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-1.1.6/cla/gui/run.py
--rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-1.1.6/cla/gui/sample.csv
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.635755 cla-1.1.6/cla/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.6/cla/gui/static/__init__.py
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.1.6/cla/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.1.6/cla/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.1.6/cla/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.1.6/cla/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.1.6/cla/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.1.6/cla/gui/static/sample.csv
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.639748 cla-1.1.6/cla/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.1.6/cla/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.1.6/cla/gui/templates/home.html
--rw-rw-rw-   0        0        0    72189 2023-06-25 05:38:43.000000 cla-1.1.6/cla/metrics.py
--rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.1.6/cla/unify.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.655760 cla-1.1.6/cla/vis/
--rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.1.6/cla/vis/__init__.py
--rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.1.6/cla/vis/feature_importance.py
--rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.1.6/cla/vis/plotComponents1D.py
--rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.1.6/cla/vis/plotComponents2D.py
--rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.1.6/cla/vis/plotComponents3D.py
--rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.1.6/cla/vis/plt2base64.py
--rw-rw-rw-   0        0        0     4959 2023-03-15 01:20:08.000000 cla-1.1.6/cla/vis/unsupervised_dimension_reductions.py
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.588156 cla-1.1.6/cla.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.655760 cla-1.1.6/data/
--rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.1.6/data/sample.csv
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 05:39:42.663747 cla-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-06-25 04:59:20.000000 cla-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.415040 cla-1.1.7/
+-rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.1.7/LICENCE
+-rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4563 2023-06-29 08:06:04.415040 cla-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.336884 cla-1.1.7/cla/
+-rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.1.7/cla/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.368130 cla-1.1.7/cla/gui/
+-rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-1.1.7/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.7/cla/gui/__init__.py
+-rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-1.1.7/cla/gui/run.py
+-rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-1.1.7/cla/gui/sample.csv
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.383796 cla-1.1.7/cla/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.7/cla/gui/static/__init__.py
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.1.7/cla/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.1.7/cla/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.1.7/cla/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.1.7/cla/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.1.7/cla/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.1.7/cla/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.383796 cla-1.1.7/cla/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.1.7/cla/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.1.7/cla/gui/templates/home.html
+-rw-rw-rw-   0        0        0    79377 2023-06-29 07:36:45.000000 cla-1.1.7/cla/metrics.py
+-rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.1.7/cla/unify.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.399390 cla-1.1.7/cla/vis/
+-rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.1.7/cla/vis/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-06-28 15:04:04.000000 cla-1.1.7/cla/vis/confusion_matrix.py
+-rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.1.7/cla/vis/feature_importance.py
+-rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.1.7/cla/vis/plotComponents1D.py
+-rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.1.7/cla/vis/plotComponents2D.py
+-rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.1.7/cla/vis/plotComponents3D.py
+-rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.1.7/cla/vis/plt2base64.py
+-rw-rw-rw-   0        0        0     4953 2023-06-28 11:18:59.000000 cla-1.1.7/cla/vis/unsupervised_dimension_reductions.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.368130 cla-1.1.7/cla.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-06-29 08:06:04.000000 cla-1.1.7/cla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-06-29 08:06:04.000000 cla-1.1.7/cla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:06:04.000000 cla-1.1.7/cla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:06:04.000000 cla-1.1.7/cla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 08:06:04.000000 cla-1.1.7/cla.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 08:06:04.415040 cla-1.1.7/data/
+-rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.1.7/data/sample.csv
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:06:04.415040 cla-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-06-28 07:33:38.000000 cla-1.1.7/setup.py
```

### Comparing `cla-1.1.6/PKG-INFO` & `cla-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.1.6
+Version: 1.1.7
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.1.6 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.1.7 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.1.6/README.md` & `cla-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv` & `cla-1.1.7/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/run.py` & `cla-1.1.7/cla/gui/run.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/sample.csv` & `cla-1.1.7/cla/gui/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/bootstrap.css` & `cla-1.1.7/cla/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/bootstrap.js` & `cla-1.1.7/cla/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/jquery-3.3.1.min.js` & `cla-1.1.7/cla/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/jquery.blockUI.js` & `cla-1.1.7/cla/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/jquery.form.min.js` & `cla-1.1.7/cla/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/static/sample.csv` & `cla-1.1.7/cla/gui/static/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/gui/templates/home.html` & `cla-1.1.7/cla/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/metrics.py` & `cla-1.1.7/cla/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,52 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from tqdm import tqdm
+import IPython.display
 
 from sklearn.metrics import *  # we use global() to access the imported functions
 from sklearn.preprocessing import MinMaxScaler
+from sklearn.linear_model import LogisticRegression, LogisticRegressionCV
+from sklearn.naive_bayes import BernoulliNB, GaussianNB, MultinomialNB
+from sklearn.tree import DecisionTreeClassifier # ExtraTreeClassifier only works in ensembles
+from sklearn.neural_network import MLPClassifier
+from sklearn.neighbors import KNeighborsClassifier, NearestCentroid
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.svm import LinearSVC, SVC
 # from scipy.integrate import quad
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split, GridSearchCV
-from sklearn.svm import SVC, LinearSVC
 from sklearn.feature_selection import mutual_info_classif, chi2
-from sklearn.naive_bayes import GaussianNB
-from sklearn.linear_model import LogisticRegressionCV
 from sklearn.preprocessing import OneHotEncoder
 from statsmodels.multivariate import manova
 from statsmodels.stats.contingency_tables import mcnemar, cochrans_q
 
 import rpy2
 
 if __package__:
     from .vis.plt2base64 import plt2html
     from .vis.plotComponents2D import plotComponents2D
     from .vis.feature_importance import plot_feature_importance
     from .vis.unsupervised_dimension_reductions import unsupervised_dimension_reductions
+    from .vis.confusion_matrix import plot_confusion_matrix
 else:
     VIS_DIR = os.path.dirname(__file__) + '/vis'
     if VIS_DIR not in sys.path:
         sys.path.append(VIS_DIR)
 
     from plt2base64 import plt2html
     from plotComponents2D import plotComponents2D
     from feature_importance import plot_feature_importance
     from unsupervised_dimension_reductions import unsupervised_dimension_reductions
+    from confusion_matrix import plot_confusion_matrix
 
 ENABLE_R = True
 if sys.platform == "win32" and rpy2.__version__ >= '3.0.0':
     print('rpy2 3.X may not support Windows. ECoL metrics may not be available.')
     # ENABLE_R = False
 
 if ENABLE_R:
@@ -255,21 +263,24 @@
     """
     We draw random samples from the bayes distribution models to calculate BER
 
     nobs - number of observations, i.e., sample size
     NSgima - the sampling range
     """
 
-    nb = GaussianNB(priors=[0.5, 0.5])  # we have no strong prior assumption.
-    nb.fit(X, y)
-
     labels = list(set(y))
 
-    # For multi-class classification, use one vs rest strategy
-    assert len(labels) == 2
+    # only support binary classifiction. For multi-class classification, use one vs rest strategy
+    if len(labels) != 2:
+        print("GaussianNB only support binary classifiction. Return 0 by default.")
+        return np.zeros(X.shape[1]), None
+
+
+    nb = GaussianNB(priors=[0.5, 0.5])  # we have no strong prior assumption.
+    nb.fit(X, y)
 
     Xc1 = X[y == labels[0]]
     Xc2 = X[y == labels[1]]
 
     n1 = len(Xc1)
     n2 = len(Xc2)
 
@@ -365,14 +376,29 @@
                'classification.CrossEntropy',  # cross-entropy loss / log loss
                'classification.Mean_KLD',
                # 'classification.AP',
                'classification.Brier',
                'classification.ROC_AUC',
                'classification.PR_AUC']
 
+CLF_METRICS_MULTICLASS = ['classification.ACC',
+               'classification.Kappa',
+               'classification.F1_Score',
+               'classification.Jaccard',  # The Jaccard index, or Jaccard similarity coefficient, defined as the size of the intersection divided by the size of the union of two label sets
+               'classification.Precision',
+               'classification.Recall',
+               'classification.McNemar',
+               'classification.McNemar.CHI2',
+               'classification.CochranQ',
+               'classification.CochranQ.T',
+               # The following requires a model that outputs probability
+               'classification.CrossEntropy',
+               'classification.Mean_KLD'] 
+               
+
 ########## Section: SVM / LR ###########
 
 
 def grid_search_svm_hyperparams(X, y, test_size=0.2, tuned_parameters=[
     {'kernel': ['rbf'], 'gamma': [10, 1, 1e-1, 1e-2],
         'C': [0.01, 0.1, 1, 10, 100, 1000]},
         {'kernel': ['linear'], 'C': [0.01, 0.1, 1, 10, 100, 1000, 10000, 100000]}], cv=5, verbose=True):
@@ -601,23 +627,25 @@
     '''
 
     ###
     # train a logistic regression model
     # clf = LogisticRegressionCV(cv=10, solver = 'saga', penalty = 'elasticnet', max_iter = 5000, l1_ratios = [0,0.2,0.4,0.6,0.8,1]).fit(X, y) # with Elasticnet regularization, but it is too time consuming. We don't require sparse solution, so ridge suffices.
     # LOG += "regularization strength\t" + str(clf.C_) + "\nL1 reg ratio" + str(clf.l1_ratio_) + "\n\n"
 
+    is_binary = len(set(y)) == 2
+
     grp_samples = []
     for yv in set(y):
         grp_samples.append((y == yv).sum())
 
     # min(grp_samples) is the minimum sample size among all categories.
     # CV requires to be not greater than this value.
 
     try:
-        clf = LogisticRegressionCV(cv=min(3, min(grp_samples)), max_iter=1000).fit(
+        clf = LogisticRegressionCV(cv=min(3, min(grp_samples)), max_iter=1000, multi_class='multinomial').fit(
             X, y)  # ridge(L2) regularization
     except Exception as e:
         print('Exception in LogisticRegressionCV().', e)
         return None, None, None
 
     LOG += "regularization strength\t" + str(clf.C_) + "\n\n"
     # l1_ratio: while 1 is equivalent to using penalty='l1'. For 0 < l1_ratio <1, the penalty is a combination of L1 and L2.
@@ -677,18 +705,18 @@
         else:
             plt.close()
 
     y_pred = clf.predict(X)
     clf_metrics.append(globals()["accuracy_score"](y, y_pred))
     # use ground truth and prediction as 1st and 2nd raters. 0 - no agreement, 1 - perfect agreement.
     clf_metrics.append(globals()["cohen_kappa_score"](y, y_pred))
-    clf_metrics.append(globals()["f1_score"](y, y_pred))
-    clf_metrics.append(globals()["jaccard_score"](y, y_pred))
-    clf_metrics.append(globals()["precision_score"](y, y_pred))
-    clf_metrics.append(globals()["recall_score"](y, y_pred))
+    clf_metrics.append(globals()["f1_score"](y, y_pred, average = 'micro'))
+    clf_metrics.append(globals()["jaccard_score"](y, y_pred, average = 'micro'))
+    clf_metrics.append(globals()["precision_score"](y, y_pred, average = 'micro'))
+    clf_metrics.append(globals()["recall_score"](y, y_pred, average = 'micro'))
 
     res = mcnemar(confusion_matrix(y, y_pred), exact=False, correction=True)
     clf_metrics.append(res.pvalue)
     clf_metrics.append(res.statistic)
 
     data = np.hstack((np.array(y).reshape(-1, 1),
                      np.array(y_pred).reshape(-1, 1)))
@@ -697,40 +725,49 @@
     clf_metrics.append(res.statistic)
 
     ###
     # train a logistic regression model to compute Brier score, PR AUC, etc.
     # clf = LogisticRegressionCV(cv=5, random_state=0).fit(X, y)
     y_prob_ohe = clf.predict_proba(X)
     # for binary classification, use the second proba as P(Y=1|X)
-    y_prob = y_prob_ohe[:, 1]
+    # y_prob = y_prob_ohe[:, 1]
+    y_prob = y_prob_ohe # for multi-class
 
     enc = OneHotEncoder(handle_unknown='ignore')
     y_ohe = enc.fit_transform(np.array(y).reshape(-1, 1)).toarray()
     # print(y_ohe)
     # print(y_prob_ohe)
 
     clf_metrics.append(globals()["log_loss"](y, y_prob))
 
     mkld, _ = Mean_KLD(y_ohe, y_prob_ohe)
     clf_metrics.append(mkld)
 
     # clf_metrics.append(globals()["average_precision_score"](y, y_prob)) # According to the sklearn doc, this should equal to the P-R curve AUC. However, the actual result diifers. Implementation may have problems.
-    # The Brier score measures the mean squared difference between the predicted probability and the actual outcome.
-    clf_metrics.append(globals()["brier_score_loss"](y, y_prob))
-    clf_metrics.append(globals()["roc_auc_score"](y, y_prob))
-
-    # set pos_label for cases when y is not {0,1} or {-1,1}
-    precisions, recalls, _ = precision_recall_curve(
-        y, y_prob, pos_label=max(y))
-    clf_metrics.append(globals()["auc"](recalls, precisions))
+    # The Brier score measures the mean squared difference between the predicted probability and the actual outcome. 
+    # The Brier score only support binary classification.
+    if is_binary:
+        clf_metrics.append(globals()["brier_score_loss"](y, y_prob[:, 1]))
+        clf_metrics.append(globals()["roc_auc_score"](y, y_prob[:, 1]))# set pos_label for cases when y is not {0,1} or {-1,1}
+        precisions, recalls, _ = precision_recall_curve(y, y_prob[:, 1], pos_label=max(y))
+        clf_metrics.append(globals()["auc"](recalls, precisions))
+    else:
+        if verbose:
+            print('Brier score is not applicable for multi-class classification. We use log loss instead.')
+        clf_metrics.append(globals()["log_loss"](y, y_prob))
+        if verbose:
+            print('ROC and P-R curve AUC is not applicable for multi-class classification. Set 0.5 by default.')
+        clf_metrics.append(0.5)
+        clf_metrics.append(0.5)
 
     rpt = ''
     for v in zip(CLF_METRICS, clf_metrics):
-        rpt += v[0] + "\t" + str(v[1]) + "\n"
-        dic[v[0]] = v[1]
+        if is_binary or v[0] in CLF_METRICS_MULTICLASS:
+            rpt += v[0] + "\t" + str(v[1]) + "\n"
+            dic[v[0]] = v[1]
 
     LOG += "\n\n" + rpt
 
     # acc_train, acc_test, acc_all # , vertice_set # vertice_set[0] is the decision boundary
     return dic, IMG, LOG
 
 
@@ -755,14 +792,15 @@
     w = svc_model.coef_[0]
     p = np.linalg.norm(w, ord=2)
     width = 2/p
 
     IMG = ''
 
     if len(support_vectors[1]) == 2 and len(set(y)) == 2:
+
         df = pd.DataFrame(X)
 
         x_min = np.min(df.iloc[:, 0]) - 0.5
         x_max = np.max(df.iloc[:,  0]) + 0.5
         y_min = np.min(df.iloc[:, 1]) - 0.5
         y_max = np.max(df.iloc[:, 1]) + 0.5
 
@@ -872,15 +910,17 @@
     Recall that the chi-square test measures dependence between stochastic 
     variables, so using this function “weeds out” the features that are the 
     most likely to be independent of class and therefore irrelevant for 
     classification.
     """
 
     if (len(set(y)) < 2):
-        raise Exception('The dataset must have at least two classes.')
+        if verbose:
+            print('The dataset must have at least two classes for chisq gof test.')
+        return None, None, None
 
     IMG = ''
 
     # chi2 test requires scaling to [0,1]
     mm_scaler = MinMaxScaler()
     X_mm_scaled = mm_scaler.fit_transform(X)
 
@@ -923,15 +963,16 @@
     Mann-Whitney或Wilcoxon检验比较两组，而Kruskal-Wallis检验比较3组及以上。
     Kruskal-Wallis检验是一种非参数的单因素方差分析。它是基于秩（排序的，只考虑相对大小）的。
 
     由于KW检验考虑了样本的排序信息,而不仅仅是大于或小于中位数,因此比median test具有更大的power
     '''
 
     if len(set(y)) < 2:
-        print('The dataset must have at least 2 classes.')
+        if verbose:
+            print('The dataset must have at least two classes for Kruskal-Wallis test.')
         return None, None
 
     ps = []
     Hs = []
 
     for i in range(X.shape[1]):
         Xi = X[:, i]
@@ -950,15 +991,16 @@
                 Xcis[0], Xcis[1], Xcis[2], nan_policy='omit')
         elif len(set(y)) == 4:
             H, p = scipy.stats.kruskal(
                 Xcis[0], Xcis[1], Xcis[2], Xcis[3], nan_policy='omit')
         elif len(set(y)) >= 5:
             H, p = scipy.stats.kruskal(
                 Xcis[0], Xcis[1], Xcis[2], Xcis[3], Xcis[4], nan_policy='omit')
-            print("WARN: only the first 5 classes will be analyzed.")
+            if verbose:
+                print("WARN: only the first 5 classes will be analyzed for KW-test.")
 
         ps.append(p)
         Hs.append(H)
 
     if verbose:
         print('The P values for X in dimensions 1 to {}:{}'.format(
             len(X[0]), ps))
@@ -970,15 +1012,16 @@
 
 def T_IND(X, y, verbose=False, show=False, max_plot_num=5):
     '''
     independent t test. requires two classes/groups.
     '''
 
     if (len(set(y)) != 2):
-        print('The dataset must have 2 classes.')
+        if verbose:
+            print('The dataset must have two classes for t test.')
         return None, None, None
 
     ps = []
     Ts = []
     cnt = 0
     IMG = ''
 
@@ -1039,15 +1082,16 @@
     中位数检验是独立性卡方检验的一种特殊情况。
 
     给定k组样本，n1, n2 …… nk观测值，计算所有n1 +n2 + ……+nk观测值的中位数。
     然后构造一个2xk列联表，其中第一行包含k个样本的中位数以上的观测值，第二行包含k个样本的中位数以下或等于中位数的观测值。
     然后可以对该表应用独立性卡方检验。
     '''
     if (len(set(y)) < 2):
-        print('The dataset must have at least 2 classes.')
+        if verbose:
+            print('The dataset must have at least two classes for median test.')
         return None, None, None
 
     ps = []
     Ts = []
     MED = []  # grand median
     TBL = []  # contingency table
     IMG = ''
@@ -1070,15 +1114,16 @@
                 Xcis[0], Xcis[1], Xcis[2], ties='ignore')
         elif len(set(y)) == 4:
             T, p, med, tbl = scipy.stats.median_test(
                 Xcis[0], Xcis[1], Xcis[2], Xcis[3], ties='ignore')
         elif len(set(y)) >= 5:
             T, p, med, tbl = scipy.stats.median_test(
                 Xcis[0], Xcis[1], Xcis[2], Xcis[3], Xcis[4], ties='ignore')
-            print("WARN: only the first 5 classes will be analyzed.")
+            if verbose:
+                print("WARN: only the first 5 classes will be analyzed.")
 
         ps.append(p)
         Ts.append(T)
         MED.append(med)
         TBL.append(tbl)
 
         a1 = TBL[0][:, 0]
@@ -1140,15 +1185,17 @@
     """
     Performa feature-wise ANOVA test. Returns an array of p-values on all the features and its minimum.
 
     y - support up to 5 classes
     """
 
     if (len(set(y)) < 2):
-        raise Exception('The dataset must have at least two classes.')
+        if verbose:
+            print('The dataset must have at least two classes for ANOVA test.')
+        return None, None, None
 
     ps = []
     IMG = ''
     Fs = []
 
     cnt = 0
 
@@ -1170,15 +1217,16 @@
         if (len(set(y)) == 3):
             f, p = scipy.stats.f_oneway(Xcis[0], Xcis[1], Xcis[2])
         elif (len(set(y)) == 4):
             f, p = scipy.stats.f_oneway(Xcis[0], Xcis[1], Xcis[2], Xcis[3])
         elif (len(set(y)) >= 5):  # if there are five or more classes
             f, p = scipy.stats.f_oneway(
                 Xcis[0], Xcis[1], Xcis[2], Xcis[3], Xcis[4])
-            print('WARN: only the first 5 classes will be analyzed.')
+            if verbose:
+                print('WARN: only the first 5 classes will be analyzed for ANOVA.')
 
         """
         Alternative implementation using sm.stats.anova_lm
         
         import statsmodels.api as sm
         from statsmodels.formula.api import ols
 
@@ -1230,15 +1278,15 @@
     MANOVA test of the first two features.  
 
     For some statisticians the MANOVA doesn’t only compare differences in mean scores between multiple groups but also assumes a cause effect relationship whereby one or more independent, controlled variables (the factors) cause the significant difference of one or more characteristics. The factors sort the data points into one of the groups causing the difference in the mean value of the groups.
     Internally, it uses multivariate regression
     """
 
     if (X.shape[1] <= 1):
-        txt = 'There must be more than one dependent variable to fit MANOVA! Use ANOVA to substitute MANOVA.'
+        txt = 'There must be more than one independent variable to fit MANOVA! Use ANOVA to substitute MANOVA.'
         anova_p, anova_F, _ = ANOVA(X, y)
         return anova_p, anova_F, txt
 
     X1 = X[:, 0]
     X2 = X[:, 1]
     df = pd.DataFrame({'X1': X1, 'X2': X2, 'y': y})
     # Intercept is included by default.
@@ -1271,21 +1319,23 @@
         print(LOG)
 
     return manova_p, manova_F, LOG
 
 
 def MWW(X, y, verbose=False, show=False, max_plot_num=5):
     """
-    Performa feature-wise MWW test. Returns an array of p-values on all the features and its minimum.
+    Performa feature-wise MWW test. Only support binary classificaiton. Returns an array of p-values on all the features and its minimum.
 
-    y - support 2 classes
+    y - only support 2 classes
     """
 
     if (len(set(y)) != 2):
-        raise Exception('The dataset must have 2 classes.')
+        if verbose:
+            print('The dataset must have two classes for MWW test.')
+        return None, None, None
 
     ps = []
     Us = []
     IMG = ''
 
     cnt = 0
 
@@ -1340,20 +1390,20 @@
             print(test_result)
 
     IMG += '<br/>'
 
     return ps, Us, IMG
 
 
-def es_max(X, y):
-    d, _ = cohen_d(X, y)
+def es_max(X, y, verbose = True):
+    d, _ = cohen_d(X, y, verbose=verbose)
     return d.max()
 
 
-def cohen_d(X, y, show=False, save_fig=''):
+def cohen_d(X, y, show=False, save_fig='', verbose=True):
     '''
     Cohen’s d is a type of effect size between two means. Cohen’s d values are also known as the standardised mean difference (SMD).
     e.g., partial eta sqaured is the percentage of variance in the dependent variable (y) explained by the independent variable (x). 
 
     Statistical significance (p) only tells "there is a difference not due to pure chance", while the effect size is a quantitative measure of the magnitude for the difference between two means Or the degree to which $H_0$ is false. Size of difference.   
     That's why sometimes we prefer effective size over p value.
 
@@ -1363,15 +1413,18 @@
     d > .5 : medium
     d > .8 : large
     '''
 
     labels = list(set(y))
 
     # only support binary classifiction. For multi-class classification, use one vs rest strategy
-    assert len(labels) == 2
+    if len(labels) != 2:
+        if verbose:
+            print("Cohen's d only support binary classifiction. Return 0 by default.")
+        return np.zeros(X.shape[1]), None
 
     Xc1 = X[y == labels[0]]
     Xc2 = X[y == labels[1]]
 
     n1 = len(Xc1)
     n2 = len(Xc2)
     dof = n1 + n2 - 2
@@ -1488,25 +1541,26 @@
             # plt.ylabel(key)
             plt.title(key)
             plt.show()
 
     return dic, LOG
 
 
-def KS(X, y, show=False, max_plot_num=5):
+def KS(X, y, verbose = True, show=False, max_plot_num=5):
     """
     Performa feature-wise KS test.
 
     y - Because it is two-sample KS test, only support 2 classes
     """
 
     if (len(set(y)) != 2):
-        raise Exception(
-            'The dataset must have two classes. If you have more than 2 classes, use OVR (one-vs-rest) strategy.')
-
+        if verbose:
+            print('The dataset must have two classes for KS test.')
+        return None, None, None
+    
     ps = []
     Ds = []
     IMG = ''
     cnt = 0
 
     for i in range(X.shape[1]):
         Xi = X[:, i]
@@ -1667,119 +1721,136 @@
     if os.path.isfile(fn) == False:
         return 'File ' + fn + ' does not exist.'
 
     X, y = load_file(fn)
     return get_html(X, y)
 
 
-def get_metrics(X, y):
+def get_metrics(X, y, verbose = True):
     '''
     Addionally, we can do a PCA for high-dim data to get X beforehand.   
     We assume the covariance matrix is diagnal, i.e.   
 
     $\Sigma = \begin{bmatrix} \sigma^2_1 & 0 \\ 0 & \sigma^2_2 \end{bmatrix}  $
 
     This means x1 and x2 are linearly uncorrelated.   
     If we plot two PCs from PCA，the PCs will also be linearly uncorrelated, because they are the projections on two different orthogonal eigenvectors. 
     '''
 
-    dic, _, _ = CLF(X, y)
+    is_binary = len(np.unique(y)) == 2
+
+    dic, _, _ = CLF(X, y, verbose = verbose)
     if dic is None:
         dic = {}
 
-    ber = 1  # set maximum BER
-    try:
-        ber, _ = BER(X, y)
-    except Exception as e:
-        print('Exception in GaussianNB.', e)
-    dic['classification.BER'] = ber
+    if is_binary:
+
+        ber = 1  # set maximum BER
+        try:
+            ber, _ = BER(X, y)
+        except Exception as e:
+            print('Exception in GaussianNB.', e)
+        dic['classification.BER'] = ber
 
     svm_width, _ = SVM_Margin_Width(X, y)
     dic['classification.SVM.Margin'] = svm_width
 
     ig, _ = IG(X, y)
     if ig is not None:
         dic['correlation.IG'] = ig
         dic['correlation.IG.max'] = ig.max()
 
-    dic_cor, _ = correlate(X, y)
-    dic.update(dic_cor)
 
-    es, _ = cohen_d(X, y)
-    dic['test.ES'] = es
-    dic['test.ES.max'] = es.max()
-
-    p, T, _ = T_IND(X, y)
-    dic['test.student'] = p
-    dic['test.student.min'] = np.min(p)
-    dic['test.student.min.log10'] = np.log10(np.min(p))
-    dic['test.student.T'] = T
-    dic['test.student.T.max'] = np.max(T)
+    if is_binary:
+
+        dic_cor, _ = correlate(X, y, verbose = verbose)  # in case of multi-class, y is not a regression target but a class label. 
+        dic.update(dic_cor)
+
+        es, _ = cohen_d(X, y)
+        dic['test.ES'] = es
+        dic['test.ES.max'] = es.max()
+
+        p, T, _ = T_IND(X, y, verbose)
+        if p is not None:
+            dic['test.student'] = p
+            dic['test.student.min'] = np.min(p)
+            dic['test.student.min.log10'] = np.log10(np.min(p))
+        if T is not None:
+            dic['test.student.T'] = T
+            dic['test.student.T.max'] = np.max(T)
 
-    p, F, _ = ANOVA(X, y)
+    p, F, _ = ANOVA(X, y, verbose)
     dic['test.ANOVA'] = p
     dic['test.ANOVA.min'] = np.min(p)
     dic['test.ANOVA.min.log10'] = np.log10(np.min(p))
     dic['test.ANOVA.F'] = F
     dic['test.ANOVA.F.max'] = np.max(F)
 
-    p, F, log = MANOVA(X, y)
+    p, F, log = MANOVA(X, y, verbose)
     if log == 'Exception in MANOVA':
         pass
     else:
         dic['test.MANOVA'] = p
         dic['test.MANOVA.log10'] = np.log10(p)
         dic['test.MANOVA.F'] = F
 
-    p, U, _ = MWW(X, y)
-    dic['test.MWW'] = p
-    dic['test.MWW.min'] = np.min(p)
-    dic['test.MWW.min.log10'] = np.log10(np.min(p))
-    dic['test.MWW.U'] = U
-    dic['test.MWW.U.min'] = np.min(U)
-
-    p, D, _ = KS(X, y)
-    dic['test.KS'] = p
-    dic['test.KS.min'] = np.min(p)
-    dic['test.KS.min.log10'] = np.log10(np.min(p))
-    dic['test.KS.D'] = D
-    dic['test.KS.D.max'] = np.max(D)
+    if is_binary:
+
+        p, U, _ = MWW(X, y, verbose)
+        if p is not None:
+            dic['test.MWW'] = p
+            dic['test.MWW.min'] = np.min(p)
+            dic['test.MWW.min.log10'] = np.log10(np.min(p))
+        if U is not None:
+            dic['test.MWW.U'] = U
+            dic['test.MWW.U.min'] = np.min(U)
+
+        p, D, _ = KS(X, y)
+        if p is not None:
+            dic['test.KS'] = p
+            dic['test.KS.min'] = np.min(p)
+            dic['test.KS.min.log10'] = np.log10(np.min(p))
+        if D is not None:
+            dic['test.KS.D'] = D
+            dic['test.KS.D.max'] = np.max(D)
 
     p, C, _ = CHISQ(X, y)
     dic['test.CHISQ'] = p
     dic['test.CHISQ.min'] = np.min(p)
     dic['test.CHISQ.min.log10'] = np.log10(np.min(p))
     dic['test.CHISQ.CHI2'] = C
     dic['test.CHISQ.CHI2.max'] = np.max(C)
 
     # H follows chi2, its critical value of chi2(k-1) at 0.5
     H = [scipy.stats.chi2.ppf(.5, len(set(y))-1)] * X.shape[1]
     p = [.5] * X.shape[1]
     try:
-        p, H = KW(X, y)
+        p, H = KW(X, y, verbose)
     except Exception as e:
         print('KW Exception: ', e)
     dic['test.KW'] = p
     dic['test.KW.min'] = np.min(p)
     dic['test.KW.min.log10'] = np.log10(np.min(p))
     dic['test.KW.H'] = H
     dic['test.KW.H.max'] = np.max(H)
 
-    # T follows chi2, its critical value of chi2(k-1) at 0.5
-    T = [scipy.stats.chi2.ppf(.5, len(set(y))-1)] * X.shape[1]
-    p = [.5] * X.shape[1]
-    try:
-        p, T, _ = MedianTest(X, y)
-    except Exception as e:
-        print('MedianTest Exception: ', e)
-    dic['test.Median'] = p
-    dic['test.Median.min'] = np.min(p)
-    dic['test.Median.min.log10'] = np.log10(np.min(p))
-    dic['test.Median.CHI2'] = T
-    dic['test.Median.CHI2.max'] = np.max(T)
+    if is_binary:
+
+        # T follows chi2, its critical value of chi2(k-1) at 0.5
+        T = [scipy.stats.chi2.ppf(.5, len(set(y))-1)] * X.shape[1]
+        p = [.5] * X.shape[1]
+        try:
+            p, T, _ = MedianTest(X, y, verbose)
+        except Exception as e:
+            print('MedianTest Exception: ', e)
+        dic['test.Median'] = p
+        dic['test.Median.min'] = np.min(p)
+        dic['test.Median.min.log10'] = np.log10(np.min(p))
+        dic['test.Median.CHI2'] = T
+        dic['test.Median.CHI2.max'] = np.max(T)
 
     if ENABLE_R:
         try:
             dic_ecol, _ = ECoL_metrics(X, y)
             dic.update(dic_ecol)
         except Exception as e:
             print(e)
@@ -1793,15 +1864,15 @@
             dic_s[k] = v
 
     return dic, dic_s
 
 
 def metrics_keys():
     X, y = mvg(md=2, nobs=10)
-    dic = get_metrics(X, y)
+    dic = get_metrics(X, y, verbose = False)
     return list(dic[0].keys())
 
 
 # Defines how each metric's polarity, i.e., how to compare each metric.
 #   np.nanargmax - the metric and classifiability are positively correlated
 #   np.nanargmin - the metric and classifiability are negatively correlated
 metric_polarity_dict = {
@@ -1881,34 +1952,39 @@
     'neighborhood.LSC': np.nanargmax,
     'linearity.L1.mean': np.nanargmin,
     # 'linearity.L1.sd':np.nanargmin
 }
 
 
 def get_json(X, y):
-    return json.dumps(get_metrics(X, y))
+    return json.dumps(get_metrics(X, y, verbose = False))
 
 
 def get_html(X, y):
     '''
     Generate a summary report in HTML format
     '''
+
+    is_binary = len(np.unique(y)) == 2
+
     html = '<table class="table table-striped">'
 
     tr = '<tr><th> Metric/Statistic </th><tr>'  # <th> Value </th><th> Details </th>
     html += tr
 
-    try:
-        ber, ber_img = BER(X, y, show=False)
+    if is_binary:
 
-        # tr = '<tr><td> BER </td><td>' + str(ber) + '</td><td>' + ber_img + '</td><tr>'
-        tr = '<tr><td> BER = ' + str(ber) + '<br/>' + ber_img + '</td><tr>'
-        html += tr
-    except:
-        print('Exception in GaussianNB.')
+        try:
+            ber, ber_img = BER(X, y, show=False)
+
+            # tr = '<tr><td> BER </td><td>' + str(ber) + '</td><td>' + ber_img + '</td><tr>'
+            tr = '<tr><td> BER = ' + str(ber) + '<br/>' + ber_img + '</td><tr>'
+            html += tr
+        except Exception as e:
+            print('Exception in GaussianNB.', e)
 
     svm_margin, svm_margin_img = SVM_Margin_Width(X, y, show=False)
 
     tr = '<tr><td> SVM Margin Width = ' + \
         str(svm_margin) + '<br/>' + svm_margin_img + '</td><tr>'
     html += tr
 
@@ -1920,15 +1996,15 @@
     html += tr
 
     ig, ig_img = IG(X, y, show=False)
 
     tr = '<tr><td> IG = ' + str(ig) + '<br/>' + ig_img + '</td><tr>'
     html += tr
 
-    _, corr_log = correlate(X, y, verbose=False)
+    _, corr_log = correlate(X, y, verbose)
     tr = '<tr><td><pre>' + corr_log + '</pre></td><tr>'
     html += tr
 
     t_p, _, t_img = T_IND(X, y)
 
     tr = '<tr><td> Independent t-test p' + \
         str(t_p) + '<br/>' + t_img + '</td><tr>'
@@ -2189,7 +2265,88 @@
     plt.title('loadings / coefficients')
     plt.xticks(rotation=90)
     plt.show()
 
     print("1st PC: ", PCs[:, 0])
 
     return pca
+
+def run_multiclass_clfs(X, y, split = .3, show = True):
+    '''
+
+    原生支持多分类的模型：
+
+    naive_bayes.BernoulliNB (only for binary features)
+    tree.DecisionTreeClassifier
+    ensemble.ExtraTreesClassifier (only in ensembles)
+    naive_bayes.GaussianNB
+    neighbors.KNeighborsClassifier
+    discriminant_analysis.LinearDiscriminantAnalysis
+    svm.LinearSVC (multi_class=”crammer_singer”)
+    linear_model.LogisticRegression(CV) (multi_class=”multinomial”)
+    neural_network.MLPClassifier
+    neighbors.NearestCentroid
+    ensemble.RandomForestClassifier
+    '''
+
+    matplotlib.rcParams.update({'font.size': 17})
+
+    n_classes = len(np.unique(y))
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=split, random_state = 2, stratify=y)
+
+    html_str = ''
+    for clf in [GaussianNB(), DecisionTreeClassifier(), RandomForestClassifier(n_estimators=max(10, n_classes)), 
+                LinearSVC(multi_class="crammer_singer"), LogisticRegressionCV (multi_class="multinomial", max_iter=1000), 
+                MLPClassifier(hidden_layer_sizes=(max(n_classes, X.shape[1]),)), 
+                KNeighborsClassifier(n_neighbors=max(5, n_classes)), 
+                NearestCentroid(), LinearDiscriminantAnalysis()]:
+        
+        html_str += '<h4>' + str(clf) + '</h4>'
+        if show:
+            IPython.display.display(IPython.display.HTML('<h3>' + str(clf) + '</h3>'))
+                                
+        clf.fit(X_train, y_train)   
+        y_pred = clf.predict(X_test) 
+        
+        # y_score = OneHotEncoder(categories = list( range(len(np.unique(y)))) ).fit_transform(y_pred.reshape(-1, 1))
+        y_score = np.eye(n_classes)[y_pred] # one-hot encoding
+        if hasattr(clf, 'predict_proba') and callable(clf.predict_proba):
+            y_score = clf.predict_proba(X_test)        
+
+        report = '<br/><pre>' + str(classification_report(y_test, y_pred)) + '</pre>'
+        if len(np.unique(y)) >= 8:
+            report += '<p>top-3 acc = ' + str(round( top_k_accuracy_score(y_test, y_score, k=3),3)) + '</p>'
+            report += '<p>top-5 acc = ' + str(round( top_k_accuracy_score(y_test, y_score, k=5),3)) + '</p>'
+
+        if show:
+            IPython.display.display(IPython.display.HTML(report)) 
+        html_str += report
+
+        n_classes = len(np.unique(y))
+        _, ax = plt.subplots(1, 2, figsize=(6 + n_classes, 3 + round(n_classes/2))) # gridspec_kw={'width_ratios': [6, 3 + n_classes, 3 + n_classes]})
+
+        # ax[0].set_title('classification report\n')
+        #ax[0].text(0.1, 0, classification_report(y_test, y_pred), 
+        #           fontsize = 18, horizontalalignment='right', verticalalignment='top')
+        #ax[0].axis('off')
+
+        # ax[1].set_title('confusion matrix\n')
+        plot_confusion_matrix(y_test, y_pred, normalize=False, ax=ax[0], cax = None) # cax = ax[2]
+ 
+        # ax[2].set_title('confusion matrix \n(normalized)')
+        plot_confusion_matrix(y_test, y_pred, normalize=True, ax=ax[1], cax = None) # cax = ax[4]
+        
+        # plt.tight_layout()
+        html_str += plt2html(plt)
+
+        if show:
+            plt.show()
+        else:
+            plt.close()
+
+        html_str = html_str + '<br/>'
+        if show:
+            IPython.display.display(IPython.display.HTML('<br/>'))
+
+    matplotlib.rcParams.update({'font.size': 12})
+    
+    return html_str
```

### Comparing `cla-1.1.6/cla/unify.py` & `cla-1.1.7/cla/unify.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/vis/feature_importance.py` & `cla-1.1.7/cla/vis/feature_importance.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/vis/plotComponents1D.py` & `cla-1.1.7/cla/vis/plotComponents1D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/vis/plotComponents2D.py` & `cla-1.1.7/cla/vis/plotComponents2D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/vis/plotComponents3D.py` & `cla-1.1.7/cla/vis/plotComponents3D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/cla/vis/unsupervised_dimension_reductions.py` & `cla-1.1.7/cla/vis/unsupervised_dimension_reductions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from plotComponents1D import plotComponents1D
 
 def unsupervised_dimension_reductions(X, y, labels=None):
 
     # %matplotlib notebook
 
     if X is None or X.shape[1] < 1:
-        print('ERROR: X HAS NO FEATURE/COLUMN!')
+        print('Error: X has NO features!')
         return
 
     if labels is None:
         labels = list(set(y))
 
     fig = plt.figure(figsize=(18, 10))
     # plt.title("", fontsize=14)
```

### Comparing `cla-1.1.6/cla.egg-info/PKG-INFO` & `cla-1.1.7/cla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.1.6
+Version: 1.1.7
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.1.6 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.1.7 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.1.6/cla.egg-info/SOURCES.txt` & `cla-1.1.7/cla.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 cla/gui/static/jquery-3.3.1.min.js
 cla/gui/static/jquery.blockUI.js
 cla/gui/static/jquery.form.min.js
 cla/gui/static/sample.csv
 cla/gui/templates/__init__.py
 cla/gui/templates/home.html
 cla/vis/__init__.py
+cla/vis/confusion_matrix.py
 cla/vis/feature_importance.py
 cla/vis/plotComponents1D.py
 cla/vis/plotComponents2D.py
 cla/vis/plotComponents3D.py
 cla/vis/plt2base64.py
 cla/vis/unsupervised_dimension_reductions.py
 data/sample.csv
```

### Comparing `cla-1.1.6/data/sample.csv` & `cla-1.1.7/data/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.6/setup.py` & `cla-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 setup(
     # Application name:
     name="cla",
     
     # Version number (initial):
-    version="1.1.6",
+    version="1.1.7",
     
     # Application author details:
     author="Zhang",
     author_email="oo@zju.edu.cn",
     
     # Packages
     packages=["cla", "cla.vis", "cla.gui", "cla.gui.templates", "cla.gui.static"],
```

