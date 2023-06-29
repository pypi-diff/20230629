# Comparing `tmp/trailml-1.0.0.tar.gz` & `tmp/trailml-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailml-1.0.0.tar", last modified: Mon May 29 20:18:59 2023, max compression
+gzip compressed data, was "trailml-1.0.1.tar", last modified: Thu Jun 29 12:19:21 2023, max compression
```

## Comparing `trailml-1.0.0.tar` & `trailml-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.460216 trailml-1.0.0/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-05-29 20:18:59.460058 trailml-1.0.0/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.0/README.md
--rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-05-29 20:17:34.000000 trailml-1.0.0/pyproject.toml
--rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-05-29 20:18:59.460265 trailml-1.0.0/setup.cfg
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.455538 trailml-1.0.0/src/
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.456561 trailml-1.0.0/src/trail/
--rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/__init__.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.457268 trailml-1.0.0/src/trail/libconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      194 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/libconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/libconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)     8416 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/trail.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.458068 trailml-1.0.0/src/trail/userconfig/
--rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/config.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/exceptions.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.459805 trailml-1.0.0/src/trailml.egg-info/
--rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/requires.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.589105 trailml-1.0.1/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-06-29 12:19:21.588973 trailml-1.0.1/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.1/README.md
+-rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-06-29 12:15:25.000000 trailml-1.0.1/pyproject.toml
+-rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-06-29 12:19:21.589156 trailml-1.0.1/setup.cfg
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.585160 trailml-1.0.1/src/
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.585943 trailml-1.0.1/src/trail/
+-rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/__init__.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.586633 trailml-1.0.1/src/trail/libconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      235 2023-06-05 14:32:13.000000 trailml-1.0.1/src/trail/libconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-30 16:59:12.000000 trailml-1.0.1/src/trail/libconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)    10795 2023-06-22 15:45:14.000000 trailml-1.0.1/src/trail/trail.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.587845 trailml-1.0.1/src/trail/userconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.1/src/trail/userconfig/exceptions.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-06-29 12:19:21.588755 trailml-1.0.1/src/trailml.egg-info/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/requires.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-06-29 12:19:21.000000 trailml-1.0.1/src/trailml.egg-info/top_level.txt
```

### Comparing `trailml-1.0.0/PKG-INFO` & `trailml-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.0
+Version: 1.0.1
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trailml-1.0.0/README.md` & `trailml-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `trailml-1.0.0/pyproject.toml` & `trailml-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trailml"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Trail ML", email="python@trail-ml.com" },
 ]
 description = "Trail ML library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `trailml-1.0.0/src/trail/trail.py` & `trailml-1.0.1/src/trail/trail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import base64
+from collections import defaultdict
 import json
 import os.path
+import signal
 import sys
 from typing import Union
 
 import mlflow
 import pyrebase
 import requests
 from gql import gql, Client
@@ -21,36 +23,43 @@
     ADD_EXPERIMENT_MUTATION = """
         mutation (
             $projectId: String!,
             $parentExperimentId: String!,
             $title: String!,
             $comments: String!,
             $instanceRunParameters: JSONString!,
-            $instanceRunMetrics: JSONString!
+            $instanceRunMetrics: JSONString!,
+            $instanceRunComplete: Boolean!
+            $hypothesis: String,
+            $metricsHistoryEntries: [MetricsHistoryInput]
         ) {
             addExperiment(
                 projectId: $projectId,
                 parentExperimentId: $parentExperimentId,
                 title: $title,
                 comments: $comments,
+                hypothesis: $hypothesis
+                metricsHistory: $metricsHistoryEntries
                 instanceRuns: {
                     comment: "",
                     parameters: $instanceRunParameters,
-                    metrics: $instanceRunMetrics
+                    metrics: $instanceRunMetrics,
+                    isComplete: $instanceRunComplete
                 }
             ) {
                 experiment {
                     id
                     title
                     comments
                     instanceRuns {
                         id
                         comment
                         parameters
                         metrics
+                        isComplete
                     }
                 }
             }
         }
     """
 
     PUT_ARTIFACT_MUTATION = """
@@ -104,39 +113,49 @@
         )
         self.client = Client(transport=transport)
         self.project_config = userconfig.project(project_alias)
         self.project_id = self.project_config.id
         self.parent_experiment_id = self.project_config.parent_experiment_id
         self.experiment_title = experiment_title
         self.artifacts = []
+        self.default_handler = signal.getsignal(signal.SIGINT)
+        self.is_complete = True
+        self.hypothesis = ""
+
+    def signal_handler(self, signum, frame):
+        self.is_complete = False
+        self.__exit__
+        print("Latest run is logged.")
+        raise KeyboardInterrupt()
 
     def __enter__(self):
         if mlflow.active_run() is None:
             raise Exception('No active mlflow run found!')
-
+        signal.signal(signal.SIGINT, self.signal_handler)  # type: ignore
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         run = mlflow.active_run()
         if run is None:
             raise Exception('No active mlflow run found!')
 
         # we fetch the run like this because of
         # https://mlflow.org/docs/latest/python_api/mlflow.html#mlflow.active_run
         materialized_run = mlflow.get_run(run_id=run.info.run_id)
 
         if materialized_run:
             self._log_experiment(materialized_run)
             self._upload_artifacts(materialized_run)
+        signal.signal(signal.SIGINT, self.default_handler)
 
     def put_artifact(
             self,
             src:  Union[str, bytes],
             name: str,
-            tags: Union[str, list] = None
+            tags: Union[str, list, None]
     ):
         """Queues an artifact for upload to Trail. The artifact is uploaded when
         leaving the `with Trail` block.
         The `src` parameter can be either a string or a bytes object. In case
         of a string, it is assumed to be a path to a file. In case of a bytes
         object, it is assumed to be the raw data of the artifact.
 
@@ -167,14 +186,17 @@
                 'experimentId': self.parent_experiment_id,
                 'name': name,
                 'base64Data': base64.b64encode(data).decode(),
                 'tags': tags
             }
         )
 
+    def put_hypothesis(self, hypothesis: str):
+        self.hypothesis = hypothesis
+
     def _log_experiment(self, run: Run):
         run_id = run.info.run_id
         tags = {
             k: v for k, v in run.data.tags.items()
             if not k.startswith('mlflow.')
         }
         mlflow_artifacts = [
@@ -184,26 +206,38 @@
         d = {  # noqa: F841
             'run_id': run_id,
             'timestamp': run.info.start_time / 1000.0,
             'user': run.info.user_id,
             'artifacts': mlflow_artifacts,
             'tags': tags
         }
+        # Convert numeric parameter values to their respective types
+        converted_params = run.data.params.copy()
+        for key, value in converted_params.items():
+            try:
+                converted_params[key] = float(value)
+            except ValueError:
+                pass
 
         try:
             result = self.client.execute(
                 document=gql(self.ADD_EXPERIMENT_MUTATION),
                 variable_values={
                     'projectId': self.project_id,
                     'parentExperimentId': self.parent_experiment_id,
                     'title': self.experiment_title,
                     'comments': '',
-                    'instanceRunParameters': json.dumps(run.data.params),
-                    'instanceRunMetrics': json.dumps(run.data.metrics)
-                }
+                    'instanceRunParameters': json.dumps(converted_params),
+                    'instanceRunMetrics': json.dumps(run.data.metrics),
+                    'instanceRunComplete': self.is_complete,
+                    'hypothesis': self.hypothesis,
+                    'metricsHistoryEntries': self.get_metric_history_data(
+                        run_id=run_id
+                    ),
+                },
             )
 
             experiment_id = result['addExperiment']['experiment']['id']
             self.project_config.update_parent_experiment_id(experiment_id)
             self.parent_experiment_id = experiment_id
         except TransportQueryError:
             print(
@@ -237,26 +271,49 @@
         except TransportQueryError:
             print(
                 'Error uploading experiment artifacts to Trail. Please contact '
                 'us if the problem persists.',
                 file=sys.stderr
             )
 
+    def get_metric_history_data(self, run_id):
+        client = mlflow.tracking.MlflowClient()
+        run = mlflow.active_run()
+        mlflowrun = mlflow.get_run(run_id=run.info.run_id)  # type: ignore
+        metric_list = list(mlflowrun.data.metrics.keys())
+        metrics = defaultdict(list)
+        for metric in metric_list:
+            metric_history = client.get_metric_history(run_id, metric)
+            for entry in metric_history:
+                metric_name = entry.key
+                data_point = {
+                    "value": entry.value,
+                    "timeStamp": str(entry.timestamp),
+                    "step": entry.step,
+                }
+                metrics[metric_name].append(data_point)
+        metrics_history = []
+        for metric in metrics:
+            metrics_history.append(
+                {"metricName": metric, "history": metrics[metric]}
+            )
+        return metrics_history
+
     @staticmethod
     def _retrieve_jwt_token(email, password):
         firebase = pyrebase.initialize_app({
             'apiKey': libconfig.FIREBASE_API_KEY,
             'authDomain': libconfig.FIREBASE_AUTH_DOMAIN,
             'databaseURL': 'THIS_IS_NOT_USED',
             'storageBucket': 'THIS_IS_NOT_USED',
         })
         auth = firebase.auth()
 
         try:
             user = auth.sign_in_with_email_and_password(email, password)
         except requests.exceptions.HTTPError as e:
-            if e.errno.response.status_code == 400:
+            if e.errno.response.status_code == 400:  # type: ignore
                 raise Exception('Invalid credentials') from None
 
             raise e
 
         return user['idToken']
```

### Comparing `trailml-1.0.0/src/trail/userconfig/__init__.py` & `trailml-1.0.1/src/trail/userconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.0/src/trail/userconfig/config.py` & `trailml-1.0.1/src/trail/userconfig/config.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.0/src/trail/userconfig/exceptions.py` & `trailml-1.0.1/src/trail/userconfig/exceptions.py`

 * *Files identical despite different names*

### Comparing `trailml-1.0.0/src/trailml.egg-info/PKG-INFO` & `trailml-1.0.1/src/trailml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailml
-Version: 1.0.0
+Version: 1.0.1
 Summary: Trail ML library
 Author-email: Trail ML <python@trail-ml.com>
 Project-URL: Homepage, https://trail-ml.com
 Project-URL: Bug Tracker, https://github.com/trail-ml/bugtracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

