# Comparing `tmp/irisml-tasks-fiftyone-0.0.1.tar.gz` & `tmp/irisml-tasks-fiftyone-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-fiftyone-0.0.1.tar", last modified: Sat Jun 10 02:23:55 2023, max compression
+gzip compressed data, was "irisml-tasks-fiftyone-0.0.2.tar", last modified: Thu Jun 29 16:44:37 2023, max compression
```

## Comparing `irisml-tasks-fiftyone-0.0.1.tar` & `irisml-tasks-fiftyone-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/irisml/tasks/launch_fiftyone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 02:23:55.000000 irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:23:55.168191 irisml-tasks-fiftyone-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-10 02:19:45.000000 irisml-tasks-fiftyone-0.0.1/test/test_launch_fiftyone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:44:37.494459 irisml-tasks-fiftyone-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-29 16:41:16.000000 irisml-tasks-fiftyone-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 16:44:37.494459 irisml-tasks-fiftyone-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-29 16:41:16.000000 irisml-tasks-fiftyone-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:44:37.490459 irisml-tasks-fiftyone-0.0.2/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:44:37.490459 irisml-tasks-fiftyone-0.0.2/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-29 16:41:16.000000 irisml-tasks-fiftyone-0.0.2/irisml/tasks/launch_fiftyone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:44:37.494459 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 16:44:37.000000 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-29 16:44:37.000000 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:44:37.000000 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:44:37.000000 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 16:44:37.000000 irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 16:41:16.000000 irisml-tasks-fiftyone-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-29 16:44:37.494459 irisml-tasks-fiftyone-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:44:37.494459 irisml-tasks-fiftyone-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-29 16:41:16.000000 irisml-tasks-fiftyone-0.0.2/test/test_launch_fiftyone.py
```

### Comparing `irisml-tasks-fiftyone-0.0.1/LICENSE` & `irisml-tasks-fiftyone-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-fiftyone-0.0.1/PKG-INFO` & `irisml-tasks-fiftyone-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-fiftyone
-Version: 0.0.1
+Version: 0.0.2
 Summary: IrisML tasks for fiftyone
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-fiftyone-0.0.1/README.md` & `irisml-tasks-fiftyone-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-fiftyone-0.0.1/irisml/tasks/launch_fiftyone.py` & `irisml-tasks-fiftyone-0.0.2/irisml/tasks/launch_fiftyone.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     This task will wait for the specified time, then returns an output. You can also finish the task by sending a SIGINT signal.
 
     Config:
         task_type (str): The type of the task. One of ``multiclass_classification``, ``multilabel_classification``, or ``object_detection``.
         duration (int): The duration of the task in seconds.
     """
-    VERSION = '0.2.0'
+    VERSION = '0.2.1'
     CACHE_ENABLED = False
 
     @dataclasses.dataclass
     class Inputs:
         dataset: torch.utils.data.Dataset
         predictions: typing.Optional[typing.List[torch.Tensor]] = None
         class_names: typing.Optional[typing.List[str]] = None
@@ -77,15 +77,20 @@
     @staticmethod
     def _make_fo_labels(targets, task_type, label_names):
         def get_name(class_id: typing.Union[int, float]):
             class_id = int(class_id)
             return label_names[class_id] if class_id < len(label_names) else f'label_{class_id}'
 
         if task_type == 'multiclass_classification':
-            label_id = targets if isinstance(targets, int) else targets[0]
+            if isinstance(targets, int):
+                label_id = targets
+            elif isinstance(targets, torch.Tensor) and targets.ndim == 0:
+                label_id = targets.item()
+            else:
+                label_id = targets[0]
             return fiftyone.Classification(label=get_name(label_id))
         elif task_type == 'multilabel_classification':
             return fiftyone.Classifications(classifications=[fiftyone.Classification(label=get_name(i)) for i in targets])
         elif task_type == 'object_detection':
             return fiftyone.Detections(detections=[fiftyone.Detection(label=get_name(class_id), bounding_box=[x, y, x2 - x, y2 - y]) for class_id, x, y, x2, y2 in targets])
         else:
             logger.warning(f"Failed to parse {targets} as {task_type} data.")
```

### Comparing `irisml-tasks-fiftyone-0.0.1/irisml_tasks_fiftyone.egg-info/PKG-INFO` & `irisml-tasks-fiftyone-0.0.2/irisml_tasks_fiftyone.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-fiftyone
-Version: 0.0.1
+Version: 0.0.2
 Summary: IrisML tasks for fiftyone
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-fiftyone-0.0.1/test/test_launch_fiftyone.py` & `irisml-tasks-fiftyone-0.0.2/test/test_launch_fiftyone.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pathlib
 import tempfile
 import unittest
 import PIL.Image
+import torch
 from irisml.tasks.launch_fiftyone import Task
 
 
 class TestLaunchFiftyone(unittest.TestCase):
     def test_load_classification_dataset(self):
         fake_dataset = [(PIL.Image.new('RGB', (100, 100)), 1),
                         (PIL.Image.new('RGB', (100, 100)), 2),
-                        (PIL.Image.new('RGB', (100, 100)), 3)]
-        predictions = [[0, 1, 0, 0], [0, 0, 1, 0], [0, 1, 1, 1]]
+                        (PIL.Image.new('RGB', (100, 100)), [3]),
+                        (PIL.Image.new('RGB', (100, 100)), torch.tensor([4])),
+                        (PIL.Image.new('RGB', (100, 100)), torch.tensor(0))]
+        predictions = [[0, 1, 0, 0, 0], [0, 0, 1, 0, 0], [0, 1, 1, 1, 0], [0, 0, 0, 1, 1], [1, 0, 0, 0, 1]]
 
         with tempfile.TemporaryDirectory() as temp_dir:
             dataset = Task.convert_to_fiftyone_dataset(fake_dataset, None, None, 'multiclass_classification', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
         with tempfile.TemporaryDirectory() as temp_dir:
             dataset = Task.convert_to_fiftyone_dataset(fake_dataset, predictions, None, 'multiclass_classification', pathlib.Path(temp_dir))
             self._assert_dataset(dataset)
```

