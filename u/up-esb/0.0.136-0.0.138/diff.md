# Comparing `tmp/up_esb-0.0.136.tar.gz` & `tmp/up_esb-0.0.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_esb-0.0.136.tar", last modified: Fri Jun 23 10:08:35 2023, max compression
+gzip compressed data, was "up_esb-0.0.138.tar", last modified: Thu Jun 29 12:30:10 2023, max compression
```

## Comparing `up_esb-0.0.136.tar` & `up_esb-0.0.138.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.034140 up_esb-0.0.136/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.018140 up_esb-0.0.136/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.026140 up_esb-0.0.136/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-23 10:08:18.000000 up_esb-0.0.136/.github/scripts/update_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.026140 up_esb-0.0.136/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-23 10:08:18.000000 up_esb-0.0.136/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 10:08:18.000000 up_esb-0.0.136/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-23 10:08:18.000000 up_esb-0.0.136/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-23 10:08:18.000000 up_esb-0.0.136/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 10:08:18.000000 up_esb-0.0.136/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-23 10:08:35.034140 up_esb-0.0.136/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 10:08:18.000000 up_esb-0.0.136/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.026140 up_esb-0.0.136/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 10:08:18.000000 up_esb-0.0.136/docs/callable_interface.md
--rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-06-23 10:08:18.000000 up_esb-0.0.136/docs/create_action_interface.drawio.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.026140 up_esb-0.0.136/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-23 10:08:18.000000 up_esb-0.0.136/examples/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-23 10:08:18.000000 up_esb-0.0.136/examples/partialorderplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-23 10:08:18.000000 up_esb-0.0.136/examples/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-23 10:08:18.000000 up_esb-0.0.136/examples/time_triggered.py
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-06-23 10:08:18.000000 up_esb-0.0.136/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:08:35.034140 up_esb-0.0.136/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 10:08:18.000000 up_esb-0.0.136/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.030140 up_esb-0.0.136/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.030140 up_esb-0.0.136/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/components/test_expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/test_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/test_create_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-23 10:08:18.000000 up_esb-0.0.136/tests/test_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.030140 up_esb-0.0.136/up_esb/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.034140 up_esb-0.0.136/up_esb/components/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/components/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/components/expression_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/components/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.034140 up_esb-0.0.136/up_esb/plexmo/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/plexmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/plexmo/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-23 10:08:18.000000 up_esb-0.0.136/up_esb/plexmo/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:08:35.030140 up_esb-0.0.136/up_esb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-23 10:08:34.000000 up_esb-0.0.136/up_esb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 10:08:35.000000 up_esb-0.0.136/up_esb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:08:34.000000 up_esb-0.0.136/up_esb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 10:08:34.000000 up_esb-0.0.136/up_esb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 10:08:34.000000 up_esb-0.0.136/up_esb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.250705 up_esb-0.0.138/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.242705 up_esb-0.0.138/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.242705 up_esb-0.0.138/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-29 12:29:52.000000 up_esb-0.0.138/.github/scripts/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.246705 up_esb-0.0.138/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-29 12:29:52.000000 up_esb-0.0.138/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-29 12:29:52.000000 up_esb-0.0.138/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-29 12:29:52.000000 up_esb-0.0.138/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-29 12:29:52.000000 up_esb-0.0.138/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 12:29:52.000000 up_esb-0.0.138/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-29 12:30:10.250705 up_esb-0.0.138/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-29 12:29:52.000000 up_esb-0.0.138/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.246705 up_esb-0.0.138/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-29 12:29:52.000000 up_esb-0.0.138/docs/callable_interface.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37750 2023-06-29 12:29:52.000000 up_esb-0.0.138/docs/create_action_interface.drawio.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.246705 up_esb-0.0.138/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-29 12:29:52.000000 up_esb-0.0.138/examples/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-29 12:29:52.000000 up_esb-0.0.138/examples/partialorderplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-29 12:29:52.000000 up_esb-0.0.138/examples/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-06-29 12:29:52.000000 up_esb-0.0.138/examples/time_triggered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-06-29 12:29:52.000000 up_esb-0.0.138/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:30:10.250705 up_esb-0.0.138/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 12:29:52.000000 up_esb-0.0.138/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.246705 up_esb-0.0.138/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.246705 up_esb-0.0.138/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/components/test_expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/test_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/test_create_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-29 12:29:52.000000 up_esb-0.0.138/tests/test_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.250705 up_esb-0.0.138/up_esb/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18907 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.250705 up_esb-0.0.138/up_esb/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/components/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/components/expression_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/components/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.250705 up_esb-0.0.138/up_esb/plexmo/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/plexmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/plexmo/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-29 12:29:52.000000 up_esb-0.0.138/up_esb/plexmo/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:30:10.250705 up_esb-0.0.138/up_esb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-29 12:30:10.000000 up_esb-0.0.138/up_esb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-29 12:30:10.000000 up_esb-0.0.138/up_esb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:30:10.000000 up_esb-0.0.138/up_esb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 12:30:10.000000 up_esb-0.0.138/up_esb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 12:30:10.000000 up_esb-0.0.138/up_esb.egg-info/top_level.txt
```

### Comparing `up_esb-0.0.136/.github/scripts/update_version.py` & `up_esb-0.0.138/.github/scripts/update_version.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/.github/workflows/deploy.yml` & `up_esb-0.0.138/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/.github/workflows/main.yml` & `up_esb-0.0.138/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/.gitignore` & `up_esb-0.0.138/.gitignore`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/.pre-commit-config.yaml` & `up_esb-0.0.138/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/LICENSE` & `up_esb-0.0.138/LICENSE`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/PKG-INFO` & `up_esb-0.0.138/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up_esb
-Version: 0.0.136
+Version: 0.0.138
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.136/README.md` & `up_esb-0.0.138/README.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/docs/callable_interface.md` & `up_esb-0.0.138/docs/callable_interface.md`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/docs/create_action_interface.drawio.png` & `up_esb-0.0.138/docs/create_action_interface.drawio.png`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/examples/parallel.py` & `up_esb-0.0.138/examples/parallel.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/examples/partialorderplan.py` & `up_esb-0.0.138/examples/partialorderplan.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/examples/sequential.py` & `up_esb-0.0.138/examples/sequential.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/examples/time_triggered.py` & `up_esb-0.0.138/examples/time_triggered.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/pyproject.toml` & `up_esb-0.0.138/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 description = "General functionalities for using unified-planning in robotic applications"
 keywords = ["unified-planning", "embedded-systems-bridge"]
 license = {text = "Apache-2.0 License"}
 name = "up_esb"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.136"
+version = "0.0.138"
 
 [project.urls]
 Repository = "https://github.com/aiplan4eu/embedded-systems-bridge"
 Homepage = "https://www.aiplan4eu-project.eu/"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "pytest", "pre-commit"]
```

### Comparing `up_esb-0.0.136/tests/components/test_expression_manager.py` & `up_esb-0.0.138/tests/components/test_expression_manager.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/tests/test_bridge.py` & `up_esb-0.0.138/tests/test_bridge.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from typing import Callable, Dict
 
 import pytest
 from unified_planning.shortcuts import Equals, Not, OneshotPlanner
 
+from tests import ContextManager, get_example_plans
 from up_esb.bridge import Bridge
 from up_esb.components import ActionDefinition
 
 # pylint: disable=all
 ############################################################################################################
 ######################################### ESSENTIALS #######################################################
 ############################################################################################################
@@ -477,7 +478,79 @@
             if result is None:
                 raise Exception("No solution found")
 
             print("*** Result ***")
             for action_instance in result.plan.actions:
                 print(action_instance)
             print("*** End of result ***")
+
+
+class TestBridgeExecutableGraph:
+    @pytest.mark.parametrize("plan_name, plan", get_example_plans().items())
+    def test_bridge_executable_graph(self, plan_name, plan):
+        bridge = Bridge()
+        ContextManager.plan = plan
+
+        bridge._api_actions = ContextManager.get_actions_context()
+        bridge._fluent_functions = ContextManager.get_fluents_context()
+        bridge._api_objects = ContextManager.get_objects_context()
+
+        bridge.get_executable_graph(plan)
+
+    @pytest.mark.parametrize("plan_name, plan", get_example_plans().items())
+    def test_bridge_executable_action(self, plan_name, plan):
+        bridge = Bridge()
+        ContextManager.plan = plan
+
+        bridge._api_actions = ContextManager.get_actions_context()
+        bridge._fluent_functions = ContextManager.get_fluents_context()
+        bridge._api_objects = ContextManager.get_objects_context()
+
+        graph = bridge.get_executable_graph(plan)
+
+        for _, node in graph.nodes(data=True):
+            if node["action"] in ["start", "end"]:
+                continue
+
+            node["context"][node["action"]](**node["parameters"])
+
+    @pytest.mark.parametrize("plan_name, plan", get_example_plans().items())
+    def test_bridge_executable_preconditions(self, plan_name, plan):
+        bridge = Bridge()
+        ContextManager.plan = plan
+
+        bridge._api_actions = ContextManager.get_actions_context()
+        bridge._fluent_functions = ContextManager.get_fluents_context()
+        bridge._api_objects = ContextManager.get_objects_context()
+
+        graph = bridge.get_executable_graph(plan)
+
+        for _, node in graph.nodes(data=True):
+            if node["action"] in ["start", "end"]:
+                continue
+            print(node["node_name"])
+
+            import ast
+
+            for preconditions in node["preconditions"].values():
+                for expression in preconditions:
+                    print(ast.dump(ast.parse(expression)))
+                    eval(compile(expression, "<ast>", "eval"), node["context"])
+
+    @pytest.mark.parametrize("plan_name, plan", get_example_plans().items())
+    def test_bridge_executable_postconditions(self, plan_name, plan):
+        bridge = Bridge()
+        ContextManager.plan = plan
+
+        bridge._api_actions = ContextManager.get_actions_context()
+        bridge._fluent_functions = ContextManager.get_fluents_context()
+        bridge._api_objects = ContextManager.get_objects_context()
+
+        graph = bridge.get_executable_graph(plan)
+
+        for _, node in graph.nodes(data=True):
+            if node["action"] in ["start", "end"]:
+                continue
+
+            for post_conditions in node["postconditions"].values():
+                for expression, _ in post_conditions:
+                    eval(compile(expression, "<ast>", "eval"), node["context"])
```

### Comparing `up_esb-0.0.136/tests/test_create_action.py` & `up_esb-0.0.138/tests/test_create_action.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/tests/test_dispatcher.py` & `up_esb-0.0.138/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/tests/test_graph.py` & `up_esb-0.0.138/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/tests/test_monitor.py` & `up_esb-0.0.138/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/__init__.py` & `up_esb-0.0.138/up_esb/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/bridge.py` & `up_esb-0.0.138/up_esb/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,30 +394,30 @@
                     []
                     if interval not in executable_preconditions
                     else executable_preconditions[interval]
                 )
 
                 for precondition in preconditions:
                     executable_preconditions[interval].append(
-                        exp_manager.convert(precondition, parameters=parameters)
+                        exp_manager.convert(precondition, parameters=action_parameters)
                     )
             executable_graph.nodes[node_id]["preconditions"] = executable_preconditions
 
             # Action Effects
             executable_effects: Dict[str, List[Tuple[Callable, typing.Any]]] = {}
             for interval, effects in executable_graph.nodes[node_id]["postconditions"].items():
                 executable_effects[interval] = (
                     [] if interval not in executable_effects else executable_effects[interval]
                 )
 
                 for effect in effects:
                     executable_effects[interval].append(
                         (
-                            exp_manager.convert(effect.fluent, parameters=parameters),
-                            exp_manager.convert(effect.value, parameters=parameters),
+                            exp_manager.convert(effect.fluent, parameters=action_parameters),
+                            exp_manager.convert(effect.value, parameters=action_parameters),
                         )
                     )
             executable_graph.nodes[node_id]["postconditions"] = executable_effects
 
             # Finally setup execution context to the nodes
             executable_graph.nodes[node_id]["context"] = context
```

### Comparing `up_esb-0.0.136/up_esb/components/__init__.py` & `up_esb-0.0.138/up_esb/components/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/components/actions.py` & `up_esb-0.0.138/up_esb/components/actions.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/components/expression_manager.py` & `up_esb-0.0.138/up_esb/components/expression_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,33 +58,33 @@
                     op=ast.Or(),
                     values=[self._map_expression(arg) for arg in exp.args],
                 )
             elif exp.is_equals():
                 assert len(exp.args) == 2
 
                 return ast.Compare(
-                    op=ast.Eq(),
+                    ops=[ast.Eq()],
                     left=self._map_expression(exp.args[0]),
-                    right=self._map_expression(exp.args[1]),
+                    comparators=[self._map_expression(exp.args[1])],
                 )
             elif exp.is_le():
                 assert len(exp.args) == 2
 
                 return ast.Compare(
-                    op=ast.LtE(),
+                    ops=[ast.LtE()],
                     left=self._map_expression(exp.args[0]),
-                    right=self._map_expression(exp.args[1]),
+                    comparators=[self._map_expression(exp.args[1])],
                 )
             elif exp.is_lt():
                 assert len(exp.args) == 2
 
                 return ast.Compare(
-                    op=ast.Lt(),
+                    ops=[ast.Lt()],
                     left=self._map_expression(exp.args[0]),
-                    right=self._map_expression(exp.args[1]),
+                    comparators=[self._map_expression(exp.args[1])],
                 )
 
             elif exp.is_constant():
                 if exp.is_bool_constant():
                     return ast.Constant(value=exp.bool_constant_value())
                 elif exp.is_int_constant():
                     return ast.Constant(value=exp.int_constant_value())
```

### Comparing `up_esb-0.0.136/up_esb/components/graph.py` & `up_esb-0.0.138/up_esb/components/graph.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/executor.py` & `up_esb-0.0.138/up_esb/executor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/plexmo/__init__.py` & `up_esb-0.0.138/up_esb/plexmo/__init__.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/plexmo/dispatcher.py` & `up_esb-0.0.138/up_esb/plexmo/dispatcher.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb/plexmo/monitor.py` & `up_esb-0.0.138/up_esb/plexmo/monitor.py`

 * *Files identical despite different names*

### Comparing `up_esb-0.0.136/up_esb.egg-info/PKG-INFO` & `up_esb-0.0.138/up_esb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-esb
-Version: 0.0.136
+Version: 0.0.138
 Summary: General functionalities for using unified-planning in robotic applications
 License: Apache-2.0 License
 Project-URL: Repository, https://github.com/aiplan4eu/embedded-systems-bridge
 Project-URL: Homepage, https://www.aiplan4eu-project.eu/
 Keywords: unified-planning,embedded-systems-bridge
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `up_esb-0.0.136/up_esb.egg-info/SOURCES.txt` & `up_esb-0.0.138/up_esb.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .github/workflows/main.yml
 docs/callable_interface.md
 docs/create_action_interface.drawio.png
 examples/parallel.py
 examples/partialorderplan.py
 examples/sequential.py
 examples/time_triggered.py
+tests/__init__.py
 tests/test_bridge.py
 tests/test_create_action.py
 tests/test_dispatcher.py
 tests/test_graph.py
 tests/test_monitor.py
 tests/components/__init__.py
 tests/components/test_expression_manager.py
```

