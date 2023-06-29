# Comparing `tmp/dbt-graph-builder-0.2.0.tar.gz` & `tmp/dbt-graph-builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.2.0.tar", last modified: Wed Jun 28 13:11:18 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.3.0.tar", last modified: Thu Jun 29 07:30:14 2023, max compression
```

## Comparing `dbt-graph-builder-0.2.0.tar` & `dbt-graph-builder-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-28 13:11:18.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-28 13:11:18.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:11:18.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 13:11:18.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-28 13:11:18.000000 dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:11:18.566602 dbt-graph-builder-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/tests/test_graph_dag_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/tests/test_graph_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-28 13:10:59.000000 dbt-graph-builder-0.2.0/tests/test_graph_ephemeral_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.742375 dbt-graph-builder-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 07:30:14.000000 dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:30:14.746375 dbt-graph-builder-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_dag_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-29 07:29:54.000000 dbt-graph-builder-0.3.0/tests/test_graph_ephemeral_operator.py
```

### Comparing `dbt-graph-builder-0.2.0/LICENSE` & `dbt-graph-builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/PKG-INFO` & `dbt-graph-builder-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.2.0
+Version: 0.3.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,25 +25,27 @@
             OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
             SOFTWARE
         
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Project Template
-
-This project follows the Python Standards declared in [PEP 621](https://peps.python.org/pep-0621/).
-This uses a pyproject.yaml to configuration the project. In this example, [flit](https://pypi.org/project/flit/) is used to simplify the build process, and publish to pypi.
+# dbt-graph-builder
 
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
+[![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
     - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
```

### Comparing `dbt-graph-builder-0.2.0/README.md` & `dbt-graph-builder-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Python Project Template
-
-This project follows the Python Standards declared in [PEP 621](https://peps.python.org/pep-0621/).
-This uses a pyproject.yaml to configuration the project. In this example, [flit](https://pypi.org/project/flit/) is used to simplify the build process, and publish to pypi.
+# dbt-graph-builder
 
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
+[![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
     - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
```

### Comparing `dbt-graph-builder-0.2.0/pyproject.toml` & `dbt-graph-builder-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,23 @@
     {name = "Piotr Tutak", email = "piotr.tutak@getindata.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
     "networkx>=2.6,<3",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 
 [tool.bandit]
 exclude_dirs = ["build","dist","tests","scripts"]
 number = 4
@@ -42,15 +44,15 @@
     "E203",
     "D100",  # public module
     "D104",  # public package
     "D105",  # magic methods
     "DCO010", # duplicate of public method
     "DCO060", # public attributes - they're already documented if it is a property.
 ]
-exclude = ["build", "tests"]
+exclude = ["build", "tests", ".venv"]
 convention = "google"
 
 [tool.mypy]
 packages = ["src"]
 exclude = ["tests"]
 ignore_missing_imports = true
 strict = true
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
 from typing import Any, NamedTuple, cast
 
 from dbt_graph_builder.gateway import GatewayConfiguration, TaskGraphConfiguration
 from dbt_graph_builder.graph import DbtManifestGraph
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Any
 
 from dbt_graph_builder.utils import is_model_run_task
 
 
 @dataclass
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import logging
 from typing import Any
 
 import networkx as nx
 from networkx.classes.reportviews import NodeDataView, OutEdgeDataView
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+
 def is_task_type(node_name: str, task_type: str) -> bool:
     """Check if node name is of a certain task type.
 
     Args:
         node_name (str): Node name.
         task_type (str): Task type.
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.2.0
+Version: 0.3.0
 Summary: DBT Graph Builder
 Author-email: Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,25 +25,27 @@
             OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
             SOFTWARE
         
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Project Template
-
-This project follows the Python Standards declared in [PEP 621](https://peps.python.org/pep-0621/).
-This uses a pyproject.yaml to configuration the project. In this example, [flit](https://pypi.org/project/flit/) is used to simplify the build process, and publish to pypi.
+# dbt-graph-builder
 
+[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-graph-builder)
+[![PyPI Version](https://badge.fury.io/py/dbt-graph-builder.svg)](https://pypi.org/project/dbt-graph-builder/)
+[![Downloads](https://pepy.tech/badge/dbt-graph-builder)](https://pepy.tech/project/dbt-graph-builder)
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
     - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
```

### Comparing `dbt-graph-builder-0.2.0/src/dbt_graph_builder.egg-info/SOURCES.txt` & `dbt-graph-builder-0.3.0/src/dbt_graph_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/tests/test_gateway.py` & `dbt-graph-builder-0.3.0/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/tests/test_graph.py` & `dbt-graph-builder-0.3.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/tests/test_graph_dag_dependencies.py` & `dbt-graph-builder-0.3.0/tests/test_graph_dag_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/tests/test_graph_dependencies.py` & `dbt-graph-builder-0.3.0/tests/test_graph_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.2.0/tests/test_graph_ephemeral_operator.py` & `dbt-graph-builder-0.3.0/tests/test_graph_ephemeral_operator.py`

 * *Files identical despite different names*

