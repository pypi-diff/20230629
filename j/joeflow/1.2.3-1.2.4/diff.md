# Comparing `tmp/joeflow-1.2.3.tar.gz` & `tmp/joeflow-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joeflow-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "joeflow-1.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `joeflow-1.2.3.tar` & `joeflow-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1522 2023-05-22 11:15:09.599767 joeflow-1.2.3/LICENSE
--rw-r--r--   0        0        0     3128 2023-05-22 11:15:09.599767 joeflow-1.2.3/README.rst
--rw-r--r--   0        0        0      158 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/__init__.py
--rw-r--r--   0        0        0      160 2023-05-22 11:15:25.075769 joeflow-1.2.3/joeflow/_version.py
--rw-r--r--   0        0        0     4220 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/admin.py
--rw-r--r--   0        0        0      286 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/apps.py
--rw-r--r--   0        0        0      824 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/conf.py
--rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/contrib/__init__.py
--rw-r--r--   0        0        0     1234 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/contrib/reversion.py
--rw-r--r--   0        0        0     1387 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/forms.py
--rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/commands/__init__.py
--rw-r--r--   0        0        0     2304 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/commands/render_workflow_graph.py
--rw-r--r--   0        0        0     4955 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/migrations/__init__.py
--rw-r--r--   0        0        0    18595 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/models.py
--rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/__init__.py
--rw-r--r--   0        0        0     1995 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/celery.py
--rw-r--r--   0        0        0     2158 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/dramatiq.py
--rw-r--r--   0        0        0      288 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/__init__.py
--rw-r--r--   0        0        0      807 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/human.py
--rw-r--r--   0        0        0     3763 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/machine.py
--rw-r--r--   0        0        0       36 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/typing.py
--rw-r--r--   0        0        0     2745 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/utils.py
--rw-r--r--   0        0        0     3399 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/views.py
--rw-r--r--   0        0        0     2622 2023-05-22 11:15:09.599767 joeflow-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 joeflow-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-06-29 12:29:25.438561 joeflow-1.2.4/LICENSE
+-rw-r--r--   0        0        0     3128 2023-06-29 12:29:25.438561 joeflow-1.2.4/README.rst
+-rw-r--r--   0        0        0      158 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-29 12:29:47.886471 joeflow-1.2.4/joeflow/_version.py
+-rw-r--r--   0        0        0     4220 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/admin.py
+-rw-r--r--   0        0        0      286 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/apps.py
+-rw-r--r--   0        0        0      824 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/conf.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/contrib/__init__.py
+-rw-r--r--   0        0        0     1234 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/contrib/reversion.py
+-rw-r--r--   0        0        0     1387 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/forms.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/management/commands/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/management/commands/render_workflow_graph.py
+-rw-r--r--   0        0        0     4955 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/migrations/__init__.py
+-rw-r--r--   0        0        0    18595 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/models.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/runner/__init__.py
+-rw-r--r--   0        0        0     1995 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/runner/celery.py
+-rw-r--r--   0        0        0     2158 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/runner/dramatiq.py
+-rw-r--r--   0        0        0      288 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/tasks/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/tasks/human.py
+-rw-r--r--   0        0        0     3829 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/tasks/machine.py
+-rw-r--r--   0        0        0       36 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/typing.py
+-rw-r--r--   0        0        0     2745 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/utils.py
+-rw-r--r--   0        0        0     3399 2023-06-29 12:29:25.442561 joeflow-1.2.4/joeflow/views.py
+-rw-r--r--   0        0        0     2622 2023-06-29 12:29:25.442561 joeflow-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 joeflow-1.2.4/PKG-INFO
```

### Comparing `joeflow-1.2.3/LICENSE` & `joeflow-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/README.rst` & `joeflow-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/admin.py` & `joeflow-1.2.4/joeflow/admin.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/conf.py` & `joeflow-1.2.4/joeflow/conf.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/contrib/reversion.py` & `joeflow-1.2.4/joeflow/contrib/reversion.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/forms.py` & `joeflow-1.2.4/joeflow/forms.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/management/commands/render_workflow_graph.py` & `joeflow-1.2.4/joeflow/management/commands/render_workflow_graph.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/migrations/0001_initial.py` & `joeflow-1.2.4/joeflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/models.py` & `joeflow-1.2.4/joeflow/models.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/runner/celery.py` & `joeflow-1.2.4/joeflow/runner/celery.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/runner/dramatiq.py` & `joeflow-1.2.4/joeflow/runner/dramatiq.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/tasks/human.py` & `joeflow-1.2.4/joeflow/tasks/human.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/tasks/machine.py` & `joeflow-1.2.4/joeflow/tasks/machine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Set of reusable machine tasks."""
 from collections.abc import Iterable
 
 from django.utils import timezone
 
+from ..typing import MACHINE
+
 __all__ = (
     "Start",
     "Join",
     "Wait",
 )
 
 try:
@@ -47,15 +49,16 @@
 
         workflow = StartWorkflow.start(a_text_field="initial data")
 
     """
 
     def __call__(self, **kwargs):
         workflow = self.workflow_cls.objects.create(**kwargs)
-        task = workflow.task_set.create(name=self.name, workflow=workflow)
+        task = workflow.task_set.create(name=self.name, type=MACHINE, workflow=workflow)
+        task.finish()
         task.start_next_tasks()
         return workflow
 
 
 class Join:
     """
     Wait for all parent tasks to complete before continuing the workflow.
```

### Comparing `joeflow-1.2.3/joeflow/utils.py` & `joeflow-1.2.4/joeflow/utils.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/joeflow/views.py` & `joeflow-1.2.4/joeflow/views.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/pyproject.toml` & `joeflow-1.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.3/PKG-INFO` & `joeflow-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joeflow
-Version: 1.2.3
+Version: 1.2.4
 Summary: The lean workflow automation framework for machines with heart.
 Keywords: django,process,automation,workflow,framework,task
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

