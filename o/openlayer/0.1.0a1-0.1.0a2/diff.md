# Comparing `tmp/openlayer-0.1.0a1.tar.gz` & `tmp/openlayer-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlayer-0.1.0a1.tar", last modified: Thu Jun  8 15:58:16 2023, max compression
+gzip compressed data, was "openlayer-0.1.0a2.tar", last modified: Thu Jun 29 21:23:33 2023, max compression
```

## Comparing `openlayer-0.1.0a1.tar` & `openlayer-0.1.0a2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.635725 openlayer-0.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 15:58:16.635725 openlayer-0.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.631725 openlayer-0.1.0a1/openlayer/
--rw-r--r--   0 runner    (1001) docker     (123)    53757 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.631725 openlayer-0.1.0a1/openlayer/prediction_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/prediction_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/prediction_jobs/classification_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/prediction_jobs/regression_prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.635725 openlayer-0.1.0a1/openlayer/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/baseline_model_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/commit_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/dataset_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/model_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/validators/project_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/openlayer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.631725 openlayer-0.1.0a1/openlayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 15:58:16.000000 openlayer-0.1.0a1/openlayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-08 15:58:16.635725 openlayer-0.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:58:16.635725 openlayer-0.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 15:57:37.000000 openlayer-0.1.0a1/tests/test_openlayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-29 21:23:33.678828 openlayer-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/
+-rw-r--r--   0 runner    (1001) docker     (123)    55482 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/prediction_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/classification_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/prediction_jobs/regression_prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9513 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/baseline_model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/commit_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27173 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/dataset_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/model_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/validators/project_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/openlayer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/openlayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:23:33.000000 openlayer-0.1.0a2/openlayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 21:23:33.678828 openlayer-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:33.674828 openlayer-0.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 21:22:48.000000 openlayer-0.1.0a2/tests/test_openlayer.py
```

### Comparing `openlayer-0.1.0a1/LICENSE` & `openlayer-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/PKG-INFO` & `openlayer-0.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a1/README.md` & `openlayer-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/__init__.py` & `openlayer-0.1.0a2/openlayer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import uuid
 from typing import Optional
 
 import pandas as pd
 import yaml
 
 from . import api, exceptions, utils
+from .project_versions import ProjectVersion
 from .projects import Project
 from .schemas import BaselineModelSchema, DatasetSchema, ModelSchema
 from .tasks import TaskType
 
 # from validators import models as model_validators
 from .validators import (
     baseline_model_validators,
@@ -469,15 +470,15 @@
                 resource_dir=temp_dir,
                 project_id=project_id,
                 force=force,
             )
 
     def add_baseline_model(
         self,
-        project_id: int,
+        project_id: str,
         task_type: TaskType,
         model_config_file_path: Optional[str] = None,
         force: bool = False,
     ):
         """
         **Coming soon...**
 
@@ -990,15 +991,15 @@
                 file_path=file_path,
                 project_id=project_id,
                 dataset_config_file_path=dataset_config_file_path,
                 force=force,
                 task_type=task_type,
             )
 
-    def commit(self, message: str, project_id: int, force: bool = False):
+    def commit(self, message: str, project_id: str, force: bool = False):
         """Adds a commit message to staged resources.
 
         Parameters
         ----------
         message : str
             The commit message, between 1 and 140 characters.
         force : bool
@@ -1077,15 +1078,15 @@
             "date": time.ctime(),
         }
         with open(f"{project_dir}/commit.yaml", "w", encoding="UTF-8") as commit_file:
             yaml.dump(commit, commit_file)
 
         print("Committed!")
 
-    def push(self, project_id: int, task_type: TaskType):
+    def push(self, project_id: str, task_type: TaskType) -> Optional[ProjectVersion]:
         """Pushes the commited resources to the platform.
 
         Notes
         -----
         - To use this method, you must first have committed your changes with the :obj:`commit`
             method.
 
@@ -1120,23 +1121,25 @@
                 # Upload the tar file
                 print(
                     "Pushing changes to the platform with the commit message: \n"
                     f"\t - Message: {commit['message']} \n"
                     f"\t - Date: {commit['date']}"
                 )
                 payload = {"commit": {"message": commit["message"]}}
-                self.api.upload(
+                response_body = self.api.upload(
                     endpoint=f"projects/{project_id}/versions",
                     file_path=tar_file_path,
                     object_name="tarfile",
                     body=payload,
                 )
+                project_version = ProjectVersion(json=response_body, client=self)
 
             self._post_push_cleanup(project_dir=project_dir)
             print("Pushed!")
+            return project_version
 
     def _ready_for_push(self, project_dir: str, task_type: TaskType) -> bool:
         """Checks if the project's staging area is ready to be pushed to the platform.
 
         Parameters
         ----------
         project_dir : str
@@ -1179,15 +1182,15 @@
         return True
 
     def _post_push_cleanup(self, project_dir: str) -> None:
         """Cleans up and re-creates the project's staging area after a push."""
         shutil.rmtree(project_dir)
         os.makedirs(project_dir, exist_ok=True)
 
-    def export(self, destination_dir: str, project_id: int, task_type: TaskType):
+    def export(self, destination_dir: str, project_id: str, task_type: TaskType):
         """Exports the commited resources as a tarfile to the location specified
         by ``destination_dir``.
 
         This is useful if you want to drag and drop the tarfile into the platform's
         UI to upload it instead of using the :obj:`push` method.
 
         Parameters
@@ -1225,15 +1228,15 @@
 
                 print(f"Exporting staging area to {destination_dir}.")
                 shutil.copy(tar_file_path, os.path.expanduser(destination_dir))
 
             self._post_push_cleanup(project_dir=project_dir)
             print("Exported tarfile!")
 
-    def status(self, project_id: int):
+    def status(self, project_id: str):
         """Shows the state of the staging area.
 
         Examples
         --------
 
         You can use the :obj:`status` method to check the state of the staging area.
 
@@ -1273,15 +1276,15 @@
         for file in os.listdir(project_dir):
             if file in VALID_RESOURCE_NAMES:
                 print(f"\t - {file}")
         print(f"Commit message from {commit['date']}:")
         print(f"\t {commit['message']}")
         print("Use the `push` method to push your changes to the platform.")
 
-    def restore(self, *resource_names: str, project_id: int):
+    def restore(self, *resource_names: str, project_id: str):
         """Removes the resource specified by ``resource_name`` from the staging area.
 
         Parameters
         ----------
         *resource_names : str
             The names of the resources to restore, separated by comma. Valid resource names
             are ``"model"``, ``"training"``, and ``"validation"``.
@@ -1324,15 +1327,15 @@
             # Remove commit if there are no more resources staged
             if len(os.listdir(project_dir)) == 1 and os.path.exists(
                 f"{project_dir}/commit.yaml"
             ):
                 os.remove(f"{project_dir}/commit.yaml")
 
     def _stage_resource(
-        self, resource_name: str, resource_dir: str, project_id: int, force: bool
+        self, resource_name: str, resource_dir: str, project_id: str, force: bool
     ):
         """Adds the resource specified by `resource_name` to the project's staging directory.
 
         Parameters
         ----------
         resource_name : str
             The name of the resource to stage. Can be one of "model", "training",
@@ -1366,7 +1369,47 @@
             else:
                 print(f"Keeping the existing `{resource_name}` resource staged.")
                 return
 
         shutil.copytree(resource_dir, project_dir + "/" + resource_name)
 
         print(f"Staged the `{resource_name}` resource!")
+
+    def load_project_version(self, version_id: str) -> Project:
+        """Loads an existing project version from the Openlayer platform. Can be used
+        to check the status of the project version and the number of passing, failing
+        and skipped goals.
+
+        Parameters
+        ----------
+        id : str
+            UUID of the project to be loaded. You can find the UUID of a project by
+            navigating to the project's page on the Openlayer platform.
+
+            .. note::
+                When you run :obj:`push`, it will return the project version object,
+                which you can use to check your goal statuses.
+
+        Returns
+        -------
+        ProjectVersion
+            An object that is used to check for upload progress and goal statuses.
+            Also contains other useful information about a project version.
+
+        Examples
+        --------
+        Instantiate the client and load the project version:
+
+        >>> import openlayer
+        >>> client = openlayer.OpenlayerClient('YOUR_API_KEY_HERE')
+        >>>
+        >>> version = client.load_project_version(id='YOUR_PROJECT_ID_HERE')
+        >>> version.wait_for_completion()
+        >>> version.print_goal_report()
+
+        With the ProjectVersion object loaded, you are able to check progress and
+        goal statuses.
+        """
+        endpoint = f"versions/{version_id}"
+        version_data = self.api.get_request(endpoint)
+        version = ProjectVersion(version_data, self)
+        return version
```

### Comparing `openlayer-0.1.0a1/openlayer/api.py` & `openlayer-0.1.0a2/openlayer/api.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/datasets.py` & `openlayer-0.1.0a2/openlayer/datasets.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/exceptions.py` & `openlayer-0.1.0a2/openlayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/models.py` & `openlayer-0.1.0a2/openlayer/models.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/prediction_jobs/classification_prediction_job.py` & `openlayer-0.1.0a2/openlayer/prediction_jobs/classification_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/prediction_jobs/regression_prediction_job.py` & `openlayer-0.1.0a2/openlayer/prediction_jobs/regression_prediction_job.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/projects.py` & `openlayer-0.1.0a2/openlayer/projects.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/schemas.py` & `openlayer-0.1.0a2/openlayer/schemas.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/tasks.py` & `openlayer-0.1.0a2/openlayer/tasks.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/utils.py` & `openlayer-0.1.0a2/openlayer/utils.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/base_validator.py` & `openlayer-0.1.0a2/openlayer/validators/base_validator.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/baseline_model_validators.py` & `openlayer-0.1.0a2/openlayer/validators/baseline_model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/commit_validators.py` & `openlayer-0.1.0a2/openlayer/validators/commit_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/dataset_validators.py` & `openlayer-0.1.0a2/openlayer/validators/dataset_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/model_validators.py` & `openlayer-0.1.0a2/openlayer/validators/model_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/validators/project_validators.py` & `openlayer-0.1.0a2/openlayer/validators/project_validators.py`

 * *Files identical despite different names*

### Comparing `openlayer-0.1.0a1/openlayer/version.py` & `openlayer-0.1.0a2/openlayer/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,8 +18,8 @@
          headers=headers,
          params=params,
          json=body,
          files=files,
          data=data,
       )
 """
-__version__ = "0.1.0a1"
+__version__ = "0.1.0a2"
```

### Comparing `openlayer-0.1.0a1/openlayer.egg-info/PKG-INFO` & `openlayer-0.1.0a2/openlayer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlayer
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: The official Python API library for Openlayer: the Testing and Debugging Platform for AI
 Home-page: https://github.com/openlayer-ai/openlayer-python
 Author: Unbox Inc.
 Project-URL: Documentation, https://docs.openlayer.com/
 Project-URL: Openlayer User Slack Group, https://l.linklyhq.com/l/1DG73
 Keywords: MLOps,AI,Openlayer
 Classifier: Operating System :: OS Independent
```

### Comparing `openlayer-0.1.0a1/openlayer.egg-info/SOURCES.txt` & `openlayer-0.1.0a2/openlayer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.cfg
 setup.py
 openlayer/__init__.py
 openlayer/api.py
 openlayer/datasets.py
 openlayer/exceptions.py
 openlayer/models.py
+openlayer/project_versions.py
 openlayer/projects.py
 openlayer/schemas.py
 openlayer/tasks.py
 openlayer/utils.py
 openlayer/version.py
 openlayer.egg-info/PKG-INFO
 openlayer.egg-info/SOURCES.txt
```

### Comparing `openlayer-0.1.0a1/setup.cfg` & `openlayer-0.1.0a2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 	openlayer.validators
 	openlayer.prediction_jobs
 install_requires = 
 	jupyter
 	pandas
 	requests
 	tqdm
+	tabulate
 	marshmallow
 	marshmallow_oneofschema
 	requests_toolbelt
 	requests>=2.28.2
 	urllib3>=1.26.14
 python_requires = >=3.7
 include_package_data = True
```

