# Comparing `tmp/InterpretME-1.2.2.tar.gz` & `tmp/InterpretME-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InterpretME-1.2.2.tar", last modified: Sat Mar 11 11:44:38 2023, max compression
+gzip compressed data, was "InterpretME-1.3.0.tar", last modified: Thu Jun 29 14:03:00 2023, max compression
```

## Comparing `InterpretME-1.2.2.tar` & `InterpretME-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:44:38.359378 InterpretME-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:44:38.355378 InterpretME-1.2.2/InterpretME/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    79475 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/dtreeviz_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/federated_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:44:38.359378 InterpretME-1.2.2/InterpretME/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/classes.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/cross_validation.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/definition_feature.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/endpoint.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/entity_alignment.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/imp_features.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/lime_features.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/model_details.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/precision_recall.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/prediction_probabilities.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/sampling_strategy.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/mappings/shacl_validation_results.ttl
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/preprocessing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/sampling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/semantification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/shacl_api_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-11 11:44:26.000000 InterpretME-1.2.2/InterpretME/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 11:44:38.355378 InterpretME-1.2.2/InterpretME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-03-11 11:44:38.000000 InterpretME-1.2.2/InterpretME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-11 11:44:38.000000 InterpretME-1.2.2/InterpretME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 11:44:38.000000 InterpretME-1.2.2/InterpretME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-11 11:44:38.000000 InterpretME-1.2.2/InterpretME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-11 11:44:38.000000 InterpretME-1.2.2/InterpretME.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-03-11 11:44:26.000000 InterpretME-1.2.2/LIBRARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-11 11:44:26.000000 InterpretME-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-11 11:44:26.000000 InterpretME-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-03-11 11:44:38.359378 InterpretME-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-03-11 11:44:26.000000 InterpretME-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 11:44:38.359378 InterpretME-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-11 11:44:26.000000 InterpretME-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:03:00.360753 InterpretME-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:03:00.356753 InterpretME-1.3.0/InterpretME/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78080 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/dtreeviz_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/federated_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:03:00.360753 InterpretME-1.3.0/InterpretME/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/classes.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/cross_validation.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/definition_feature.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/endpoint.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/entity_alignment.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/imp_features.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/lime_features.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/model_details.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/precision_recall.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/prediction_probabilities.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/sampling_strategy.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/mappings/shacl_validation_results.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/preprocessing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/sampling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/semantification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/shacl_api_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-29 14:02:47.000000 InterpretME-1.3.0/InterpretME/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:03:00.356753 InterpretME-1.3.0/InterpretME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-29 14:03:00.000000 InterpretME-1.3.0/InterpretME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-29 14:03:00.000000 InterpretME-1.3.0/InterpretME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:03:00.000000 InterpretME-1.3.0/InterpretME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-29 14:03:00.000000 InterpretME-1.3.0/InterpretME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 14:03:00.000000 InterpretME-1.3.0/InterpretME.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-29 14:02:47.000000 InterpretME-1.3.0/LIBRARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-29 14:02:47.000000 InterpretME-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 14:02:47.000000 InterpretME-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-29 14:03:00.360753 InterpretME-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-29 14:02:47.000000 InterpretME-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:03:00.360753 InterpretME-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-29 14:02:47.000000 InterpretME-1.3.0/setup.py
```

### Comparing `InterpretME-1.2.2/InterpretME/classification.py` & `InterpretME-1.3.0/InterpretME/classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
-import optuna
+
 import lime
 import lime.lime_tabular
 import numpy as np
+import optuna
 import pandas as pd
 import sklearn
 import validating_models.stats as stats
 from sklearn import tree
 from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier
 from sklearn.metrics import classification_report
 from sklearn.model_selection import StratifiedShuffleSplit
 from sklearn.model_selection import train_test_split
 from slugify import slugify
 
+import InterpretME.utils as utils
 from . import dtreeviz_lib
 
+optuna.logging.set_verbosity(optuna.logging.ERROR)
+
 
 class AutoMLOptuna(object):
     def __init__(self, min_max_depth, max_max_depth, X, y):
         self.min_max_depth = min_max_depth
         self.max_max_depth = max_max_depth
         self.X = X
         self.y = y
@@ -41,31 +45,18 @@
                                                          min_weight_fraction_leaf=dt_min_weight_fraction_leaf,
                                                          ccp_alpha=dt_ccp_alpha)
 
         score = sklearn.model_selection.cross_val_score(classifier_obj, self.X, self.y, n_jobs=-1, cv=3)
         return score.mean()
 
 
-def is_notebook() -> bool:
-    try:
-        shell = get_ipython().__class__.__name__
-        if shell == 'ZMQInteractiveShell':
-            return True  # Jupyter notebook or qtconsole
-        elif shell == 'TerminalInteractiveShell':
-            return False  # Terminal running IPython
-        else:
-            return False  # Other type (?)
-    except NameError:
-        return False  # Probably standard Python interpreter
-
+class AdvanceProgressBarCallback:
+    def __call__(self, study: optuna.study.Study, trial: optuna.trial.FrozenTrial) -> None:
+        utils.pbar.update(1)
 
-if is_notebook():
-    from tqdm import tqdm_notebook as tqdm
-else:
-    from tqdm import tqdm
 
 os.environ["PATH"] += os.pathsep + 'C:/Program Files (x86)/Graphviz2.38/bin/'
 
 time_lime = stats.get_decorator('PIPE_LIME')
 time_output = stats.get_decorator('PIPE_OUTPUT')
 
 
@@ -174,39 +165,32 @@
         discretize_continuous=True,
         random_state=123
     )
 
     lst = []
     lst_prob = []
 
-    if lime_results is None:
-        print("###############################################################################")
-        print("********* LIME results will not be saved as the path is not specified *********")
-        print("###############################################################################")
-    else:
+    if lime_results is not None:
         if not os.path.exists(lime_results):
-            os.makedirs(lime_results)
-        print("#############################################################")
-        print("***************** Saving LIME results ***********************")
-        print("#############################################################")
-        with tqdm(total=min(len(ind_test), len(X_test))) as pbar:
-            for i, j in zip(ind_test, X_test):
-                explainer.explain_instance(j, best_clf.predict_proba, num_features=10).save_to_file(
-                    lime_results + '/Lime_' + slugify(str(i)) + '.html'
-                )
-                pbar.update(1)
+            os.makedirs(lime_results, exist_ok=True)
 
+    utils.pbar.total += min(len(ind_test), len(X_test))
+    utils.pbar.update(0)
+    utils.pbar.set_description('LIME explanations', refresh=True)
     for i, j in zip(ind_test, X_test):
         exp = explainer.explain_instance(j, best_clf.predict_proba, num_features=10)
+        if lime_results is not None:
+            exp.save_to_file(lime_results + '/Lime_' + slugify(str(i)) + '.html')
         df = pd.DataFrame(exp.as_list())
         df['index'] = i
         lst.append(df)
         df2 = pd.DataFrame(exp.predict_proba.tolist())
         df2['index'] = i
         lst_prob.append(df2)
+        utils.pbar.update(1)
 
     df1 = pd.concat(lst)
     df1.loc[:, 'run_id'] = st
     df1 = df1.set_index('index')
     df1.rename(columns={df1.columns[0]: "features", df1.columns[1]: "weights"}, inplace=True)
     df1['tool'] = 'LIME'
     df1.to_csv("interpretme/files/lime_interpretation_features.csv")
@@ -258,34 +242,31 @@
     y = sampled_target['class']
 
     X_input, y_input = X.values, y.values
     with stats.measure_time('PIPE_IMPORTANT_FEATURES'):
         # print("---------------- Random Forest Classification with Stratified shuffle split -----------------------")
         # print(model)
         if model == 'Random Forest':
-            print('Random Forest Classifier')
+            # print('Random Forest Classifier')
             estimator = RandomForestClassifier(max_depth=4, random_state=0)
         elif model == 'AdaBoost':
-            print('AdaBoost Classifier')
+            # print('AdaBoost Classifier')
             estimator = AdaBoostClassifier(random_state=0)
         elif model == 'Gradient Boosting':
-            print('Gradient Boosting Classifier')
+            # print('Gradient Boosting Classifier')
             estimator = GradientBoostingClassifier(random_state=0)
 
         cv = StratifiedShuffleSplit(n_splits=cross_validation, test_size=test_split, random_state=123)
         important_features = set()
         important_features_size = imp_features
-        print("###########################################################################")
-        print("************** Classification report for every iteration ******************")
-        print("###########################################################################")
+
+        # Classification report for every iteration
         for i, (train, test) in enumerate(cv.split(X_input, y_input)):
             estimator.fit(X_input[train], y_input[train])
-            y_predicted = estimator.predict(X_input[test])
-
-            print(classification_report(y_input[test], y_predicted))
+            y_predicted = estimator.predict(X_input[test])  # TODO: Is it necessary to do the prediction here if nothing happens with the prediction?
 
             fea_importance = estimator.feature_importances_
             indices = np.argsort(fea_importance)[::-1]
             for f in range(important_features_size):
                 important_features.add(X.columns.values[indices[f]])
 
     data = plot_feature_importance(estimator.feature_importances_, X.columns)
@@ -297,19 +278,21 @@
     # print(indices)
     X_train, X_test, y_train, y_test, ind_train, ind_test = train_test_split(
         new_sampled_data.values, sampled_target['class'].values, indices, random_state=123
     )
 
     feature_names = new_sampled_data.columns
 
+    utils.pbar.total += 100
+    utils.pbar.set_description('Model Training', refresh=True)
     with stats.measure_time('PIPE_TRAIN_MODEL'):
         # Hyperparameter Optimization using AutoML
         study = optuna.create_study(direction="maximize")
         automl_optuna = AutoMLOptuna(min_max_depth, max_max_depth, X_train, y_train)
-        study.optimize(automl_optuna, n_trials=100)
+        study.optimize(automl_optuna, n_trials=100, callbacks=[AdvanceProgressBarCallback()])
         # print(study.best_value)
         # print(study.best_params)
         params = study.best_params
         del params['classifier']
         best_clf = tree.DecisionTreeClassifier(**params)
         best_clf.fit(X_train, y_train)
 
@@ -335,47 +318,45 @@
         res.loc[:, 'model'] = model_name
         res.loc[:, 'accuracy'] = acc
         res = res.set_index('run_id')
         res.to_csv('interpretme/files/model_accuracy_hyperparameters.csv')
 
     lime_interpretation(X_train, new_sampled_data, best_clf, ind_test, X_test, classes, st, lime_results)
 
+    # Saving the classification report
     with stats.measure_time('PIPE_OUTPUT'):
-        print("#########################################################################################")
-        print("****************** Classification report saved in output folder *************************")
-        print("#########################################################################################")
-
         report = classification_report(y_test, y_pred, target_names=classes, output_dict=True)
         classificationreport = pd.DataFrame(report).transpose()
         classificationreport.loc[:, 'run_id'] = st
         classificationreport = classificationreport.reset_index()
         classificationreport = classificationreport.rename(columns={classificationreport.columns[0]: 'classes'})
-        print(classificationreport)
+        # print(classificationreport)
         report = classificationreport.iloc[:-3, :]
         # print(report)
         report.to_csv("interpretme/files/precision_recall.csv", index=False)
 
+    utils.pbar.set_description('Preparing Plots Data', refresh=True)
     with stats.measure_time('PIPE_DTREEVIZ'):
         bool_feature = []
         for feature in new_sampled_data.columns:
             values = new_sampled_data[feature].unique()
             if len(values) == 2:
                 values = sorted(values)
                 if values[0] == 0 and values[1] == 1:
                     bool_feature.append(feature)
 
         viz = dtreeviz_lib.dtreeviz(best_clf, new_sampled_data, sampled_target['class'], target_name='class',
                                     feature_names=feature_names, class_names=classes, fancy=True,
                                     show_root_edge_labels=True, bool_feature=bool_feature)
         results['dtree'] = viz
+    utils.pbar.update(1)
 
     return new_sampled_data, best_clf, results
 
 
-
 def multiclass(sampled_data, sampled_target, imp_features, cv, classes,
                st, lime_results, test_split, model, results, min_max_depth, max_max_depth):
     """Multiclass classification technique
 
     Parameters
     ----------
     sampled_data : dataframe
@@ -409,34 +390,31 @@
     X = sampled_data
     y = sampled_target['class']
 
     X_input, y_input = X.values, y.values
     with stats.measure_time('PIPE_IMPORTANT_FEATURES'):
         # print("---------------- Random Forest Classification with Stratified shuffle split -----------------------")
         if model == 'Random Forest':
-            print('Random Forest Classifier')
+            # print('Random Forest Classifier')
             estimator = RandomForestClassifier(max_depth=4, random_state=0)
         elif model == 'AdaBoost':
-            print('AdaBoost Classifier')
+            # print('AdaBoost Classifier')
             estimator = AdaBoostClassifier(random_state=0)
         elif model == 'Gradient Boosting':
-            print('Gradient Boosting Classifier')
+            # print('Gradient Boosting Classifier')
             estimator = GradientBoostingClassifier(random_state=0)
 
         cv = StratifiedShuffleSplit(n_splits=cv, test_size=test_split, random_state=123)
         important_features = set()
         important_features_size = imp_features
-        print("#################################################################################")
-        print("************** Classification report for every iteration ************************")
-        print("#################################################################################")
+
+        # Classification report for every iteration
         for i, (train, test) in enumerate(cv.split(X_input, y_input)):
             estimator.fit(X_input[train], y_input[train])
-            y_predicted = estimator.predict(X_input[test])
-
-            print(classification_report(y_input[test], y_predicted))
+            y_predicted = estimator.predict(X_input[test])  # TODO: Is it necessary to do the prediction here if nothing happens with the prediction?
 
             fea_importance = estimator.feature_importances_
             indices = np.argsort(fea_importance)[::-1]
             for f in range(important_features_size):
                 important_features.add(X.columns.values[indices[f]])
 
     data = plot_feature_importance(estimator.feature_importances_, X.columns)
@@ -490,25 +468,22 @@
         if not os.path.isfile('interpretme/files/model_accuracy_hyperparameters.csv'):
             res.to_csv('interpretme/files/model_accuracy_hyperparameters.csv')
         else:
             res.to_csv('interpretme/files/model_accuracy_hyperparameters.csv', mode='a', header=False)
 
     lime_interpretation(X_train, new_sampled_data, best_clf, ind_test, X_test, classes, st, lime_results)
 
+    # Saving the classification report
     with stats.measure_time('PIPE_OUTPUT'):
-        print("#########################################################################################")
-        print("****************** Classification report saved in output folder *************************")
-        print("#########################################################################################")
-
         report = classification_report(y_test, y_pred, target_names=classes, output_dict=True)
         classificationreport = pd.DataFrame(report).transpose()
         classificationreport.loc[:, 'run_id'] = st
         classificationreport = classificationreport.reset_index()
         classificationreport = classificationreport.rename(columns={classificationreport.columns[0]: 'classes'})
-        print(classificationreport)
+        # print(classificationreport)
         report = classificationreport.iloc[:-3, :]
         report.to_csv("interpretme/files/precision_recall.csv", index=False)
 
     with stats.measure_time('PIPE_DTREEVIZ'):
         bool_feature = []
         for feature in new_sampled_data.columns:
             values = new_sampled_data[feature].unique()
```

### Comparing `InterpretME-1.2.2/InterpretME/dtreeviz_lib.py` & `InterpretME-1.3.0/InterpretME/dtreeviz_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
 import tempfile
+from numbers import Number
 from pathlib import Path
 from sys import platform as PLATFORM
+from typing import Mapping, List
 
-import numpy as np
-import pandas as pd
+import graphviz
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 from colour import Color, rgb2hex
-import graphviz
-from sklearn import tree
-from typing import Mapping, List
-from numbers import Number
-
 from dtreeviz import interpretation as prediction_path
 from dtreeviz.colors import adjust_colors
 from dtreeviz.models.shadow_decision_tree import ShadowDecTree
 from dtreeviz.models.shadow_decision_tree import ShadowDecTreeNode
 from dtreeviz.utils import inline_svg_images, myround, scale_SVG
+from sklearn import tree
 
 # How many bins should we have based upon number of classes
 NUM_BINS = [0, 0, 10, 9, 8, 6, 6, 6, 5, 5, 5]
 
 
 class DTreeViz:
     def __init__(self, dot, scale=1.0):
@@ -98,16 +97,16 @@
                     split_linewidth=.5,
                     mean_linewidth=2,
                     markersize=15,
                     colors=None):
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, y_data, feature_names, target_name, None, tree_index
     )
-    x_data = shadow_tree.x_data.reshape(-1, )
-    y_data = shadow_tree.y_data
+    x_data = shadow_tree.X_train.reshape(-1, )
+    y_data = shadow_tree.y_train
 
     # ax as first arg is not good now that it's optional but left for compatibility reasons
     if ax is None:
         fig, ax = plt.subplots(1, 1)
 
     if x_data is None or y_data is None:
         raise ValueError(f"x_train and y_train must not be none")
@@ -158,15 +157,15 @@
 def rtreeviz_bivar_heatmap(tree_model,
                            x_data: (pd.DataFrame, np.ndarray) = None,  # dataframe with only one column
                            y_data: (pd.Series, np.ndarray) = None,
                            feature_names: List[str] = None,
                            target_name: str = None,
                            tree_index: int = None,  # required in case of tree ensemble
                            ax=None,
-                           fontsize=14, ticks_fontsize=12, fontname="Arial",
+                           fontsize=14, ticks_fontsize=12,
                            show={'title'},
                            n_colors_in_map=100,
                            colors=None,
                            markersize=15
                            ) -> tree.DecisionTreeClassifier:
     """
     Show tessellated 2D feature space for bivariate regression tree. X_train can
@@ -174,16 +173,16 @@
     """
     if ax is None:
         fig, ax = plt.subplots(1, 1)
 
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, y_data, feature_names, target_name, None, tree_index
     )
-    x_data = shadow_tree.x_data
-    y_data = shadow_tree.y_data
+    x_data = shadow_tree.X_train
+    y_data = shadow_tree.y_train
 
     colors = adjust_colors(colors)
 
     y_lim = np.min(y_data), np.max(y_data)
     y_range = y_lim[1] - y_lim[0]
     color_map = [rgb2hex(c.rgb, force_long=True) for c in
                  Color(colors['color_map_min']).range_to(Color(colors['color_map_max']), n_colors_in_map)]
@@ -200,16 +199,16 @@
                                  edgecolor=colors['edge'], facecolor=color)
         ax.add_patch(rect)
 
     color_map = [color_map[int(((y - y_lim[0]) / y_range) * (n_colors_in_map - 1))] for y in y_data]
     x, y, z = x_data[:, 0], x_data[:, 1], y_data
     ax.scatter(x, y, marker='o', c=color_map, edgecolor=colors['scatter_edge'], lw=.3, s=markersize)
 
-    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, color=colors['axis_label'])
+    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, color=colors['axis_label'])
 
     ax.tick_params(axis='both', which='major', width=.3, labelcolor=colors['tick_label'], labelsize=ticks_fontsize)
 
     if 'title' in show:
         accur = shadow_tree.get_score()
         title = f"Regression tree depth {shadow_tree.get_max_depth()}, training $R^2$={accur:.3f}"
         ax.set_title(title, fontsize=fontsize, color=colors['title'])
@@ -221,30 +220,30 @@
                       x_data: (pd.DataFrame, np.ndarray) = None,  # dataframe with only one column
                       y_data: (pd.Series, np.ndarray) = None,
                       feature_names: List[str] = None,
                       target_name: str = None,
                       class_names: (Mapping[Number, str], List[str]) = None,  # required if classifier,
                       tree_index: int = None,  # required in case of tree ensemble
                       ax=None,
-                      fontsize=14, ticks_fontsize=10, fontname="Arial",
+                      fontsize=14, ticks_fontsize=10,
                       azim=0, elev=0, dist=7,
                       show={'title'},
                       colors=None,
                       markersize=15,
                       n_colors_in_map=100
                       ) -> tree.DecisionTreeClassifier:
     """
     Show 3D feature space for bivariate regression tree. X_train should have
     just the 2 variables used for training.
     """
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, y_data, feature_names, target_name, class_names, tree_index
     )
-    x_data = shadow_tree.x_data
-    y_data = shadow_tree.y_data
+    x_data = shadow_tree.X_train
+    y_data = shadow_tree.y_train
 
     if ax is None:
         fig = plt.figure()
         ax = fig.add_subplot(111, projection='3d')
     colors = adjust_colors(colors)
     ax.view_init(elev=elev, azim=azim)
     ax.dist = dist
@@ -271,17 +270,17 @@
     for node, bbox in tesselation:
         plane(node, bbox, color_spectrum)
 
     x, y, z = x_data[:, 0], x_data[:, 1], y_data
     ax.scatter(x, y, z, marker='o', alpha=colors['scatter_marker_alpha'], edgecolor=colors['scatter_edge'],
                lw=.3, c=y_colors, s=markersize)
 
-    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-    ax.set_zlabel(f"{shadow_tree.target_name}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, color=colors['axis_label'])
+    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, color=colors['axis_label'])
+    ax.set_zlabel(f"{shadow_tree.target_name}", fontsize=fontsize, color=colors['axis_label'])
 
     ax.tick_params(axis='both', which='major', width=.3, labelcolor=colors['tick_label'], labelsize=ticks_fontsize)
 
     if 'title' in show:
         accur = shadow_tree.get_score()
         title = f"Regression tree depth {shadow_tree.get_max_depth()}, training $R^2$={accur:.3f}"
         ax.set_title(title, fontsize=fontsize, color=colors['title'])
@@ -293,35 +292,34 @@
                     x_data: (pd.DataFrame, np.ndarray) = None,  # dataframe with only one column
                     y_data: (pd.Series, np.ndarray) = None,
                     feature_names: List[str] = None,
                     target_name: str = None,
                     class_names: (Mapping[Number, str], List[str]) = None,  # required if classifier,
                     tree_index: int = None,  # required in case of tree ensemble
                     ax=None,
-                    fontsize=14, fontname="Arial", nbins=25, gtype='strip',
+                    fontsize=14, nbins=25, gtype='strip',
                     show={'title', 'legend', 'splits'},
                     colors=None):
     if ax is None:
         fig, ax = plt.subplots(1, 1)
 
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, y_data, feature_names, target_name, class_names, tree_index
     )
-    x_data = shadow_tree.x_data.reshape(-1, )
-    y_data = shadow_tree.y_data
+    x_data = shadow_tree.X_train.reshape(-1, )
+    y_data = shadow_tree.y_train
     colors = adjust_colors(colors)
     n_classes = shadow_tree.nclasses()
     overall_feature_range = (np.min(x_data), np.max(x_data))
     class_values = shadow_tree.classes()
     color_values = colors['classes'][n_classes]
     color_map = {v: color_values[i] for i, v in enumerate(class_values)}
     X_colors = [color_map[cl] for cl in class_values]
 
-    ax.set_xlabel(f"{shadow_tree.feature_names}", fontsize=fontsize, fontname=fontname,
-                  color=colors['axis_label'])
+    ax.set_xlabel(f"{shadow_tree.feature_names}", fontsize=fontsize, color=colors['axis_label'])
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.yaxis.set_visible(False)
     ax.spines['left'].set_visible(False)
     ax.spines['bottom'].set_linewidth(.3)
 
     X_hist = [x_data[y_data == cl] for cl in class_values]
@@ -390,30 +388,29 @@
                    y_data: (pd.Series, np.ndarray) = None,
                    feature_names: List[str] = None,
                    target_name: str = None,
                    class_names: (Mapping[Number, str], List[str]) = None,  # required if classifier,
                    tree_index: int = None,  # required in case of tree ensemble
                    ax=None,
                    fontsize=14,
-                   fontname="Arial",
                    show={'title', 'legend', 'splits'},
                    colors=None):
     """
     Show tesselated 2D feature space for bivariate classification tree. X_train can
     have lots of features but features lists indexes of 2 features to train tree with.
     """
     # ax as first arg is not good now that it's optional but left for compatibility reasons
     if ax is None:
         fig, ax = plt.subplots(1, 1)
 
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, y_data, feature_names, target_name, class_names, tree_index
     )
-    x_data = shadow_tree.x_data
-    y_data = shadow_tree.y_data
+    x_data = shadow_tree.X_train
+    y_data = shadow_tree.y_train
     colors = adjust_colors(colors)
     tesselation = shadow_tree.tesselation()
     n_classes = shadow_tree.nclasses()
     class_values = shadow_tree.classes()
     color_values = colors['classes'][n_classes]
     color_map = {v: color_values[i] for i, v in enumerate(class_values)}
 
@@ -429,16 +426,16 @@
 
     dot_w = 25
     X_hist = [x_data[y_data == cl] for cl in class_values]
     for i, h in enumerate(X_hist):
         ax.scatter(h[:, 0], h[:, 1], marker='o', s=dot_w, c=color_map[i],
                    edgecolors=colors['scatter_edge'], lw=.3)
 
-    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(f"{shadow_tree.feature_names[0]}", fontsize=fontsize, color=colors['axis_label'])
+    ax.set_ylabel(f"{shadow_tree.feature_names[1]}", fontsize=fontsize, color=colors['axis_label'])
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.spines['bottom'].set_linewidth(.3)
 
     if 'legend' in show:
         add_classifier_legend(ax, shadow_tree.class_names, class_values, color_map, shadow_tree.target_name, colors)
 
@@ -493,15 +490,14 @@
              histtype: ('bar', 'barstacked', 'strip') = 'barstacked',
              highlight_path: List[int] = [],
              X: np.ndarray = None,
              max_X_features_LR: int = 10,
              max_X_features_TD: int = 20,
              label_fontsize: int = 16,
              ticks_fontsize: int = 12,
-             fontname: str = "Arial",
              colors: dict = None,
              scale=1.0,
              bool_feature=None) -> DTreeViz:
     """
     Given a decision tree regressor or classifier, create and return a tree visualization
     using the graphviz (DOT) language.
     We can call this function in two ways :
@@ -538,15 +534,14 @@
     :type highlight_path: List[int]
     :param X: Instance to run down the tree; derived path to highlight from this vector.
               Show feature vector with labels underneath leaf reached. highlight_path
               is ignored if X is not None.
     :type X: np.ndarray
     :param label_fontsize: Size of the label font
     :param ticks_fontsize: Size of the tick font
-    :param fontname: Font which is used for labels and text
     :param max_X_features_LR: If len(X) exceeds this limit for LR layout,
                             display only those features
                            used to guide X vector down tree. Helps when len(X) is large.
                            Default is 10.
     :param max_X_features_TD: If len(X) exceeds this limit for TD layout,
                             display only those features
                            used to guide X vector down tree. Helps when len(X) is large.
@@ -756,16 +751,16 @@
 
     # Fix the mapping from target value to color for entire tree
     if shadow_tree.is_classifier():
         class_values = shadow_tree.classes()
         color_map = {v: color_values[i] for i, v in enumerate(class_values)}
         draw_legend(shadow_tree, shadow_tree.target_name, f"{tmp}/legend_{os.getpid()}.svg", colors=colors)
 
-    X_data = shadow_tree.x_data
-    y_data = shadow_tree.y_data
+    X_data = shadow_tree.X_train
+    y_data = shadow_tree.y_train
     if isinstance(X_data, pd.DataFrame):
         X_data = X_data.values
     if isinstance(y_data, pd.Series):
         y_data = y_data.values
     if y_data.dtype == np.dtype(object):
         try:
             y_data = y_data.astype('float')
@@ -790,26 +785,24 @@
                                 precision=precision,
                                 colors={**color_map, **colors},
                                 histtype=histtype,
                                 node_heights=node_heights,
                                 X=X,
                                 ticks_fontsize=ticks_fontsize,
                                 label_fontsize=label_fontsize,
-                                fontname=fontname,
                                 highlight_node=node.id in highlight_path)
             else:
                 regr_split_viz(node, X_data, y_data,
                                filename=f"{tmp}/node{node.id}_{os.getpid()}.svg",
                                target_name=shadow_tree.target_name,
                                y_range=y_range,
                                precision=precision,
                                X=X,
                                ticks_fontsize=ticks_fontsize,
                                label_fontsize=label_fontsize,
-                               fontname=fontname,
                                highlight_node=node.id in highlight_path,
                                colors=colors)
 
         nname = node_name(node)
         bool_var = bool_feature
 
         feature_name_nsample = 'S=' + str(node.nsamples()) + '<br/>' + node.feature_name()
@@ -832,15 +825,14 @@
                           y_data,
                           target_name=shadow_tree.target_name,
                           filename=f"{tmp}/leaf{node.id}_{os.getpid()}.svg",
                           y_range=y_range,
                           precision=precision,
                           ticks_fontsize=ticks_fontsize,
                           label_fontsize=label_fontsize,
-                          fontname=fontname,
                           colors=colors)
             leaves.append(regr_leaf_node(node))
 
     if show_just_path:
         show_root_edge_labels = False
     show_edge_labels = True
     all_llabel = '&lt;' if show_edge_labels else ''
@@ -924,15 +916,14 @@
                     X_train: np.ndarray,
                     y_train: np.ndarray,
                     colors: dict,
                     node_heights,
                     filename: str = None,
                     ticks_fontsize: int = 8,
                     label_fontsize: int = 9,
-                    fontname: str = "Arial",
                     precision=1,
                     histtype: ('bar', 'barstacked', 'strip') = 'barstacked',
                     X: np.array = None,
                     highlight_node: bool = False
                     ):
     height_range = (.5, 1.5)
     h = prop_size(n=node_heights[node.id], counts=node_heights.values(), output_range=height_range)
@@ -948,15 +939,15 @@
     n_classes = node.shadow_tree.nclasses()
     nbins = get_num_bins(histtype, n_classes)
     overall_feature_range = (np.min(X_train[:, node.feature()]), np.max(X_train[:, node.feature()]))
 
     overall_feature_range_wide = (overall_feature_range[0] - overall_feature_range[0] * .08,
                                   overall_feature_range[1] + overall_feature_range[1] * .05)
 
-    ax.set_xlabel(f"{feature_name}", fontsize=label_fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(f"{feature_name}", fontsize=label_fontsize, color=colors['axis_label'])
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.spines['left'].set_linewidth(.3)
     ax.spines['bottom'].set_linewidth(.3)
 
     class_names = node.shadow_tree.class_names
 
@@ -1011,15 +1002,14 @@
         t = patches.Polygon(tria, facecolor=color)
         t.set_clip_on(False)
         ax.add_patch(t)
         ax.text(node.split(), -2 * th,
                 f"{myround(node.split(), precision)}",
                 horizontalalignment='center',
                 fontsize=ticks_fontsize,
-                fontname=fontname,
                 color=colors['text_wedge'])
 
     wedge(ax, node.split(), color=colors['wedge'])
     if highlight_node:
         wedge(ax, X[node.feature()], color=colors['highlight'])
 
     if filename is not None:
@@ -1050,32 +1040,31 @@
                    X_train: np.ndarray,
                    y_train: np.ndarray,
                    target_name: str,
                    filename: str = None,
                    y_range=None,
                    ticks_fontsize: int = 8,
                    label_fontsize: int = 9,
-                   fontname: str = "Arial",
                    precision=1,
                    X: np.array = None,
                    highlight_node: bool = False,
                    colors: dict = None):
     colors = adjust_colors(colors)
 
     figsize = (2.5, 1.1)
     fig, ax = plt.subplots(1, 1, figsize=figsize)
     ax.tick_params(colors=colors['tick_label'])
 
     feature_name = node.feature_name()
 
-    ax.set_xlabel(f"{feature_name}", fontsize=label_fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(f"{feature_name}", fontsize=label_fontsize, color=colors['axis_label'])
 
     ax.set_ylim(y_range)
     if node == node.shadow_tree.root:
-        ax.set_ylabel(target_name, fontsize=label_fontsize, fontname=fontname, color=colors['axis_label'])
+        ax.set_ylabel(target_name, fontsize=label_fontsize, color=colors['axis_label'])
 
     ax.spines['top'].set_visible(False)
     ax.spines['right'].set_visible(False)
     ax.spines['left'].set_linewidth(.3)
     ax.spines['bottom'].set_linewidth(.3)
     ax.tick_params(axis='both', which='major', width=.3, labelcolor=colors['tick_label'], labelsize=ticks_fontsize)
 
@@ -1131,15 +1120,14 @@
                   y: (pd.Series, np.ndarray),
                   target_name,
                   filename: str = None,
                   y_range=None,
                   precision=1,
                   label_fontsize: int = 9,
                   ticks_fontsize: int = 8,
-                  fontname: str = "Arial",
                   colors=None):
     colors = adjust_colors(colors)
 
     samples = node.samples()
     y = y[samples]
 
     figsize = (.75, .8)
@@ -1156,15 +1144,15 @@
     ax.spines['left'].set_linewidth(.3)
     ax.set_xticks([])
 
     ticklabelpad = plt.rcParams['xtick.major.pad']
     ax.annotate(f"{target_name}={myround(m, precision)}\nn={len(y)}",
                 xy=(.5, 0), xytext=(.5, -.5 * ticklabelpad), ha='center', va='top',
                 xycoords='axes fraction', textcoords='offset points',
-                fontsize=label_fontsize, fontname=fontname, color=colors['axis_label'])
+                fontsize=label_fontsize, color=colors['axis_label'])
 
     ax.tick_params(axis='y', which='major', width=.3, labelcolor=colors['tick_label'], labelsize=ticks_fontsize)
 
     mu = .5
     sigma = .08
     X = np.random.normal(mu, sigma, size=len(y))
     ax.set_xlim(0, 1)
@@ -1218,15 +1206,15 @@
     ax.yaxis.set_visible(False)
 
     if filename is not None:
         plt.savefig(filename, bbox_inches='tight', pad_inches=0)
         plt.close()
 
 
-def draw_piechart(counts, size, colors, filename, label=None, fontname="Arial", graph_colors=None):
+def draw_piechart(counts, size, colors, filename, label=None, graph_colors=None):
     graph_colors = adjust_colors(graph_colors)
     n_nonzero = np.count_nonzero(counts)
 
     if n_nonzero != 0:
         i = np.nonzero(counts)[0][0]
         if n_nonzero == 1:
             counts = [counts[i]]
@@ -1248,15 +1236,15 @@
     ax.xaxis.set_visible(False)
     ax.yaxis.set_visible(False)
 
     if label is not None:
         ax.text(size / 2 - 6 * tweak, -10 * tweak, label,
                 horizontalalignment='center',
                 verticalalignment='top',
-                fontsize=9, color=graph_colors['text'], fontname=fontname)
+                fontsize=9, color=graph_colors['text'])
 
     plt.savefig(filename, bbox_inches='tight', pad_inches=0)
     plt.close()
 
 
 def prop_size(n, counts, output_range=(0.00, 0.3)):
     min_samples = min(counts)
@@ -1281,15 +1269,14 @@
                      x_data: (pd.DataFrame, np.ndarray) = None,
                      feature_names: List[str] = None,
                      tree_index: int = None,  # required in case of tree ensemble
                      figsize: tuple = (10, 5),
                      display_type: str = "plot",
                      colors: dict = None,
                      fontsize: int = 14,
-                     fontname: str = "Arial",
                      grid: bool = False,
                      bins: int = 10,
                      min_samples: int = 0,
                      max_samples: int = None):
     """Visualize the number of data samples from each leaf.
     Interpreting leaf samples can help us to see how the data is spread over the tree:
     - if we have a leaf with many samples and a good impurity, it means that we can be pretty confident
@@ -1334,16 +1321,14 @@
         The plot size
     :param display_type: str, optional
        'plot', 'text'. 'hist'
     :param colors: dict
         The set of colors used for plotting
     :param fontsize: int
         Plot labels font size
-    :param fontname: str
-        Plot labels font name
     :param grid: bool
         True if we want to display the grid lines on the visualization
     :param bins: int
         Number of histogram bins
     :param min_samples: int
         Min number of samples for a leaf
     :param max_samples: int
@@ -1366,16 +1351,16 @@
         ax.set_xticks(range(0, len(leaf_id)))
         ax.set_xticklabels(leaf_id)
         barcontainers = ax.bar(range(0, len(leaf_id)), leaf_samples, color=colors["hist_bar"],
                                lw=.3, align='center', width=1)
         for rect in barcontainers.patches:
             rect.set_linewidth(.5)
             rect.set_edgecolor(colors['rect_edge'])
-        ax.set_xlabel("leaf ids", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-        ax.set_ylabel("samples count", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+        ax.set_xlabel("leaf ids", fontsize=fontsize, color=colors['axis_label'])
+        ax.set_ylabel("samples count", fontsize=fontsize, color=colors['axis_label'])
         ax.grid(b=grid)
     elif display_type == "text":
         for leaf, samples in zip(leaf_id, leaf_samples):
             print(f"leaf {leaf} has {samples} samples")
     elif display_type == "hist":
         colors = adjust_colors(colors)
 
@@ -1384,26 +1369,25 @@
         ax.spines['right'].set_visible(False)
         ax.spines['left'].set_linewidth(.3)
         ax.spines['bottom'].set_linewidth(.3)
         n, bins, patches = ax.hist(leaf_samples, bins=bins, color=colors["hist_bar"])
         for rect in patches:
             rect.set_linewidth(.5)
             rect.set_edgecolor(colors['rect_edge'])
-        ax.set_xlabel("leaf sample", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-        ax.set_ylabel("leaf count", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+        ax.set_xlabel("leaf sample", fontsize=fontsize, color=colors['axis_label'])
+        ax.set_ylabel("leaf count", fontsize=fontsize, color=colors['axis_label'])
         ax.grid(b=grid)
 
 
 def viz_leaf_criterion(tree_model,
                        tree_index: int = None,  # required in case of tree ensemble,
                        figsize: tuple = (10, 5),
                        display_type: str = "plot",
                        colors: dict = None,
                        fontsize: int = 14,
-                       fontname: str = "Arial",
                        grid: bool = False,
                        bins: int = 10):
     """Visualize leaves criterion.
     The most common criterion/impurity for tree regressors is “mse”, “friedman_mse”, “mae” and for tree classifers are
     "gini" and "entropy". This information shows the leaf performance/confidence for its predictions, namely how pure or
     impure are the samples from each leaf. Each leaf performance, in the end, will determine the general tree performance.
     This visualisation can be used together with viz_leaf_samples() for a better leaf interpretation. For example,
@@ -1432,16 +1416,14 @@
         The plot size
     :param display_type: str, optional
        'plot', 'text'. 'hist'
     :param colors: dict
         The set of colors used for plotting
     :param fontsize: int
         Plot labels font size
-    :param fontname: str
-        Plot labels font name
     :param grid: bool
         True if we want to display the grid lines on the visualization
     :param bins:  int
         Number of histogram bins
     :return:
     """
     shadow_tree = ShadowDecTree.get_shadow_tree(tree_model, None, None, None, None, None, tree_index)
@@ -1458,17 +1440,16 @@
         ax.set_xticks(range(0, len(leaf_id)))
         ax.set_xticklabels(leaf_id)
         barcontainers = ax.bar(range(0, len(leaf_id)), leaf_criteria, color=colors["hist_bar"],
                                lw=.3, align='center', width=1)
         for rect in barcontainers.patches:
             rect.set_linewidth(.5)
             rect.set_edgecolor(colors['rect_edge'])
-        ax.set_xlabel("leaf ids", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-        ax.set_ylabel(f"{shadow_tree.criterion()}", fontsize=fontsize, fontname=fontname,
-                      color=colors['axis_label'])
+        ax.set_xlabel("leaf ids", fontsize=fontsize, color=colors['axis_label'])
+        ax.set_ylabel(f"{shadow_tree.criterion()}", fontsize=fontsize, color=colors['axis_label'])
         ax.grid(b=grid)
     elif display_type == "text":
         for leaf, criteria in zip(leaf_id, leaf_criteria):
             print(f"leaf {leaf} has {criteria} {shadow_tree.criterion()}")
     elif display_type == "hist":
         colors = adjust_colors(colors)
 
@@ -1477,30 +1458,29 @@
         ax.spines['right'].set_visible(False)
         ax.spines['left'].set_linewidth(.3)
         ax.spines['bottom'].set_linewidth(.3)
         n, bins, patches = ax.hist(leaf_criteria, bins=bins, color=colors["hist_bar"])
         for rect in patches:
             rect.set_linewidth(.5)
             rect.set_edgecolor(colors['rect_edge'])
-        ax.set_xlabel(f"{shadow_tree.criterion()}", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-        ax.set_ylabel("leaf count", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+        ax.set_xlabel(f"{shadow_tree.criterion()}", fontsize=fontsize, color=colors['axis_label'])
+        ax.set_ylabel("leaf count", fontsize=fontsize, color=colors['axis_label'])
         ax.grid(b=grid)
 
 
 def ctreeviz_leaf_samples(tree_model,
                           x_data: (pd.DataFrame, np.ndarray) = None,
                           y_data: (pd.DataFrame, np.ndarray) = None,
                           feature_names: List[str] = None,
                           tree_index: int = None,  # required in case of tree ensemble,
                           figsize: tuple = (10, 5),
                           display_type: str = "plot",
                           plot_ylim: int = None,
                           colors: dict = None,
                           fontsize: int = 14,
-                          fontname: str = "Arial",
                           grid: bool = False):
     """Visualize the number of data samples by class for each leaf.
     It's a good way to see how classes are distributed in leaves. For example, you can observe that in some
     leaves all the samples belong only to one class, or that in other leaves the distribution of classes is almost
     50/50.
     You could get all the samples from these leaves and look over/understand what they have in common. Now, you
     can understand your data in a model driven way.
@@ -1533,16 +1513,14 @@
     :param plot_ylim: int, optional
         The max value for oY. This is useful in case we have few leaves with big sample values which 'shadow'
         the other leaves values.
     :param colors: dict
         The set of colors used for plotting
     :param fontsize: int
         Plot labels fontsize
-    :param fontname: str
-        Plot labels font name
     :param grid: bool
         True if we want to display the grid lines on the visualization
     """
     shadow_tree = ShadowDecTree.get_shadow_tree(tree_model, x_data, y_data, feature_names, None, None, tree_index)
     index, leaf_samples_0, leaf_samples_1 = shadow_tree.get_leaf_sample_counts_by_class()
 
     if display_type == "plot":
@@ -1564,16 +1542,16 @@
         bar_container1 = ax.bar(range(0, len(index)), leaf_samples_1, bottom=leaf_samples_0,
                                 color=colors_classes[1], lw=.3, align='center', width=1)
         for bar_container in [bar_container0, bar_container1]:
             for rect in bar_container.patches:
                 rect.set_linewidth(.5)
                 rect.set_edgecolor(colors['rect_edge'])
 
-        ax.set_xlabel("leaf ids", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
-        ax.set_ylabel("samples by class", fontsize=fontsize, fontname=fontname, color=colors['axis_label'])
+        ax.set_xlabel("leaf ids", fontsize=fontsize, color=colors['axis_label'])
+        ax.set_ylabel("samples by class", fontsize=fontsize, color=colors['axis_label'])
         ax.grid(grid)
         ax.legend([bar_container0, bar_container1],
                   [f'class {shadow_tree.classes()[0]}', f'class {shadow_tree.classes()[1]}'])
     elif display_type == "text":
         for leaf, samples_0, samples_1 in zip(index, leaf_samples_0, leaf_samples_1):
             print(f"leaf {leaf}, samples : {samples_0}, {samples_1}")
 
@@ -1583,15 +1561,15 @@
     y = []
     means = []
     means_range = []
     x_labels = []
     sigma = .05
     for i, node in enumerate(shadow_tree.leaves):
         leaf_index_sample = node.samples()
-        leaf_target = shadow_tree.y_data[leaf_index_sample]
+        leaf_target = shadow_tree.y_train[leaf_index_sample]
         leaf_target_mean = np.mean(leaf_target)
         np.random.seed(0)  # generate the same list of random values for each call
         X = np.random.normal(i, sigma, size=len(leaf_target))
 
         x.extend(X)
         y.extend(leaf_target)
         means.append([leaf_target_mean, leaf_target_mean])
@@ -1607,15 +1585,14 @@
                     feature_names: List[str] = None,
                     target_name: str = None,
                     tree_index: int = None,  # required in case of tree ensemble,
                     show_leaf_labels: bool = True,
                     colors: dict = None,
                     markersize: int = 50,
                     label_fontsize: int = 14,
-                    fontname: str = "Arial",
                     precision: int = 1,
                     figsize: tuple = None,
                     grid: bool = False,
                     prediction_line_width: int = 2):
     """Visualize leaf target distribution for regression decision trees.
     In case there is a big tree with a lot of leaves, the visualisations can become hard to interpret. In these
     scenarios, you can use the plot_leaf_count parameter to adjust the number of leaves per plot.
@@ -1669,17 +1646,16 @@
 
     ax.set_xlim(min(y), max(y) + 10)
     ax.set_ylim(-1, len(y_labels))
     ax.set_yticks(np.arange(0, len(y_labels), 1))
     ax.set_yticklabels([])
     ax.scatter(y, x, marker='o', alpha=colors['scatter_marker_alpha'] - 0.2, c=colors['scatter_marker'],
                s=markersize, edgecolor=colors['scatter_edge'], lw=.3)
-    ax.set_xlabel(shadow_tree.target_name.lower(), fontsize=label_fontsize,
-                  fontname=fontname, color=colors['axis_label'])
-    ax.set_ylabel("leaf", fontsize=label_fontsize, fontname=fontname, color=colors['axis_label'])
+    ax.set_xlabel(shadow_tree.target_name.lower(), fontsize=label_fontsize, color=colors['axis_label'])
+    ax.set_ylabel("leaf", fontsize=label_fontsize, color=colors['axis_label'])
     ax.grid(b=grid)
 
     if show_leaf_labels:
         for i in range(len(y_labels)):
             ax.text(max(y) + 10, i - 0.15, y_labels[i])
         ax.text(max(y) + 10, len(y_labels) - 0.15, shadow_tree.target_name.lower())
 
@@ -1720,15 +1696,15 @@
     :return: pd.DataFrame
         Node training samples' stats
     """
     shadow_tree = ShadowDecTree.get_shadow_tree(
         tree_model, x_data, None, feature_names, None, None, tree_index
     )
     node_samples = shadow_tree.get_node_samples()
-    return pd.DataFrame(shadow_tree.x_data, columns=shadow_tree.feature_names).iloc[node_samples[node_id]].describe()
+    return pd.DataFrame(shadow_tree.X_train, columns=shadow_tree.feature_names).iloc[node_samples[node_id]].describe()
 
 
 def explain_prediction_path(tree_model,
                             x: np.ndarray,
                             x_data=None,
                             y_data=None,  # required for XGBoost
                             explanation_type: ('plain_english', 'sklearn_default') = "plain_english",
```

### Comparing `InterpretME-1.2.2/InterpretME/mappings/classes.ttl` & `InterpretME-1.3.0/InterpretME/mappings/classes.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/cross_validation.ttl` & `InterpretME-1.3.0/InterpretME/mappings/cross_validation.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/definition_feature.ttl` & `InterpretME-1.3.0/InterpretME/mappings/definition_feature.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/endpoint.ttl` & `InterpretME-1.3.0/InterpretME/mappings/endpoint.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/entity_alignment.ttl` & `InterpretME-1.3.0/InterpretME/mappings/entity_alignment.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/imp_features.ttl` & `InterpretME-1.3.0/InterpretME/mappings/imp_features.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/lime_features.ttl` & `InterpretME-1.3.0/InterpretME/mappings/lime_features.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/model_details.ttl` & `InterpretME-1.3.0/InterpretME/mappings/model_details.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/precision_recall.ttl` & `InterpretME-1.3.0/InterpretME/mappings/precision_recall.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/prediction_probabilities.ttl` & `InterpretME-1.3.0/InterpretME/mappings/prediction_probabilities.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/sampling_strategy.ttl` & `InterpretME-1.3.0/InterpretME/mappings/sampling_strategy.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/mappings/shacl_validation_results.ttl` & `InterpretME-1.3.0/InterpretME/mappings/shacl_validation_results.ttl`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/pipeline.py` & `InterpretME-1.3.0/InterpretME/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import hashlib
 import json
+import os
 import os.path
 import time
 from pathlib import Path
-import csv
+
 import pandas as pd
 import validating_models.stats as stats
 from pkg_resources import resource_filename
 from validating_models.checker import Checker
 from validating_models.constraint import ShaclSchemaConstraint
 from validating_models.dataset import BaseDataset, ProcessedDataset
 from validating_models.models.decision_tree import get_shadow_tree_from_checker
 from validating_models.shacl_validation_engine import ReducedTravshaclCommunicator
 
+import InterpretME.utils as utils
 from InterpretME import preprocessing_data, sampling_strategy, classification
 from InterpretME.semantification import rdf_semantification
 from InterpretME.upload import upload_to_virtuoso
 
 
 def constraint_md5_sum(constraint):
     """Generates checksum for SHACL constraints.
@@ -41,19 +43,19 @@
     return hash_md5.hexdigest()
 
 def read_dataset(input_data,st):
     path = input_data['path_to_data']
     if os.path.splitext(path)[1].lower() == '.json':
         with stats.measure_time('PIPE_DATASET_EXTRACTION'):
             annotated_dataset = pd.read_json(path)
-            print("Reading the data in json format", annotated_dataset)
+            # print("Reading the data in json format", annotated_dataset)
     else:  # assuming CSV
         with stats.measure_time('PIPE_DATASET_EXTRACTION'):
             annotated_dataset = pd.read_csv(path)
-            print("Reading the data in csv format")
+            # print("Reading the data in csv format")
     seed_var = input_data['Index_var']
     sampling = input_data['sampling_strategy']
     cv = input_data['cross_validation_folds']
     test_split = input_data['test_split']
     num_imp_features = input_data['number_important_features']
     train_model = input_data['model']
     min_max_depth = input_data.get('min_max_depth', 4)
@@ -142,42 +144,45 @@
         query_select_clause = query_select_clause + "?" + k + " "
         query_where_clause = query_where_clause + v
         target_name = k
         definition.append(v)
 
         query_where_clause = query_where_clause + "}"
         sparqlQuery = query_select_clause + " " + query_where_clause
-        print(sparqlQuery)
+        # print(sparqlQuery)
 
         features = independent_var + dependent_var
 
         shacl_engine_communicator = ReducedTravshaclCommunicator(
         '', endpoint, resource_filename('InterpretME', 'shacl_api_config.json')
            )
 
     def hook(results):
         bindings = [{key: value['value'] for key, value in binding.items()}
                     for binding in results['results']['bindings']]
         df = pd.DataFrame.from_dict(bindings)
         for column in df.columns:
-            df[column] = df[column].str.rsplit('/', 1).str[-1]
+            df[column] = df[column].str.rsplit('/', n=1).str[-1]
         return df
 
     with stats.measure_time('PIPE_DATASET_EXTRACTION'):
         base_dataset = BaseDataset.from_knowledge_graph(endpoint, shacl_engine_communicator, sparqlQuery,
                                                     target_name, seed_var=seed_var,
                                                     raw_data_query_results_to_df_hook=hook)
 
     constraints = [ShaclSchemaConstraint.from_dict(constraint) for constraint in input_data['Constraints']]
     constraint_identifiers = [constraint_md5_sum(constraint) for constraint in constraints]
 
+    utils.pbar.total += len(constraints)
+    utils.pbar.set_description('SHACL Validation', refresh=True)
     with stats.measure_time('PIPE_SHACL_VALIDATION'):
         shacl_validation_results = base_dataset.get_shacl_schema_validation_results(
                 constraints, rename_columns=True, replace_non_applicable_nans=True
         )
+    utils.pbar.update(len(constraints))
 
     sample_to_node_mapping = base_dataset.get_sample_to_node_mapping().rename('node')
 
     annotated_dataset = pd.concat(
             (base_dataset.df, shacl_validation_results, sample_to_node_mapping), axis='columns'
     )
 
@@ -232,15 +237,14 @@
     annotated_dataset = annotated_dataset.drop(columns=['node'])
     num = len(input_data['Constraints'])
     annotated_dataset = annotated_dataset.iloc[:, :-num]
 
     return seed_var, independent_var, dependent_var, classes, class_names, annotated_dataset, constraints, base_dataset, st, input_data['3_valued_logic'], sampling, test_split, num_imp_features, train_model, cv, min_max_depth, max_max_depth
 
 
-
 # get the start time and use it as run_id
 def current_milli_time():
     return round(time.time() * 1000)
 
 
 def pipeline(path_config, lime_results, server_url=None, username=None, password=None,
              sampling=None, cv=None, imp_features=None, test_split=None, model=None):
@@ -279,39 +283,38 @@
     -------
     dict
         Pipeline function will return a dictionary with all the results stored as
         objects which can be used for further analysis.
 
     """
     st = current_milli_time()
-    print(st)
-
     results = {'run_id': st}
 
+    utils.pbar = utils.tqdm(total=5, miniters=1, desc='InterpretME Pipeline', unit='task')
+
     if not os.path.exists('interpretme/files'):
         os.makedirs('interpretme/files')
-        print("The directory for files is created")
+        # print("The directory for files is created")
 
     stats.STATS_COLLECTOR.activate(hyperparameters=[])
     stats.STATS_COLLECTOR.new_run(hyperparameters=[])
 
     with open(path_config, "r") as input_file_descriptor:
         input_data = json.load(input_file_descriptor)
 
+    utils.pbar.set_description('Read input data', refresh=True)
     input_is_kg = None
     if "Endpoint" in input_data.keys() and "path_to_data" not in input_data.keys():
         # input from SPARQL endpoint
         input_is_kg = True
         seed_var, independent_var, dependent_var, classes, class_names, annotated_dataset, constraints, base_dataset, st, non_applicable_counts, samplingstrategy, train_test_split, num_imp_features, train_model, cross_validation, min_max_depth, max_max_depth = read_KG(input_data, st)
-
     elif "Endpoint" not in input_data.keys() and "path_to_data" in input_data.keys():
         # input from dataset
         input_is_kg = False
         seed_var, independent_var, dependent_var, classes, class_names, st, sampling, test_split, num_imp_features, train_model, cv, annotated_dataset, min_max_depth, max_max_depth = read_dataset(input_data, st)
-
     else:
         # error
         raise Exception("Please provide either SPARQL endpoint or Dataset")
 
     if sampling is None:
         sampling = samplingstrategy
     else:
@@ -347,26 +350,33 @@
     else:
         test_split = test_split
 
     if model is None:
         model = train_model
     else:
         model = model
+    utils.pbar.update(1)  # end of reading the input dataset
 
+    utils.pbar.set_description('Preprocessing', refresh=True)
     with stats.measure_time('PIPE_PREPROCESSING'):
         encoded_data, encode_target = preprocessing_data.load_data(seed_var, dependent_var, classes, annotated_dataset)
+    utils.pbar.update(1)
 
+    utils.pbar.set_description('Sampling', refresh=True)
     with stats.measure_time('PIPE_SAMPLING'):
         sampled_data, sampled_target, results = sampling_strategy.sampling_strategy(encoded_data, encode_target, sampling, results)
+    utils.pbar.update(1)
 
     new_sampled_data, clf, results = classification.classify(sampled_data, sampled_target, imp_features, cv, classes, st, lime_results, test_split, model, results, min_max_depth, max_max_depth)
     processed_df = pd.concat((new_sampled_data, sampled_target), axis='columns')
     processed_df.reset_index(inplace=True)
 
     if "Endpoint" in input_data.keys() and "path_to_data" not in input_data.keys():
+        utils.pbar.total += 1
+        utils.pbar.set_description('Preparing Plots Data', refresh=True)
         with stats.measure_time('PIPE_CONSTRAINT_VIZ'):
             processedDataset = ProcessedDataset.from_node_unique_columns(
                 processed_df,
                 base_dataset,
                 base_columns=[seed_var],
                 target_name='class',
                 categorical_mapping={'class': {i: classes[i] for i in range(len(classes))}}
@@ -375,25 +385,33 @@
 
             shadow_tree = get_shadow_tree_from_checker(clf, checker)
 
             results['checker'] = checker
             results['shadow_tree'] = shadow_tree
             results['constraints'] = constraints
             results['non_applicable_counts'] = non_applicable_counts
-
-    with stats.measure_time('PIPE_InterpretMEKG_SEMANTIFICATION'):
-        rdf_semantification(input_is_kg)
+        utils.pbar.update(1)
 
     categories_stats = ['PIPE_DATASET_EXTRACTION', 'PIPE_SHACL_VALIDATION', 'PIPE_PREPROCESSING',
                         'PIPE_SAMPLING', 'PIPE_IMPORTANT_FEATURES', 'PIPE_LIME', 'PIPE_TRAIN_MODEL',
                         'PIPE_DTREEVIZ', 'PIPE_CONSTRAINT_VIZ', 'PIPE_OUTPUT', 'join',
                         'PIPE_InterpretMEKG_SEMANTIFICATION']
 
+    utils.pbar.set_description('Semantifying Results', refresh=True)
+    with stats.measure_time('PIPE_InterpretMEKG_SEMANTIFICATION'):
+        rdf_semantification(input_is_kg)
+    utils.pbar.update(1)
+
     if server_url is not None and username is not None and password is not None:
         categories_stats.append('PIPE_InterpretMEKG_UPLOAD_VIRTUOSO')
+        utils.pbar.total += 1
+        utils.pbar.set_description('Uploading to Virtuoso', refresh=True)
         with stats.measure_time('PIPE_InterpretMEKG_UPLOAD_VIRTUOSO'):
             upload_to_virtuoso(run_id=st, rdf_file='./rdf-dump/interpretme.nt',
                                server_url=server_url, username=username, password=password)
+        utils.pbar.update(1)
 
     stats.STATS_COLLECTOR.to_file('times.csv', categories=categories_stats)
 
+    utils.pbar.set_description('InterpretME Pipeline')
+    utils.pbar.close()
     return results
```

### Comparing `InterpretME-1.2.2/InterpretME/plots.py` & `InterpretME-1.3.0/InterpretME/plots.py`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/InterpretME/preprocessing_data.py` & `InterpretME-1.3.0/InterpretME/preprocessing_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,13 +103,13 @@
 
     Returns
     -------
     (dataframe, dataframe)
         Returns preprocessed dataset.
 
     """
-    print("--------- Preprocessing Data --------------")
-    print(annotated_dataset)
+    # print("--------- Preprocessing Data --------------")
+    # print(annotated_dataset)
     encode_target = define_class(classes, dependent_var, annotated_dataset)
     ann_data = annotated_dataset.drop(dependent_var, axis=1)
     encode_data = hot_encode(ann_data, seed_var)
     return encode_data, encode_target
```

### Comparing `InterpretME-1.2.2/InterpretME/sampling_strategy.py` & `InterpretME-1.3.0/InterpretME/sampling_strategy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
-from imblearn.under_sampling import RandomUnderSampler
 from imblearn.over_sampling import RandomOverSampler
+from imblearn.under_sampling import RandomUnderSampler
 
 
 def sampling_strategy(encode_data, encode_target, strategy, results):
     """Sampling strategy to balance the imbalanced data for predictive model.
 
     Parameters
     ----------
```

### Comparing `InterpretME-1.2.2/InterpretME/semantification.py` & `InterpretME-1.3.0/InterpretME/semantification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from rdfizer import semantify
 import validating_models.stats as stats
 from pkg_resources import resource_filename
+from rdfizer import semantify
+
+from InterpretME.utils import HiddenPrints
 
 semantification = stats.get_decorator('PIPE_InterpretMEKG_SEMANTIFICATION')
 
 
 @semantification
 def rdf_semantification(input_is_kg: bool):
-    print("#####################################################################")
-    print("******* Semantifying traced metadata from predictive pipeline *******")
-    print("#####################################################################")
     main_path = resource_filename('InterpretME', '')
     if input_is_kg:
         number_of_datasets = 12
     else:
         number_of_datasets = 8
 
     config = '[default]\n' \
@@ -64,8 +63,9 @@
                   'mapping: ${default:main_directory}/mappings/shacl_validation_results.ttl\n\n' \
                   '[dataset12]\n' \
                   'name: entity_alignment\n' \
                   'mapping: ${default:main_directory}/mappings/entity_alignment.ttl\n\n'
     with open('config_rdfizer.ini', 'w', encoding='utf8') as config_file:
         config_file.write(config)
 
-    semantify("config_rdfizer.ini")
+    with HiddenPrints():
+        semantify("config_rdfizer.ini")
```

### Comparing `InterpretME-1.2.2/InterpretME/upload.py` & `InterpretME-1.3.0/InterpretME/upload.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
-from requests.auth import HTTPBasicAuth
 import validating_models.stats as stats
+from requests.auth import HTTPBasicAuth
 
 uploading = stats.get_decorator('PIPE_InterpretMEKG_UPLOAD_VIRTUOSO')
 
 
 @uploading
 def upload_to_virtuoso(run_id, rdf_file, server_url, username, password):
     """
@@ -18,22 +18,16 @@
     server_url : str
         InterpretME knowledge graph endpoint.
     username : str
         Username of virtuoso.
     password : str
         Password of virtuoso.
 
-    Returns
-    -------
-
     """
     # server_url does not end with /sparql
-    print("#####################################################################")
-    print("******************* Uploading to Virtuoso **************************")
-    print("#####################################################################")
     address = server_url + 'DAV/home/' + username + '/rdf_sink/' + str(run_id) + '.ttl'
     with open(rdf_file, 'r') as f:
         r = requests.put(
             address,
             auth=HTTPBasicAuth(username, password),
             data=f.read(),
             headers={'Content-Type': 'text/turtle'}
```

### Comparing `InterpretME-1.2.2/InterpretME.egg-info/PKG-INFO` & `InterpretME-1.3.0/InterpretME.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: InterpretME
-Version: 1.2.2
+Version: 1.3.0
 Summary: An interpretable machine learning pipeline over knowledge graphs
 Home-page: https://github.com/SDM-TIB/InterpretME
+Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.0.tar.gz
 Author: Yashraj Chudasama, Disha Purohit, Philipp Rohde, Julian Gercke
 Author-email: yashraj.chudasama@tib.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `InterpretME-1.2.2/InterpretME.egg-info/SOURCES.txt` & `InterpretME-1.3.0/InterpretME.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 InterpretME/pipeline.py
 InterpretME/plots.py
 InterpretME/preprocessing_data.py
 InterpretME/sampling_strategy.py
 InterpretME/semantification.py
 InterpretME/shacl_api_config.json
 InterpretME/upload.py
+InterpretME/utils.py
 InterpretME.egg-info/PKG-INFO
 InterpretME.egg-info/SOURCES.txt
 InterpretME.egg-info/dependency_links.txt
 InterpretME.egg-info/requires.txt
 InterpretME.egg-info/top_level.txt
 InterpretME/mappings/classes.ttl
 InterpretME/mappings/cross_validation.ttl
```

### Comparing `InterpretME-1.2.2/LIBRARY.md` & `InterpretME-1.3.0/LIBRARY.md`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/LICENSE` & `InterpretME-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/PKG-INFO` & `InterpretME-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: InterpretME
-Version: 1.2.2
+Version: 1.3.0
 Summary: An interpretable machine learning pipeline over knowledge graphs
 Home-page: https://github.com/SDM-TIB/InterpretME
+Download-URL: https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v1.3.0.tar.gz
 Author: Yashraj Chudasama, Disha Purohit, Philipp Rohde, Julian Gercke
 Author-email: yashraj.chudasama@tib.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
```

### Comparing `InterpretME-1.2.2/README.md` & `InterpretME-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `InterpretME-1.2.2/setup.py` & `InterpretME-1.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from setuptools import setup
 
 with open("LIBRARY.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
+VERSION = '1.3.0'
+
 setup(
     name='InterpretME',
     packages=['InterpretME'],
-    version='1.2.2',
+    version=VERSION,
     description='An interpretable machine learning pipeline over knowledge graphs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Yashraj Chudasama, Disha Purohit, Philipp Rohde, Julian Gercke',
     author_email='yashraj.chudasama@tib.eu',
     url='https://github.com/SDM-TIB/InterpretME',
+    download_url='https://github.com/SDM-TIB/InterpretME/archive/refs/tags/v' + VERSION + '.tar.gz',
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         "Operating System :: OS Independent",
         'License :: OSI Approved :: MIT License',
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.8, <3.10',
     install_requires=[
-        'pandas>=1.4.1',
+        'pandas>=1.4.0,<2.0.0',
         'imbalanced-learn>=0.9.0',
         'lime>=0.2.0',
         'pydotplus>=2.0.2',
         'svglib>=1.2.1',
         'colour>=0.1.5',
         'matplotlib<=3.3.4',
         'rdflib<=6.1.1',
         'seaborn>=0.11.2',
         'numpy>=1.23.5',
-        'dtreeviz>=1.3.0,<2.0.0',
+        'dtreeviz>=2.2.0',
         'python-slugify>=6.0.0',
-        'requests>=2.27.0',
+        'requests>=2.31.0',
         'rdfizer>=4.5.5',
-        'DeTrusty>=0.11.1',
-        'validating-models>=0.9.0',
-        'optuna>=3.1.0'
+        'DeTrusty>=0.12.3',
+        'validating-models>=0.9.5',
+        'optuna>=3.2.0',
+        'scikit-learn>=1.2.0'
     ]
 )
```

